---
{"dg-publish":true,"permalink":"/bit-stuffing/","tags":["kommunikationssystem"]}
---

Om man har en flagga som är 01111110 behöver vi undvika att payloaden innehåller 6 ettor på rad. I sändaren sätter man då in en nolla efter 5 ettor, och i mottagaren tar man bort den bit som följer efter 5 ettor.
![bit stuffing.png](/img/user/images/bit%20stuffing.png)