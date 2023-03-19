---
{"dg-publish":true,"permalink":"/time-varying-fields/","tags":["elektromagnetiskfältteori"]}
---

The useful equations [[Coulomb's Law\|Coulomb's Law]] and [[Biot-Savart Law\|Biot-Savart Law]] describe how the fields depend on the sources and materials, but they only hold for [[Electrostatics\|Electrostatics]] and [[Magnetostatics\|Magnetostatics]]. For time-varying fields it is easier to use potential functions.

$$
\vec{E}=-\nabla V -\frac{ \partial \vec{A} }{ \partial t } 
$$
where we can write the [[Electric Potential\|Electric Potential]] $V$ as a function of sources and materials
$$
V(R,t)=\frac{1}{4\pi \varepsilon} \int_{V'} \frac{\rho\left( 1-\frac{R}{u} \right)}{R}dv' 
$$
where $R$ is the distance between the [[Field Point\|field point]] and source point, $u$ is the velocity of a wave. At time $t$ the [[Charge Distribution\|charge distribution]] depends on the [[Charge Distribution\|charge distribution]] at an earlier time $t-\frac{R}{u}$, which is called the **retarded scalar potential**.

Similarly we can obtain an equation for only the [[Vector Magnetic Potential\|Vector Magnetic Potential]] $\vec{A}$:
$$
\vec{A}(R,t)=\frac{\mu}{4\pi} \int_{V'} \frac{\vec{J}(t-R/u)}{R}dv'
$$
We can also find the [[Magnetic Field\|Magnetic Field]] using $\vec{B}=\nabla\times\vec{A}$.

