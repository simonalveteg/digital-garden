---
{"dg-publish":true,"permalink":"/electric-potential/","tags":["elektromagnetiskfältteori"]}
---

Electric [[Potential\|potential]] $V$ is a measure related to the amount of work to move a test charge $q_{0}$ in the field $\vec{E}$ due to another charge. Analogous to [[Potential\|potential]] [[Energi\|energy]]. 

By convention the work done against the field is negative 
$$W=-\int_{p_{i}}^{p_{f}}\vec{F}\cdot d \vec{l}=-q_{0}\int_{p_{i}}^{p_{f}}\vec{E}\cdot d \vec{l}$$

The change of electric potential $\Delta V =V_{1}-V_{0}$ is defined as $$V_{1}-V_{0}= \frac{W}{q_{0}}=\frac{q_{1}}{4 \pi \varepsilon_{0}}\left( \frac{1}{R_{p_{f}}}- \frac{1}{R_{p_{i}}}\right)$$where $R_{p_{i}}$ and $R_{p_{f}}$ are the distance between point charge $q_{1}$ and points $p_{i}$ and $p_{f}$ respectively. If $p_{i}$ goes towards infinity (test charge moved from infinitely far away) we can define electric potential at $p_{f}$ to be 
$$V_{1}= \frac{q_{1}}{4 \pi \varepsilon_{0}R_{p_{f}}}$$
For multiple charges we can use the [[Superposition\|superposition]] method
$$V= \frac{1}{4 \pi \varepsilon_{0}}\sum\limits_{k=1}^{n} \frac{qk}{|\vec{R}-\vec{R}_{k}'|}$$

In order to go from the [[Scalar field\|scalar field]] of electric potential to the [[Vector field\|vector field]] of the [[Electric Field\|electric field]] we simply use a [[Gradient\|gradient]]
$$\vec{E}=-\nabla V$$
or 
$$
V=\int \vec{E}\cdot d\vec{l}
$$

[[Electric Potential for distributed charges\|Electric Potential for distributed charges]]