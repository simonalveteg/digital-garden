---
{"dg-publish":true,"permalink":"/exponentiella-fourierserier/","tags":["funktionsteori"]}
---

Om vi antar att $f$ är [[Periodiska Funktioner\|T-periodisk]] och $L^{1}$ så ges funktionens exponentiella fourierserie av 
$$\mathcal{FS}_{f}(t)=\sum\limits_{k=-\infty}^{\infty}c_{k}e^{ik\Omega t}$$
där [[Konvergens\|konvergensen]] av [[Funktionsserier\|funktionsserien]] är [[Likformig konvergens\|likformig]] och $\Omega T = 2\pi$. $c_{k}$ kallas funktionens **exponentiella Fourierkoefficienter** som kan beräknas med
$$c_{k}=\frac{1}{T}\int_{P}f(t)e^{-ik\Omega t}dt$$

> Fourierkoefficienten beskriver alltså fourierseriens utseende typ

obs: $FS_{f}$ behöver inte [[Konvergens\|konvergera]], och även om den [[Konvergens\|konvergerar]] behöver summan inte vara $f(t)$. $c_{0}$ är medelvärdet av $f$ över intervallet $[0,T)$ och ges av 
$$c_{0}=\frac{1}{T}\int_{P}f(t)dt$$
___
Om $f : I\rightarrow\mathbb{C}$ där $I$ är ett intervall på $\mathbb{R}$, så kallas $f$ [[Absolut Integrerbar\|absolut integrerbar]] eller $L^{1}$ om
$$\int_{I}|f(t)|dt<\infty$$
[[Periodiska Funktioner\|Periodiska funktioner]] kallas $L^{1}$ om de är $L^{1}$ på ett intervall som motsvarar *en* period.

## Räkneregler för Fourierkoefficienter
Anta att $f$, $g$, är [[Periodiska Funktioner\|T-periodiska]] och $L^{1}$ och låt $c_{k}(f)$ beteckna koefficienterna för $f$. Då gäller
1. $c_{k}(f+g)=c_{k}(f)+c_{k}(g)$ och  $c_{k}(\alpha f)=\alpha c_{k}(f)$ (linjäritet)
2. $c_{k}(f')=ik\Omega c_{k}(f)$ alltså $f$ deriverbar 
3. $c_{k}(f(t-\tau))=e^{-ik\Omega\tau}c_{k}(f)$ 
 3.  $c_{k}(e^{im\Omega t}f(t))=c_{k-m}(f)$ där $m\in\mathbb{Z}$

```ad-Bevis
title: härledning av $c_{k}$
collapse: closed
Om vi multiplicerar båda sidor av den exponentiella fourierserien med $e^{-in\Omega T}$ och integrerar över en period
$$
\int_{P}f(t)e^{-in\Omega T}dt=\int_{P}\left(\sum\limits_{k=-\infty}^{\infty}c_{k}e^{i(k-n)\Omega t}dt\right)=\sum\limits_{k=-\infty}^{\infty}c_{k}\int_{P}e^{-i(k-n)\Omega T}
$$
om $n=k$ blir det
$$\int_{P}e^{-i(k-n)\Omega T}dt=\int_{P}1dt=T$$
annars blir det
$$\int_{P}e^{-i(k-n)\Omega T}dt=\left[\frac{e^{-i(k-n)\Omega T}}{i(k-n)}\right]_{0}^{T}=0$$
eftersom primitiven är periodisk med period T. Slutsatsen blir att
$$\int_{P}f(t)e^{-in\Omega T}dt=Tc_{n}\Rightarrow c_{n}=\frac{1}{T}\int_{P}f(t)e^{-in\Omega T}dt$$
```
```ad-Bevis
title: samband med [[trigonometriska Fourierserier]]
collapse: closed

Detta är **härledningen** som ger upphov till den trigonometriska tolkningen av [[Fourierserier]].

Vi tar en symmetrisk partiasumma av vår exponentiella Fourierserie
$$
\sum\limits_{k=-N}^{N}c_{k}e^{ik\Omega t} + c_{0} + \sum\limits_{k=1}^{N}c_{k}e^{ik\Omega t}= 
$$
vi utför variabelbytet $n=-k$ för den vänstra delsumman, vilket ger $n: 1 \rightarrow N$
$$
= \sum\limits_{n=1}^{N}c_{-k}e^{-in\Omega t}+c_{o}+\sum\limits_{k=1}^{N}c_{k}e^{ik\Omega t}=c_{0}+\sum\limits_{k=1}^{N}(c_{-k}e^{-ik\Omega t}+c_{k}e^{ik\Omega t})=
$$
$$
= c_{0}+\sum\limits_{k=1}^{N}\left[(c_{k}+c_{-k})cos(k\Omega t)+i(c_{k}-c_{-k})sin(k\Omega t)\right] = c_{0}+\sum\limits_{k=1}^{N}[a_{k}cos(k\Omega t)+b_{k}sin(k\Omega t)]
$$

```
