---
{"dg-publish":true,"permalink":"/generalized-ampere-s-circuital-law/","tags":["elektromagnetiskfältteori"]}
---

[[Ampere's Circuital Law\|Ampere's Circuital Law]] does not hold for [[Time-Varying Fields\|time-varying fields]], since [[Null identities#Null identity 2\|Null identities#Null identity 2]] is in contradiction with the [[Equation of Continuity\|Equation of Continuity]]. When Maxwell compiled his [[Maxwell's Equations\|equations]] he noticed this and derived a generalized version that works for [[Time-Varying Fields\|time-varying fields]].

On **point form**:
$$
\nabla\times\vec{H}=\vec{J}+ \frac{ \partial \vec{D} }{ \partial t } 
$$
On **intergal form** (derived by taking surface integrals on both sides and using [[Stoke's Theorem\|Stoke's Theorem]]):
$$
\oint_{C}\vec{H}\cdot d\vec{l}=I+ \frac{d}{dt}\int_S \vec{D}\cdot d\vec{s} 
$$
The total current passing through any surface S of which the closed loop C is the perimeter is the sum of the conduction current and the displacement current.
