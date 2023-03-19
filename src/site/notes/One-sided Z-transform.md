---
{"dg-publish":true,"permalink":"/one-sided-z-transform/","tags":["digitalsignalbehandling"]}
---

Just as with [[Ensidig Laplacetransform\|one-sided laplacetransform]] we can use a one-sided [[Z-transform\|z-transform]] ($z^{+}\text{-transform}$). For [[Kausala Signaler\|causal signals]] this transform delivers the same result as the normal [[Z-transform\|z-transform]]. The important part is that we get a different time-shift property (delay by k).

$$Y^{+}(z)=\sum\limits_{n=0}^{\infty}y(n)z^{-n}$$
The one-sided [[Z-transform\|z-transform]] is depending only on the positive values of $n$.