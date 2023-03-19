---
{"dg-publish":true,"permalink":"/distributionsderivata/","tags":["systemochtransformer"]}
---


> **Alla** [[Distributioner\|distributioner]] är deriverbara, genom
> $$<\mathcal{U}',\varphi> = <\mathcal{U},-\varphi'>$$
> för alla testfunktioner $\varphi$ (kan härledas mha [[Partial Integration\|Partial Integration]]).

1. $(c_{1}\mathcal{U}+c_{2}\mathcal{V})'=c_{1}\mathcal{U}'+c_{2}\mathcal{V}'$
2. $(f(t)\mathcal{ U})'=f'(t)\mathcal{U}+f(t)\mathcal{U}'$ för alla $f(t)\in C^\infty(\mathbb{R})$ och alla [[Distributioner\|distributioner]]  $\mathcal{ U}$
3. $<f(t)\mathcal{U,\varphi>=<\mathcal{U},f(t)\varphi>}$



Antag att $f(t)$ har en språngpunkt i brytpunkten $a$ 
![Pasted image 20220410120445.png](/img/user/images/Pasted%20image%2020220410120445.png)
skriver vi
$$\begin{cases} f_{1}(t) , t\leq a \\
f_{2}(t),t>a \end{cases}$$
då är derivatan
$$f'(t)=\begin{cases}f'_{1}(t) \text{ då } t\leq a \\\\
f'_{2}(t)\text{ då }t>a \end{cases}\space+(f_{2}(a+0)-f_{1}(a-0))\delta_{a}$$
dvs derivatan plus “språnget” gånger [[Delta Funktionen\|deltafunktionen]]. Derivatan vid varje intervall, plus ökningen i språnget (skillnaden i höjd gånger [[Delta Funktionen\|deltafunktionen]]) för varje brytpunkt!

[[Samband mellan stegfunktion och deltafunktion\|Samband mellan stegfunktion och deltafunktion]]