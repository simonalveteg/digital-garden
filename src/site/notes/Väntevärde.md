---
{"dg-publish":true,"permalink":"/vaentevaerde/","tags":["matematiskstatistik"]}
---

Väntevärde är i princip samma sak som [medelvärde](https://dataverktyg.se/medelvarde-median) och beräknas på samma sätt. Skillnaden är att väntevärde används för att beskriva _slumpvariabler_ ([[Stokastisk Variabel\|stokastiska variabler]]). Väntevärdet är det genomsnittliga värde (medelvärdet) som man kan förvänta sig att få om man gör ett stort antal slumpmässiga försök.

> Väntevärdet är ett [[Lägesmått\|Lägesmått]] som ger upplysning om var massan är belägen "i genomsnitt".

Väntevärdet för den [[Stokastisk Variabel\|stokastiska variabeln]] $X$ definieras av
$$
E(X)=\begin{cases}
\sum\limits_k kp_X(k) & \text{(diskret s.v.)} \\
\int\limits_{-\infty}^{\infty} xf_X \, dx & \text{(kontinuerlig s.v.)} 
\end{cases}
$$

Väntevärdet för en funktion $Y=g(X)$ av en [[Stokastisk Variabel\|stokastisk variabel]] $X$ är
$$
E(Y)=\begin{cases}
\sum\limits_k g(k)p_X(k) & \text{diskret s.v.} \\
\int\limits_{-\infty}^{\infty} g(x)f_Xdx  &  \text{kontinuerlig s.v.}
\end{cases}
$$
Väntevärdet för en funktion av flera [[Stokastisk Variabel\|stokastiska variabler]]
$$
E(Z)=\begin{cases}
\sum\limits_{j,k} g(j,k)p_{X,Y}(j,k) & \text{diskret s.v.} \\
\iint\limits_{-\infty}^{\infty} g(x,y)f_{X,Y}(x,y)dx  &  \text{kontinuerlig s.v.}
\end{cases}
$$



<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/vaentevaerdesbildningens-linjaeritet/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




Om $X$ och $Y$ är [[Stokastisk Variabel\|stokastiska variabler]] med [[Väntevärde\|väntevärden]] $E(X)$ och $E(Y)$ och om $a,b,c$ är konstanter så gäller att
$
E(aX+bY+c)=aE(X)+bE(Y)+c
$


</div></div>


Om $X$ och $Y$ är [[Oberoende Stokastiska Variabler\|oberoende]] gället att
$$
E(XY)=E(X)E(Y).
$$
Om $X_{1},X_{2}X_{3},\dots,X_n$ är [[Oberoende Stokastiska Variabler\|Oberoende Stokastiska Variabler]] gäller
$$
E(X_{1}X_{2}\dots X_n)=E(X_{1})E(X_{2})\dots E(X_n).
$$
