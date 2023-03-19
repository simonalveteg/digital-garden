---
{"dg-publish":true,"permalink":"/faltning/","tags":["systemochtransformer"]}
---

![faltning2.gif](/img/user/images/faltning2.gif)
![faltning1.gif](/img/user/images/faltning1.gif)
Innebär att en ny integrerbar summafunktion kan bildas av två andra integrerbara funktioner. Den ena arean “dras” genom den andra, och faltningen blir arean under grafen som fås av produkten av funktionerna i olika tidpunkter.
$$(f*g)(t)=(g*f)(t)=\int_{-\infty}^{\infty}f(t-\tau)g(\tau)d \tau=\int_{-\infty}^{\infty}g(t-\tau)f(\tau)d \tau$$
om integralen existerar (dvs är [[Konvergens\|konvergent]]) kallas den för **faltningen** av $f$ och $g$. 

> Att beräkna en faltning innebär att bestämma värdet av oändligt många generaliserade integraler, därför förenklar vi beräkningarna så myket som möjligt.

Allmänt gäller 
$$(f(t)\theta(t))*(g(t)\theta(t))=\theta(t)(f(t)*g(t))=\theta(t)\int_{0}^{t}f(t-\tau)g(\tau)d \tau$$
då $\theta(t)$ är [[Stegfunktion\|Stegfunktion]] (alltså en [[Kausala Funktioner\|kausal funktion]]). Man bryter **inte** ut $\theta$, men det är ett sätt att komma ihåg funktionen på. 

Alla funktioner får inte faltas!
1. om $f(t)$ och $g(t)$ är [[Absolut Integrerbar\|absolut integrerbara]] så existerar faltningen, och är [[Absolut Integrerbar\|absolut integrerbar]]!
2. om $f(t),g(t)$ är [[Kausala Funktioner\|kausala]] och kontinuerliga då $t>0$ existerar faltningen och är [[Kausala Funktioner\|kausal]].
basically: två [[Absolut Integrerbar\|absolut integrerbara]] funktioner får faltas, och två [[Kausala Funktioner\|kausala funktioner]] får faltas. 

> Om $f(t),g(t)$ är [[Kausal\|kausala]] så är $f*g$ [[Kausal\|kausal]]!


## Räkneregler
Nästan samma egenskaper som produkt mellan tal! man kan tolka det som multiplikation när man förenklar och håller på
$$f*g=g*f$$
$$f*(g+h)=f*g+f*h$$
$$f*(g*h)=(f*g)*h$$
i följande fall fungerar det inte som multplikation!
$$(f*g)'=f'*g=f*g'$$
$$T_{a}(f*g)=(T_{a}f)*g=(T_{a}g)*f$$
$T_{a}$ = [[Förflyttningsfunktionen\|förflyttningsfunktionen]]

## Beräkning
Vid direkt beräkning av faltningsintegraler, där faktorerna innehåller [[Stegfunktion\|stegfunktioner]] måste man dela upp området i delintervall! 


Bra videor:
[Convolutions are not Convoluted - YouTube](https://www.youtube.com/watch?v=aEGboJxmq-w)
[How Convolution Works - YouTube](https://www.youtube.com/watch?v=B-M5q51U8SM)

See also → [[Convolution of Discrete Signals\|Convolution of Discrete Signals]]