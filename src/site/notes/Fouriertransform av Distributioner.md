---
{"dg-publish":true,"permalink":"/fouriertransform-av-distributioner/","tags":["systemochtransformer"]}
---


Vi vet att [[Distributioner\|distributioner]] går att derivera ([[Distributionsderivata\|Distributionsderivata]])

> $$<\mathcal{\widehat{U}},\varphi>=<\mathcal{U},\widehat{\varphi}>$$

För $f(t)\in L_{1}$ och $\varphi\in \mathcal{D}$ gäller
$$<\hat{f},\varphi> =\int_{-\infty}^{\infty}\hat{f}(w)\varphi(w)dw=\int_{-\infty}^{\infty}\left(\int_{-\infty}^{\infty}e^{-iwt}f(t)dt)\right)\varphi(w)dw$$
vilket kan skrivas om mha [[Fouriertransformationer\|fouriertransformen]] för $\varphi$
$$=\int_{-\infty}^{\infty}f(t)\widehat{\varphi}(t)dt=<f(t),\widehat{\varphi}>$$
vilket bevisar definitionen. 

