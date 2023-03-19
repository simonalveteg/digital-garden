---
{"dg-publish":true,"permalink":"/aliasing/","tags":["mätteknik","digitalsignalbehandling"]}
---

Aliasing is when contributions from repeated copies of the [[Signal\|signal]] appear inside the main period of $X(f)$?

If our analog signal has information outside of $\pm \frac{F_{s}}{2}$ we will get aliasing
![Pasted image 20220926134818.png](/img/user/images/Pasted%20image%2020220926134818.png)
which leads us to the [[Nyquists Samplingskriterium\|nyquist sampling theorem]]!

Vikningsdistortion är när [[Sampling Period\|samplingsfrekvensen]] är för låg i förhållande till insignalen så att man får en falsk kurvåtergivning. Är man inte medveten om undersamplingen kan man luras att tro att den återgivna [[Signal\|signalen]] är korrekt.
![vikningsdistortion.png](/img/user/images/vikningsdistortion.png)
Vikningsdistortion kan undvikas genom att lågpassfiltrera ingångssignalen, så att inga [[Signal\|signaler]] som är högre än halva [[Sampling Period\|samplingsfrekvensen]] slipper igenom. [[Anti-Aliasing Filter\|Anti-Aliasing Filter]].

See also → [[Anti-Aliasing Filter\|Anti-Aliasing Filter]]
