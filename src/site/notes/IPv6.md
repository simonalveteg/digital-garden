---
{"dg-publish":true,"permalink":"/i-pv6/","tags":["kommunikationssystem"]}
---

IPv6 tillåter inte [[Fragmentering\|Fragmentering]]. Sändaren måste därför veta vilken som är den minsta [[Maximum Transfer Unit\|MTU:n]] på vägen till mottagaren, det tar den reda på med *path [[Maximum Transfer Unit\|MTU]] discovery technique*. Fragmentering är en tidskrävande procedur, och i IPv6 vill man ha ett så effektivt [[Network Layer\|nätprotokoll]] som möjligt.