---
{"dg-publish":true,"permalink":"/inversionsformeln-foer-fouriertransformationer/","tags":["systemochtransformer"]}
---


Om $f$ och $\hat{f}$ är kontinuerliga funktioner i $L_{1}$ ([[Absolut Integrerbar\|absolut integrerbar]]? #question), så är 
$$f(t)=\frac{1}{2 \pi}\int_{-\infty}^{\infty}e^{iwt}F(w)dw = \mathcal{F}^{-1}(F(w))(t)$$
för alla t, förutsatt att $F$ också är $L_{1}$. $\hat{f}(w)=F(w)$.

det följer att $$\frac{1}{2\pi}F(-w)\xrightarrow{\mathcal{F}} f(t) \xrightarrow{\mathcal{F}}F(w)\xrightarrow{\mathcal{F}}2\pi f(-t)$$(om man går åt motsatt håll mot pilarna utför man en [[Invers Fouriertransformation\|invers fouriertransformation]])
1. $\widehat{\widehat{f(t)}}=2\pi f(-t)$
2. $\mathcal{F}^{-1}(F(w))(t)=\frac{1}{2\pi}\mathcal{F}(F(w))(-t)$


  ## Se också
  [[Inversionsformeln\|Inversionsformeln]]

