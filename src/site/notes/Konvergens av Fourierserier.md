---
{"dg-publish":true,"permalink":"/konvergens-av-fourierserier/","tags":["funktionsteori"]}
---

Anta att $f\in L^{1}$ är [[Periodiska Funktioner\|T-periodisk]] och **begränad** dvs. att det finns ett tal M sådant att $|f(t)|\leq M$ för alla t. Då är
$$|c_{k}(f)|\leq M$$
där beviset följer direkt ur definitionen av $c_{k}$ och [[Triangelolikheten\|triangelolikheten]]. 
___ 
vi får ett intressantare resultat om vi kombinerar detta med räkneregeln $c_{k}(f')=ik\Omega c_{k}(f)$.

Om $f$ är $L^{1}$ och T-perodisk och $C^{m}$ (dvs funktionen $f$ och alla deras derivator av ordning $\leq m$ existerar). Då finns en konstant $C$, så att
$$|c_{k}(f)| \leq \frac{C}{|k|^{m}}$$ för $k\neq0$ . Ju större m vi kan ta desto fortare kan termerna gå mot noll
___
det leder till ett vettigt resultat:
> Om $f$ är $C^{2}$ och [[Periodiska Funktioner\|T-periodisk]] [[Konvergens\|konvergerar]] Fourierserien $f$ **[[Likformig konvergens\|likformigt]]** mot $f(t)$ på hela $\mathbb{R}$.

samma resultat gäller för [[Trigonometriska Fourierserier\|trigonometriska Fourierserier]], samt även om vi bara antar $f$ är $C^{1}$ (eller t.om om den är kontinuerlig och styckvis $C^{1}$). Om den [[Exponentiella Fourierserier\|exponentiella Fourierserien]] [[Konvergens\|konvergerar]] (ev absolut eller likformigt) så gäller samma sak för den [[Trigonometriska Fourierserier\|trigonometriska Fourierserien]] (men inte tvärt om!)