---
{"dg-publish":true,"permalink":"/hybrid-pi-modellen-foer-bjt/","tags":["analogelektronik"]}
---

Linjärisering av den [[Bipolär transistor\|bipolära transistorns]] överföringsdiagram ger en modell med linjära element. Linjära modeller är enkla att räkna på men gäller bara i ett begränsat område kring linjäriseringspunkten - vi kallar detta [[Småsignal\|småsignal]]! Kollektorströmmen ([[Storsignal\|storsignal]]) ges av
$$
I_{C}=I_{S}e^{\frac{V_{BE}}{V_{T}}}\left(\frac{1+V_{CE}}{V_{A}}\right) \space ,\space V_{BE}>0 \space and \space V_{BC}<0
$$
Med [[Taylorutveckling\|taylorutveckling]] kan man få fram ett uttryck för totalsignalen $i_C$ runt [[Arbetspunkt\|arbetspunkten]] $Q$
$$
i_{C}=I_{C}+i_{c}=f(V_{BE})+f'(V_{BE})\cdot v_{be}+\sum\limits_{n=2}^{\infty} \frac{1}{n!} \frac{\delta^{n}f(V_{BE})}{\delta v^{n}_{BE}} = BIAS+Gain\cdot signal+distortion
$$
hybrid $pi$-modellen är likadan för både [[Bipolär transistor\|PNP]] och [[Bipolär transistor\|NPN]] och ser ut som i bilden nedan. Kondensatorerna brukar försummas.
![hybrid-pi-modellen-bjt.png|450](/img/user/images/hybrid-pi-modellen-bjt.png)
där konstanterna ges av 
![hybrid-pi-bjt-rpi-ro-gm.png|450](/img/user/images/hybrid-pi-bjt-rpi-ro-gm.png)
man kan härleda ekvationerna ovan från den exponentiella grafen typ, och utifrån ekvationerna kan man sedan resonera sig fram till kretsschemat ovan. Man vet att $I_{C}$ ska gå från Collector till Emittor. $V_{T}$ är ca 25mV i rumstemperatur

### Modellens parametrar 
Genom att beräkna derivatorna i [[Arbetspunkt\|arbetspunkten]] får man uttryck på modellens parametrar.
$$\frac{i_{c}}{i_{b}}=\beta_f$$
där $\beta_f$ står i transistorns datablad “common emitter current gain”