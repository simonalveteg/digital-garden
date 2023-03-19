---
{"dg-publish":true,"permalink":"/overlap-add-method/","tags":["digitalsignalbehandling"]}
---

Assume we have a [[System (matematisk definition)\|System (matematisk definition)]] with relatively short [[Impulssvar\|impulse response]] $h(n)$ of duration $K$ and a much longer input [[Signal\|signal]] $x(n)$ possibly of "infinite" duration. Where the output [[Signal\|signal]] is calculated using [[Faltning\|linear convolution]] $$y(n)=h(n)*x(n)$$
By splitting $x(n)$ into non-overlapping blocks $x_{m}(n)$ each of length $L$ as $$x_{m}(n)=\begin{cases} x(n) \text{ for } mL \leq n<(m+1)L \\0 \text{ otherwise} \end{cases}$$
we can write the input signal $$x(n)=\sum\limits_{m=-\infty}^{\infty}x_{m}(n)$$
and $$y(n)=h(n)*\sum\limits_{m=-\infty}^{\infty}x_{m}(n)=\sum\limits_{m=-\infty}^{\infty}y_{m}(n)$$
where $y_{m}(n)=h(n)*x_{m}(n)$.

We have now reduced the very long [[Faltning\|convolution]] into a series of shorter convolutions, whose individual results $y_{m}(n)$ added together give the same output $y(n)$.
![overlap-add.png](/img/user/images/overlap-add.png)

the overlap is there because the [[Faltning\|convolution]] of two signals have the length $K+L+1$, so the overlap is necessary.

1. Zero-pad $h(n)$ to length $N$
2. Calculate $H(k)=DFT(h(n))$
3. For each input block $x_{m}(n)$
	1. Zero-pad $x_{m}(n)$ to length $N$
	2. Calculate $X_{m}(k)=DFT(x_{m}(n))$
	3. Calculate $Y_{m}(k)=H(k)X_{m}(k)$
	4. Calculate $y_{m}(n)=IDFT(Y_{m}(k))$
	5. Add $y_{m}(n)$ to previous output (at correct position/correct overlap)

The first two steps are only performed once for a time-invariant filter, since $h(k)$ doesn't change.

The larger $N$, the more efficient the [[Faltning\|convolution]] becomes in terms of operations per output sample, if a fast Foruier transform algorithm is used, at the cost of *extra delay*.
