---
{"dg-publish":true,"permalink":"/handpalaeggningsmetoden-foer-partialbraksuppdelning/","tags":["systemochtransformer"]}
---

säg att vi har uttrycket
$$\frac{s^{2}+5s+1}{s(s+4)(s+1)}$$
och vill partialbråksuppdela skiten på vanligt sätt
$$\frac{s^{2}+5s+1}{s(s+4)(s+1)}=\frac{A}{s}+ \frac{B}{s+4}+ \frac{C}{s+1}$$
med handpåläggning blir detta superlätt verkligen.
$$A=\left.\frac{s^{2}+5s+1}{(s+4)(s+1)}\right|_{s=0}$$
$$B=\left.\frac{s^{2}+5s+1}{s(s+1)}\right|_{s=-4}$$
$$C=\left.\frac{s^{2}+5s+1}{s(s+4)}\right|_{s=-1}$$
Man tar alltså vänsterledet, tar bort den del av nämnaren som ens konstant berör, och sätter $s=a$ där a är den relevanta polen.

## Dubbelrot
Om det är en dubbelrot i $(s+1)^{2}$, så blir det som vanligt
$$\frac{1}{s+1}+ \frac{1}{(s+1)^{2}}$$
för den högra är det exakt som vanligt med handpåläggning enligt ovan, men för den vänstra tar man istället derivatan innan man sätter in värdet på s.