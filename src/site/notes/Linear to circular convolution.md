---
{"dg-publish":true,"permalink":"/linear-to-circular-convolution/","tags":["digitalsignalbehandling"]}
---

[[Faltning\|Linear convolution]] can be done efficiently by using [[Zero-Padding\|zero-padding]] and [[Circular Convolution\|circular convolution]], allowing the [[Discrete Fourier Transform\|DFT]] to deliver a [[Faltning\|linear convolution]] result.

Assume we have an [[Linjära och Tidsinvarianta System\|LTI system]] with an [[Impulssvar\|impulse response]] $h(n)$ of duration $K$, and an input signal of duration $N$, where the output $y(n)$ is the result of a [[Faltning\|linear convolution]] $$y(n)=h(n)*x(n)=\sum\limits_{k=0}^{K-1}h(k)x(n-k)$$ What happens if we extend the input $x(n)$, in front, by $K-1$ samples from its end. ![Pasted image 20221003142016.png](/img/user/images/Pasted%20image%2020221003142016.png)
The [[Faltning\|linear convolution]] now produced one period of the [[Circular Convolution\|circular convolution]] (for $n=0,1,...,N-1$).
