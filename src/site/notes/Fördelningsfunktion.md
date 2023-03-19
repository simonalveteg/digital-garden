---
{"dg-publish":true,"permalink":"/foerdelningsfunktion/","tags":["matematiskstatistik"]}
---

Givet en [[Stokastisk Variabel\|Stokastisk Variabel]] $X$ definierar vi dess fördelningsfunktion som $$
F_{X}(x)=P(\left\{ \omega:X(\omega)\leq x \right\} )
$$
![Pasted image 20221101145223.png|250](/img/user/images/Pasted%20image%2020221101145223.png)

För en fördelningsfunktion $F_X(x)$ gäller att 
1. $$
F_X(x) \rightarrow \begin{cases}
0 & \text{då } x \rightarrow-\infty \\
1 & \text{då } x \rightarrow+\infty
\end{cases}$$ 
2. $F_X(x)$ är en icke-avtagande funktion av $x$
3. $F_X(x)$ är kontinuerlig till höger för varje $x$.

Varje funktion som uppfyller villkoren ovan är en fördelningsfunktion för någon [[Stokastisk Variabel\|Stokastisk Variabel]].

> Om $a<b$ gäller att $$
P(a)<X\leq b)=F_X(b)-F_X(a)$$

[[Flerdimensionell Fördelningsfunktion\|Flerdimensionell Fördelningsfunktion]]