---
{"dg-publish":true,"permalink":"/line-integral-of-vector-functions/","tags":["elektromagnetiskfältteori"]}
---

The line integral is used when calculating the work done against the field when moving a point charge in a straight line
$$W=-\int_{p_{i}}^{p_{f}}\vec{F}d \vec{l}=-q_{0}\int_{p_{i}}^{p_{f}}\vec{E}d \vec{l}$$
in the general case the line is not straight
![Pasted image 20220926114808.png](/img/user/images/Pasted%20image%2020220926114808.png)
and we can evaluate the work done as
$$W=-\int\limits_{C}\vec{F}d \vec{l}=-\int\limits_{a}^{b}\vec{F}(\vec{R}(u))\cdot \frac{d \vec{l}}{du}du$$

In the special case of a closed curve $C$ the line integral is called "circulation".
$$C=\oint\limits_{C}\vec{F}d \vec{l}$$
The closed line integral is used to define [[Stoke's Theorem\|Stoke's Theorem]].

How to evaluate the integral:
1. Choose a [[Coordinate Systems\|coordinate system]]
2. Form the line element $d \vec{l}$
3. Perform the integral
