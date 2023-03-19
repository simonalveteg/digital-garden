---
{"dg-publish":true,"permalink":"/poission-foerdelning/","tags":["matematiskstatistik"]}
---

Poisson-fördelningen är en statistisk fördelning som används för att modellera antalet gånger som en [[Händelse\|händelse]] inträffar inom en given tidsperiod. Den används vanligen när frekvensen för [[Händelse\|händelsen]] är konstant och känd, och händelserna är oberoende av varandra. Den kan till exempel användas för att modellera antalet kunder som kommer till en affär under en timme eller antalet defekter i en tillverkningsprocess.
$$
P_{X}(k)=e^{-\mu}\frac{\mu^k}{k!}
$$
betecknas $X\in Po(\mu)$.

# Exakta egenskaper
Poisson-fördelningen uppträder även som approximation till [[Binomialfördelning\|binomialfördelningen]] och [[Hypergeometrisk Fördelning\|hypergeometriska fördelningen]].

Om den [[Stokastisk Variabel\|s.v.]] $X$ är poisson-fördelad gället att
$$
\begin{align}
E(X)&=\mu \\
V(X)&=\mu \\
D(X)&=\sqrt{ \mu }
\end{align}
$$
[[Väntevärde\|Väntevärde]], [[Varians\|Varians]], [[Standardavvikelse\|Standardavvikelse]].

Om $X\in Po(\mu_{1})$ och $Y\in Po(\mu_{2})$, där $X$ och $Y$ är [[Oberoende Stokastiska Variabler\|oberoende]], gäller att $X+Y\in Po(\mu_{1}+\mu_{2})$. 

# Approximativ egenskap
Poisson-fördelningen är lättare att hantera än [[Binomialfördelning\|binomialfördelningen]] och [[Hypergeometrisk Fördelning\|hypergeometriska fördelningen]] eftersom att den endast innehåller en parameter. Man har alltså inte lika stort behov av approximationer, men följande approximation är användbar.

För stora $\mu$ gäller ungefär att $X\in N(\mu,\sqrt{ \mu })$. Approximationen är ganska bra om $mu> \text{ca } 15$.