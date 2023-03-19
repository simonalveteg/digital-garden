---
{"dg-publish":true,"permalink":"/transmissionsledning/","tags":["mätteknik"]}
---

![transmissionsledning LFsystem.png](/img/user/images/transmissionsledning%20LFsystem.png)
I lågfrekventa system, dvs när våglängden är betydligt längre än ledningens längd, kan man se det som att det är samma [[Potential\|potential]] längs hela ledaren. Då kan det modelleras som en [[Resistans\|resistans]], en [[Spole\|spole]], och en [[Kapacitans\|kondensator]]. Om man ökar frekvensen kan man inte längre se det som att man har samma [[Potential\|potential]] längs hela ledningen. Då får man bryta upp ledningen i massa små element.
![transmissionsledning hfsystem.png](/img/user/images/transmissionsledning%20hfsystem.png)
## När är en ledning en transmissionsledning?
Om ledningens längd är av samma storleksordning som en kvarts våglängd av [[Signal\|signalen]] eller större (sinussignaler) $L>\lambda/4$
Om ledningens fördröjningstid, $t_p$, för t.ex en puls är av samma storleksordning som signalens [[Stigtid\|stigtid]]/falltid eller längre (pulssignaler) $t_{p}>t_{r}$ eller $t_{p}>t_f$
![frekvensvåglängdtransmission.png](/img/user/images/frekvensv%C3%A5gl%C3%A4ngdtransmission.png)
Vi kan inte dra en ledare väldigt långa sträckor utan att ha transformatorstationer längs vägen, annars bildar det reflexioner i ledningens ändar. 

# Karakteristisk impedans
$Z_{0}=\sqrt{\frac{l}{c}}$ . Rent resistiv och saknar fasvridning
# Utbredningshastighet
$v=\frac{1}{\sqrt{lc}}$ 

# Anpassning
För att undvika reflektioner på en transmissionsledning måste ledningen avslutas med [[Impedans\|impedanser]] med samma storlek som den karakteristiska impedansen.

Reflektionskoefficienten är 
$\rho = \frac{Z_{L}-Z_{0}}{ Z_{L}+Z_{0}}$ 
om $\rho\neq0$ erhålls reflektioner, vilket ger upphov till stående [[Vågor\|vågor]] och därmed mätfel! 