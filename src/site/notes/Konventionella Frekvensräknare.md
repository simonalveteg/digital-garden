---
{"dg-publish":true,"permalink":"/konventionella-frekvensraeknare/","tags":["mätteknik"]}
---

Den äldsta sortens [[Frekvensräknare\|frekvensräknare]]. Räknar antalet ingångscykler (N) under exakt en sekund. Sedan beräknar den frekvensen med $\frac{N}{1}(s^{-1})$. Detta blir fel då vi inte mäter tiden för helt antal perioder (som i definitionen för frekvens). Konventionella räknaren räknar antalet perioder under en sekund. Antalet perioder kanske inte blir ett heltal, vilket leder till upplösningsfel.
![konventionell frekvensmätning.png](/img/user/images/konventionell%20frekvensm%C3%A4tning.png)
Ju högre frekvens desto mindre andel av en period blir felet.

> **Mätosäkerheten** är $\pm1$ **ingångscykel**, eftersom insignalpulsen är totalt osynkroniserad med insignalen. När OCH-grinden öppnas eller stängs kan delar av perioden ibland räknas med och ibland inte.