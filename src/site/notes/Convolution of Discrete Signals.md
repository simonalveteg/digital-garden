---
{"dg-publish":true,"permalink":"/convolution-of-discrete-signals/","tags":["digitalsignalbehandling"]}
---

For discrete signals the [[Faltning\|convolution]] is easier to calculate by setting up a table. In the example below the input signal is $x(n) = \begin{pmatrix}2 & 4 & 6 & 4 & 2\end{pmatrix}$ and the [[Impulssvar\|impulse response]] is $h(n)=\begin{pmatrix}3 & 2 & 1\end{pmatrix}$. The resulting signal becomes $y(n)=x(n)*h(n)=\begin{pmatrix}6 & 16 & 28 & 28 & 20 & 8 & 2\end{pmatrix}$ with a length of $7$.

![Pasted image 20220831090853.png|500](/img/user/images/Pasted%20image%2020220831090853.png)

[[Faltning\|Convolution]] fulfills the [[Kommutativ\|commutative]] law
![commutative law convolution.png|300](/img/user/images/commutative%20law%20convolution.png)
the [[Associativ\|associative]] law
![associative law convolution.png|300](/img/user/images/associative%20law%20convolution.png)
and the distributive law
![distributive law convolution.png|300](/img/user/images/distributive%20law%20convolution.png)
(illustrated using block diagrams).

## Convolution of Finite-length signals
If we perform the [[Faltning\|convolution]] $y(n)=h(n)*x(n)$ between two finite-length signals, where the length of $x$ and $h$ are $M$ and $N$ respectively, the maximum length of the resulting signal $y(n)$ is $M+N-1$.


## Causality
An [[Linjära och Tidsinvarianta System\|LTI system]] is only [[Kausal\|causal]] if $h(n)=0$ for all $n<0$. Samma som för vanlig kausalitet.