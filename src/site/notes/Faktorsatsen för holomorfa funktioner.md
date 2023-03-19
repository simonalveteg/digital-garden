---
{"dg-publish":true,"permalink":"/faktorsatsen-foer-holomorfa-funktioner/","tags":["funktionsteori"]}
---

Anta att $f$ är [[Holomorf\|holomorf]] på $\Omega$. Om $\alpha\in\Omega$ så att $f(\alpha)=0$, då finns en [[Holomorfa Funktioner\|holomorf funktion]] $g$ sådan att 
$$f(z)=(z-a)g(z)$$
för [[Polynom\|polynom]] blir graden för $g$ ett mindre än graden för $f$.

Tänk att man tittar på funktionens [[Potensserier\|potensserie]] och bryter ut något från varje term.

## Exempel: $sinz$
$sinz$ har ett enkelt nollställe i $z=0$. Ur Maclaurinserie för $sinz$ ser vi att
$$sinz=z-\frac{z^{3}}{3!}+ \frac{z^{5}}{5!}+...=z\left(1- \frac{z^{2}}{3!}+ \frac{z^{4}}{5!}+...\right)=zg(z)$$
Vi kan bryta ut ett $z$ men inte ett $z^{2}$. Det betyder att $sinz$ har ett *enkelt nollställe* i $z=0$. Även om det ser ut som att $\frac{sinz}{z}$ skulle ha en [[Singularitet\|singularitet]] i $z=0$, är det faktskt inte så. [[Singularitet\|Singularitet]] är *hävbar*.

## Se också
[[Satsen om isolerade nollställen\|Satsen om isolerade nollställen]]

