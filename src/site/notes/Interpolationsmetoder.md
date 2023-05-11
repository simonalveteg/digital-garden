---
{"dg-publish":true,"permalink":"/interpolationsmetoder/","tags":["mätteknik, numeriskanalys"]}
---


Vanligtvis förenas de samplade mätpunkterna med räta linjer **linjär interpolation** (linear spline). Man får en mer naturtrogen kurvformsåtergivning med hjälp av en så kallad *sinusinterpolator* - vilket även kräver färre punkter per period för att återge en sinusvåg. Nackelen med sinusinterpolering är att pulser med mycket branta flanker kommer bli väldigt ‘avrundade’.

Ett annat vanligt alternativ är att anpassa ett polynom till kurvan.
![Pasted image 20230327163102.png](/img/user/images/Pasted%20image%2020230327163102.png)
For models of gas dynamics one needs a discrete model $P(\rho)$ with smooth $P$ (as one needs $P'$ and $P''$). Piecewise linear interpolation would produce kinks in the measuring point and hence is not smooth. Two alternatives are
![Pasted image 20230327163316.png](/img/user/images/Pasted%20image%2020230327163316.png)

# Reasons for Interpolating
- Graph a curve that passes through some discrete number of points: computer graphics
- Evaluate a mathematical function easily and quickly: sine, cosine, log, exponential, …
- Substitute a "difficult" function b an "easy" one: simplifying a mathematical model for the weather report, integrating numerically.
- Extract information from a table of values: predict what the data would be at points where it wasn't measured, or analyse the growth pattern of the data.

# How to choose the form of the interpolating function
- Are there relevant mathematical or physical considerations?
- How should the function behave between the data points?
- Should the function have some properties like periodicity?
- Should the graph be pleasant to the eye?
- Do we need the mathematical description of the interpolating function or do we only need its graph?


[[Polynomial Interpolation\|Polynomial Interpolation]]
[[Piecewise Interpolation\|Piecewise Interpolation]]
