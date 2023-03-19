---
{"dg-publish":true,"permalink":"/maximal-flat-frekvensgang/","tags":["analogelektronik"]}
---


Ett vanligt önskemål är att [[Förstärkning\|förstärkningen]] skall vara lika för alla frekvenser hos [[Signal\|signalen]]. Detta stämmer när [[Systempoler\|systempolerna]] ligger i [[Butterworthposition\|Butterworthposition]]

$$A \beta(s)=A \beta(0) \frac{1}{1+\frac{s}{(\omega_{0})^{n}}}$$
alla [[Poler\|poler]] ges av $1+(\frac{s}{\omega_{0}})^{n}=0$ , skriv om s på [[Polär form\|polär form]] - alla [[Poler\|poler]] kommer ligga på en halvcirkel i vänster halvplan, där radien är lika med [[Bandbredd\|bandbredden]]. Vinkeln mellan alla [[Poler\|poler]] ges av $\theta=\frac{k\pi}{n}$. För att [[System (matematisk definition)\|systemet]] ska bli [[Stabila och Instabila System\|stabilt]] behöver man ibland flytta [[Poler\|polerna]] längs cirkelns omkrets så att [[System (matematisk definition)\|systemet]] blir [[Stabila och Instabila System\|stabilt]]. Det görs via [[Frekvenskompensering\|Frekvenskompensering]]

[[Hur frekvenskompensering kan påverka rotorten - MFM system\|Hur frekvenskompensering kan påverka rotorten - MFM system]]

By converting our [[System (matematisk definition)\|System (matematisk definition)]] to a butterworthsystem we can find the ideal [[Systempoler\|system poles]] (if we want maximum flat magnitude)

If our [[System (matematisk definition)\|System (matematisk definition)]] is a second order [[System (matematisk definition)\|System (matematisk definition)]]:
$$p_{1,2}'=-\frac{\omega_{0}}{\sqrt{2}}(1\pm j) \Rightarrow \sum\limits p'=-\sqrt{2}\omega_{0}$$
![2nd order mfm system.png|350](/img/user/images/2nd%20order%20mfm%20system.png)
(ska stå 45 grader)
If our [[System (matematisk definition)\|System (matematisk definition)]] is a third order [[System (matematisk definition)\|System (matematisk definition)]]:
$$\begin{cases} p_{1}'= -\omega_{0}   \\ p_{2,3}'=-\omega_{0}\left( \frac{1}{2}\pm j\frac{\sqrt{3}}{2} \right)
\end{cases}\space\space\space \Rightarrow \sum\limits p'=-2\omega_{0}
$$
![3rd order mfm system.png](/img/user/images/3rd%20order%20mfm%20system.png)
(här är det 60 grader 🤡)