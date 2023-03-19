---
{"dg-publish":true,"permalink":"/geometriska-serier/","tags":["funktionsteori"]}
---

$$a_{k}=Cr^{k}$$där C och r är konstanter. 

Multiplicera $s_N$ med r. $s_{N}$ och $rs_{N}$ blir nästan lika, om man subtraherar $s_N-rs_{N}=Cr^{0}-Cr^{N+1}=C(1-r^{N+1})$ dvs $s_{N}=C(\frac{1-r^{N+1}}{1-r})$. När $N\rightarrow\infty$ går summan mot oändligheten om $|r|>1$. Om $|r|<1$ så går $r^{N+1}$ mot oändligheten och summan får ett gränsvärde $\frac{C}{1-r}$. Om $|r|=1$ kommer den snurra runt på enhetscirklen och inte ha ett gränsvärde.

> VIKTIGT OCH ÅTERKOMMANDE EXEMPEL!!!

**Minnesregel**: Summan av en [[Konvergens\|konvergent]] geometrisk serie är första termen delat med 1-r. 
$$s_{N} = \frac{a_{0}}{1-r}$$
