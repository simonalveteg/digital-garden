---
{"dg-publish":true,"permalink":"/nedspaenningsomvandlare/","tags":["elenergiteknik"]}
---

Nedspänningsomvandlaren är en [[Enkvadrantomvandlare\|Enkvadrantomvandlare]] som kan accelerera/driva ($i>0$) en [[Likströmsmaskinen\|likströmsmaskin]] i en rotationsriktning ($u>0$). Styrs med [[OnOff Control Strategy\|till-från reglering]].

![Pasted image 20230206145348.png](/img/user/images/Pasted%20image%2020230206145348.png)
[[Induktans\|Induktansen]] är strömtrög, och används alltså för att "jämna ut" strömmen, så att den inte är en fyrkantsvåg som spänningen u. När [[Transistor\|transistorn]] kopplas från kommer strömmen att gå till noll (en oändligt stor negativ strömderivata). Det innebär att spänningen över [[Transistor\|transistorn]] hade gått mot oändligheten, vilket hade tagit sönder den. För att undvika den sätter man in en [[Diod\|diod]], som erbjuder strömmen en alternativ väg så att den inte går till noll direkt.

![Pasted image 20230208114215.png](/img/user/images/Pasted%20image%2020230208114215.png)

Strömmen varierar kring ett visst medelvärde och når aldrig noll. Avvikelsen från medelvärdet kallas **strömrippel**. Lasten är resistiv och spänningen över den kommer alltså få samma utseende (med rippel) vilket i många fall är oönskat. Genom att sätta in en [[Kapacitans\|kondensator]] parallellt med lasten kan man få rippledelen att flyta ned i den istället för lasten, vilket gör strömmen i lasten konstant.

![Pasted image 20230208114301.png](/img/user/images/Pasted%20image%2020230208114301.png)


Se också [[Uppspänningsomvandlare\|Uppspänningsomvandlare]]
[Boost Converters and Buck Converters: Power Electronics - YouTube](https://www.youtube.com/watch?v=vwJYIorz_Aw)