---
{"dg-publish":true,"permalink":"/phasors/","tags":["elektromagnetiskfältteori"]}
---

In electrical engineering, we often deal with periodic signals as expressed sinusoidal functions. [[Maxwell's Equations\|Maxwell's Equations]] are linear [[Differentialekvationer\|differential equations]], so sinusoidal source functions of a given frequency will result in [[Electric Field\|Electric Field]] and [[Magnetic Field Intensity\|Magnetic Field Intensity]] with the same frequency at steady state.

Since any periodic signals in the time domain can be decomposed into its components via the [[Fourierserier\|fourier series]] we can solve the problem of arbitrary periodic signals by solving for the sinusoidal components and then combining the solutions with [[Superposition\|Superposition]].

If a signal is $i(t)=I\cos(\omega t+\phi)$ where the angular frequency $\omega=2\pi f$, then it can be written as
$$
i(t)=Re(Ie^{ j(\omega t+\phi) })=Re(I_se^{ j\omega t })
$$
where $I_s=Ie^{ j\phi }$ is the phasor form for $i(t)$. $I$ is the [[Root Mean Square\|rms]] and $\phi$ is the [[Argument\|Argument]].

[[Converting sinusoids to phasors\|Converting sinusoids to phasors]]
