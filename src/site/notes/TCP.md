---
{"dg-publish":true,"permalink":"/tcp/","tags":["kommunikationssystem"]}
---

Transmission Control Protocol (TCP) är det [[Transportprotokoll\|Transportprotokoll]] som används när en applikation vill ha en kontrollerad och tillförlitlig dataöverföring. TCP kompletterar [[Internet Protocol\|IP]]:s förbindelsefria, best-effort paketförmedling med en förbindelseorienterad och felfri process-to-process kommunikation. 

# Segmentformat
Data som kommer från applikationen delas upp i block, så kallade segment, och öveförs sedan till mottagaren. TCP är ett *stream oriented protocol*, dvs data överförs som en ström av byte. TCP delar upp data i block av lämplig storlek, som sedan skickas över på ett tillförlitligt sätt till mottagaren. 

TCP-headern består av
1. Sändarens portadress
2. Mottagarens portadress
3. Sekvensnummer: Anger det nummer som är tilldelat den första byten av data som ingår i segmentet. Varje byte som skickas är numrerat.
4. ACK-nummer: Anger det byte-nummer som mottagaren förväntar sig skall komma i nästa segment. TCP är ett *piggybacked* protokoll, vilket innebär at tACK kan skickas samtidigt med data.
5. Längd: Längden på headern mätt i 32-bitars ord. Kan vara mellan 20 och 60 byte.
6. Reserverad: ett fält som är reserverat för framtida funktioner
7. Kontrollflaggor: sex flaggor används för att hantera TCP-förbindelsen, dataöverföring och flödeskontroll.
	1. URG: urgent pointer används
	2. ACK: ACK-fältet används
	3. PSH: Mottagaren skall lämna data till applikationen så fort som möjligt
	4. RST: förbindelsen skall kopplas upp igen (reset)
	5. SYN: Sekvensnummer skall synkroniseras. Anväds vid uppkoppling av förbindelse
	6. FIN: Sändaren har skickat all data.
8. Fönsterstorlek: används i TCP:s felhanterinsmekanism. Anger hur många byte sändaren får skicka utan att få ACK tillbaka. Mottagaren bestämmer fönsterstorleken.
9. Kontrollsumma: En 16 bitar kontrollsumma beräknas på TCP-heaern, TCP-data samt vissa fält  IP-headern.
10. Urgent pointer: används för högprioriterade data och innehåller ett extra sekvensnummer
11. Eventuella tillval: det finns utrymme för 40 byte av tillvalsinformation i TCP-headern.

# TCP-förbindelsen
TCP-segment skickas via [[Internet Protocol\|IP]] som är förbindelsefritt, därför sparar TCP segment som inte kommer i ordningsföljd och sorterar dem innan de levereras till applikationen. Mottagarapplikationen är på så sätt garanterad att få data i samma ordning som de skickades.

En förbindelse måste därför kopplas upp mellan sändare och mottagare, för att sedan kopplas ned när sändningen är klar.

## Uppkoppling
TCP använder sig av en three-way handshake för att sätta upp en förbindelse, se bild nedan.
![Pasted image 20230221171718.png](/img/user/images/Pasted%20image%2020230221171718.png)
Dator 1 (client) skickar ett TCP-segment med SYN-flaggan satt till 1 och ett inledande sekvensnummer i sekvensnummer-fältet. Dator 2 (server) skickar tillbaka ett TCP-segment med SYN- och ACK-flaggorna satta till 1. Sekvensnummer-fältet innehåller dator 2:s inledande sekvensnummer. ACK-fältet är satt till det sekvensnummer den förväntar sig att dator 1 skickar nästa gång. Sist skickar dator 1 ett nytt TCP-segment med ACK satt till 1.

En TCP förbindelse är egentligen två separata förbindelser, en i vardera riktning.

## Nedkoppling
Båda parter kan när som helst stänga förbindelsen.
![Pasted image 20230221172248.png](/img/user/images/Pasted%20image%2020230221172248.png)

## Dataöverföring
Sändarapplikationen lagrar data i en sänd-buffert. TCP tar data från bufferten och skapar TCP-segment som skickas till mottagaren. Data får ligga kvar i bufferten tills de blivit ACK:ade.

På mottagarsidan läggs de mottagna datasegmenten i en buffert. Data levereras sedan till applikationen vid en lämplig tidpunkt. Segment som är i fel ordning sorteras. 

Ett TCP-segment med URG-flaggan satt till 1 kommer levereras direkt till applikationen.

# Felkorrigering
TCP är till för tillförlitlig dataöverföring, dvs alla data ska garanterat komma fram korrekt. Pga [[Internet Protocol\|IP]] kan segment gå förlorade pga överfulla buffertar i routrar. Även bitfel kan uppkomma. TCP innehåller ett antal funktioner för felkorrigering och flödeskontroll.

TCP använder sig av en så kallad [[Automatic Repeat Request algorithm\|Automatic Repeat Request algorithm]] som bygger på [[Go-back-N ARQ\|Go-back-N ARQ]].

# Flödeskontroll
Syfter med flödeskontroll är att inte skicka mer data än vad mottagaren och nätet kan hantera. När TCP har en aktiv förbindelse igång befinner den sig i en av tre faser:

## Slow Start
När en förbindelse har blivit uppkopplad. Varje gång sändaren tar emot ett ACK ökas *cwind* med 1. Fler och fler segment kan skickas utan att få ACK tillbaka. ALgoritmen ger en exponentiell ökning av sändfönstret (förutsatt att rwind är större än cwind). Ökningen kan inte hålla på hur länge som helst. När cwind når slow-start threshold går TCP över i fasen Congestion Avoidance.

## Congestion avoidance
cwind ökas fortfarande, men inte lika snabbt som i slow-start. cwind ökas med ett när det har kommit cwind nya ACK. TCP befinner sig här tills överbelastning i nätet har detekterats.

## Congestion detection
När sändaren måste skicka om ett segment kan det bero på två saker. Antingen har RTO-timern gått ut eller så har den fått tre duplicerade ACK.

Om RTO-timern har gått ut innebär detta att inget ACK kommit från mottagaren på ett bra tag, vilket antagligen beror på överbelastning i nätet, och en eller flera routrar måste kasta paket pga överfulla buffertar. Då görs följande:
1. ssthresh sätts till hälften av cwind
2. cwind sätts till 1 igen
3. TCP återgår till fasen slow start

Om tre duplicerade ACK tagits emot är det mindre troligt att nätet är överbelastat eftersom att mottagaren kan ta emot och skicka segment. Då görs istället följande
1. sstrhesh stts till hälften av cwind
2. cwind sätts till det nya värdet av ssthresh
3. TCP återfår till fasen congestion avoidance.

# Varianter av TCP
Det används flera olika varianter av TCP i olika system. De grundläggande funktionerna är samma.