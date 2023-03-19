---
{"dg-publish":true,"permalink":"/faelteffekttransistor/","tags":["komponentfysik","analogelektronik"]}
---

Metal Oxide Semiconductor Field Effect [[Transistor\|Transistor]]
![nMOS fälteffekttransistor.png](/img/user/images/nMOS%20f%C3%A4lteffekttransistor.png)
$V_{GS}$ måste vara högre än tröskelspänningen $V_{TH}$ för att det ska gå en ström $I_{DS}$ genom [[Transistor\|transistorn]].
![mos.png](/img/user/images/mos.png)
en [[nMOSFET\|nMOS]] [[Transistor\|transistor]] har en [[Dopning\|p-typ]] [[Halvledare\|halvledare]]. Det finns alltså en jävla massa hål, men varje hål kommer från en acceptor - som har en proton mindre och alltså ger upphov till negativa laddningar. När man lägger på en spänning på gaten repelleras hålen, vilket skapar ett negativt laddat område - **[[Utarmningsområdet\|utarmningsområde]]** ([[Utarmningsområdet\|depletion region]]) som är tömt på rörliga laddningar. De få elektroner som finns kommer hopas i [[Utarmningsområdet\|utarmningsområdet]], och dess laddning ges av $Q_{n}=C_{ox}(U_{GS}-U_{TH})$.
![MOStransistor.png](/img/user/images/MOStransistor.png)
När man lägger på en spänning $V_{DS}$ får man elektronerna i [[Utarmningsområdet\|utarmningsområdet]] att röra sig, vilket skapar strömmen $I_{DS}$! [[Strömtäthet\|Strömtätheten]] för kanalen av elektroner ges av 
$$J=en \frac{\mu}{n}\mathcal{E}$$
det elektriska fältet ges av
$$\mathcal{E}=\frac{U_{DS}}{L_{g}}$$
vilket ger 
$$J=\frac{Zh}{L_{g}}en \mu_{n}U_{DS}$$
där $L_{g}$ är längden på kanalen, $Z$ är dess bredd, $h$ dess tjocklek och $n$ är koncentrationen. Om man ökar $U_{GS}$ kommer koncentrationen av elektroner att öka, vilket ökar [[Strömtäthet\|strömtätheten]] (ledningsförmågan).

Tröskelspänning - koncentrationen av elektroner i [[Utarmningsområdet\|utarmningsområdet]] är lika hög som koncentrationen av acceptorer. 


Source och Drain n-dopas så att det finns gott om elektroner. Följande [[Banddiagram\|Banddiagram]] kan ritas upp
![mosfet-banddiagram.png](/img/user/images/mosfet-banddiagram.png)
där Gate-spänningen indikeras av det gråa rätblocket. Energinivån på elektronerna kan ses som en vattennivå, och transistorns olika lägen kan beskrivas av hur vattnet flödar. 

## Strypd mod
![mosfet strypt.png](/img/user/images/mosfet%20strypt.png)
$$V_{GS} < V_t$$ Strömmen kan inte ta sig från source till drain.

![Pasted image 20220117140430.png](/img/user/images/Pasted%20image%2020220117140430.png)
$$V_{GS}>V_t$$
Genom att öka gatespänningen över tröskelspänningen kan en ström börja gå från source till drain
## Mättnadsområdet
Mättnadsområdet kan lätt förstås med vattenanalogen
![Pasted image 20220117140633.png](/img/user/images/Pasted%20image%2020220117140633.png)
oavsett hur mycket man ökar drain-spänningen kommer det inte påverka hur mycket ström som flödar från source till drain.
$$V_{DS} > V_t - V_{GS}$$
$I_d$ oberoende av $V_{GS}$

## Linjära området
![linjärt område mosfet.png](/img/user/images/linj%C3%A4rt%20omr%C3%A5de%20mosfet.png)
$$V_{DS} > V_t - V_{GS}$$
$I_d$ beror av $V_{DS}$ . Strömmen ökar med drainspänningen i det linjära området.

[[nMOSFET\|nMOSFET]]
[[pMOSFET\|pMOSFET]]