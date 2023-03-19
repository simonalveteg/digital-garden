---
{"dg-publish":true,"permalink":"/electromagnetic-boundary-conditions/","tags":["elektromagnetiskfältteori"]}
---

Electromagnetics is time-varying, as opposed to [[Electrostatics\|Electrostatics]] and [[Magnetostatics\|Magnetostatics]].

In order to solve electromagnetic problems involving contiguous regions of different mediums, it is necessary to know the [[Boundary Conditions\|boundary conditions]] that the [[Vector field\|vector fields]] must satisfy at the interfaces.

The [[Boundary Conditions\|boundary conditions]] for the tangential components of the [[Electric Field\|electric field]] and the [[Magnetic Field Intensity\|magnetic field intensity]] are exactly the same as for [[Boundary Conditions for Electrostatic Fields\|electrostatics]] and [[Boundary Conditions for Magnetostatic Fields\|magnetostatics]]:
$$
E_{1t}=E_{2t}
$$
$$
\vec{a}_{n2}\times(\vec{H}_1-\vec{H}_2)=\vec{J}_s
$$
And the same is true for the normal components of the [[Electric Flux Density\|electric flux density]] and [[Magnetic Field\|magnetic field]]:
$$
\vec{a}_{n_{2}}\cdot(\vec{D}_1-\vec{D}_2)=\rho_s
$$
$$
B_{1n}=B_{2n}
$$
The following general statements can be made
1. The tangential component of an $\vec{E}$ field is **continuous** across an interface.
2. The tangential component of an $\vec{H}$ field is **discontinuous** across an interface where a surface current exists, the amount of discontinuity being determined by the equation above.
3. The normal component of a $\vec{D}$ field is **discontinuous** across an interface where a surface charge exists, the amount of discontinuity being determined by the equation above.
4. The normal component of a $\vec{B}$ field is **continuous** across an interface.
