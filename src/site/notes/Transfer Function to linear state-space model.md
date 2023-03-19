---
{"dg-publish":true,"permalink":"/transfer-function-to-linear-state-space-model/","tags":["reglerteknik"]}
---

There are an infinite amount of ways to introduce state, which means that there is no one solution when converting a [[Överföringsfunktion\|transfer function]] to a [[Linear state-space model\|linear state-space model]].

Sätt $\dot{x_{1}}=\dot{y}=x_{2}$ och $\dot{x_{2}}=\ddot{y}$. Från den ursprungliga differentialekvationen kan man nu bryta ut $\ddot{y}$, och i det uttrycket sätta in $\dot{y}=x_{2}$. Men typ bättre att bara kolla i formelbladet nedan och trycka in värden på rätt ställe?


I formelbladet finns det a few different forms which the [[Linear state-space model\|linear state-space model]] can be written, with constants extracted from the [[Överföringsfunktion\|transfer function]] (written at the form at the bottom of the following image)
![Pasted image 20220831120008.png](/img/user/images/Pasted%20image%2020220831120008.png)
