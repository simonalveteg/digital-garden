---
{"dg-publish":true,"permalink":"/the-servo-problem/","tags":["reglerteknik"]}
---

The servo problem is the case for a [[Feedback System\|feedback system]] where the load disturbances are zero. In this case we only study the [[Setpoint\|setpoint]] tracking properties of the controller (how close it gets to our desired value).

The [[Överföringsfunktion\|transfer function]] for how the error signal relates to the reference signal is 
$$E(s)=R(s)-Y(s)=\frac{1}{1+G_{0}(s)}R(s)$$
and the [[Final Value Theorem\|Final Value Theorem]] is used to determine the control error $e(t)$ as $t \rightarrow \infty$
$$e_{\infty}=\lim\limits_{t \rightarrow \infty}e(t)=\lim\limits_{s \rightarrow 0}sE(s)$$
# The general case
A general loop transfer function is given by
$$G_{0}=\frac{KB(s)}{s^{n}A(s)}e^{-sL}$$
and covers most of the processes and controllers we will encounter in this course. $K/s^{n}$ is a low-frequency part, $L$ is the delay and $A$ and $B$ are two polynomials with [[Static Gain\|static gain]] ($A(0)=B(0)=1$).

We let the [[Setpoint\|setpoint]] be given by 
$$r(t)= \begin{cases} \frac{t^{m}}{m!}, t\geq0 \\ 0 ,t<0 \end{cases}$$
where $m$ is a positive integer. The laplace transformation of the [[Setpoint\|setpoint]] is given by (from formula)
$$R(s)=\frac{1}{s^{m+1}}$$
For this general case the [[Stationary Error\|stationary error]] (computed with [[Final Value Theorem\|Final Value Theorem]])
$$e_{\infty}=\lim\limits_{t \rightarrow \infty}e(t)=\lim\limits_{s \rightarrow0} \frac{A(s)}{s^{n}A(s)+KB(s)e^{-sL}} \cdot\frac{s^{n}}{s^{m}}$$
since the [[Final Value Theorem\|final value theorem]] necessitates the existance of a limit, and the two polynomials have [[Static Gain\|static gain]] we get
$$e_{\infty}=\lim\limits_{s \rightarrow0} \frac{1}{s^{n}+K}s^{n-m}$$
The only things that matter are $n$ (the degree of $s$), $K$ (the gain), and $m$ (a measure of how quickly the [[Setpoint\|reference value]] changes). This gives us a few different cases

$n>m \Rightarrow e_{\infty}=0$
$n=m=0 \Rightarrow e_{\infty}=\frac{1}{1+K}$
$n=m\geq1 \Rightarrow e_{\infty}=\frac{1}{K}$
$n<m \Rightarrow \text{Limit does not exist}$

$n$ is the number of integrators in the loop transfer function.

If there are no integrators we will always get a [[Stationary Error\|stationary error]]. If there is one integrator we can handle a step function without error. If there are two integrators we can handle ramp functions and so on.
