---
{"dg-publish":true,"permalink":"/magnetic-force-on-a-current-carrying-circuit/","tags":["elektromagnetiskfältteori"]}
---

In order to calculate the [[Magnetic Force\|Magnetic Force]] on a current carrying circuit we divide the circuit into small parts 
$$
d\vec{F}_m=dQ\vec{u}\times\vec{B}
$$
and $dQ=-NeSdl$ (amount of charges times their magnitude, times the volume). Using [[Strömtäthet\|current density]] we can write 
$$
\begin{align}
\vec{J}&=Nq\vec{u}=-Ne\vec{u} \\
I&=\vec{J}\cdot\vec{S}=-Ne|\vec{u}|S
\end{align}$$
which gives $d\vec{F}_m=Id\vec{l}\times\vec{B}$
$$
\vec{F}_m=I_1 \oint_{C_1}d\vec{l}_1\times\vec{B}
$$
For a **two circuit system** where the [[Magnetic Field\|Magnetic Field]] comes from another closed circuit $C_2$ with current $I_2$, we can then write the force on circuit $C_{1}$ as $F_{21}=F_m$
$$
\vec{F}_{21}=I_{1} \oint_{C_{1}} d\vec{l}_1\times\vec{B}_{21}
$$
which can be written as (using [[Biot-Savart Law\|Biot-Savart Law]])
$$
\vec{B}_{21}=\frac{\mu_{0}I_{2}}{4\pi}\oint_{C_{2}} \frac{d\vec{l}_2\times\vec{a}_R}{R_{21}^{2}}
$$
$$
\vec{F}_{21}=\frac{\mu_{0}I_{1}I_{2}}{4\pi}\oint_{C_{1}}\oint_{C_{2}} \frac{d\vec{l}_1\times(d\vec{l}_2\times\vec{a}_{R_{21}})}{R_{21}^{2}}
$$
which is [[Ampere's Force Law\|Ampere's Force Law]].
