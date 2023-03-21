---
{"dg-publish":true,"permalink":"/system-och-transformer-f15/","tags":["föreläsning","systemochtransformer"]}
---


## Tillämpningar av Laplace-transformation

### Lösa [[Differentialekvationer\|differentialekvationer]]

Exempel:
	Hitta [[Kausal\|kausal]] lösning $y(t)$ till $y'''-2y=\delta^{(4)}+\delta'''-\delta' \, , \,-\infty<t<\infty$.
	(standarduppgift på godkäntdelen av tenta)
Lösning:
	$\mathcal{L}(y'''+y''-2y)(s)=\mathcal{L}(\delta^{(4)}+\delta'''-\delta')(s)$
	laplace utav summa = laplace utav termer
	$s^{3}\mathcal{L}(y)+s^{2}\mathcal{L}(y)-2\mathcal{L}(y)=s^{4}\mathcal{L}(\delta)+s^{3}\mathcal{L}(\delta)-s \mathcal{L}(\delta)$
	där $\mathcal{L}(\delta)=1$ (står i formelbladet)
	$\mathcal{L}(y)(s^{3}+s^{2}-2)=s^{4}+s^{3}-s$
	$\Rightarrow \mathcal{L}(y)(s)=\frac{s^{4}+s^{3}-s}{s^{3}+s^{2} -2}$ 
	men vi vill ha $y$, vilket fås av den inversa [[Laplacetransformationer\|laplacetransformen]] av högerledet.
	$y(t)=\mathcal{L}^{-1}_{\text{kausal}}(\frac{s^{4}+s^{3}-s}{s^{3}+s^{2} -2})(t)$
	där högerledet kan lösas med [[Partialbråksuppdelning\|partialbråksuppdelning]] eller [[Residykalkyl\|residykalkyl]]. Först måste nämnare ha lägre grad än täljare => polynomdivision.
	$y(t)=\mathcal{L}^{-1}_\text{kausal}(s+\frac{s}{s^{3}+s^{2}-2})(t)=\delta'(t)+\mathcal{L}^{-1}_\text{kausal}(\frac{s}{s^{3}+s^{2}-2})(t)$
	där $\delta'$ kommer från den [[Invers Laplacetransformation\|inversa laplacetransformationen]] av s.
	$s^{3}+s^{2}-2$ har ett [[Nollställen\|nollställe]] som är 1, polynomdivision igen leder till
	$=(s-1)(s^{2}+2s+2)=(s-1)(s+1+i)(s+1-i)$
	om vi sen ritar dessa [[Nollställen\|nollställen]] i [[Laplace-planet\|laplace-planet]] så kan vi se vilket område vi måste välja för att få en [[Kausal\|kausal]] strimla. Vilket ger
	$Res_{s_{1}=1}(e^{st}F(s))=Res_{1}(\frac{e^{st}s}{s^{3}+s^{2}-2})=\left.\frac{e^{st}s}{3s^{2}+2s}\right|_{s=1}=\frac{e^{t}}{5}$ med standardmetod för [[Residy\|residy]], samma görs sedan för övriga [[Nollställen\|nollställen]].
	till slut blir 
	$y(t)=\delta'(t)+\theta(t)(Res_{s_{1}}+Res_{s_{2}}+Res_{s_{3}})$

Exempel:
	Bestäm en [[Kausal\|kausal]] lösning till 
	$$y'+y=\begin{cases}0 \text{ , } -\infty<t<0 \\
1 \text{ , } 0<t<1 \\
0\text{ , }1<t<\infty \end{cases}$$
Lösning:
	[[Laplacetransformationer\|Laplacetransformation]] ger $s \mathcal{L}(y)+\mathcal{L}(y)=\mathcal{L}(\theta_{0}(t)-\theta_{1}(t))$ (vl=hl)
	$\mathcal{L}(y)(s+1)=\frac{1}{s}-e^{-s} \frac{1}{s}$
	man kan bara använda [[Residy\|residy]] på rationella uttryck, så vi vill bli av med den exponentiella termen
	$\Rightarrow y(t)=\mathcal{L}^{-1}_\text{kausal}\left(\frac{(s+1)-s}{s(s+1)}-e^{-s} \frac{1}{s(s+1)}\right)(t) = \theta(t)-e^{-t}\theta(t)-\mathcal{L}_\text{kausal}^{-1}\left(\frac{1}{s(s+1)}\right)(t-1)$ $=\theta(t)-e^{-t}\theta(t)-(\theta(t-1)-e^{-(t-1)}\theta(t-1))$
	 man använder laplacetransformer med formelbladet. För fourier har vi kedjor, men för laplace måste man använda formeln baklänges - eller [[Residykalkyl\|residykalkyl]]. [[Residy\|Residy]] gäller dock endast för [[Rationella Funktioner\|rationella funktioner]].


[[Laplacetransformationer\|Laplacetransformationen]] av en [[Faltning\|faltning]]
$$\mathcal{L}(f*g)=\mathcal{L}(f)\cdot \mathcal{L}(g)$$
utsignalen kan uttryckas genom [[Faltning\|faltning]], [[Impulssvar\|impulssvar]] [[Faltning\|faltas]] med insignal. Så en tillämpning av ovan är att för ett [[Linjära och Tidsinvarianta System\|LTI-system]] $w(t)\xrightarrow{S}y(t)$ gäller
$$y(t)=h(t)*w(t)$$
$$\mathcal{L}(y)=\mathcal{L}(h)\cdot \mathcal{L}(w)=H(s)\cdot\mathcal{L}(w)$$
[[Laplacetransformationer\|laplacetransformen]] av [[Impulssvar\|impulssvar]] är [[Överföringsfunktion\|överföringsfunktionen]]. Om man känner till två av tre okända så kan man teoretiskt räkna ut den tredje. 

Exempel:
	$S$ är kausalt, [[Linjära och Tidsinvarianta System\|LTI]] och $sint \theta(t)\xrightarrow{S}sin(2t)\theta(t)$. Bestäm $h(t)$ och svaret $y_{1}(t)$ på insignalen $w_{1}(t)=tsint \theta(t)$.
Lösning:
	Vi vet att $sin(2t)\theta(t)=h*(sint \theta(t))$ och $y_{1}(t)=h*(tsint \theta(t))$.
	Laplacetransformering ger (se formelblad)
	$\frac{2}{s^{2}+4}=\mathcal{L}(h)\cdot \left(\frac{1}{s^{2}+1}\right) \Rightarrow \mathcal{L}(h)(s)=2\frac{s^{2}+1}{s^{2}+4}=2-\frac{6}{s^{2}+4}$ och $\mathcal{L}(y_{1})=\mathcal{L}(h)\cdot \mathcal{L}(tsint \theta(t))(s)=\mathcal{L}(h)\cdot(- \frac{d}{ds}\left(\frac{1}{s^{2}+1}\right))=\mathcal{L}(h)\left(\frac{2s}{(s^{2}+1)^{2}}\right)$ 
	från det får vi att
	$h(t)=\mathcal{L}^{-1}_\text{kausal}\left(\frac{2-6}{s^{2}+4}\right)(t)=2\delta(t)-3sin2t \theta(t)$ 
	med vilken vi kan ta reda på $y_{1}$:
	 

### Studera [[Linjära och Tidsinvarianta System\|LTI-system]]






# Subject
[[FMAF05 System och Transformer\|FMAF05 System och Transformer]]
