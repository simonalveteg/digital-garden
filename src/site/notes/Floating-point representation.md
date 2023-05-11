---
{"dg-publish":true,"permalink":"/floating-point-representation/","tags":["numeriskanalys"]}
---

$$
x_\beta=(-1)^{s}d_{0}.d_{1}\dots d_{k-1}\cdot\beta^{e}
$$
![Pasted image 20230320162429.png](/img/user/images/Pasted%20image%2020230320162429.png)

There are there commonly used levels of precision for floating-point numbers ($\beta=2$ (base 2)):
![Pasted image 20230320162512.png](/img/user/images/Pasted%20image%2020230320162512.png)

>[!warning] IEEE floating-point number
>We denote the IEEE double precision floating point number associated to $x\in \mathbb{R}$ using the Rounding to Nearest Rule, by $fl(x)$

# IEEE 754 Floating Point Standard
![Pasted image 20230320162642.png](/img/user/images/Pasted%20image%2020230320162642.png)
Each $b$ is 0 or 1. $e$ is an $M$-bit binary number representing the exponent. Normalization means that the leading (leftmost) bit must be 1.

# Representation of infinite ([[Binary Numbers\|binary numbers]])
How do we fit an infinite recurring sequence in a finite representation? There are a few alternatives

## Chopping
Simply throw away the bits that fall of in the end. Enkel lösning men den är biased mot noll, då talet alltid kommer bli mindre.

## Rounding
In base 10, if next digit is $\geq5$ round up, if it's $<5$ round down. For binary the rounding technique in IEEE standard is:
If bit 53 is 1, then add 1 to bit 52 (round up)
If bit 53 is 0, then do nothing (round down)
With one exception. If the bits following bit 52 are 100…0…0… (exactly half way between up and down) we round up or down accrding to which choce makes the final bit 52 equal to 0. Called *Rounding to nearest rule*. Annars kommer man istället att biasera mot oändligheten.

