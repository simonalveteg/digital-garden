---
{"dg-publish":true,"permalink":"/moduloraeknare-pa-hoegre-abstraktionsniva/","tags":["digitalteknik"]}
---

## Moduloräknare på högre [[Abstraktionsnivåer\|abstraktionsnivå]]
Konstruktion av mod-16 räknare med [[adderare\|adderare]], [[Register\|Register]] och [[mux\|mux]].
![Pasted image 20211101104826.png](/img/user/images/Pasted%20image%2020211101104826.png)

Gör en algoritm!
input: $r_1$, $r_2$
output: $Q$

```VHDL
if $r_1=0$ and $r_2=0$
	Q = 0
else if $r_1=1$ 
	if $r_2=1$
		Q+=1
	else
		Q+=3
else
	Q+=2
end
```
![Pasted image 20211101105534.png|300](/img/user/images/Pasted%20image%2020211101105534.png)
IF-satserna motsvaras av multiplexar! 
