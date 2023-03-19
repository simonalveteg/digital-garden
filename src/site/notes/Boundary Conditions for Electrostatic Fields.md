---
{"dg-publish":true,"permalink":"/boundary-conditions-for-electrostatic-fields/","tags":["elektromagnetiskfältteori"]}
---



![Pasted image 20221012102852.png](/img/user/images/Pasted%20image%2020221012102852.png)
When an [[Electric Field\|electric field]] hits the boundary of a medium there is a tangential component and a normal component.

## Tangential component
We find the boundary condition for the tangential component of the [[Electric Field\|electric field]] using the concept of potential difference
![Pasted image 20221012103113.png](/img/user/images/Pasted%20image%2020221012103113.png)
for a small closed loop C (a→b→c→d→a) $$\Delta V=-\oint\limits_{abcda}\vec{E}\cdot d \vec{l}=V(a)-V(a)=0$$which is equivalent to integrating each side of the rectangle and adding up the result. If $\Delta h \rightarrow0$ ($\vec{E}$ is very close to the boundary) the two integrals over bc and da is zero.  Therefore $$\begin{flalign}\oint\limits_{abcda}\vec{E}\cdot d\vec{l}=\left[\int\limits_{ab}+\int\limits_{cd}\right]\vec{E}\cdot d \vec{l}&=\vec{E}_{1}\cdot\Delta\vec{w}+\vec{E}_{2}\cdot(-\Delta\vec{w}) \\&=(\vec{E}_{1}-\vec{E}_{2})\cdot\Delta w \end{flalign}$$if $\Delta w$ is small and $\vec{E}$ is constant. In other words we are projecting $\vec{E}_{1}$ onto $\Delta\vec{w}$, which gives us the tangential component.

When medium 1 is a [[Conductor\|conductor]] the [[Electric Field\|electric field]] is 0 inside it, which leads to the tangential [[Electric Field\|electric field]] being zero? #question 

When both media are linear [[Dielectrics\|dielectrics]], $\vec{D}=\varepsilon \vec{E}$, and so $E_{1t}=E_{2t} \Leftrightarrow \frac{D_{1t}}{\varepsilon_{1}}=\frac{D_{2t}}{\varepsilon_{2}}$. If the permittivites are not the same the $\vec{D}$ field is not continuous. 

## Normal component
We find the boundary condition for the normal component of the [[Electric Field\|electric field]] using [[Gauss' Law\|Gauss' Law]] for a boundary surface where surface charge of density $\rho_{s}$ exists.
![Pasted image 20221012104940.png](/img/user/images/Pasted%20image%2020221012104940.png)
We want to find the relationship between $D_{1}$ and $D_{2}$ (normal component).

Applying the [[Gaussian Surface\|gaussian surface]] of a small pillbox with area of top and bottom faces being $\Delta S$ and the height $\Delta h$
$$\begin{flalign}LHS&=\oint\limits_{S}\vec{D}\cdot d \vec{s}=\left[ 
\int\limits_{top}+\int\limits_{bottom}+\int\limits_{side} \right]\vec{D}\cdot d \vec{s} \\&=D_{1}\cdot \vec{a}_{n2}\Delta S+\vec{D}_{2}\cdot \vec{a}_{n1}\Delta S=\rho_{s}\Delta S\\ &\Rightarrow D_{1n}-D_{2n}=\rho_{s}
\end{flalign}$$
 We derive this using $\vec{D}$ instead of $\vec{E}$ because it's not continuous in $\vec{E}_{n}$ (because $\varepsilon$ is not the same).

When medium 2 is a [[Conductor\|conductor]] and medium 1 is a linear [[Dielectrics\|dielectric]] then $\vec{D}_{2}=0$ inside the [[Conductor\|conductor]] $\Rightarrow D_{1n}=\rho_{s}=\varepsilon E_{1n}$.

When both media 1 and 2 are linear [[Dielectrics\|dielectrics]] $\rho_{s}=0$:
	$D_{1n}=D_{2n} \Leftrightarrow \varepsilon_{1}E_{1n}=\varepsilon_{2}E_{2n}$

The [[Skalär\|scalar]] [[Electric Potential\|electric potential]] $V$ is continuous across the boundary.