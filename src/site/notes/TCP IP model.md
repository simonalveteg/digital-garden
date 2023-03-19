---
{"dg-publish":true,"permalink":"/tcp-ip-model/","tags":["kommunikationssystem"]}
---

- [[Application Layer\|Application Layer]]  (L5-L7)
- [[Transportprotokoll\|Transport Layer]] (L4)
- [[Network Layer\|Internet Layer]] (L3)
- Link/Network Interface Layer(L1-L2)

the language of L1-L7 has stuck around, so we have a four layer model with seven layer names..
![Pasted image 20230116193222.png](/img/user/images/Pasted%20image%2020230116193222.png)

TCP/IP definierar inte de lägsta två lagren. Det innebär att ett datagram kan passera ett antal olika nät från sändare till mottagare med sin aegna länkprotokoll och ramformat. Olika länkprotokoll har olika maxlängd på sina ramar - kallad [[Maximum Transfer Unit\|Maximum Transfer Unit]] ([[Maximum Transfer Unit\|MTU]]). Datagrammets längd får inte vara längre än [[Maximum Transfer Unit\|MTU]], och måste i så fall [[Fragmentering\|fragmenteras]] innan det skickas ut på länken.

Nackdelen med TCP/IP modellen är att varje lager bidrar med sin egen overhead (i form av en header). Det är mindre effektivt än en cross-layer approach.