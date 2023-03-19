---
{"dg-publish":true,"permalink":"/constant-coefficient-difference-equations/","tags":["digitalsignalbehandling"]}
---


Constant coefficient difference equations describe [[Linjära och Tidsinvarianta System\|LTI systems]]. 
![Pasted image 20221010132946.png](/img/user/images/Pasted%20image%2020221010132946.png)

[[Stabila och Instabila System\|Stability]] is an important property, but showing that these systems are [[Insignal-utsignalstabilt\|BIBO stable]] using the definition is typically very difficult, but can be done more efficiently using the [[Z-transform\|Z-transform]].


The block diagram for a [[System (matematisk definition)\|System (matematisk definition)]] described with constant coefficient difference equations can look like this:
![Pasted image 20220831100323.png](/img/user/images/Pasted%20image%2020220831100323.png)
$$y(n)=ay(n-1)+x(n)$$
where the output consists of the [[Zero-state response\|Zero-state response]] and the [[Zero-input response\|Zero-input response]]. 
> The number of previous output values $N$ we need to be able to compute the current output is called the **order** of the [[System (matematisk definition)\|System (matematisk definition)]].
