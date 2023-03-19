---
{"dg-publish":true,"permalink":"/electric-field/","tags":["elektromagnetiskfältteori"]}
---

The concept of electric field is based on electric force. If we want to know the force that will be exerted on a "test charge" $q_{0}$ due to a given charge $q_{1}$ the answer is [[Coulomb's Law\|Coulomb's Law]]. If we normalize the force by the test charge $\frac{\vec{F_{10}}}{q_{0}}$ 
$$\vec{E}=\frac{\vec{F_{10}}}{q_{0}}=\frac{1}{4 \pi \varepsilon_{0}} \frac{q_{1}}{R_{10}^{2}}\vec{a}_{R_{10}}$$
> A measure of the force exerted on a charge in the field

The magnitude of the electric field can be seen by looking at the density of the [[Electric Flux\|flux lines]]


![Pasted image 20220919113834.png](/img/user/images/Pasted%20image%2020220919113834.png)
When our point source is not in the origin (as in image above) the [[Enhetsvektor\|unit vector]] $\vec{a}_{R}$, that is the vector pointing from the source to our field point, becomes $$\vec{a}_{R}=\frac{\vec{R}-\vec{R}'}{|\vec{R}-\vec{R}'|}$$which gives us 
$$\vec{E}=\frac{1}{4 \pi \varepsilon_{0}} \frac{q_{1}}{|\pmb{R}-\pmb{R}'|^2}\vec{a}_{R}=\frac{1}{4 \pi \varepsilon_{0}} \frac{q_{1}(\pmb{R}-\pmb{R}')}{|\pmb{R}-\pmb{R}'|^{3}}$$
can be expressed using [[Gradient\|Gradient]]
$$\vec{E}=\frac{1}{4 \pi \varepsilon_{0}} \int\left(- \nabla\frac{1}{|\pmb{R}-\pmb{R}'|^{3}}\right)\rho(\vec{R'})d \vec{v}$$

For more than one charge we can apply [[Superposition\|superposition]] and assume test charge $q$ $$\vec{E}=\frac{1}{4 \pi \varepsilon_{0}} \sum\limits_{k=1 }^{n}\frac{q_{k}(\pmb{R}-\pmb{R}_{k}')}{|\pmb{R}-\pmb{R}_{k}'|^3}$$
$\vec{E}$ tells us the force that a test charge $q$ in the field $\vec{E}$ will experience when placed at a position $p$, $\vec{F}=q \vec{E}$.

[[Electric Field relation to Electric Potential\|Electric Field relation to Electric Potential]]
[[Electric Field for distributed charges\|Electric Field for distributed charges]]
[[Electric Field for point dipoles\|Electric Field for point dipoles]]
