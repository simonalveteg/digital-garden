---
{"dg-publish":true,"permalink":"/error/","tags":["numeriskanalys"]}
---

Let $x_c$ be a computed version of the exact quantity $x\in\mathbb R /\{0\}$. Then
$$
\begin{align}
\text{absolute error} &= \left| x_c-x \right|  \\
\text{relative error} &= \frac{\left| x_c-x \right|}{\left| x \right| }
\end{align}
$$
In the IEEE machine arithmetic model, the relative roundin gerror of $fl(x)$ is no more than one half [[Machine Epsilon\|machine epsilon]].
$$
\frac{\left| fl(x)-x \right|}{\left| x \right| }\leq \frac{1}{2}\epsilon_{mach}
$$
[[Cancellation Error\|Cancellation Error]]
[[Interpolation Error\|Interpolation Error]]
[[Backward Error and Forward error\|Backward Error and Forward error]]
