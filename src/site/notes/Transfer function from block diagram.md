---
{"dg-publish":true,"permalink":"/transfer-function-from-block-diagram/","tags":["reglerteknik"]}
---

[[Överföringsfunktion\|överföringsfunktionen]] är alltid $\frac{\text{produkten av allt som finns mellan}}{1-(\text{produkten av allt som finns i loopen})}$ 

For the [[Överföringsfunktion\|transfer function]] $H(s)$ given by
$$Y(s)=H(s)X(s)$$
the täljare is the product of all the blocks the signal passes when going from $x$ to $y$. The denominator is $1$ minus the product of *all* the blocks in the loop

This only works for simple feedback loops like the one above, it can have many blocks and inputs, but it has to be one path that goes in a single loop. For more complex feedback loops it can be applied creatively to iteratively transform one loop at the time typ?
