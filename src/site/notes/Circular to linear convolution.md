---
{"dg-publish":true,"permalink":"/circular-to-linear-convolution/","tags":["digitalsignalbehandling"]}
---


Can we use the [[Discrete Fourier Transform\|DFT]] to efficiently calculate the [[Faltning\|linear convolution]] as well?

The [[Circular Convolution\|circular convolution]] only produces a result of the same length as the sequences involved in the [[Faltning\|convolution]] and a [[Faltning\|linear convolution]] produces an output that is longer than the seuences.

If we zero-pad the two sequences (length $K$ and $L$) so that they are both of length $K+L+1$, and then perform a [[Circular Convolution\|circular convolution]] with period $N=K+L+1$. 
![Pasted image 20221003133014.png](/img/user/images/Pasted%20image%2020221003133014.png)

> If you make the [[Discrete Fourier Transform\|DFT]] big enough to fit the final result, then whatever you get out is the [[Faltning\|linear convolution]]

1. Zero-pad both sequences of length $K$ and $L$ to a common length $N \geq K+L-1$
2. Calcuate the $N$-point [[Discrete Fourier Transform\|DFT]] of both sequences so you get the points in frequency domain
3. Multiply the two DFTs element wise
4. Perform an N-pont inverse [[Discrete Fourier Transform\|DFT]] on the product

Performing a linear "direct" [[Faltning\|convolution]] in the time domain takes $KL$ operations and, if one of $K$ or $L$ is small enough compared to the other, doing the [[Faltning\|convolution]] the [[Discrete Fourier Transform\|DFT]]-way may not be more efficient (if performed only once).

This can lead to substantial delays. If we are processing a long input [[Signal\|signal]] we need to receive the entire [[Signal\|signal]] before we can start our calculations. If our [[Impulssvar\|impulse response]] is short, the time that it takes to receive the [[Signal\|signal]] is significant. 
