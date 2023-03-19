---
{"dg-publish":true,"permalink":"/linearization/","tags":["reglerteknik"]}
---

For a [[System (matematisk definition)\|System (matematisk definition)]] written in the [[Linear state-space model\|Linear state-space model]]:
$$\dot{x}=f(x,u)$$$$y=g(x,u)$$
where f and g are nonlinear functions of x and u. 

To linearise you need
1. An equlibrium (a point to linearise about)
2. To use the taylor series 

The equilibrium point can be found by looking at solutions to our [[Differentialekvationer\|differential equations]] where all derivatives are zero.

Step by step:
1. Determine a [[Stationary Point\|stationary point]] around which we shall approximate the [[System (matematisk definition)\|System (matematisk definition)]]. 
2. Make [[Taylorutveckling\|taylor series expansions]] of $f$ and $g$ around $(x_{0},u_{0})$. Keep only the first order terms ![Pasted image 20220905104923.png](/img/user/images/Pasted%20image%2020220905104923.png)
4. Introduce new variables $\Delta x = x-x_{0}$,  $\Delta u = u-u_{0}$,  $\Delta y = y-y_{0}$.
5. The [[Linear state-space model\|state-space equations]] in the new variables are given by ![Pasted image 20220905105051.png](/img/user/images/Pasted%20image%2020220905105051.png)Note that $x$ and $f$ are [[Vektorer\|vectors]], the equations hold the same structure for higher order systems. 