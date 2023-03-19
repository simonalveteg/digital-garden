---
{"dg-publish":true,"permalink":"/discrete-time-sinusoids/","tags":["digitalsignalbehandling"]}
---

$$x(n)=Acos(\omega n+\theta)$$
$\omega$ = angular frequency (rad/sample), $n$ is an integer called the **sample number**
$$x(n)=Acos(2\pi fn+\theta)$$
$\omega=2\pi f$

The [[Discrete-time signals\|discrete-time signal]] is only periodic if its frequency is a rational number, since you need it to come back to the same integer over and over exactly which can only happen if the frequency is rational.

Discrete time sinusoids whose angular frequencies are separated by an integer multiple of $2\pi$ are identical. This is called [[Aliasing\|aliasing]]. Tänk dig att du går runt cirkeln, om vinkeln är större än $2\pi$ ser det ut som en mindre vinkel. 

The highest rate of oscillation in a disrete time sinusoid is attained when $\omega= \pm \pi$ (because of cosine)

$$- \frac{1}{2}<f<\frac{1}{2}$$
$$-\pi<\omega<\pi$$