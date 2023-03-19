---
{"dg-publish":true,"permalink":"/rekursionsekvationer/","tags":["funktionsteori"]}
---

Rekursionsekvationer kallas ibland differensekvationer. Finns samband med [[Differentialekvationer\|Differentialekvationer]]. [[Differentialekvationer\|Differentialekvationer]] används i kontinuerliga sammanhang medan rekursionsekvationer används i diskreta sammanhang. Exempelvis används [[Differentialekvationer\|differentialekvationer]] ofta för att beskriva fysikaliska fenomen där tiden är en kontinuerlig variabel. 

## Linjära rekursionsekvationer av första ordningen
Går att skriva på formen
$$
a_{n+1}=g_{n}a_{n}+f_{n} \space,\space a_{0}=A
$$
lösningsformeln är
$$
a_{n}=g^{n}a_{0}+\sum\limits_{k=0}^{n-1}g^{n-1-k}f_{k}
$$
## Homogena Linjära Rekursionsekvationer (av andra ordningen)
[[Step by step lösning rekursionsekvation\|Step by step lösning rekursionsekvation]]. 
Den allmänna lösningen till en homogen andra ordningens rekursionsekvation med konstanta koefficienter,
$$
x_{n+2} + ax_{n+1} + bx_{n} = 0
$$
ges av
1. $x_{n}= C_{1}r_{1}^{n}+C_{2}r_{2}^{n}$ om [[den karakteristiska ekvationen\|den karakteristiska ekvationen]] har två olika lösningar $r_{1}\neq r_{2}$.
2. $x_{n}=C_{1}r_{1}^{n}+C_2nr_{1}^{n}$ om [[den karakteristiska ekvationen\|den karakteristiska ekvationen]] har en dubbelrot $r=r_1$.

## Inhomogena Linjära Rekursionsekvationer (av andra ordningen)
Om $x_{n}^{h}$ är den allmänna lösningen till motsvarande homogena ekvation och $x_{n}^{p}$ är en partikulärlösning, så ges den allmänna lösningen av 
$$x_{h}=x_{n}^{h}+x_{n}^{p}$$

## Se också:
[[Rekursion\|Rekursion]]