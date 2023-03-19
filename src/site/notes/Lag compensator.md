---
{"dg-publish":true,"permalink":"/lag-compensator/","tags":["reglerteknik"]}
---

Good at reducing steady-state errors.

A generalisation of a PI-controller

$$G_{K}(s)=M \frac{1+ \frac{s}{a}}{1+ \frac{sM}{a}}$$
where the corner frequency  $a=0.1 \omega_{0}$ by convention (which guarantees that the [[Fasmarginal\|phase margin]] is reduced by less than $6 \degree$), and the low-frequency [[Förstärkning\|gain]] $M>1$.

![lag compensators.png](/img/user/images/lag%20compensators.png)


Because of the negative phase it rotates the [[Nyquist plot\|nyquist plot]] clockwise so that the [[Fasmarginal\|phase margin]] becomes smaller, thereby making the [[System (matematisk definition)\|System (matematisk definition)]] less [[Robustness\|robust]]. If we pick $a$ to be small enough we can avoid the negative effects as long as we pick a large enough $M$. We still want $a$ to be as big as possible. The smaller $a$ is the slower the effect of our [[Control System\|controller]] is. Too big $\Rightarrow$ [[Stabila och Instabila System\|stability]] problems.

> If I make $M$ 10 I reduce my steady-state errors by a factor $M$