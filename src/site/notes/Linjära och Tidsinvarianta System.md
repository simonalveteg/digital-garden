---
{"dg-publish":true,"permalink":"/linjaera-och-tidsinvarianta-system/","tags":["systemochtransformer"]}
---


[[System (matematisk definition)\|System (matematisk definition)]] som är både [[Linjära System\|linjära]] och [[Tidsinvarianta System\|tidsinvarianta]]. Ges av [[Faltning\|faltningen]] av [[Impulssvar\|impulssvar]] och insignal.

$$S(\delta(t))=h*\delta$$

Practically no real world systems are linear and time-invariant. 
> "Linear systems are important because we can solve them" 
> - Richard Feynman

But many systems can be approximated by LTI systems for small signals.

Ett linjärt tidsinvariant [[System (matematisk definition)\|System (matematisk definition)]] är [[Insignal-utsignalstabilt\|IU-stabilt]] om $\int_{-\infty}^{\infty}S|h(t)|dt<\infty$, dvs if it's [[Impulssvar\|impulse response]] is *absolutely summable*.

$S$ är LTI $\Leftrightarrow$ $S$ har [[Impulssvar\|impulssvaret]] $h(t)$. 
Dessutom gäller 
$$h(t)=S(\delta(t))=h*\delta=h*(\theta)'=(h*\theta)'=S(\theta(t))'$$ där $\delta$ är [[Delta Funktionen\|deltafunktionen]] och $\theta$ är [[Stegfunktion\|Stegfunktion]]. (* är [[Faltning\|Faltning]])

![lti block diagram.png](/img/user/images/lti%20block%20diagram.png)


## [[Kausala System\|Kausalt]]

> Ett LTI-system $S$ är **[[Kausala System\|kausalt]]** om [[Impulssvar\|impulssvaret]] $h(t)$ är en [[Kausala Funktioner\|kausal funktion]] och vice versa!

Ett kausalt LTI-system $w(t)\xrightarrow{S}y(t)$ ges genom 
$$\begin{cases} \begin{pmatrix}x_{1}(t) \\ x_{2}(t)\end{pmatrix}'=\begin{pmatrix} a_{1} & a_{2} \\ a_{2} & a_{4}\end{pmatrix}\begin{pmatrix}x_{1}(t) \\ x_{2}(t)\end{pmatrix}+\begin{pmatrix} b_{1} \\ b_{2}\end{pmatrix}w(t)\\ \\
y(t)=(c_{1},c_{2})\begin{pmatrix}x_{1}(t) \\ x_{2}(t)\end{pmatrix}  
\end{cases}$$
och har [[Impulssvar\|impulssvaret]] $h(t)=(Ce^{At}B)\theta(t)$ 

## [[Svängningar\|Svängningar]]
Om insignalen till ett linjärt tidsinvariant system är en komplex svängning med frekvens $s$, så är också utsignalen en komplex svängning med samma frekvens. Kvoten mellan utsignal och insignal är konstant i tiden, och systemets svar på en komplex svängning karakteriseras av ett enda komplext tal för varje frekvens. Det ger oss en [[Överföringsfunktion\|Överföringsfunktion]].