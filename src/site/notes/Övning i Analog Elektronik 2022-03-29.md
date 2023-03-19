---
{"dg-publish":true,"permalink":"/oevning-i-analog-elektronik-2022-03-29/","tags":["övning","analogelektronik"]}
---



# 2-pole [[System (matematisk definition)\|System (matematisk definition)]]

$$A \beta(s)=\frac{N(s)}{P(s)}$$
zeroes of [[Slingförstärkning\|loop gain]] are exactly the zeroes of [[System (matematisk definition)\|System (matematisk definition)]], but poles are different. [[Systempoler\|System poles]] are written $p_{1}',p_{2}'$ while [[Slingpoler och Slingnollställen\|loop gain poles]] are written $p_{1},p_{2}$. 
![Pasted image 20220329152059.png|400](/img/user/images/Pasted%20image%2020220329152059.png)
we have no zeroes. If the number of poles is greater than the number of explicit zeroes..

the [[Slingförstärkning\|loop gain]] goes to zero as as s approaches infinity. But how does it go to zero? Det är därför vi undersöker [[Poler\|poler]] och [[Nollställen\|nollställen]]

n=number of poles
m=number of explicit zeros.

n-m is the number of asymptotes. Vinkeln mellan dessa ges av $\frac{\pi}{n-m}+(2l-1) \frac{\pi}{n-m}$
$$\begin{cases} \frac{pi}{2}\\\\ \frac{3\pi}{2} \end{cases}$$
![Pasted image 20220329152733.png|400](/img/user/images/Pasted%20image%2020220329152733.png)
but where do the asymptotes intersect? “canonical point?”

The interception point är mitt mellan p_1 och p_2 enligt funktionen
$$0= \frac{\sum\limits p-\sum\limits n}{n-m} \rightarrow \frac{p_{1}+p_{2}}{2}$$


explicit zero is a zero that we can see in the [[Överföringsfunktion\|transfer function]]

two poles => three traces, one pole => two traces. Traces är [[Rotort\|rotorten]]? 

när vi fändrar [[DC-slingförstärkning\|DC-loop-gain]] $A \beta(0)$ förflyttas [[Systempoler\|systempolerna]] längs [[Rotort\|rotorten]]

när man är i en [[Poler\|pol]] är [[DC-slingförstärkning\|DC-loop gain]] 0. 







## Subject
[[Analog Elektronik\|Analog Elektronik]]
