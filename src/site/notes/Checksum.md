---
{"dg-publish":true,"permalink":"/checksum/","tags":["kommunikationssystem"]}
---

![checksum.png](/img/user/images/checksum.png)
Vi lägger till ett antal bitar på slutet, som genereras utav datan. 

För en fyra bitars checksum adderar man alla block av fyra bitar, och lägger till komplementet till slutet. Mottagaren summerar alla och får noll om det är rätt.

Används bland annat av [[IPv4\|IPv4]], [[TCP\|TCP]] och [[UDP\|UDP]], fast bara på deras header information. Det hade varit för långsamt att göra det på hela paketet.