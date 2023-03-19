---
{"dg-publish":true,"permalink":"/systematisk-foerstaerkardesign/","tags":["analogelektronik"]}
---


1. Rita upp [[Förstärkare\|förstärkaren]] och [[feedback\|återkopplingsnätverket]] med hjälp av [[Nullor\|nullor]]
2. Byt ut [[Nullor\|nullorn]] mot dina [[Förstärkande Steg\|förstärkande steg]], kopplade så att polariteten på in- och utgång av [[Nullor\|nullorn]] stämmer
3. Byt ut [[Transistor\|transistorerna]] mot dess hybrid-pi modeller
4. Beräkna [[Slingförstärkning\|slingförstärkningen]] $A \beta(s)$ genom att ersätta delar av kretsen med en testgenerator och [[Nodanalys\|nodanalys]]/[[Kirchoffs lagar\|kcl]] 
5. Ta fram [[Slingpoler och Slingnollställen\|slingpolerna]] ur ditt uttryck för [[Slingförstärkning\|slingförstärkningen]]
6. Gör [[Bandbreddsuppskattning\|Bandwidth Estimation]] för att ta reda på den maximala [[Bandbredd\|bandbredden]] man kan uppnå med dessa [[Slingpoler och Slingnollställen\|slingpoler]]. Det görs med hjälp av [[LP-produkten\|LP-produkten]]
7. Hitta önskade [[Systempoler\|systempoler]] genom att göra om [[System (matematisk definition)\|systemet]] till ett [[Maximal Flat Frekvensgång\|butterworthsystem]] (i kursen vill vi alltid ha [[Systempoler\|systempolerna]] i [[Butterworthposition\|butterworthposition]]? - typ ja, men det beror egentligen på vad man är ute efter)
8. Om summan av [[Systempoler\|systempoler]] $\geq$ summan av [[Slingpoler och Slingnollställen\|slingpoler]] är det “rimligt” annars har vi inkluderat en [[Dominanta och Icke-dominanta poler\|icke-dominant pol]] i beräkningarna, och får ta bort den minsta polen och göra [[Bandbreddsuppskattning\|Bandwidth Estimation]] igen.
9. Hitta [[Phantom Zero\|fantomnolla]], och räkna ut [[Kapacitans\|kondensator]]. Metoden fungerar om $\delta \geq 7$ (eller väldigt nära 7). Annars måste vi använda andra [[Frekvenskompenseringsmetoder\|frekvenskompenseringsmetoder]]


 Hur vet man var man sätter ut kondensatorerna i sin krets?? hur räknar man ut storlekten på dem? 
 - Man vill sätta sina kompenserande komponenter på ett sätt så att [[Slingförstärkning\|slingförstärkningen]] får ett till [[Nollställen\|nollställe]] för någon frekvens. Det kan vara en [[Kapacitans\|kondensator]] parallellt med [[Resistans\|resistans]] för att skapa ett avbrott, eller en [[Spole\|spole]] [[Serie- och paralell-kopplingar\|i serie]] med en [[Resistans\|resistans]] för att skapa en kortslutning. Man räknar ut storleken på komponenten med hjälp av en formel. 
