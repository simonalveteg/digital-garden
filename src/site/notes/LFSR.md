---
{"dg-publish":true,"permalink":"/lfsr/","tags":["digitalteknik"]}
---


Ett linjärt återkopplat skiftregister är en kaskad av [[Minneselement\|Minneselement]] vars input är en linjär kombination (ges av [[återkopplingspolynom\|Återkopplingspolynom]])

The input of a Linear-feedback Shift Register is a [[linear function\|linear function]] of it's previous state. 

![Pasted image 20211026154648.png|400](/img/user/images/Pasted%20image%2020211026154648.png)

Ett LFSR med [[återkopplingspolynom\|Återkopplingspolynom]] [[återkopplingspolynom\|C(D)]] kan generera sekvensen $s$ endast om den kan skrivas
$$S(D) = \frac{P(D)}{C(D)}$$
där [[P(D)\|P(D)]] har **lägre** grad än [[återkopplingspolynom\|C(D)]]. 