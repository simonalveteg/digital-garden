---
{"dg-publish":true,"permalink":"/halvperiodutvecklingar/","tags":["funktionsteori"]}
---

Ibland vill man ha [[Trigonometriska Fourierserier\|Trigonometriska Fourierserier]] som bara innehåller cosinus- eller bara sinus-termer. 

Fourierserien för en udda periodisk funktion innehåller bara sinus-termer och en jämn innehåller bara cosinus-termer.

Om man **inte** börjar med en periodisk funktion:

Starta med en funktion $f$ som är definierad på intervallet $0<x<L$ för något $L>0$. 
![Pasted image 20220217143155.png|200](/img/user/images/Pasted%20image%2020220217143155.png)
Vi kan utvidga till en L-periodisk funktion
![Pasted image 20220217143232.png|200](/img/user/images/Pasted%20image%2020220217143232.png)
men denna kommer innehålla både sinus- och cosinus-termer.

Om vi bara vill ha cosinus-termer kan vi göra utvidgningen i *två* steg.
Definiera om intervallet till $-L<x<L$ och speglar funktionen i y-axeln 
![Pasted image 20220217143411.png|300](/img/user/images/Pasted%20image%2020220217143411.png)
då har vi gjort en **jämn utvidgning** av funktionen $f$ till $-L<x<L$.
I nästa steg utvidgar vi till en 2L-periodisk funktion
![Pasted image 20220217143517.png|350](/img/user/images/Pasted%20image%2020220217143517.png)
det blir en jämn funktion vars [[Trigonometriska Fourierserier\|trigonometriska Fourierserie]] endast kommer innehålla cosinus-termer! Vi kan sedan skita i vad som händer överallt förutom på startintervallet $0<x<L$. 

På motsvarande sätt fås “endast sinustermer”:
![Pasted image 20220217143812.png|300](/img/user/images/Pasted%20image%2020220217143812.png)
![Pasted image 20220217143829.png|350](/img/user/images/Pasted%20image%2020220217143829.png)

>Den udda speglingen introducerar en språngvis diskontinutet, vilket är varför den trigonometriska Fourierserie som endast innehåller cosinustermer ofta [[Konvergens\|konvergerar]] lite bättre. 