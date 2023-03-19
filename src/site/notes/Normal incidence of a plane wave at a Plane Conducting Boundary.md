---
{"dg-publish":true,"permalink":"/normal-incidence-of-a-plane-wave-at-a-plane-conducting-boundary/","tags":["elektromagnetiskfältteori"]}
---

When an electromagnetic wave travelling in one medium impinges on another medium with a different [[Intrinsic Impedance\|intrinsic impedance]], it experiences a reflection. We assume that the incident wave travels in a lossless medium (where the [[Conductivity\|Conductivity]] $\sigma=0$) for simplicity. In this case we also assume the boundary is an interface with a perfect conductor ($\sigma=\infty$).

![Pasted image 20221207082852.png](/img/user/images/Pasted%20image%2020221207082852.png)

In the image above we have incident [[Electric Field\|electric field]] and [[Magnetic Field Intensity\|magnetic field intensity]] [[Phasors\|phasors]] of
$$
\begin{align}
E_i(z)=&\vec{a}_x E_{i_{0}}e^{ -j\beta_iz }\\\\
H_i(z)=&\vec{a}_y \frac{E_{i_{0}}}{\eta_{1}}e^{ -j\beta_iz }
\end{align}
$$
where $E_{i_{0}}$ is the magnitude of $E_i$ at $z=0$ and $\beta_{1}$ and $\eta_{1}$ are the [[Phase Constant\|phase constant]] and the [[Intrinsic Impedance\|intrinsic impedance]] of medium 1. The direction of propagation is given by the [[Poynting Vector\|poynting vector]], $\vec{P}_i=\vec{E}_i\times\vec{H}_i$, and is in the $\vec{a}_z$ direction. The variable $z$ is negative in medium 1 (see image).

Inside medium 2 both electric and magnetic fields vanish (since it's a perfect conductor) hence no wave is transmitted across the boundary, meaninig that the incident wave is reflected. The reflected electric field intensity can be written as 
$$
\vec{E}_r(z)=\vec{a}_xE_{r_{0}}e^{ +j\beta_{1}z }
$$
and travels in the $-z$ direction. The total electric field intensity in medium 1 has to be the sum of $\vec{E}_i$ and $\vec{E}_r$:
$$
\vec{E}_1(z)=\vec{E}_i(z)+\vec{E}_r(z)=\vec{a}_x(E_{i_{0}}e^{ -j\beta_{1}z }+E_{r_{0}}e^{ +j\beta_{1}z })
$$
due to [[Electromagnetic Boundary Conditions\|continuity of the tangential component]] of the $\vec{E}$-field at the boundary demands that
$$
\vec{E}_1(0)=\vec{a}_x(E_{i_{0}}+E_{r_{0}})=\vec{E}_2(0)=0 \Rightarrow E_{r_{0}}=-E_{i_{0}}
$$
which gives
$$
\vec{E}_1(z)=\vec{a}_xE_{i_{0}}(e^{ -j\beta_{1}z }-e^{ +j\beta_{1}z })=-\vec{a}_xj2E_{i0}\sin\beta_{1}z
$$
The magnetic field intensity of the reflected wave is related to $\vec{E}_r$ as
$$
\vec{H}_r(z)=\frac{1}{\eta_{1}}\vec{a}_{nr}\times\vec{E}_r(z)=\vec{a}_y \frac{E_{io}}{\eta_{1}}e^{ +j\beta_{1}z }
$$
combining with $\vec{H}_i$ we get the total magnetic field intensity in medium 1:
$$
\vec{H}_1(z)=\vec{H}_i(z)+\vec{H}_r(z)=\vec{a}_y2 \frac{E_{i0}}{\eta_{1}}\cos\beta_{1}z.
$$
These are called standing waves, since they do not appear to propagate with time.