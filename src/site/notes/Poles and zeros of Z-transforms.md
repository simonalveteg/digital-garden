---
{"dg-publish":true,"permalink":"/poles-and-zeros-of-z-transforms/","tags":["digitalsignalbehandling"]}
---

The [[Region of convergence\|region of convergence]] cannot contain any poles, since poles go to infinity and therefore do not converge. Since the unit circle roughly corresponds to the left hand [[Laplace-planet\|s-plane]] the pole placement in the z-plane affects the [[Stabila och Instabila System\|stability]] in a similar way
![Pasted image 20220907092402.png](/img/user/images/Pasted%20image%2020220907092402.png)
![Pasted image 20220907093509.png](/img/user/images/Pasted%20image%2020220907093509.png)
![Pasted image 20220907093519.png](/img/user/images/Pasted%20image%2020220907093519.png)

Poles inside the unit circle make the [[Signal\|signal]] vanish with time
poles outside the unit circle make the [[Signal\|signal]] grow with time
conjugate poles inside the unit circle correspond to an oscillation that declines with time
conjugate poles outside the unit circle correspond to an oscillation that amplifies with time.

We say that a [[Kausala Signaler\|causal signal]] is [[Stabila och Instabila System\|stable]] if all its poles are inside then unit circle.

A zero close to the unit circle will attenuate $X(\omega)$ near its location. The closer the stronger the [[Attenuation\|attenuation]]. 
A pole close to the unit circle will amplify $X(\omega)$ near its location, the close the stronger the [[Förstärkning\|amplification]].
Since poles and zeros have the opposite effect they can cancel each others influence. Entirely if in same location and "almost" if they are relatively close.
To achieve a [[Insignal-utsignalstabilt\|BIBO stable]] filter the poles need to be inside the unit circle (or on it for marginally [[Insignal-utsignalstabilt\|BIBO stable]]), while zeros can be anywhere.
If we want real-valued filter coefficients in $H(z)$ the complex-valued poles and zeros must come in conjugate pairs.