---
{"dg-publish":true,"permalink":"/bipolaer-transistor/","tags":["analogelektronik"]}
---

Bipolära [[Transistor\|transistorer]] är [[Halvledare\|halvledare]] med både elektroner (n) och hål (p). ELektroner i [[Ledningsband\|ledningsbandet]] - potentiell [[Energi\|energi]] minskar med positiv [[Potential\|potential]]. Hål i valenssbandet - potentiell [[Energi\|energi]] ökar med positiv [[Potential\|potential]]. Vi kan rita de i samma diagram. Elektroner uppför sig som vatten och hål uppför sig som 'bubblor' i vatten. Bipolär = både elektroner och hål!
![bipoläratransistorer.png|300](/img/user/images/bipol%C3%A4ratransistorer.png)

De använder sig av samma princip som [[PN-diod\|pn-dioder]] (PN-övergång) och kan ses som två [[PN-diod\|PN-dioder]] riktade åt olika håll (se bild ovan). Det är alltså två övergångar, vilket leder till att [[Transistor\|transistorn]] har två [[Kapacitans\|kapacitanser]].

![npn transistor.png|400](/img/user/images/npn%20transistor.png)

![Pasted image 20220510111757.png|250](/img/user/images/Pasted%20image%2020220510111757.png)
Emittorn emitterar elektroner till kollektorn. När man framspänner PN-övergången mellan bas och emittorn flödar elektroner från emittor till kollektor, men samtidigt flödar det in hål genom basen! Det är därför det uppkommer både en kollektorström och en basström.


Till skillnad från i [[Fälteffekttransistor\|Fälteffekttransistor]] kan det även uppstå en basström $I_B$, då hålen kan flöda upp till emittorn. En annan skillnad är att strömmen $I_c$ är exponentiell.

$$\omega_{T}=\frac{g_{m}}{c_{\pi}}=\frac{\beta_{f}}{r_{\pi}c_{\pi}}$$

$\beta=\frac{I_{C}}{I_{B}}=\frac{\mu_{n}W_{E}N_{DE}}{\mu_{p}W_{B}N_{AB}}$ och är ett mått på strömförstärkningen! “Hur mycket större är Ic än Ib”


Utnyttjar att strömmen är oberoende av spänningen i en backspänd PN-övergång. (tänk kurvan för hur strömmen $I_{C}$ beror på spänningen exponentiellt. På vänster halvplan är strömmen linjär och ligger väldigt nära under x-axeln!) 

“För att kunna hålla en framspänning måste det tillföras hål till basen”. 



# Modeller
![bjt-modeller.png|450](/img/user/images/bjt-modeller.png)
[[Hybrid pi-modellen för bjt\|Hybrid pi-modellen för bjt]]
[[Högfrekvensmodell för bjt\|Högfrekvensmodell för bjt]]
