---
{"dg-publish":true,"permalink":"/seminarium-i-system-och-transformer-2022-05-03/","tags":["seminarium","systemochtransformer"]}
---



# [[Faltning\|Faltning]]
[[Faltning\|faltningen]] har samma egenskaper som mutiplikation mellan tal
$$\theta(t)*\theta(t)=t \theta(t)$$
[[Faltning\|faltning]] mellan två [[Kausala Funktioner\|kausala funktioner]]: ([[Kausal\|kausala]] då 0 för negativa t)
$$(f(t)\theta(t))*(g(t)\theta(t))=\theta(t)\int_{0}^{t}f(t-\tau)g(\tau)d \tau$$
$$f(t)*\delta(t)=f(t)$$
$$f(t)*\delta'(t)=(f(t)*\delta(t))'=f'(t)\delta(t)=f'(t)$$

# [[Distributioner\|Distributioner]]

$\delta$ och $\theta$ är två viktiga [[Distributioner\|distributioner]].

[[Distributioner\|distributioner]] kan betecknas på några olika sätt:
$$\mathcal{U}(\varphi)= <\mathcal{U},\varphi>=\int_{-\infty}^{\infty}\mathcal{U}(t)\varphi(t)dt$$
där $\varphi\in\mathcal{D}$ är en testfunktion. 

[[Distributioner\|distribution]] får inte multipliceras med en annan [[Distributioner\|distribution]]

Vissa [[Distributioner\|distributioner]] får fouriertransformeras (tempererade distributioner)
$$<\widehat{\mathcal{U}},\varphi>=<\mathcal{U},\widehat{\varphi}>$$

$$\theta_{a}'(t)=\delta_{a}$$
$$f(t)\delta_{a}(t)=f'(t)\delta(t-a)=f(a)\delta_a(t)$$
Om man vill integrera först uttrycket så blir det jobbiga partial integrationer, men om man kan förenkla till tredje uttrycket blir det mycket mycket lättare!


Uttrycket
$$f(t)\delta'(t)=(f(t)\delta(t))'-f'(t)\delta(t)=f(0)\delta'(t)-f'(0)\delta(t)$$
fås av produktregeln.

$$(f(t)\mathcal{U})'=f'(t)\mathcal{U}+f(t)\mathcal{U}'$$

# överföringsfunktion?
S är [[Linjära och Tidsinvarianta System\|LTI]] $\Rightarrow H(s) = \frac{S(e^{st})}{e^{st}}=\mathcal{L}(h(t))(s)$
[[Överföringsfunktion\|överföringsfunktionen]] ger laplacesvaret?





## Subject
[[FMAF05 System och Transformer\|FMAF05 System och Transformer]]
