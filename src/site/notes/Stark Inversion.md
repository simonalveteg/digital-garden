---
{"dg-publish":true,"permalink":"/stark-inversion/","tags":["komponentfysik"]}
---

Allt nedan beskriver en [[nMOSFET\|nMOSFET]] men det är **samma sak** för en [[pMOSFET\|pMOSFET]], fast “tvärtom” (dvs hål istället för elektroner och strömmen rör sig därmed i motsatt riktning)
![nmos stark inversion.png](/img/user/images/nmos%20stark%20inversion.png)
Vid stark inversion blir det en ledande [[Kanal\|kanal]] av elektroner vid ytan så att elektroner kan röra sig från source till drain (och strömmen från drain till source).
![geometrik nmosfet.png](/img/user/images/geometrik%20nmosfet.png)
Hur mycket elektroner vi har i kanalen ges av skillnaden mellan gatespänning och tröskelspänning
$$Q'_{n}=C_{ox}'(U_{GS}-U_{TH})$$
$$I_{DS }=Z\mu_{n}Q_{n}'\mathcal{E}$$
$$\mathcal{E}=\frac{U_{DS}}{L_{g}}$$
där $L_{g}$ är bredden på gaten, Z är kanaldjup, $\mu_{n}$ är [[Mobilitet\|mobiliteten]], $\mathcal{E}$ är det elektriska fältet och $C_{ox}'$ är oxidens [[Kapacitans\|kapacitans]] per kvadratmeter.

Egentligen är kanalen inte en rektangel! Eftersom att spänningen $U_{GS}$ ligger mellan gate och source, dvs ju närmre drain man kommer desto mindre påverkan har den spänningen. Därför är koncentrationen av elektroner lägre närmre drain. 
![kanalskillnad nmos.png](/img/user/images/kanalskillnad%20nmos.png)
Strömmen $I_{DS}$ ökar när man ökar $U_{DS}$, men når en gräns som sätts av $U_{GS}$! Om man ökar gatespänningen gör man kanalens maxbredd (höjd i bilden ovan) större, vilket gör att man med tillräcklig drainspänning kan få ut en större ström! Det ger upphov till diagrammet nedan (“utgångskaraktäristik”)
![idsvsudsnmos.png](/img/user/images/idsvsudsnmos.png)
det platta området kallas för **mättnadsområdet** och den stigande för det **linjära området**. 
