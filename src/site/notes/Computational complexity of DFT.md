---
{"dg-publish":true,"permalink":"/computational-complexity-of-dft/","tags":["digitalsignalbehandling"]}
---

Performing the "raw computation" of the entire [[Discrete Fourier Transform\|DFT]] requires $N^{2}$ multiply and add operations (n terms to calculate and each term requires n operations). The most time consuming part is creating a variable that holds the [[Vektorer\|vector]], so increasing the number of terms doesn't increase the time needed by $n^{2}$, see figure below![Pasted image 20221003132433.png](/img/user/images/Pasted%20image%2020221003132433.png)
The fastest computations are for $N$ with many prime factors (blue colors).
