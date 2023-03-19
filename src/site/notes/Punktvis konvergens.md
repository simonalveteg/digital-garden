---
{"dg-publish":true,"permalink":"/punktvis-konvergens/","tags":["funktionsteori"]}
---

Anta att vi har en [[Funktionsföljder\|funktionsföljd]] $f_1,f_2,f_3,...$ definierad för $x\in D$. Då säger vi att ***[[Funktionsföljder\|funktionsföljden]] konvergerar punktvis*** mot $f$ om det för varje $x \in D$ gäller att *talföljden* $(f_n(p))$ [[Konvergens\|konvergerar]] mot $f(p)$.

Man får en [[Gränsfunktion\|gränsfunktion]] $f$
$$\lim_{k\rightarrow\infty}f_{k}(x)=f(x)$$
ofta skriver man detta mer kortfattat som $f_{n}\rightarrow f$. [[Gränsfunktion\|Gränsfunktionen]] behöver inte vara kontinuerlig även om [[Funktionsföljder\|funktionsföljden]] är det.

Gränsvärden kommuterar inte
$$\lim_{m\rightarrow\infty}\left(\lim_{n\rightarrow\infty}\frac{n}{n+m}\right) = 0$$
men
$$
\lim_{n\rightarrow\infty}\left(\lim_{m\rightarrow\infty}\frac{n}{n+m}\right) = 1
$$
