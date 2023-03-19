---
{"dg-publish":true,"permalink":"/lead-lag-compensation/","tags":["reglerteknik"]}
---


We add a compensation link that's either lead or lag (or both!) to our [[Feedback System\|feedback system]] in order to meet the criteria imposed on us ([[Förstärkning\|gain]], [[Fasmarginal\|phase margin]], speed, reducing steady-state errors etc). It is based on the [[Bode plot\|bode plot]] of 
$$G_{0}^{new}(s)=G_{K}(s)G_{0}(s)$$
![Pasted image 20220919164838.png](/img/user/images/Pasted%20image%2020220919164838.png)

Since $$\begin{flalign}\log|G_{0}^{new}(i \omega)|&=\log|G_{K}(i \omega)|+\log|G_{0}(i \omega)| \\
\arg{G_{0}^{new}}(i \omega)&=\arg{G_{K}(i \omega)}+\arg{G_{0}(i \omega)}
\end{flalign}$$
it is easy to determine the compensation link $G_{K}(s)$ as the difference between the desired [[Open-Loop Transfer Function\|open-loop transfer function]] and the uncompensated [[Överföringsfunktion\|transfer function]]

[[Lead compensator\|Lead compensator]]
[[Lag compensator\|Lag compensator]]