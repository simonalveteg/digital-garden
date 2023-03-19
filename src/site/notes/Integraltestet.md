---
{"dg-publish":true,"permalink":"/integraltestet/","tags":["funktionsteori"]}
---

Anta att $a_{n}=f(k)$ där $f$ är en positiv, avtagande funktion. Då är 
$$
\sum\limits_{k=n+1}^{m}a_{k} \geq \int_{n+1}^{m+1}f(x)dx
$$
det kan lätt bevisas grafiskt genom att rita ut den avtagande funktionen $f$
![integraltest serier.png|450](/img/user/images/integraltest%20serier.png)
om man summerar areorna av alla rektanglar blir det självklart större än integralen.

På precis samma sätt blir (rektanglarna är alltid under grafen)
$$\sum\limits_{k=n+1}^{m}a_{k}\leq \int_{n}^{m}f(x)dx$$
Sammanfattningsvis blir då 
$$\int_{n+1}^{m+1}f(x)dx \leq \sum\limits_{k=n+1}^{m}a_{k}\leq \int_{n}^{m}f(x)dx$$
summan $a_{k}$ blir då [[Konvergens\|konvergent]] om integralen är [[Konvergens\|konvergent]]. Integraler är lättare att lista ut.

Anta att $a_{k}=f(k)$ där $f$ är en positiv, avtagande funktion. Då är serien  $\sum\limits_{k=1}^{\infty}a_{k}$ [[Konvergens\|konvergent]] om och endast om $\int_{1}^{\infty}f(x)dx$ är [[Konvergens\|konvergent]]. Integraler kan vi beräkna! 

> Integraltestet används inte lika ofta som de andra testerna. Fungerar bäst som test för [[Serier\|serier]] som ligger väldigt nära gränsen mellan [[Konvergens\|konvergens]] och [[Divergens\|divergens]], de klarar man knappast med andra tester.

Viktigaste användingsområdet är att härleda [[P-Serier\|p-serier]]