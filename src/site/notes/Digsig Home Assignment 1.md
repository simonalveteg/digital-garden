---
{"dg-publish":true,"permalink":"/digsig-home-assignment-1/","tags":["digitalsignalbehandling"]}
---


# 1
a) False. 
	A recursive system is [[Insignal-utsignalstabilt\|BIBO-stable]] if for every bounded input there is a bounded output, which is true when all the poles are inside the unit circle. 
b) True. 
	The [[Z-transform\|Z-transform]] plays the same role in the analysis of discrete-time signals as the laplace transform does for continuous-time signals. See formula 2.3.1 → 9 on page 16.
c) False. 
	A FIR filter has only has poles in the origin and a system is unstable if it has poles *outside* of the unit circle (in the Z-plane). A FIR filter is therefore always [[Stabila och Instabila System\|stable]].
d) False.
	The delay in samples is given by $\Delta=-\angle H(\omega)/\omega$ (see Lecture 8 slide 17). To get a result that is in samples it wouldn't make sense to multiply by the frequency, since the unit would be $[1/samples]$.
e) True.
	If the impulse response has conjugate-even or conjugate-odd symmetry around the midpoint the FIR filter has [[Linear phase\|linear phase]].
# 2
$$y(n)-y(n-1)+ \frac{4}{25}y(n-2)=x(n)$$
a)
![Pasted image 20221004143258.png](/img/user/images/Pasted%20image%2020221004143258.png)
b)
Performing the [[Z-transform\|z-transform]] gives
$$Y(z)-z^{-1}Y(z)+ \frac{4}{25}z^{-2}Y(z)=X(z)$$
which can be rewritten to
$$\frac{Y(z)}{X(z)}=\frac{1}{1-z^{-1}+ \frac{4}{25}z^{-2}}=\frac{z^{2}}{z^{2}-z+ \frac{4}{25}}$$
c)
The system has two zeros in $z=0$. The poles are given by the denominator
$$z^{2}-z+ \frac{4}{25}=0 \Rightarrow (z- \frac{4}{5})(z- \frac{1}{5})=0$$
![Pasted image 20221004144242.png|400](/img/user/images/Pasted%20image%2020221004144242.png)
d) 
The impulse response is given by the inverse [[Z-transform\|Z-transform]] of the system function $H(z)$. With [[Partialbråksuppdelning\|partial fraction expansion]] we can write
$$\frac{H(z)}{z}=\frac{z}{\left(z- \frac{4}{5}\right)\left(z- \frac{1}{5}\right)}= \frac{A}{\left(z- \frac{4}{5}\right)}+ \frac{B}{\left(z- \frac{1}{5}\right)}$$
$$\Rightarrow \begin{cases} A= \frac{4}{3}  \\
B=- \frac{1}{3} \end{cases}$$
$$H(z)= \frac{4z}{3(z- \frac{4}{5})}- \frac{z}{3(z- \frac{1}{5})}= \frac{4}{3(1- z^{-1}\frac{4}{5})}- \frac{1}{3(1- z^{-1}\frac{1}{5})}$$
so that we can use the formula sheet to perform the inverse transformation on page 17 (formula 18). The impulse response is then
$$h(n)=\frac{4}{3} \left(\frac{4}{5}\right)^{n}u(n)- \frac{1}{3} \left(\frac{1}{5}\right)^{n}u(n)$$
