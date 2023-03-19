---
{"dg-publish":true,"permalink":"/fyrkvadrantomvandlare/","tags":["elenergiteknik"]}
---

Om man kombinerar två stycken [[Tvåkvadrantomvandlare\|Tvåkvadrantomvandlare]] får man en omvandlare som kan arbeta i alla fyra [[Driftkvadranter\|Driftkvadranter]].

![Pasted image 20230208141714.png](/img/user/images/Pasted%20image%2020230208141714.png)

Transistorerna T1 och T2 är fortfarande varandras invers, och det samma gäller T3 och T4. De två bryggbenen kan däremot styras separat, och man behöver därför ett [[Setpoint\|börvärde]] till spänningen $u_a$ och en till $u_b$. Spänningen $u_{ut}$ som ligger över lasten är skillnaden mellan spänningarna på de två bryggbenen, dvs $u_{ut}=u_a-u_b$. Referenserna till bryggbenen väljs därför enligt
$$
\begin{align}
u_{a,ref}&=\frac{1}{2}u_{ut,ref} \\
u_{b,ref}&=-\frac{1}{2}u_{ut,ref} \\
\end{align}
$$
![Pasted image 20230208142132.png](/img/user/images/Pasted%20image%2020230208142132.png)
