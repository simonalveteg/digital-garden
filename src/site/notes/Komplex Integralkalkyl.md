---
{"dg-publish":true,"permalink":"/komplex-integralkalkyl/","tags":["funktionsteori"]}
---

Enklaste varianten av komplexa integraler:
Ta en funktion $f: R \rightarrow C$, $f(t) = e^{it}$ 

Där $f(t) = u(t) + iv(t)$. Då definierar vi integralen
$$\int_{a}^{b}f(t)dt=\int_{a}^{b}u(t)dt+i\int_{a}^{b}v(t)dt$$med andra ord integrerar man realdelen och imaginärdelen för sig. Men man kan ta fram en primitiv funktion direkt utan att dela upp i real och imaginärdelar. De vanliga räknereglerna för integraler gäller även i det komplexa fallet. 

En komplexvärd funktion av en reell variabel kan man se som en [[Parametrisering\|Parametrisering]] av en kurva i det komplexa planet. Man kan därmed räkna ut dess [[Kurvintegraler\|Kurvintegraler]].

![Pasted image 20220221115732.png](/img/user/images/Pasted%20image%2020220221115732.png)
Om $F$ är en primitiv till $f$ på $\Omega$ och $\gamma$ är en kurva i $\Omega$, så
$$
\int_{\gamma}f(z)dz=F(b)-F(a)
$$
Om $\gamma$ är sluten är $\int_{\gamma}f(z)dz=0$

[[Cauchys Integralsats\|Cauchys Integralsats]]
[[Cauchys Integralformel\|Cauchys Integralformel]]