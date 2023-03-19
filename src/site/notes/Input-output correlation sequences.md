---
{"dg-publish":true,"permalink":"/input-output-correlation-sequences/","tags":["digitalsignalbehandling"]}
---

If we have an [[Linjära och Tidsinvarianta System\|LTI system]] with [[Impulssvar\|impulse response]] $h(n)$, then the [[Crosscorrelation\|crosscorrelation]] between output and input is
$$r_{yx}(l)=y(l)*x(-l)=(x(l)*h(l))*x(-l)$$
and since [[Faltning\|convolution]] is [[Kommutativ\|commutative]] and [[Associativ\|associative]],
$$r_{yx}(l)=h(l)*(x(l)*x(-l))$$
where we recognize the last part as the [[Autocorrelation\|autocorrelation]] of x(n) and 
$$r_{yx}=h(l)*r_{xx}(l)$$
The [[Crosscorrelation\|crosscorrelation]] between input and output can be found using the same technique and becomes
$$r_{xy}(l)=h(-l)*r_{xx}(l)$$

The [[Autocorrelation\|autocorrelation]] of the output
$$r_{yy}=y(l)*y(-l)=((h(l)*x(l))*(h(-l)*x(-l))$$
which becomes (since [[Faltning\|convolution]] is [[Kommutativ\|commutative]] and [[Associativ\|associative]])
$$r_{yy}(l)=r_{hh}(l)*r_{xx}(l)$$