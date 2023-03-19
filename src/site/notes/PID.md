---
{"dg-publish":true,"permalink":"/pid/","tags":["reglerteknik"]}
---

The PID [[Control System\|controller]] is kind of like wrapping a [[Lead compensator\|Lead compensator]] and a [[Lag compensator\|Lag compensator]] into one package. The lead part corresponds to the derivative action and the lag part corresponds to the integral action.

It can be written on **series form**:
$$u(t)=K\left(e(t)+ 1/T_{i}\int_{0}^{t}e(\tau)d \tau+K_{d} \frac{de(t)}{dt}\right)$$
$$\frac{U(s)}{E(s)}=C(s)=\left(K+ \frac{K}{T_{i}s}+KK_{d}s\right)$$
Or on **parallell form**:
$$\frac{U(s)}{E(s)}=C(s)=K'\left(1+ \frac{1}{sT_{i}'}\right)\left(1+sT_{d}'\right)$$
The parallell form consists of terms that we know how to draw a [[Bode plot\|bode plot]] of, as opposed to the series form.


Consists of 
[[Proportional Control Strategy\|Proportional Control Strategy]]
[[Integral Control Strategy\|Integral Control Strategy]]
[[Derivative Control Strategy\|Derivative Control Strategy]]


Everything you're doing with [[Lead-Lag Compensation\|Lead-Lag Compensation]] you can probably do with PID.
$$C(s)=K_{p}+sK_{D}=K_{p}\left(1+ \frac{K_{D}}{K_{p}}s\right)= K_{p}(1+\alpha i \omega)$$
$$|C(i \omega)P(i \omega)|=1$$
$$arg(C(i \omega))=arctan(\alpha \omega)=\text{phase compensation?}$$
From the phase compensation #question we can use the equation for the [[Argument\|argument]] to get alpha ($\alpha=\frac{K_{D}}{K_{p}}$ ). With alpha we can now calculate $K_{p}$
$$|C(i \omega)|=K_{p}\sqrt{1+\alpha^{2}\omega^{2}} \Rightarrow K_{p}=\frac{|C(i \omega)|}{\sqrt{1+\alpha^{2}\omega^{2}}}=\frac{1}{|P(i \omega_{c})|\sqrt{1+\alpha^{2}\omega_{c}^{2}}}$$
Now that we know both $\alpha$ and $K_{p}$ we can easily calculate $K_{D}$.


