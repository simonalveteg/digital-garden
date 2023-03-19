---
{"dg-publish":true,"permalink":"/sammansatta-system/","tags":["systemochtransformer"]}
---

En insignal $w$ skickas in i ett [[System (matematisk definition)\|System (matematisk definition)]] $S_{1}$, som har en utsignal $S_{1}(w(t))$, som skickas in som en insignal till ett annat [[System (matematisk definition)\|System (matematisk definition)]] $S_{2}$, som får en utsignal $S_{2}(S_{1}(w(t)))$. Då har $S_{1}$ seriekopplats med $S_{2}$; ($S_{2}\circ S_{1}$) där $w$ är insignal och $S_{2}(S_{1}(w(t)))$ är utsignalen. Det är helt analogt med avbildningar!

$$S_{2}\circ S_{1}(w(t))=S_{2}(S_{1}(w(t)))$$
Om $S_{1}$ och $S_{2}$ är [[Linjära och Tidsinvarianta System\|linjärt tidsinvarianta]] med [[Impulssvar\|impulssvaren]] $h_{1}(t)$ och $h_{2}(t)$ så är $S_{2}\circ S_{1}$ också [[Linjära och Tidsinvarianta System\|linjärt tidsinvariant]] med [[Impulssvar\|impulssvaret]] $h_{2}*h_{1}$ (se [[Faltning\|Faltning]]).
