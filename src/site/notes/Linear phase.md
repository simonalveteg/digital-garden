---
{"dg-publish":true,"permalink":"/linear-phase/","tags":["digitalsignalbehandling"]}
---


We often want all frequency components going through a filter to experience the same delay. Therefore we want $\Delta \omega$ to be constant for all $\omega$.

The delay at a certain frequency is $$\Delta \omega=-\angle H(\omega)/\omega ~\text{[samples]}$$
For [[FIR Filter\|FIR filters]] the [[Impulssvar\|impulse response]] must have conjugate-even or conjugate-odd symmetry around the midpoint to have linear phase. For [[FIR Filter\|FIR filters]] of length $N$ with real-valued coefficients there are three types that have linear phase:
1. Non-[[Kausal\|causal]] with symmetry around $n=0$. $$h(n)=h(-n)$$ for which $H(\omega)$ is real-valued
2. [[Kausal\|Causal]] with symmetry around $n=N/2$ $$h(n)=h(N-n)$$ 
3. [[Kausal\|Causal]] with anti-symmetry around $n=N/2$ $$h(n)=-h(N-n)$$
[[Kausal\|Causal]] = negative slope of phase

![Pasted image 20220921095103.png](/img/user/images/Pasted%20image%2020220921095103.png)
If we want to have a linear phase filter a zero at $z_{0}$ of $H(z)$ also needs a zero at its reciprocal $z_{1}=\frac{1}{z_{0}}$. For real impulse responses we also know that the zeros must come in conjugate pairs.
![Pasted image 20220921095408.png](/img/user/images/Pasted%20image%2020220921095408.png)
Linear phase requires each zero inside the unit circle to have a corresponding one outside the unit circle.

[[IIR Filter\|IIR filters]] that are [[Insignal-utsignalstabilt\|BIBO stable]] can not have linear phase! Since they (with the same reasoning as above) need a pole outside the unit circle for every pole inside the unit circle.
