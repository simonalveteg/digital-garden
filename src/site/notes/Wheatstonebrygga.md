---
{"dg-publish":true,"permalink":"/wheatstonebrygga/","tags":["mätteknik"]}
---

Har historiskt använts för resistansbestämning.
![wheatstonebrygga.png](/img/user/images/wheatstonebrygga.png)
$R_{1}$ och $R_{2}$ är fasta resistorer. $R_{x}$ är en okänd [[Resistans\|resistans]] som man vill mäta. När $R_{x}$ är inkopplad justerar man $R_{3}$ tills spänningen i A och B är lika, varpå $\frac{R_{1}}{R_{2}}=\frac{R_{3}}{R_{x}}$. 


Idag används wheatstonebryggan inte för resistansmätning av okända resistanser - man använder [[Multimeter\|multimeter]] istället. Används istället för utslagsmetoden.

## Utslagsmetoden
![wheatstonebrygga utslagsmetod.png](/img/user/images/wheatstonebrygga%20utslagsmetod.png)
Istället för att justera en [[Resistans\|resistans]] så att vi får noll spänning ut, så omvandlar vi en resistiv förändring till en spänning. Spänningar är väldigt enkla att ta hand  om och mäta. I [[Sensor and Transducer\|sensorer]] är det väldigt vanligt att en wheatstonebrygga är implementerad direkt.

Alla resistorer är fasta utom $R_{x}$, som är en [[Resistiva Givare\|resistiv givare]]. I grundtillståndet är den balanserad så att det inte är någon spänningsskillnad mellan A och B. När $R_{x}$ förändras kommer spänningen mellan A och B förändras. 

>Man omvandlar en resistiv förändring till en spänning, som är lätt att mäta

Man brukar behöva en [[Förstärkare\|förstärkare]] efter, då utspänningen är så liten.

