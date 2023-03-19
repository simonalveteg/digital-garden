---
{"dg-publish":true,"permalink":"/analog-elektronik-f14/","tags":["föreläsning","analogelektronik"]}
---

# tenta
1. Förstå [[feedback\|återkoppling]] och konstruera [[Förstärkare\|förstärkare]] me [[Nullor\|nullor]]- [[Superposition\|superpositionsmetoden]]
2. Nullorimplementation, negativt årekopplade förstärkares in- och utimpedanser blir mr ideala med faktorn 1+AB
3. Frekvensegenskaper och [[Frekvenskompensering\|frekvenskompensering]] (fantomnolle uppgift på andra delen av tentan, en fråga om narrowbanding på första delen)
4. [[Storsignaldistorsion\|Storsignaldistorsion]] (klippning) med resistiv last

man ska kunna ta fram sambanden och härleda ekvationen för $A_{t}$ ur diagrammet [[superpositionsmodellen.png]].

Nullorns egenskaper - kunna de fyra grundkopplingarna utantill. Viktigt att behärska [[Nodanalys\|nodanalys]]. Kunna ta bort redundanta komponenter ([[Redundancy\|Redundancy]]).

[[Förstärkande Steg\|Förstärkande steg]] - om det är oåterkopplade steg finns det bara AS och GE
GB - används aldrig som ingång eller utgång. Isolerande steg i mitten, sänker [[Millereffekten\|millereffekten]] vilket ger större [[Bandbredd\|bandbredd]] om man har stor spänningsförstärkning.
[[Ingångssteg\|Ingångssteg]]: [[GE-steget\|GE-steg]]/[[Antiseriesteget\|AS-steg]]. AS måste användas när man har samma enhetstyp på ingång och utgång, annars kortsluter man?

[[Biasering\|BIAS]]:
	Kunna ta fram nodpotentialer och strömmar ur en [[Biasering\|biaserad]] koppling
	Kunna ta fram ett småsignalschema från en [[Biasering\|biaserad]] koppling
	Kunna beräkna småsignalegenskaperna för en [[Biasering\|biaserad]] koppling
	Kunna beräkna när klippning inträffar för en [[Biasering\|biaserad]] koppling

Frekvensegenskaper:
	Förstå sambandet mellan tidsdomän och frekvensdomän
	[[Rotort\|Rotort]] kan dyka upp på första delen
	Känna till sambandet mellan bode-diagram och [[Laplace-planet\|s-planet]]

Högfrekvent-småsignalmodell
	Känna till den [[Frekvensberoende\|frekvensberoende]] småsignalmodellen för [[Bipolär transistor\|BJT]] (med kondensatorerna)
	Kunna beräkna den komplexa slingförstärknignen för en flerstegsfrstärkare. Dra slutsatser och beräkna den slutna förstärkningens frekvensegenskaper.

Återkopplad [[Förstärkare\|förstärkare]]
	Förstås killnaden mellan slingoler oc [[Systempoler\|systempoler]]. Kunna identifiera [[Dominanta och Icke-dominanta poler\|icke-dominanta poler]]
	Förstå hur [[Slingpoler och Slingnollställen\|slingpolerna]] tillsammans med $A\beta(0)$ kan estimera maximal [[Bandbredd\|bandbredd]] (LP-produkt)
	Kunna uppskatta maximal [[Bandbredd\|bandbredd]] hos en [[Flerstegsförstärkare\|flerstegsförstärkare]].‘

[[Frekvenskompensering\|Frekvenskompensering]]
	Förstå varför [[Frekvenskompensering\|frekvenskompensering]] är nödvändig - för att man inte vill ta sönder elektronik ([[Stabila och Instabila System\|instabilt]] => ringning => ajdå)
	Förstå på vilka sätt vi kan påverka förstärkarens frekvensegenskaper ([[Phantom Zero\|fantomnolla]], [[Capacitive Narrowbanding\|capacitive narrowbanding]])
	kunna skissa [[Rotort\|rotort]] (kan förekomma enkel [[Rotort\|rotort]] på första delen)

[[Phantom Zero\|Fantomnolla]]
	Förstå skillnaden mellan ett [[Slingpoler och Slingnollställen\|slingnollställe]] och ett fantomnollställen
	Känna till hur en [[Phantom Zero\|fantomnolla]] påverkar [[Rotort\|rotorten]]
	Kunna implementera och dimensionera en [[Phantom Zero\|fantomnolla]] i en negativt återkopplad [[Förstärkare\|förstärkare]]
	Känna till snabbmetoden i labbet - sätt $\omega_0=\omega_{T}$ KOMMER INTE PÅ TENTA

[[Storsignaldistorsion\|Storsignaldistorsion]]
	Förstå [[Switchmodellen\|switchmodellen]] för [[GE-steget\|GE-steget]]. 
	Känna till klippningsegenskaper
		[[Antiseriesteget\|AS-steg]] har endast strömklippning
		CP-steg har endast spänningsklippning
	Kunna beräkna när klippning inträffar för en koppling med angiven [[Biasering\|bias]]


# Extenta 220420

## uppgift 1
ta fram småsignalparametrarna $r_{\pi}$, $g_{m}$, och $r_{0}$ genom att linjärisera $I_{c}$i en given [[Arbetspunkt\|arbetspunkt]]. ([[Taylorutveckling\|taylorutveckling]])

kolla vad komponenterna sitter mellan. 
$$r_\pi=\left.\left(\frac{\delta i_{C}}{\delta V_{BE}}\right)^{-1}\right|_{i_{B}=I_{B}}$$ 
$$g_{m}=\left. \frac{\delta i_{C}}{\delta V_{BE}}\right|_{i_{C}=I_{C}}$$
$$r_{0}=\left. \left(\frac{\delta i_{C}}{\delta V_{CE}}\right)^{-1}\right|_{i_{C}=I_{C}}$$
## uppgift 3
VV ska realiseras med ett [[Förstärkande Steg\|förstärkande steg]]. 
Vilket steg ska användas och varför? - Antiserie för att man måste isolera in och utsignal för att inte kortsluta [[feedback\|återkopplingsnätet]].
Rita signalschemat och småsignalschemat, ange tecken i nullorn för negativ återkoppling samt den asymptotiska förstärknignen$A_{t\infty}$. - Enkelt?
Ta fram DC-slingförstärkningen - hyfsat enkelt?

## uppgift 4
under vilka förutsättnignar kan man implementera en fantomnolla i en VI-förstärkare?

## uppgift 5


# Subject
[[Analog Elektronik\|Analog Elektronik]]
