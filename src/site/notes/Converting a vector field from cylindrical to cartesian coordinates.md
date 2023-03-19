---
{"dg-publish":true,"permalink":"/converting-a-vector-field-from-cylindrical-to-cartesian-coordinates/","tags":["elektromagnetiskfältteori"]}
---

For a [[Vector field\|vector field]] $\vec{A}$ at a point in space, the conversion leaves $\vec{a}_{z}$, since the two systems share a [[Basvektor\|basis vector]].

The direction of the [[Basvektor\|base vectors]] can also be position dependent, like for [[Cylindrical Coordinates\|cylindrical coordinates]] where $\vec{a}_{r}$ changes depending on the angle.

We can use [[Projektion\|projection]] to find out the components of the cylindrical [[Basvektor\|basis vectors]]. $\vec{a_{r}} \cdot \vec{a_{x}}=\cos\phi$, $\vec{a_{r}} \cdot \vec{a_{y}}=\sin\phi$, $\vec{a_{r}} \cdot \vec{a_{z}}=0$
![Pasted image 20220921115539.png](/img/user/images/Pasted%20image%2020220921115539.png)
The conversion contains functions of $\phi$, but anything that is desribed by $r$ and $\phi$ can be converted to $x$ and $r$
$x=r\cos\phi$, $y=\sin\phi$.
$r=\sqrt{x^{2}+y^{2}}$, $\phi=\arctan \frac{y}{x}$ 
![Pasted image 20220921115919.png](/img/user/images/Pasted%20image%2020220921115919.png)

