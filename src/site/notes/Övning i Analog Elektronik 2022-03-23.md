---
{"dg-publish":true,"permalink":"/oevning-i-analog-elektronik-2022-03-23/","tags":["övning","analogelektronik"]}
---


vi gör egentligen samma sak som vi har gjort innan fast med en djupare förståelse av [[Frekvensberoende\|frekvensberoende]]. 

en BJTs beteende kan beskrivas av $\beta_{f}$ och $\omega_{t}$, vilket är frekvensen då current gain är 1. (transient frequency). Tidigare har vi inte använt $\omega_{t}$ då vi inte kollat på [[Frekvensberoende\|frekvensberoende]]. 

$c_\pi$ och $c_\mu$ är två parasitiska [[Kapacitans\|kapacitanser]] för en [[Bipolär transistor\|BJT]], som endast spelar roll vid höga frekvenser. $c_\mu$ är mycket mindre än $c_{\pi}$, vilket beror på hur [[Transistor\|transistorerna]] är byggda, $c_\pi$ är mellan bas och emittor, och deras gemensamma area är mycket större än den för $c_\mu$ som är mellan bas och kollektor. Det är därför vi oftast skiter i $c_\mu$ (det blir också väldigt komplicerat att räkna med den).

$\omega_{t}$ kan approximeras som $\frac{g_{m}}{c_{\pi}}$, men det är värt at tkomma ihåg att i verkligheten kommer det vara lite mindre, då vi har skitit i $c_{\mu}$. Den här sortens approximeringar var väldigt vanliga när man räknade på papper, som vi gör i kursen 🤪🤪🤡🤡. I industrin används riktiga formler och simuleringar och skit. Kan skrivas om som $\frac{1}{r_{\pi}c_{\pi}}=\frac{\omega_{t}}{\beta_{f}}$

uppgifter i kursen: 
Hitta $A$ och $\beta$. Hitta dess [[Poler\|poler]] och eventuella [[Nollställen\|nollställen]]. Skriv om dem i förhållande till $\omega_{t}$ - men inte alltid (man måste inte), men det hjälper för att $1/r_{\pi}c_{\pi}$ för alla [[Transistor\|transistorer]] med samma teknologi kommer det vara konstant, för det är lika med $\omega_{t}/\beta_{f}$ som beror på teknologin. När man har två eller tre [[Förstärkare\|förstärkare]] kan man hitta två eller tre [[Poler\|poler]], och alla har $1/r_{\pi}c_{\pi}$ i sina ekvationer, och om man gör om det till  $\omega_{t}/\beta_{f}$ så kan man bryta ut det ur alla vilket underlättar för beräkningar. På så sätt blir det alltså lättare att jämföra [[Poler\|poler]] och hitta [[Dominanta och Icke-dominanta poler\|dominanta poler]] m.m. 

mindre [[Poler\|poler]] är mer dominanta, för deras respons är långsammare. De minsta [[Poler\|polerna]] påverkar hur dynamiskt ett [[System (matematisk definition)\|System (matematisk definition)]] kan vara. Ju större polen är desto snabbare är den. Det är därför man kan bortse från [[Poler\|poler]] som ligger långt bort. De påverkar helt enkelt inte transienten speciellt mycket. 

As a rule of thumb: if you have a pole which is five or ten times greater than the others you can ignore it with no harm.


## Subject
[[Analog Elektronik\|Analog Elektronik]]
