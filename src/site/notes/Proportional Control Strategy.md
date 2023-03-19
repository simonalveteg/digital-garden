---
{"dg-publish":true,"permalink":"/proportional-control-strategy/","tags":["reglerteknik"]}
---

![Pasted image 20220829163431.png](/img/user/images/Pasted%20image%2020220829163431.png)
#question vad är K och I?

The big weakness of proportional controller is that they often introduce [[Stationary Error\|stationary errors]] 

example:
![Pasted image 20220829163932.png](/img/user/images/Pasted%20image%2020220829163932.png)
In this example K is a proportional controller. 
$$y=K_{p}Ke=K_{p}K(r-y)$$
om vi bryter ut y får vi
$$y=\frac{K_{p}K}{1+K_{p}K}r$$
Man vill att $y=r$ men då måste $K_{p}K \rightarrow \infty$ vilket ger samma sak som en [[OnOff Control Strategy\|On/Off Control Strategy]], vilket inte är bra då man får samma problem med oscillationer.