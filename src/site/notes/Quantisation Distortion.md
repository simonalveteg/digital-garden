---
{"dg-publish":true,"permalink":"/quantisation-distortion/","tags":["kommunikationssystem"]}
---

Vi kan inte använda oändligt många bitar vid [[Digitization of analog signals\|Digitization of analog signals]], vilket hade behövts för att få med all information av den analoga signalen. Därför kommer det alltid att uppstå ett kvantiseringsfel.

$$
SQNR = \frac{P_\text{signal}}{P_\text{noise}}
$$

Average distortion for uniform input
$$
E\left[ (X-X_Q)^{2} \right] =\int_{-\Delta/2}^{\Delta/2}x^{2} \frac{1}{\Delta}  \, dx = \frac{\Delta}{12}
$$
Signal to quantisation noise ratio
$$
SQNR = \frac{E\left[ X^{2} \right]}{E\left[ (X-X_Q)^{2} \right] }=\frac{(M\Delta)^{2}/12}{\Delta^{2}/12}=M^{2}=2^{2k}
$$
$$
SQNR_{dB}=10\log2^{2k}=k\cdot6dB
$$
Med hjälp av denna ekvationen kan man hjälpa felet vi gör med annat brus i systemet (Signal to noise ratio). Ekvationen visar alltså kvantiseringsfelet som en funktion av antal bitar vi använder. På så sätt kan vi se till att kvantiseringsfelet blir försumbart.