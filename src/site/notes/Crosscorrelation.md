---
{"dg-publish":true,"permalink":"/crosscorrelation/","tags":["digitalsignalbehandling"]}
---

Crosscorrelation seems very similar to [[Faltning\|convolution]], but it is not [[Kommutativ\|commutative]].

The crosscorrelation between two signals $x(n)$ and $y(n)$ is expressed as
$$r_{xy}(l)=\sum\limits_{k=-\infty}^{\infty}x(n)y(n-l)=\sum\limits_{k=-\infty}^{\infty}x(n-l)y(n)$$
where $l$ is the *time shift* or *lag* between the two. 

It is used to measure "similarity" between two time-shifted sequences/signals, and has many practical applications when looking for "patterns". The crosscorrelation "peaks" at the best match to our pattern.

Can be expressed using [[Faltning\|convolution]] as 
$$r_{xy}(l)=x(l)*y(-l)$$