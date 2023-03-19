---
{"dg-publish":true,"permalink":"/z-transform/","tags":["digitalsignalbehandling"]}
---

The z-transform plays the same role in the analysis of [[Discrete-time signals\|discrete-time signals]] and [[Linjära och Tidsinvarianta System\|LTI systems]] as the [[Laplacetransformationer\|laplacetransform]] does for continuous-time signals and [[Linjära och Tidsinvarianta System\|LTI-systems]]. Just as with [[Laplacetransformationer\|laplacetransforms]] it is easier to use than performing heavy [[Faltning\|convolution]] calculations.

It's an infinite [[Potensserier\|power series]] 
$$Z(z)=\sum\limits_{n=-\infty}^{\infty}x(n)z^{-n}$$
that only exists for those values of $z$ where the series converges, known as the [[Region of convergence\|Region of convergence]]. Two signals can have the same z-transform ([[Kausal\|causal]] and [[Anti-kausal\|anti-causal]]), which is why you need to know the [[Region of convergence\|ROC]] in order to uniquely identify the corresponding sequence/[[Signal\|signal]]. 

We don't want to use the scary definition so we look at the [[Properties of the z-transform\|properties]] and [[Common z-transform pairs\|pairs]] instead. If the expression doesn't match any pairs and no properties can be applied, use the definition.

[[Properties of the z-transform\|Properties of the z-transform]]
[[Common z-transform pairs\|Common z-transform pairs]]
[[Poles and zeros of Z-transforms\|Poles and zeros of Z-transforms]]