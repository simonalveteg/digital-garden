---
{"dg-publish":true,"permalink":"/lead-compensator/","tags":["reglerteknik"]}
---


Good for improving [[Förstärkning\|gain]] and [[Fasmarginal\|phase margins]], as welll as the speed of the response.

Generalisation of a PD-[[Control System\|controller]]

$$G_{K}(s)=K_{K}N \frac{s+b}{s+bN}=K_{K} \frac{1+ \frac{s}{b}}{1+ \frac{s}{bN}}$$
where $N>1$. We get two corner frequencies, one at $b$ and one at $bN$.

![lead compensators.png](/img/user/images/lead%20compensators.png)
the phase peaks at $\omega=b \sqrt{N}$.

As opposed to for a [[Lag compensator\|Lag compensator]] the positive phase allows us to rotate the [[Nyquist plot\|nyquist plot]] counter clockwise, which increases the [[Fasmarginal\|phase margin]].

$N$ tells us how much phase advance we get.
$b$ controls at what frequency that occurs. Usually we want this to occur at the [[Crossover Frequency\|crossover frequency]] $\omega_{c}=b \sqrt{N}$ 

the [[Förstärkning\|gain]] of the compensator at this frequency is $K_{K}\sqrt{N}$

The *maximum phase advance* is given by the figure below.
![Pasted image 20221003154016.png](/img/user/images/Pasted%20image%2020221003154016.png)


# Steps
1. Calculate new $\omega_{c}^*$
2. Find $\varphi_{m}$ for $G_{0}$
3. Calculate $\Delta \varphi_{m}$ and find $N$ from graph
4. Calculate $b$
5. Choose $K$ so that $\omega_{c}^{*}$ really becomes the cutoff frequency $$
\left| G_{K}(i\omega_{c}^{*})\cdot G_{0}(i\omega_{c}^{*}) \right|=1
$$ where $G_{K}=K_{K}\sqrt{ N }$

