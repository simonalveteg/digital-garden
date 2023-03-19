---
{"dg-publish":true,"permalink":"/impulssvar/","tags":["systemochtransformer"]}
---

Om $S$ är [[Linjära och Tidsinvarianta System\|linjärt och tidsinvariant]] ([[Linjära och Tidsinvarianta System\|LTI]]) är impulssvaret $k(t,\tau)=h(t-\tau)$, där $h$ är någon [[Distributioner\|generaliserad funktion]] av en variabel 
$$S(w)=\int_{-\infty}^{\infty}h(t-\tau)w(\tau)d \tau$$
$S$ är [[Linjära och Tidsinvarianta System\|linjärt tidsinvariant]] $\Rightarrow$ 
$$S(\delta(t))=h*\delta=\int_{-\infty}^{\infty}h(t-\tau)\delta(\tau)d \tau=h(t-0)*1=h(t)$$
för ett [[Linjära och Tidsinvarianta System\|linjärt tidsinvariant system]] ges alltså motsvarande impulssvar av att skicka in [[Delta Funktionen\|delta funktionen]] i [[System (matematisk definition)\|systemet]]! 

If you take the laplace transform of the impulse response you get the [[Överföringsfunktion\|transfer function]]!
