---
{"dg-publish":true,"permalink":"/effektbalans/","tags":["elenergiteknik"]}
---

Elnätets frekvens på 50Hz speglar effektbalansen i systemet. Det är samma frekvens i hela systemet? 😲😲 Ju större energilager man har desto lättare är det att hålla sig nära rätt frekvens. Det är alltså fördelaktigt att sammankoppla system för att få större energilager. Effektbalans kan uppnås med [[Automatisk Frekvensreglering\|Automatisk Frekvensreglering]].

Finns flaskhalsar mellan elprisområden, som avgör hur mycket [[Effekt\|effekt]] som kan skickas mellan dem. Priset går upp i det område som har brist. Det område med lägst pris får exportera till sina grannar.

Elnätet saknar energilager, men [[Kraftverk\|kraftverk]] har energilager.

[[Synkronmaskinen\|Synkrongeneratorns]] momentbalans kan beskrivas som effektbalans. I turbinen får vi
$$
\frac{dW_k}{dt}=P_m-P_e
$$
där $P_m$ är mekanisk turbineffekt och $P_e$ är elektrisk generatoreffekt. Elnätet blir då
$$
\frac{dW_k}{dt}=\omega_mJ \frac{d\omega_m}{dt}\approx\omega_\text{nom}J \frac{d\omega_m}{dt}
$$
Effektbalansen påverkar generatorers varvtal som bestämmer frekvensen som kan mätas i ett vägguttag. Alla [[Kraftverk\|kraftverk]] synkroniseras mot somma vinkelhastighet. Alla generatorer tillsammans kan buntas ihop som ett stort energilager
$$
\omega_\text{mom}J_\text{total} \frac{d\omega_\text{system}}{dt}=P_\text{m,total}-P_\text{e,total}
$$
