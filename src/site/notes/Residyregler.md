---
{"dg-publish":true,"permalink":"/residyregler/","tags":["funktionsteori"]}
---

’Residyregel 1 
Om $f$ har en [[Poler\|pol]] av **ordning N** i $z=p$ så är
$$
Res_{z=\alpha}\left(\frac{g(z)}{(z-\alpha)^{N}}\right)=\frac{g^{(N-1)}(\alpha)}{(N-1)!}
$$
$$
Res_{z=p}(f)=\frac{1}{(N-1)!}\lim_{z \rightarrow p}\left(\frac{d^{(N-1)}}{dz^{(N-1)}}((z-p)^{N}f(z))\right)
$$

Residyregel 2
Om $f$ har en [[Poler\|pol]] av **ordning N** i $z=p$ så är
$$g(z)=\sum\limits_{k=0}^{\infty}c_{k}(z-p)^{k}\Rightarrow Res_{z=p}\left(\frac{g(z)}{(z-p)^{N}}\right)=c_{N-1}$$

Residyregel 3
Om f har en **enkelpol** i $z=p$ så är 
$$Res_{z=p}(f)=\lim_{z \rightarrow p}(z-p)f(z)$$
Residyregel 4
Om $f,g$ [[Holomorf\|holomorfa]] i en omgivning av $z=p$ och $f(p)\neq0$ och $g(p)=0$ där $p$ är ett **enkelt** [[Nollställen\|nollställe]] för $g(z)$ (alltså $g'(p)\neq0$) så är 
$$Res_{z=p}\left(\frac{f}{g}\right)=\frac{f(p)}{g'(p)}$$


Vilken av residyreglerna som är enklast att använda beror lite på hur funktionen ser ut.

För funktioner med enkla [[Poler\|poler]] ger residyregel 4 ofta de enklaste räkningarna