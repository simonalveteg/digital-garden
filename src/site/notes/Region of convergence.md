---
{"dg-publish":true,"permalink":"/region-of-convergence/","tags":["digitalteknik"]}
---

The region of convegence of $X(z)$ is all z values for which it attains a finite value. 

## Finding the ROC
An arbitrary sequence/[[Signal\|signal]] $x(n)$
$$X(z)=\sum\limits_{-\infty}^{\infty}x(n)z^{-n}$$
the ROC is where $|X(z)|<\infty$
To find out when that is the case
![Pasted image 20220905133628.png](/img/user/images/Pasted%20image%2020220905133628.png)
Where the result consists of an [[Anti-kausal\|anti-causal]] and a [[Kausal\|causal]] part. Each of them converges to some region. The total ROC will be the intersection of both regions. In this case the first part only converges if $r$ is small enough and the second only converges if $r$ is big enough. If the intersection is empty the [[Z-transform\|Z-transform]] does not exist.

## Characteristic ROC shapes
The ROC of a [[Kausala Signaler\|causal signal]] is the outside of a circle of some radius $r_{2}$ while the ROC of a [[Anti-kausal\|anti-causal]] signal is the interior of a circle with some radius $r_{1}$. 
![Pasted image 20220905135141.png](/img/user/images/Pasted%20image%2020220905135141.png)