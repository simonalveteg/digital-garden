---
{"dg-publish":true,"permalink":"/charge-redistribution-based-on-equation-of-continuity/","tags":["elektromagnetiskfältteori"]}
---

For an [[Ohmic Materials\|ohmic material]], $\vec{J}=\sigma\vec{E}$, which gives ([[Equation of Continuity\|Equation of Continuity]])
$$\nabla\cdot\vec{J}=\nabla\cdot\sigma\vec{E}=-\frac{ \partial \rho }{ \partial t } \Rightarrow \nabla\cdot\vec{E}=-\frac{1}{\sigma}\frac{ \partial \rho }{ \partial t }$$

If the [[Ohmic Materials\|ohmic material]] is a linear dielectric with [[Permittivity\|permittivity]] $\varepsilon$, then inside the material $\vec{D}=\varepsilon\vec{E}$.  Substituting this into [[Gauss' Law\|Gauss' Law]] in point form gives 
$$
\nabla\cdot\vec{D}=\rho \Leftrightarrow \nabla\cdot\varepsilon\vec{E}=\rho \Leftrightarrow \nabla\vec{E}=\frac{\rho}{\varepsilon}$$
combining these two equations gives a first order partial differential euation, the solution to which is 
$$
\rho(t)=\rho_0e^{ -( \sigma/\varepsilon)t  }
$$

the [[Tidskonstant\|time constant]] of which is $\tau=\frac{\varepsilon}{\sigma}$, which tells us the time needed to decrease tha value of the function to $\rho_0e^{ -1 }$.
