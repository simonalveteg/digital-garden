---
{"dg-publish":true,"permalink":"/final-value-theorem/","tags":["reglerteknik"]}
---

What does the final value appoach as time approaches infinity?
$$\lim\limits_{t \rightarrow \infty}f(t)=\lim\limits_{s \rightarrow0}sF(s)$$
Often times you already have the laplace transform $F(s)$ which makes this method very easy. 

Can't be used all the time,
![Pasted image 20220902165339.png](/img/user/images/Pasted%20image%2020220902165339.png)
If the [[System (matematisk definition)\|System (matematisk definition)]] has a pole in the right hand plane we know that it is unstable, and no final value exists. Using the final value theorem will give an answer that is **wrong**!!

If a pole exists on the imaginary axis the [[Impulssvar\|impulse response]] will be oscillatory (since $e$ raised to an imaginary number produces sinusoids). In this case the *mean* value of the oscillation, which isn't what we're going for.

If all poles exist in the left hand plane the [[Impulssvar\|impulse response]] is [[Stabila och Instabila System\|stable]] (since $e$ raised to a negative real number converges to zero). In this case the final value theorem will produce the correct answer. It will always be zero if all poles are in the left hand pane.


See also → [[Initial Value Teorem\|Initial Value Teorem]]

