---
{"dg-publish":true,"permalink":"/distributioner/","tags":["systemochtransformer"]}
---

Kallas också generaliserade funktioner. I många tillämpningar räcker inte vanliga funktioner till.

vi inför ett begrepp testfunktioner

Låt $\mathcal{D}$ vara mängden av alla testfunktioner $\varphi(t)$ som uppfyller
1. $\varphi(t)\in C^{\infty}(\mathcal{R})$, dvs den kan deriveras oändligt många gånger.
2. $\varphi(t)$ har ett kompakt stöd, dvs $\varphi(t)=0$ utanför ett slutet intervall i $\mathcal{R}^{2}$ 

En distribution är en [[Linjär Avbildning\|linjär]], kontinuerlig avbildning $\mathcal{U}$ som avbildar varje testfunktion $\varphi(t)$ i $\mathcal{D}$ på ett tal 
$$\mathcal{U}(\phi)= \space <\mathcal{U},\varphi>$$
obs: Linjär $\Leftrightarrow \mathcal{U}(c_{1}\varphi_{1}(t)+c_{2}\varphi_{2}(t)=c_{1}\mathcal{U}(\varphi_{1}(t))+c_{2}\mathcal{U}(\varphi_{2}(t))$ 
obs: Kontinuerlig $\Leftrightarrow$ om $\phi$ är liten blir $\mathcal{U}(\varphi)$ också litet
$$<\mathcal{U},\varphi> = \int_{-\infty}^{\infty}\mathcal{U}(t)\varphi(t)dt$$där $\mathcal{U}(t)$ saknar betydelse i många fall, den beror ju inte på $t$ egentligen, men det är användbart för att man då kan skriva den som en integral?

Om vi har två distributioner $\mathcal{U}$ och $\mathcal{V}$ så är alla deras [[Linjärkombination\|linjärkombinationer]] $c_{1}\mathcal{U}+c_{2}\mathcal{V}$ också distributioner. 

$\mathcal{UV}$ behöver inte vara definierad för alla distributioner $U,V$. 
$f(t)\in C^\infty(\mathbb{R})$, $\mathcal{U}$ är distribution $\Rightarrow f(t)\mathcal{U}$ är en distribution. Dvs en distribution får multipliceras med en funktion som är oändligt många gånger deriverbar.
$$<f(t) \mathcal{U}, \varphi(t)> = < \mathcal{U}, f(t)\varphi(t)>$$
dvs 
$$\int_{-\infty}^{\infty}f(t)\mathcal{U}\varphi(t)dt=\int_{-\infty}^{\infty}\mathcal{U}f(t)\varphi(t)dt$$
där $f(t)\varphi(t)$ är en ny testfunktion.


$\theta(t)^{2}$ och $\theta(t)\delta(t)$ är ej definierade!

[[Distributionsderivata\|Distributionsderivata]]
[[Primitiv distribution\|Primitiv distribution]]
[[Konvergens av distributioner\|Konvergens av distributioner]]
