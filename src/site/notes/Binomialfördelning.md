---
{"dg-publish":true,"permalink":"/binomialfoerdelning/","tags":["matematiskstatistik"]}
---

[[Sannolikhetsfunktion\|Sannolikhetsfunktionen]] är
$$
p_{X}(k)=\begin{pmatrix}
n \\
k\end{pmatrix}p^k(1-p)^{n-k}
$$
och [[Fördelningsfunktion\|fördelningsfunktionen]]
$$
F_X(k)=\sum\limits_{j=0}^{k}\begin{pmatrix}
n \\
j
\end{pmatrix} p^{j}(1-p)^{n-j}
$$


Man utför n stycken försök som har [[Sannolikhet\|sannolikhet]] p att lyckas och 1-p att misslyckas. Binomialfördelningen uppträder när antalet lyckade försök räknas vid oberoende upprepning av ett och samma försök. Har beteckningen $Bin(n,p)$.

Följande additionssats för binomialfördelningen gäller. Om $X\in Bin(n_{1},p)$ och $Y\in Bin(n_{2},p)$, där $X$ och $Y$ är oberoende, gäller att $X+Y\in Bin(n_{1}+n_{2},p)$.

se också → [[Binomialkoefficienten\|Binomialkoefficienten]]