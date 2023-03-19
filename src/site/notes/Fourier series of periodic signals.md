---
{"dg-publish":true,"permalink":"/fourier-series-of-periodic-signals/","tags":["digitalsignalbehandling"]}
---

A [[Discrete-time signals\|discrete-time signal]] has the property $x(n)=x(n+N)$ and a fundamental frequency $f_{0}=\frac{1}{N}$ (cycles/sample) and can be written as a discrete-time Fourier series (DTFS)
$$x(n)=\sum\limits_{k=0}^{N-1}c_{k}e^{j2 \pi k f_{0}n}$$
also called the *synthesis equation*. The Fourier coefficients are
$$c_{k}=\frac{1}{N}\sum\limits_{n=0}^{N-1}x(n)e^{-j2 \pi k f_{0}n}$$
which is called the *analysis equation*. The coefficients are called the *spectrum* of the [[Signal\|signal]]. In this case (discrete-time) the fourier coefficients are also periodic with the same period as the [[Signal\|signal]] itself. But only $N$ coefficients are needed to completely characterize the periodic signal.

For real signals $c_{-k}=c_{k}^{*}$ (the complex conjugate).



If you have any [[Signal\|signal]] the product of the [[Bandbredd\|bandwidth]] and the time extension of the pulse can never be smaller than $\frac{1}{2}$. 

See also → [[Fourierserier\|fourier series]]