---
{"dg-publish":true,"permalink":"/delta-funktionen/","tags":["systemochtransformer"]}
---


Kallas också **impulsfunktionen**!

Delta funktionen har integralen noll överallt utom i origo, där den har positiv massa 1. Dvs när man tar integralen av en delta funktion behöver man bara ta integralen i origo. 

Det följer att
$$\int_{-\infty}^{\infty}f(t) \delta(t)dt)=\int_{\{0\}}f(t) \delta(t)dt=f(0)\int_{\{0\}}\delta(t)dt=f(0)$$
dvs, om man tar integralen av en funktion $f$ multiplicerat med delta funktionen, så får man värdet av $f(0)$.

Om man multiplicerar deltafunktionen med en annan funktion får man deltafunktionen gånger värdet av den andra funktionen i 0? #question


Vi definerar
$$\delta_{a}(t)=\delta(t-a)$$
vilket analogt till ovan ger
$$\int_{-\infty}^{\infty}f(t)\delta_{a}(t)dt=\int_{-\infty}^{\infty}f(t)\delta(t-a)dt=f(a)\int_{-\infty}^{\infty}\delta(t-a)dt=f(a)$$
för vanlig funktion $f(x)$.

Om $f$ är en trillräckligt regulär funktion som är minst en gång kontinuerligt deriverbar, så kan $f$ multipliceras med $\delta'$ och produkten kan skrivas om som
$$f(t)\delta'(t)=f(0)\delta'(t)-f'(0)\delta(t)$$



se också [[Stegfunktion\|Stegfunktion]], [[Kronecker delta function\|Kronecker delta function]]
