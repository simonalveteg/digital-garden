---
{"dg-publish":true,"permalink":"/method-of-images/","tags":["elektromagnetiskfältteori"]}
---


Method of Images is an example application of the [[Uniqueness Theorem\|Uniqueness Theorem]], i.e. a solution of an electrostatic problem satisfying its [[Boundary Conditions\|boundary conditions]] is the only possible solution!

If [[Charge Distribution\|charge distribution]] is known everywhere, we can calculate the [[Electric Potential\|electric potential]] $V$ and [[Electric Field\|electric field]] $\vec{E}$. Otherwise we can NOT find $V$ or $\vec{E}$ with any methods taught in this course. However, when conducting bodies have boundaries of simple geometry we can replace these boundaries by image charges to satisfy the [[equipotential boundary condition\|equipotential boundary condition]] of [[Conductor\|conductors]].

We can often guess where the image charge should be placed, and if we were correct (it satisfies the [[Boundary Conditions\|boundary conditions]]) it is the only solution.

[Method of Images in Electrostatics - Wolfram Demonstrations Project](https://demonstrations.wolfram.com/MethodOfImagesInElectrostatics/)

> Naturally the medium above is imaged to the space below as well in the equivalent setup.
> - extenta

# Recipe

1. Make an initial guess of the position(s) of the image charge(s)
2. If needed, use the boundary condition to find the exact position(s) and magnitude of the charge(s)
3. Once the image charge(s) is found, then use it together with the real charge(s) to determine the $\vec{E}$ field everywhere *outside* the [[Conductor\|conductor]]

> REMEMBER THAT THE IMAGE CHARGE IS NOT REAL!

The general rule is that if the angle between two planes is $\alpha=\frac{360}{M}$ then we will need $M-1$ image charges to achieve zero potential at the boundaries.

# Example, point charge above an infinitely large conducting grounded plane

![Pasted image 20221031113143.png](/img/user/images/Pasted%20image%2020221031113143.png)
We place the image charge $q_{i}$ at an equal distance to the plane, but on the other side, and calculate $\vec{D}$ and $\vec{E}$ using [[Coulomb's Law\|Coulomb's Law]]
$$
\vec{D}=\varepsilon_{0}\vec{E}=-\vec{a_{n}} \frac{q}{4\pi d^{2}}+\vec{a_{n}} \frac{-q}{4\pi d^{2}}=\vec{a}_{n}\left( -\frac{q}{2\pi d^{2}}
 \right)=D_{n}\vec{a}_{n}
$$
And we know that $D_{n}=\rho_{s} \Rightarrow \rho_{s}=-\frac{q}{2\pi d^{2}}$

# Example, point charge near corner of two right angled infinite grounded planes
![Pasted image 20221031113839.png|400](/img/user/images/Pasted%20image%2020221031113839.png)
Here we can add three image charges (one in each quadrant). If the angle between the planes were to be  for example $60 \degree$, we would need 5 image charges. (Imagine we expand the angle to the full $360 \degree$)

# Example, point charge outside a grounded spherical conductor of radius $a$
![Pasted image 20221031114358.png](/img/user/images/Pasted%20image%2020221031114358.png)

We try to place the image charge in point $P_{i}$ at a distance of $d_{i}$ from the center of the circle, på samma linje som går från mitten av cirkeln till laddningen som är i punkt $P$. The point $M$ is on the boundary of the sphere, with a distance of $R$ to the charge. Using geometry we can create two similar triangles, $MOP$ and $MOP_{i}$ where we choose $P_{i}$ so that the triangles are similar. 