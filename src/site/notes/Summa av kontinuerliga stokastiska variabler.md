---
{"dg-publish":true,"permalink":"/summa-av-kontinuerliga-stokastiska-variabler/","tags":["matematiskstatistik"]}
---

Om $X,Y$ är [[Kontinuerliga Stokastiska Variabler\|Kontinuerliga Stokastiska Variabler]] får vi [[Fördelningsfunktion\|fördelningsfunktionen]] för $Z$ genom att integrera den [[Simultana Täthetsfunktionen\|Simultana Täthetsfunktionen]] $f_{X,Y}(x,y)$ över området $A_z=\left\{ (x,y):x+y\leq z \right\}$
$$
F_Z(z)=P(X+Y\leq z)=P((X,Y)\in A_z)=\iint_{x+y \leq z}f_{X,Y}(x,y)\,dxdy
$$

Om $X$ och $Y$ är [[Oberoende Stokastiska Variabler\|oberoende]] erhålls
$$
\begin{align}
F_Z(z)&=\iint_{x+y\leq z}f_X(x)f_Y(y)\,dxdy \\
&=\int\limits_{-\infty}^{\infty} f_X(x) \, \left( \int\limits_{-\infty}^{z-x} f_Y(y) \, dy \right)dx=\int\limits_{-\infty}^{\infty} f_X(x)f_Y(z-x) \, d  x
\end{align}
$$

Genom derivering med avseende på $z$ får man [[Faltningsformeln för oberoende kontinuerliga stokastiska variabler\|Faltningsformeln för oberoende kontinuerliga stokastiska variabler]]