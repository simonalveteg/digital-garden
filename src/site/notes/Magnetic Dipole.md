---
{"dg-publish":true,"permalink":"/magnetic-dipole/","tags":["elektromagnetiskfältteori"]}
---

A current loop behaves like a magnetic dipole (a "tiny magnet"). Anytime we need to use a magnet we can replace it with a current loop. The [[Magnetic Dipole Moment\|Magnetic Dipole Moment]] then depends on the current of the loop.


A magnetic dipole has the [[Vector Magnetic Potential\|vector magnetic potential]] 
$$
\vec{A}=\frac{\vec{a}_\phi \mu_{0}Ib^2}{4R^{2}}\sin\theta
$$
In a volume of $\Delta v$ of a magnetic material with $n$ induced dipoles $\vec{m}_k,k=1,\dots,n$ per unit volume, we can define the **magnetization vector**:
$$
\vec{M}=\lim_{ \Delta v \to 0 } \frac{\sum_{k=1}^{n\Delta v}\vec{m}_k}{\Delta v}
$$
the sum of all [[Magnetic Dipole Moment\|magnetic dipole moments]] per volume, as the volume tends to zero. Also called the *volume density of magnetic dipole moment*.

$$
\begin{align}
\vec{A}=& \frac{\mu_{0}}{4\pi} \oint_{S'} \frac{\vec{M}\times\vec{a}_n'}{R}dv' \\
=& \frac{\mu_{0}}{4\pi} \oint_{S'} \frac{\vec{M}\times\vec{a}_n'}{R}ds'+\frac{\mu_{0}}{4\pi} \int_{V'} \frac{(\nabla'\times\vec{M})}{R}dv'
\end{align}
$$
where $\vec{J}_{ms}=\vec{M}\times\vec{a}_n$ is the surface current density 
and $J_m=\nabla\times\vec{M}$ is the volume current density. Both of these are called bounded current densities. Finding $\vec{B}$ or $\vec{A}$ from a magnetized material = finding equivalent current densities.