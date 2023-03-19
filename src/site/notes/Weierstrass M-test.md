---
{"dg-publish":true,"permalink":"/weierstrass-m-test/","tags":["funktionsteori"]}
---

Anta att $u_{k}(x)$ är en följd av reell- eller komplexvärda funktioner på en mängd $D$. Om $|u_{k}(x)|\leq M_{k}$ och $\sum\limits_{k=1}^{\infty}M_{k}$ [[Konvergens\|konvergerar]] så [[Konvergens\|konvergerar]] [[Funktionsserier\|funktionsserien]]  $\sum\limits_{k=1}^{\infty}u_{k}(x)$ [[Likformig konvergens\|likformigt]] på D.

Man väljer alltså ett $M_{k}$ som är större än $|u_k|$. Om $M_k$ [[Konvergens\|konvergerar]] måste då även $u_k$ göra det.

testet är **inte** omvändbart. 
___
bevis:
$$
|r_{n}(x)|=\left|\sum\limits_{k=n+1}^{\infty}u_{k}(x)\right| \leq\sum\limits_{k=n+1}^{\infty}|u_{k}(x)|\leq\sum\limits_{k=n+1}^{\infty}M_{k}
$$
för alla $x\in D$, dvs
$$
||r_{n}||\leq\sum\limits_{k=n+1}^{\infty}M_k
$$
