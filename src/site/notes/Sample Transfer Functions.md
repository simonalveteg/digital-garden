---
{"dg-publish":true,"permalink":"/sample-transfer-functions/","tags":["reglerteknik"]}
---

All [[Överföringsfunktion\|transfer functions]] can be factored into five different sample [[Överföringsfunktion\|transfer functions]].

$G_{1}=K$
$G_{2}=s^{n}$
$G_{3}=(1+sT)^{n}$
$G_{4}=(1+2\zeta \frac{s}{\omega_{0}}+ \frac{s^{2}}{\omega_{0}})^{n}$ 
$G_{5}=e^{-sL}$
where $K, T, \zeta, \omega_{0}$ and $L$ are real numbers and $n$ is an integer.

## [[Bode plot\|Bode plot]] of $G(s)=K$
$$log|G(i \omega)|=logK$$
$$argG(i \omega)=0$$
both the [[Förstärkning\|gain]] and [[Argument\|argument]] are independent of the frequency $\omega$, and is thus made up by two horizontal lines.
![Pasted image 20220904104345.png|400](/img/user/images/Pasted%20image%2020220904104345.png)
## [[Bode plot\|Bode plot]] of $G(s)=s^{n}$
The magnitude and [[Argument\|argument]] of the [[Överföringsfunktion\|transfer function]] above are given by
$$log|G(i \omega)|=log|i \omega|^{n}=nlog \omega$$
$$\arg G(i \omega)=n\arg(i \omega)=n \frac{\pi}{2}$$
The magnitude is a straight line with slope n (due to the logarithmic scales). The [[Argument\|argument]] is independent of $\omega$ and thus forms a horizontal line.
![Pasted image 20220904105007.png|400](/img/user/images/Pasted%20image%2020220904105007.png)

## [[Bode plot\|Bode plot]] of $G(s)=(1+sT)^{n}$
$$log|G(i \omega)|=log|1+i \omega T|^{n}=nlog \sqrt{1+\omega^{2}T^{2}}$$
$$\arg G(i \omega)=n\arg(1+i \omega T)=n \cdot arctan(\omega T)$$
For small frequencies the functions are given by 
$$log|G(i \omega)| \rightarrow 0$$
$$\arg G(i \omega) \rightarrow 0$$
For large frequencies:
$$\log |G(i \omega)|\rightarrow n\log \omega T$$
$$\arg{G(i \omega)}\rightarrow n \frac{\pi}{2}$$
These two asymptotes are shown in the image below. The intersection between the low and high frequency asymptotes is given by $\log \omega T=0$ and is called the corner frequency (brytfrekvens) and is given by $\omega=\frac{1}{T}$.
![Pasted image 20220904105224.png|400](/img/user/images/Pasted%20image%2020220904105224.png)
## [[Bode plot\|Bode plot]] of $G(s)=(1+2 \zeta s/\omega_{0}+ (s/\omega_{0} )^{2})^{n}$

The low frequency asymptotes are given by $G(i \omega)\approx 1$
$$log|G(i \omega)| \rightarrow 0$$
$$\arg G(i \omega) \rightarrow 0$$
for large frequencies it's given by $G(i \omega)\approx(i \omega/\omega_{0})^{2n} =(-1)^{n}(\omega/\omega_{0}) ^{2n}$
$$\log |G(i \omega)| \rightarrow2n\log \frac{\omega}{\omega_{0}}$$
$$\arg{G(i \omega)}\rightarrow n\pi$$
asymptotes are shown in the image below with some different values of the parameter $\zeta$.
![Pasted image 20220904110444.png|400](/img/user/images/Pasted%20image%2020220904110444.png)
## [[Bode plot\|Bode plot]] of $G(s)=e^{-sL}$
This [[Överföringsfunktion\|transfer function]] describes a pure time delay. This means that the output is identical to the input exept that it has been delayed by a time L. The amplitude is therefore zero and the [[Argument\|argument]] is $-\omega L$.