---
{"dg-publish":true,"permalink":"/n-mosfet/","tags":["komponentfysik","analogelektronik"]}
---


En nMOS använder sig av ett substrat av [[Dopning\|p-typ]]. 

![nmossammanfattning.png](/img/user/images/nmossammanfattning.png)
Man kan använda antingen storsignalanalys eller småsignalanalys beroende på vad man bryr sig mest om typ.

> Datorbaserad analys och syntes är nödvändig för noggrann kretskonstruktion!

## Fysisk modell

![Pasted image 20220407103354.png](/img/user/images/Pasted%20image%2020220407103354.png)
I bilden ovan visas en nMOSFET i genomskärning till höger, sen en representation till vänster, som har roterats 90 grader. Representationen visar [[Energiband\|energibanden]], och hur dessa förändras när man lägger på en gatespänning. Längst ned till vänster visas hur mycket spänning som läggs på gaten i rött, i blått visas koncentrationen av acceptorer i det ljusgröna området. $d_{p}$ är 

När man lägger på en gatespänning som överstiger tröskelspänningen dras elektronerna mot oxidens (blå) yta. [[Elektronkoncentration\|Elektronkoncentrationen]] vid ytan ges av
$$n=n_{i}e^\frac{E_{F}-E_{i}}{hT}$$
och [[Hålkoncentration\|hålkoncentrationen]] av
$$p=n_{i}e^\frac{E_{i}-E_{F}}{hT}$$
där $E_{i}$ är den intrinsiska [[Ferminivå\|ferminivån]], $E_{F}$ är [[Ferminivå\|Ferminivån]], och $n_{i}$ är den intrinsiska [[Laddningsbärarkoncentration\|laddningsbärarkoncentrationen]].

När $E_{i}$ dras ned under $E_{F}$ pratar man om [[Svag Inversion\|svag inversion]] och [[Stark Inversion\|stark inversion]] (beroende på hur långt under $E_{F}$ man har dragit $E_{i}$)

## Linjära Området
$$U_{GS}-U_{TH}>U_{DS}$$
kallas linjärt för att det är linjärt i $U_{GS}$
$$I_{DS}=\frac{C_{ox}'Z \mu_{n}}{L}\left(\frac{(U_{GS}-U_{TH})U_{DS}-U_{DS}^{2}}{2}\right)$$

## Mättnadsområdet
$$U_{GS}-U_{TH}\leq U_{DS}$$
kallas mättnadsområdet för att det är mättat av $I_{DS}$.
$$I_{DS,sat}=\frac{C_{ox}'Z \mu_{n}}{L}\left(\frac{(U_{GS}-U_{TH})^2}{2}\right)$$
# Se också
[[Flatband-shift\|Flatband-shift]]
[[pMOSFET\|pMOSFET]]