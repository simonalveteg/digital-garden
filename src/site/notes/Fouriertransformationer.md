---
{"dg-publish":true,"permalink":"/fouriertransformationer/","tags":["systemochtransformer"]}
---

Fouriertransformer kan användas för att studera stabila [[Linjära och Tidsinvarianta System\|LTI system]]. De kan också användas för att lösa [[Differentialekvationer\|differentialekvationer]]. Det är ett specialfall av [[Laplacetransformationer\|Laplacetransformationer]], när $s=iw$.

En  orsak till att studera fouriertransformationer är för att överföra [[Faltning\|faltning]] till multiplikation! (se [[Faltningssatsen\|Faltningssatsen]])

Fouriertransformen av funktionen $f(t)\in L_{1}$ är definierad genom
$$\mathcal{F}(f(t)(w)=\widehat{f(t)}(w)=\int_{-\infty}^{\infty}e^{-iwt}f(t)dt$$
för alla $w\in \mathbb{R}$.  

Man kan visa att $f\in L_{1} \Rightarrow \hat{f}$ är begränsad, kontinuerlig och $\lim_{|w|\rightarrow \rightarrow \infty}\widehat{f(w)}=0$

> Det är viktigt att kunna använda räknereglerna och standard-fouriertransformerna

Några standard fouriertransformer (står i formelbladet!)
![fouriertransform-regler.png](/img/user/images/fouriertransform-regler.png)

## Räkneregler

1.  $\widehat{c_{1}f_{1}(t)+c_{2}f_{2}(t)}(w)=c_{1}\widehat{f_{1}(t)}(w)+c_{2}\widehat{f_{2}(t)}(w)$  
 2. Skalning: $\widehat{f(at)}(w)=\frac{1}{|a|}\widehat{f(t)}(\frac{w}{a})$
 3. Förskjutning:
 $$\begin{cases}\widehat{f(t-a)}(w)=e^{-iwa}\widehat{f(t)}(w) \\
\widehat{e^{iat}f(t)}(w)=\widehat{f(t)}(w-a) \end{cases}$$
$t-a$ och $e^{-iwa}$ är ett par, dvs om vänsterled har den ena ska högerled ha den andra och vice versa.

4. Derivata
$$\begin{cases}\widehat{f'(t)}(w)=iw\widehat{f(t)}(w) \\
\widehat{tf(t)}(w)=i \frac{d}{dw}\widehat{f(t)}(w)\end{cases}$$
där derivatan och $iw$ är ett par. dvs om vänsterled har den ena ska högerled ha den andra och vice versa.

[[Invers Fouriertransformation\|Invers Fouriertransformation]]
