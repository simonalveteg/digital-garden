---
{"dg-publish":true,"permalink":"/stegfunktion/","tags":["systemochtransformer"]}
---

Genom att subtrahera en stegfunktion från en annan får man fram bara ett intervall typ? $\theta_{2}(t)-\theta_{4}(t)$ är noll överallt förutom mellan 2 och 4 där den är 1. Om man har en funktion som defineras olika för olika intervall, ex $f(t)=t$ för 0-1 sint för 1-5 osv, så kan man skriva upp funktionen som en summa av enhetsstegsfunktioner

derivatan av en stegfunktion är en [[Delta Funktionen\|deltafunktion]].

Stegfunktioner kan användas för att ersätta integrationsgränser. T.ex
$$\int_{-\infty}^{\infty}\theta(t)f(\tau)d \tau=\int_{0}^{\infty}f(\tau)d \tau$$

## Enhetsstegfunktionen
grundfallet
$$\theta(t)=\begin{cases}0\space,\space t<0\\\\1 \space,\space t>0 \end{cases}$$
$$\theta_{a}(t)=\theta(t-a)=T_{a}(\theta(t))$$, dvs ett [[Enhetssteg\|Enhetssteg]] i punkten a, noll till vänster om a och 1 till höger om a. $T_{a}$ kallas operator, som avbildar “funktionen på funktionen?”
