---
{"dg-publish":true,"permalink":"/minsta-vaerdet-av-stokastiska-variabler/","tags":["matematiskstatistik"]}
---

För att hitta minsta värdet av två [[Stokastisk Variabel\|stokastiska variabler]] kan man göra på följande sätt. Sätt $Z=min(X,Y)$. Eftersom $Z> z$ om och endast om både $X> z$ och $Y>z$ erhålls
$$
\begin{align}
F_Z(z)&=P(Z\leq z)=1-P(Z>z)=1-P(X>Z \text{ och }Y>z)\\ \\
&=1-P(X>z)P(Y>z)
\end{align}
$$
Men $P(X>z)=1-P(X\leq z)=1-F_X(z)$ och analogt för $Y$. Alltså får man till sist
$$
F_Z(z)=1-(1-F_X(z))(1-F_Y(z)).
$$


Samma princip kan användas för flera variabler.