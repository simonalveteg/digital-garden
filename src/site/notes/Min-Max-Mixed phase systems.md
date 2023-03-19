---
{"dg-publish":true,"permalink":"/min-max-mixed-phase-systems/","tags":["digitalsignalbehandling"]}
---

**Minimum** phase [[Filters\|filters]] delay the signals the least, and **maximum** the most. **Mixed** phase systems are somewhere inbetween.

There are $2^N$ different $H(z)$ whose magnitude responses $|H(\omega)|$ are identical, if $H(z)$ has $N$ zeros. Among these there is one wiht all zeros inside the unit circle and one with all zeros outside. 

A [[FIR Filter\|FIR filter]] $H(z)$ is called 
1. minimum-phase if all its zeros are inside the unit circle
2. maximum-phase if all its zeros are outside the unit circle
3. mixed-phase or nonminimum-phase if it has zeros both inside and outside the unit circle