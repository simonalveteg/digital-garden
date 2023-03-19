---
{"dg-publish":true,"permalink":"/stoersta-vaerdet-av-stokastiska-variabler/","tags":["matematiskstatistik"]}
---

För att hitta största värdet av två [[Stokastisk Variabel\|stokastiska variabler]] kan man göra på följande sätt. Sätt $Z=max(X,Y)$. Eftersom $Z\leq z$ om och endast om både $X\leq z$ och $Y\leq z$ erhålls
$$
\begin{align}
F_Z(z)&=P(Z\leq z)=P(X\leq z \text{ och } Y\leq z) \\
&=P(X\leq z)P(Y\leq z)=F_X(z)F_Y(z)
\end{align}
$$


Samma princip kan användas för flera variabler.