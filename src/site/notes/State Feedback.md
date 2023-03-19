---
{"dg-publish":true,"permalink":"/state-feedback/","tags":["reglerteknik"]}
---

We assume that the process to be controlled is given in [[Linear state-space model\|state-space form]]
$$\begin{flalign}& \dot{x}=Ax+Bu\\&y=Cx \end{flalign}$$
the direct term $D$ has been ignored for simplicity.

For state [[feedback\|feedback]] we assume that we can measure all process states. ths is unrealistic in most cases.

![state_feedback.png](/img/user/images/state_feedback.png)
![Pasted image 20220914123543.png](/img/user/images/Pasted%20image%2020220914123543.png)
In state [[feedback\|feedback]] the control signal is a [[Linjärkombination\|linear combination]] of the [[Tillståndsvariabler\|state variables]] and the [[Setpoint\|setpoint]].

# The closed-loop system
The [[Linear state-space model\|state-space]] description of the [[Closed-loop System\|closed-loop system]] is 
$$\begin{flalign}&\dot{x}=(A-BK)x+Bk_{r}r \\&y=Cx \end{flalign}$$
The [[Setpoint\|setpoint]] $r$ is our new input, and the corresponding [[Överföringsfunktion\|transfer function]] is given by
$$Y(s)=C(sI-(A-BK))^{-1}Bk_{r}R(s)$$
where the [[Karaktäristiska Polynomet\|characteristic polynomial]] has become 
$$det(sI-(A-BK))$$
THe state feedback has changed the [[Matris\|matrix]] $A$ of the [[Open-loop System\|open-loop system]] into $A-BK$, which is the corresponding [[Matris\|matrix]] for the [[Closed-loop System\|closed-loop system]]. The eigenvalues of $A-BK$ can be chosen by choosing a value of $K$.

Choose $k_r$ so that the [[Static Gain\|static gain]] of the [[Closed-loop System\|closed-loop system]] becomes unity in order to achieve $y=r$ in stationarity.

Sätt upp slutet system på tillståndsform. Räkna ut A-matrisen för det slutna systemet. Får fram ett [[Karaktäristiska Polynomet\|karaktäristiskt polynom]] och jämför med det önskade [[Karakteristiska polynomet för matriser\|karakteristiska polynomet]] för att få fram värden för regulatorn ([[Control System\|controller]]) $k_{r}$. This is not always possible, which is why we introduce the concept of [[Controllability\|Controllability]].

