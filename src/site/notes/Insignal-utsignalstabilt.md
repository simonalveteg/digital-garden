---
{"dg-publish":true,"permalink":"/insignal-utsignalstabilt/","tags":["digitalsignalbehandling","systemochtransformer"]}
---


$S$ kallas insignal-utsignal [[Stabila och Instabila System\|stabil]] om varje begränsad insignal ger upphov till en begränsad utsignal. dvs om $S(w(t))$ är begränsad då $w(t)$ är begränsad. $|w(t)|\leq C$ för alla $t$ ($C$ är en konstant).

För linjära [[Tidsinvarianta System\|tidsinvarianta system]] finns det ett enkelt stabilitetskriterium.
$$S\text{ är insignal-utsignalstabilt} \Leftrightarrow \int_{-\infty}^{+\infty}|h(t)|dt \text{ är konvergent}$$

In discrete-time a [[Kausala System\|causal]] [[Linjära och Tidsinvarianta System\|LTI system]] is [[Insignal-utsignalstabilt\|BIBO stable]] if and only if all the poles are inside the unit circle in the Z-plane.