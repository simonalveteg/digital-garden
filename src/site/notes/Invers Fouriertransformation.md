---
{"dg-publish":true,"permalink":"/invers-fouriertransformation/","tags":["systemochtransformer"]}
---

$$f(t) \xrightarrow{\mathcal{F}}F(w)$$
där F är [[Fouriertransformationer\|fouriertransformationen]] av f, och f är den inversa [[Fouriertransformationer\|fouriertransformationen]] av F!
$$F(w) \xrightarrow{\mathcal{F}^{-1}}f(t)$$
kan också skrivas $\mathcal{F}^{-1}(F(w))(t)=f(t)$.

[[Inversionsformeln för Fouriertransformationer\|Inversionsformeln för Fouriertransformationer]]


![Pasted image 20220912144544.png](/img/user/images/Pasted%20image%2020220912144544.png)

Continuous-time: $$x(t)=\int_{-\infty}^{\infty}F_{0}X(kF_{0})e^{j2\pi kF_{0}t}dF$$
Discrete-time: $$x(m)=\int_{-\frac{1}{2}}^{\frac{1}{2}}X(f)e^{j2\pi fm}df$$
