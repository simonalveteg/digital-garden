---
{"dg-publish":true,"permalink":"/gauss-law/","tags":["elektromagnetiskfältteori"]}
---

The total outward flux of the [[Electric Field\|electric field]] over any [[Gaussian Surface\|gaussian surface]] is equal to the total charge enclosed by the surface, divided by $\epsilon_{0}$
$$\oint\limits_{S}\vec{E}\cdot d \vec{s}=\frac{1}{\epsilon}\int \rho dv = \frac{Q}{\epsilon}$$
this is gauss' law in *integral form*. If we choose a [[Gaussian Surface\|gaussian surface]] upon which the [[Electric Field\|electric field]] is uniform, i.e if we have symmetry, the $\vec{E}$ can be moved out of the integral and gauss' law becomes
$$
\vec{E}\oint\limits_{S}ds=\vec{E}A=\frac{Q}{\epsilon}
$$
where the integral of the surface just becomes the area of the surface! 


Gauss' Law derives from [[Coulomb's Law\|Coulomb's Law]] and is one of [[Maxwell's Equations\|Maxwell's Equations]].

# Differential Form
The integral form derives from the *differential form*, which is
$$\nabla \cdot\vec{D}=\rho $$
where $\vec{D}$ is [[Electric Flux Density\|electric flux density]] ($\vec{D}=\epsilon\vec{E}$) and $\rho$ is the [[Charge Density\|Charge Density]].

Using [[Divergence Theorem\|Divergence Theorem]] we can write the *integral form* of Gauss Law as $\nabla \cdot \vec{D}= \rho \Rightarrow \int_{V}\nabla \cdot \vec{D}dv=\int_{V}\rho dv \Rightarrow \oint\limits_{S}\vec{D}\cdot d \vec{s}=Q$
$$\oint\limits_{S}\vec{E}\cdot d \vec{s}= \frac{Q}{\epsilon}$$ where $Q$ is the total charge enclosed by $V$ or $S$ and $\vec{E}$ is the [[Electric Field\|Electric Field]].

![Pasted image 20221005113122.png](/img/user/images/Pasted%20image%2020221005113122.png)
