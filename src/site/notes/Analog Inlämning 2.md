---
{"dg-publish":true,"permalink":"/analog-inlaemning-2/","tags":["inlämning","analogelektronik"]}
---

1.

2.
$$
\begin{gather}
A=\frac{Q_{c}}{Q_{i}}=\frac{i_{c}}{V_{1}}\\
V_{2}=-g_{m1}V_{1}r_{\pi2} \\
V_{3}=g_{m2}V_{2}r_{\pi3}=-g_{m1}g_{m2}r_{\pi2}r_{\pi3}V_{1} \\
i_{c}=\frac{v_{3}}{r_{pi3}}+g_{m3}+v_{3}=\frac{g_{m}}{2}V_{1}\beta_{f}(1+\beta_{f}) \\
\Rightarrow A=-\frac{g_{m1}}{2}\beta_{f}(1+\beta_{f})  \\
\beta=\left.\frac{Q_{i}}{Q_{c}}\right\vert_{Q_{g}=0}=\frac{V_{1}}{i_{c}} \\
i_{c1}=\frac{R_{L}}{R_{L}+R_{2}+r_{\pi1}'}i_{c} \\
v_{1}=r_{\pi1}'i_{c1}=\frac{R_{L}r_{\pi1}'}{R_{L}+R_{2}+r_{\pi1}'}i_{c} \\
\Rightarrow \beta=\frac{R_{L}r_{\pi1}}{R_{L}+R_{2}+r_{\pi1}'} \\
\Rightarrow A\beta=-\frac{g_{m1}}{2}\beta_{f}(1\beta_{f})\frac{R_{L}r_{\pi1}'}{R_{L}+R_{2}+r_{\pi1}'}=-\frac{\beta_{f}^{2}(1+\beta_{f})R_{L}}{2\cdot20050} \\
\end{gather}
$$


3.
$$
\begin{gather}
A \beta=-\frac{\beta_{f}^{2}(1+\beta_{f})R_{L}}{2\cdot20050} \\ \Leftrightarrow r_{\pi1}=\frac{1}{2}\left( \frac{\beta_{f}^{2}(1+\beta_{f})R_{L}}{20050}-R_{L}-R_{2} \right) \\ 
\Rightarrow r_{pi1}=9999.9\Omega \\
i_{c}=\frac{\beta_{f}V_{T}}{r_{pi1}}=0.5mA
\end{gather}
$$
4.
$$
1-\frac{A_{t}}{A_{t\infty}}=1-\frac{-A\beta}{1-A\beta}=1-0.99995=0.005\%
$$