---
{"dg-publish":true,"permalink":"/potensserier/","tags":["funktionsteori"]}
---

Potensserier är [[Serier\|Serier]] på formen
$$\sum\limits_{k=0}^{\infty}a_{k}(z-c)^{k}=a_{0}+a_{1}(z-c)+a_{2}(z-c)^{2}+\space...$$
där $a_{k},z,c\subset\mathbb{C}$.

Alla potensserier uppför sig på liknande sätt! [[Konvergens\|Konvergerar]] mot en cirkelskiva och divergerar utanför cirkelskivan

![potensserier.png|400](/img/user/images/potensserier.png)

 Kan grafiskt ses som en cirkel, och medan man befinner sig **inom** denna cirkel är potensserien **[[Konvergens\|konvergent]]**. Detta kallas **konvergenscirkel**

> Man karakteriserar konvergenscirkelns storlek genom en radie, betecknad R, som kallas **[[Konvergensradie\|konvergensradie]]**, och är alltså en **längd** (ett tal)

 Serien är **centrerad** i c. Det är från denna punkt man mäter [[Konvergensradie\|konvergensradien]]

Serien [[Absolut Konvergent\|konvergerar absolut]] om $|z-c|<R$. 
Serien [[Divergens\|divergerar]] om $|z-c|>R$
Serien [[Likformig konvergens\|konvergerar likformigt]] på varje disk $|z-x|\leq r$, ${r<R}$ 

(om $|z-c|=R$ kan det hända vad som helst)

> När man ska avgöra [[Konvergens\|konvergens]] för potensserier ger [[d’Alemberts kvottest\|d’Alemberts kvottest]] och [[Cauchys rottest\|Cauchys rottest]] bra resultat

> Konvergenta potensserier kan integreras och deriveras termvis utan att ändra [[Konvergensradie\|konvergensradien]]

dvs om
$$f(z)=\sum\limits_{k=0}^{\infty}a_{k}(z-c)^{k}$$
för $|z-c|<R$. Så är 
1. $F(z)=\sum\limits_{k=0}^{\infty}a_{k}\frac{(z-c)^{k+1}}{k+1}=\sum\limits_{k=1}^{\infty}a_{k+1}\frac{(z-c)^{k}}{k}$ en primitiv funktion till $f$
2. $f'(z)=\sum\limits_{k=1}^{\infty}ka_{k}(z-c)^{k-1}=\sum\limits_{k=0}^{\infty}(k+1)a_{k+1}(z-c)^{k}$

## Potensserieutveckling
[[Maclaurinutveckling\|Maclaurinutvecklingar]] och [[Taylorutveckling\|Taylorutvecklingar]] är två vanliga typer av potensserieutvecklingar

### Konsekvenser av potensserieutveckling
[[Entydighetssatsen för holomorfa funktioner\|Entydighetssatsen för holomorfa funktioner]]
[[Faktorsatsen för holomorfa funktioner\|Faktorsatsen för holomorfa funktioner]]

