---
{"dg-publish":true,"permalink":"/fourier-transform-of-aperiodic-signals/","tags":["digitalsignalbehandling"]}
---

To derive the [[Discrete-time Fourier transform\|Discrete-time Fourier transform]] ([[Discrete-time Fourier transform\|DTFT]]) of an aperiodic signal $x(n)$ we can 
1. Create a periodic signal $x_{p}(n)$ with period $N$ from a finite duration signal $x(n)$ as $$x_{p}(n)=\sum\limits_{k=-\infty}^{\infty}x(n-kN)$$
2. Represent $x_{p}(n)$ with its Fourier coefficients $$c_{k}=\frac{1}{N}\sum\limits_{n=0}^{N-1}x_{p}(n)e^{-j2 \pi k f_{0}n}$$
3. for "large enough" $N$ (no overlap between delayed copies of $x(n)$) $$c_{k}=\frac{1}{N}\sum\limits_{n=-\infty}^{\infty}x(n)e^{-j2 \pi kf_{0}n}$$
4. Define the Fourier transform of $x(n)$ as $$X(f)=\sum\limits_{n=-\infty}^{\infty}x(n)e^{-j2\pi fn}$$