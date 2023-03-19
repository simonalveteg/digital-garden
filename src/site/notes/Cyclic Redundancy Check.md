---
{"dg-publish":true,"permalink":"/cyclic-redundancy-check/","tags":["kommunikationssystem"]}
---

Samma princip som i [[Checksum\|checksum]] att man lägger till extra bitar. 

Både sändare och mottagare är överens om ett generatorpolynom, $g(x)$, vilket används både för att generera och verifiera CRCn. Om man vill skicka ett dataord $x$ med $k$ bitar så representerar man det med ett [[Polynom\|polynom]] $d(x)$ av grad $k-1$. Kodordet $c(x)=d(x)\cdot x^{m}+r(x)$ är det som skickas till mottagaren, där $r(x)$ är resten av modulo-2 polynomdivisionen $\frac{d(x)\cdot x^m}{g(x)}$. Modulo-2 division innebär att $-x=x$ dvs man kan utföra divisionen med plus istället för minus. $x^k+x^k=0$. Resten $r(x)$ adderas alltså sedan på det ursprungliga dataordet förskjutet $k$ steg för att få kodordet $c(x)$ som skickas till mottagaren.

När mottagaren verifierar kodordet utför den polynomdivisionen $\frac{c(x)}{g(x)}$, vars rest blir noll om det inte har uppstått några bitfel.

# Standard CRC polynomials
![Pasted image 20230123162934.png](/img/user/images/Pasted%20image%2020230123162934.png)