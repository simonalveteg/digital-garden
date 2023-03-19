---
{"dg-publish":true,"permalink":"/termisk-modell-av-byggnad/","tags":["elenergiteknik"]}
---

För en byggnad kan man använda [[Den dynamiska termiska ekvationen\|Den dynamiska termiska ekvationen]] direkt, men i byggbranschen anger man hur välisolerat ett fönster eller en annan byggnadsdel är med hjälp av [[U-värde\|U-värde]] och det kan därför vara praktiskt att anpassa uttrycket efter detta.

En byggnad består normalt av flera olika delar som har olika [[U-värde\|U-värden]] och olika areor. Det är dock enkelt att kokmbinera dessa till ett totalt värde på $U\cdot A$. För N delar blir det samlade värdet:
$$
(U\cdot A)_\text{alla ytor}=\sum_{i=1}^{n}U_i\cdot A_i
$$
Förutom värmetransporten $Q_{transmission}$ genom väggar, tak och golv förloras [[Värme\|värme]] $Q_v$ även genom ventilationen. Den samlade kyleffekten i Watt för en byggnad blir därmed
$$
P_b=(Q_\text{transmission}+Q_v)\cdot(T_\text{inne}-T_\text{ute})=(U\cdot A+Q_v)\cdot(T_\text{inne}-T_\text{ute})
$$
[[Differentialekvationer\|Differentialekvationen]] som beskriver temperaturens variation i en byggnad blir
$$
C_t \frac{dT}{dt}=P_t-(U\cdot A+Q_v)\cdot(T_\text{inne}-T_\text{ute})
$$

[[Energi\|Energin]] som åtgår för att värma en byggnad motsvarar kyleffekten och kan uppskattas som tidsintegralen av ekvationen för $P_b$
$$
W=(U\cdot A+Q_v)\int(T_\text{inne}-T_\text{ute}(t))\,dt 
$$
Själva integralen har enheten Kh eller gradtimmar och hela uttrycket för $W$ har enheten (W/K)Kh=Wh. 


# Passivhus
Om kyleffekten blir tillräckligt liten räcker värmen från människor och hushållsapparater för att värma hus. Det kallas passivhus och har förutom ett tätt och välisolerat klimatskal även värmeväxlare som värmer tilluften med frånluften och på så sätt håller nere ventilationsförlusterna.

# Plusenergihus
Producerar under året mer [[Energi\|energi]] än vad det drar, exempelvis med solceller för elproduktion och solvärme för uppvärmning.


See also -> [[Modell av temperaturdynamik\|Modell av temperaturdynamik]]