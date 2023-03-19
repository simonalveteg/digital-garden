---
{"dg-publish":true,"permalink":"/biasering/","tags":["analogelektronik"]}
---

Biasing is the setting of initial operating conditions (current and voltage) of an active device in an [[Förstärkare\|amplifier]]. All non-linear functions used in amplifiers need bias to obtain the desired [[Arbetspunkt\|operating point]]. Bias is also needed to provide the [[Transistor\|transistor]] with [[Effekt\|power]] to make power [[Förstärkning\|amplification]] possible.

Det enklaste/vanligaste? är att lägga till spänningskällor till bas och kollektor. Men man kan också [[Biasering\|biasera]] med strömkällor. Voltage-mode and Current-mode. Current mode is preferrable (at least in integrated circuits) because we can make really [[Stabila och Instabila System\|stable]] currents in regards to temperature, pressure and so on. In the lab it doesn’t matter that much.

![biasering.png](/img/user/images/biasering.png)
Där Q är [[Arbetspunkt\|arbetspunkten]]. 
[[Typkoppling vid biasering av transistor.png]]

Bias är likström/spänning. Det innebär att [[Kapacitans\|kondensatorer]] blir avbrott, och [[Spole\|spolar]] blir kortslutningar. [[Biasschema\|Biasschema]]

## Biaseringsmetoder
### Direkt spänning och ström (endast i teorin)
Man måste känna till de exakta offsetspänningarna resp strömmarna

### Tidsdomän
Används i switchade [[System (matematisk definition)\|System (matematisk definition)]]
### Frekvensdomän
![frekvensdomän bias.png](/img/user/images/frekvensdom%C3%A4n%20bias.png)
![Pasted image 20220131132827.png](/img/user/images/Pasted%20image%2020220131132827.png)
### Differentiell och common-mode

# Biasering måste återkopplas
[[Arbetspunkt\|Arbetspunkten]] bestämmer transistorns småsignalparametrar $r_\pi$ , $g_m$, och $r_o$  