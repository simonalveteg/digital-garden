---
{"dg-publish":true,"permalink":"/discrete-time-fourier-transform/","tags":["digitalsignalbehandling"]}
---


The DTFT is the [[Z-transform\|z-transform]] evaluated on the unit circle (if the unit circle is inside the [[Region of convergence\|ROC]]), if the [[Impulssvar\|impulse response]] is [[Kausal\|causal]] and [[Stabila och Instabila System\|stable]]. 

for discrete-time aperiodic signals we can use the definition of the discrete-time [[Fouriertransformationer\|fourier transform]] $$X(f)=\sum\limits_{n=-\infty}^{\infty}x(n)e^{-j2 \pi fn} \Rightarrow X(\omega)=\sum\limits_{n=-\infty}^{\infty}x(n)e^{-j \omega n}$$
and the fourier-series coeficients $$c_{k}=\frac{1}{N}\sum\limits_{n=-\infty}^{\infty}x(n)e^{-j2\pi kf_{0}n}=\frac{1}{N} X(kf_{0})$$
> Take the [[Z-transform\|z-transform]] and replace $z$ with $e^{j \omega}$.

[[Fourier transform of aperiodic signals\|Fourier transform of aperiodic signals]]
[[Fourier series of periodic signals\|Fourier series of periodic signals]]
[[Invers Fouriertransformation\|Inverse fourier transform]]
[[DTFT symmetry properties\|DTFT symmetry properties]]
[[DTFT properties\|DTFT properties]]
[[DTFT transform pairs\|DTFT transform pairs]]