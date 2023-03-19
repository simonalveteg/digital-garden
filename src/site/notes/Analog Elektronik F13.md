---
{"dg-publish":true,"permalink":"/analog-elektronik-f13/","tags":["föreläsning","analogelektronik"]}
---


# repetition
## Superpositionsmodellen
Det räcker inte att kunna uttantill.. härled!😡

härled genom att förlänga med $1-A \beta$, man får blockdagrammet och utifrån den ska du kunna sätta upp ett uttryck som du sedan förlänger. #todo 

slutna förstärknngen är förhållandet mellan käll- och lastsignal. 

## In och ut[[Impedans\|impedans]] för [[Negativ Återkoppling\|negativt återkopplade]] [[Förstärkare\|förstärkare]]
[[Negativ Återkoppling\|negativ återkoppling]] förbättrar in- och utimpedanserna med $(1+|A \beta|)$. 
För en spänning på ingången : $Z_{in}=Z_{i}(1+|A \beta|)$ där $Z_{i}=\left. \frac{V_{test}}{i_{test}}\right|_{Q_{L}=0}$ .
För en ström på ingången : $Z_{in}=\frac{Z_{i}}{1+|A \beta|}$ där $Z_{i}=\left. \frac{V_{test}}{i_{test}}\right|_{Q_{L}=0}$ .

> Man ska kunna sätta upp uttryck för in- och utimpedanser för [[Negativ Återkoppling\|negativt återkopplade]] [[Förstärkare\|förstärkare]]. Ganska lätt? Om det är en spänning på ingången vill vi att all spänning faller där → oändlig inimpedans. [[feedback\|Återkopplingen]] ska göra [[Impedans\|impedanserna]] mer ideala → ökar med faktorn $(1+|A \beta|)$. Spänning på utgången → allt ska falla över $R_{L}$ → utimpedansen ska vara noll → [[feedback\|återkopplingen]] minskar med faktorn istället (division). 

När man kollar på ingången sätter man $Q_{L}=0$ och på utgången sätter man $Q_{g}=0$. Kör sen lite epic kretsanalys. Man kan skita i de styrda källorna då insignalskällan är noll och då finns det ingenting som styr.

egentligen är det [[Frekvensberoende\|frekvensberoende]] men vi räknar med $A \beta(0)$ för annars blir det skitjobbigt jao. På tentan kommer det vara rent [[Resistivitet\|resistivt]], dvs man kan skita i kondensatorerna i hybrid-pi modellen

[[Frekvenskompensering\|Frekvenskompensering]]
[[Capacitive Narrowbanding\|Capacitive Narrowbanding]]
[[Phantom Zero\|fantomnolla]]
[[Storsignaldistorsion\|Storsignaldistorsion]]
[[Transimpedansbiasering\|Transimpedansbiasering]]
# Subject
[[Analog Elektronik\|Analog Elektronik]]
