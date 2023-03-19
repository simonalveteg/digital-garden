---
{"dg-publish":true,"permalink":"/trigonometriska-fourierserier/","tags":["funktionsteori"]}
---

$$\mathcal{FS}_{f}^{trig}(t)= c_{0}+\sum\limits_{k=1}^{\infty}(a_{k}cos(k\Omega t)+b_{k}sin(k\Omega t))$$
$c_{0}$ är samma som för [[Exponentiella Fourierserier\|Exponentiella Fourierserier]], $\Omega$ är vinkelfrekvensen. $a_{k}$ och $b_{k}$ kallas de ***trigonomtriska Fourierkoefficienterna*** till $f$ och kan beräknas enligt följande formel (finns i formelbladet)
$$
\large
\begin{cases}
a_{k}=\frac{2}{T}\int_{P}f(t)cos(k\Omega t)dt \\\\
b_{k}=\frac{2}{T}\int_{P}f(t)sin(k\Omega t)dt
\end{cases}
$$
dessutom gäller följande, som kan korta ner räkningar rejält:
1. Om $f$ är en **jämn** funktion så är $b_{k}=0$
2. Om $f$ är en **udda** funktion så är $a_{k}=0$
(kan kommas ihåg med följande minnesregel: $a_{k}$ är koefficienten framför sinustermerna. Sinus är en udda funktion. Om $f$ är jämn är koefficienten framför den udda funktionen 0)

dessutom gäller
$$a_{k}(f) =c_{k}(f)+c_{-k}(f)$$
$$b_{k}(f)=i(c_{k}(f)-c_{-k}(f))$$
dvs, om vi vet $c_{k}$ kan vi enkelt beräkna både $a_{k}$ och $b_{k}$ (lättare ibland)
$$\begin{cases}
c_{k}=\frac{1}{2}(a_{k}-ib_{k}) \\\\
c_{-k}=\frac{1}{2}(a_{k}+ib_{k})
\end{cases}$$

## De magiska satserna
Uppgifter på trigonometriska [[Fourierserier\|Fourierserier]] involver ofta en funktion som man på ett eller annat sätt måste rita upp och/eller visualiser aför att kunna räkna rätt. Oavsett hur funktionenn ser ut lär man dock behöva motivera sina räkningar med hjälp av följande satser. Detta måste göras **explicit** för att få helt rätt.

Om du arbetar med en funktion som är **kontinuerlig** i alla relevanta punkter så kan du direkt skriva *“funktionen uppfyller villkoren för sats 7.16 och dess trigonometriska Fourierserie [[Konvergens\|konvergerar]] således [[Likformig konvergens\|likformigt]] mot $f$ ”*

Om du arbetar med en funktion som innehåller **diskontinuitetspunkter** - dvs inte kontinuerlig - så måste du istället skriva *“funktionen uppfyller villkoren för sats 7.16 överallt utom i punkterna x,y,z. Sats 7.18 ger att funktionens trigonometriska Foruierserie antar medelvärdet av punkternas respektive höger- och vänstergränsvärden”*

Avgör själv om satsernas villkor är uppfyllda från fall till fall, det behöver inte redovisas i uppgifterna.

### Sats 7.16
Anta att $f\in L^{1}$ är [[Periodiska Funktioner\|T-periodisk]]. Om $t_{0}$ är en punkt sådan att
1. $f$ är **kontinuerlig** i punkten $t=t_{0}$
2. Höger- och vänsterderivatorna av $f$ existerar i punkten $t=t_{0}$ dvs. gränsvärdena
$\lim_{h \rightarrow0^{+}}\frac{f(t_{0}+h)-f(t_{0})}{h}$ och $\lim_{h \rightarrow0^{-}}\frac{f(t_{0}+h)-f(t_{0})}{h}$  
existerar (måste inte vara lika).
Då gäller att $\mathcal{FS}_{f}(t_{0})=\mathcal{FS}_{f}^{trig}(t_{0})=f(t_{0})$. (dvs [[Konvergens av Fourierserier\|Konvergens av Fourierserier]])

### Sats 7.18
> Om det finns en språngpunkt [[Konvergens\|konvergerar]] den trigonometriska Fourierserien mot medelvärdet mellan höger- och vänstergränsvärdena
Anta att $f\in L^{1}$ är [[Periodiska Funktioner\|T-periodisk]]. Om $t_{0}$ är en punkt sådan att 
1. Höger- och vänstergränsvärdena av $f$, dvs. $f(t_{0}+0)=\lim_{t \rightarrow t_{0}^{+}}f(t)$ och $f(t_{0}-0)=\lim_{t \rightarrow t_{0}^{-}}f(t)$ existerar (måste inte vara lika)
2. Gränsvärdena $\lim_{h \rightarrow 0^{+}}\frac{f(t_{0}+h)-f(t_{0}+0)}{h}$ och $\lim_{h \rightarrow 0^{-}}\frac{f(t_{0}+h)-f(t_{0})}{h}$ (dvs höger- och vänsterderivatorna) existerar (måste inte vara lika). Notera att vi inte sagt att $f$ måste vara kontinuerlig i $t=t_{0}$, så punkten behöver inte existera. Vi ersätter alltså $f(t_{0})$ med det motsvarande höger- respektive vänstergränsvärdet.

Då gäller att $\mathcal{FS}_{f}^{trig}(t_{0})=\frac{1}{2}(f(t_{0}+0)+f(t_{0}-0))$, alltså **medelvärdet** mellan höger- och vänstergränsvärdena i $t_{0}$.

# Se också:
[[Halvperiodutvecklingar\|Halvperiodutvecklingar]]
[[Parsevals formel\|Parsevals formel]]
