---
{"dg-publish":true,"permalink":"/interpolerande-frekvensraeknare/","tags":["mätteknik"]}
---

Interpolerande [[Frekvensräknare\|frekvensräknare]] bygger på reciprok [[Mätteknik\|mätteknik]]. I en interpolatorkrets bestämmer man fasläget för klockpulsen vid mätningens start respektive stopp. Man har två identiska interpolatorer i drift samtidigt, en för mätstarten oh en för mätstoppet. Mätningen startar synkront med att insignalen triggar räknarens ingång (samtidigt som uppladdningen av en [[Kapacitans\|kondensator]] med en konstant ström). Spänningen över kondesnatorn växer linjärt med tiden och uppladdningen avbryts då positiv klockflank nr 2 efter insignaltriggningen kommer.

När den interpolerande räknaren är klar får vi följande delresultat:
antalet hela ingångscykler (N)
antalet digitalt räknade klockpulser ($T_{n}$) med 100ns upplösning
den analoga kondensatorspänningen i startinterpolatorn
den analoga kondensatorspänningen i stoppinterpolatorn

![interpolerande räknare.png](/img/user/images/interpolerande%20r%C3%A4knare.png)