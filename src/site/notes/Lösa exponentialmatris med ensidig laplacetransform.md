---
{"dg-publish":true,"permalink":"/loesa-exponentialmatris-med-ensidig-laplacetransform/","tags":["systemochtransformer"]}
---

Om vi laplacetransformerar 
$$\mathcal{L}(e^{at}\theta(t))(s)=\mathcal{L}(\theta(t))(s-a)=\frac{1}{s-a}$$
där A är en [[Matris\|matris]]. Att [[Laplacetransformationer\|laplacetransformera]] en [[Matris\|matris]] innebär att [[Laplacetransformationer\|laplacetransformera]] varje element. Det ger oss ett annat sätt att beräkna [[Exponentialmatriser\|Exponentialmatriser]]
$$e^{At}\theta(t)=\mathcal{L}^{-1}_\text{kausal}\left((sI-A)^{-1}\right)$$
standardmetoden är att diagonalisera A, men om A inte är [[Diagonalisering\|diagonaliserbar]] kan man använda denna metod. Det är jobbigt att [[Laplacetransformationer\|laplacetransformera]] varenda element, så metoden med [[Diagonalisering\|diagonalisering]] är att föredra.