---
{"dg-publish":true,"permalink":"/projekt-i-analog-elektronik/","tags":["inlämning","analogelektronik"]}
---


AS-CE

slow down the transistors using C1 parallel wth c_pi for the first stage, C2 for second stage. We “pull down” the poles of the [[System (matematisk definition)\|System (matematisk definition)]]. [[Asymptotisk Förstärkning\|asymptotic gain]] -10kV/A. Lowest allowed [[Slingförstärkning\|loop gain]] is 60dB. When we feed in 0.1 mA peak current should not cause clipping. dvs vi behöver klara av 1V på utgången.

sigificant factor/measure of an [[Förstärkare\|amplifier]] - maximum current consumption. We can get much less than 10mA if we design it well enough (2-3mA is possible). Max 10mA allowed. $\beta_{f}$ is assumed to be 200, but we should measure it in the lab and go back and redo our calculations if $\beta_{f}$ is much higher or lower (typ 400). 

clean flat smooth frequency response – [[Maximal Flat Frekvensgång\|butterworth system]]

## analog design flow

start from usecases 
translate into specifications for circuit and try to define some specifications like power consumption. (system engineers vet hur man gör det) i detta projektet behöver vi inte göra det. 
Do hand calculations to find values using our knowledge of eletronics. Our models for hand caluclation is too simplified, so we run some simulations. 
System-level simulations - how changing different parameters affect stuff – using matlab. **mandatory - should be reflected in the report**
Schematic simulations (LTspice) - we really look at voltages and current, can use frequency - simulations among others. *recommended but not mandatory*
Hardware implementation - bygg kretsen. 
Test and verification - funkar den som den ska.

A
B 
AB(s)
poles
[[Slingförstärkning\|loop gain]]
[[Bandbreddsuppskattning\|bandwidth estimation]] - use matlab - plot transient and fequency response?


We can neglect $c_{\pi}$ because $c_{1}$ is so much larger!


calculate Rf with Atinf=-10


# Matlab
change values and mabe equations to fit our project.
ic1 - from hand calculations
r_pi1’, ic2, rpi2, gm2 caluclate using ic1
maybe change ABnoll equation+values
caluclate poles
[[Bandbredd\|bandwidth]] calculation + validity check
calculate [[Phantom Zero\|phantom zero]]
delta_cph pole/phantomzero > 7
investigate all possible (two) [[Phantom Zero\|phantom zero]] implementations and pick the most efficient one.  The larger deltha_cph the more efficient it is.

![Pasted image 20220407161415.png](/img/user/images/Pasted%20image%2020220407161415.png)


## Simulering
I och med att vi har [[Bipolär transistor\|PNP]] och [[Bipolär transistor\|NPN]] kan $\beta_{f}$ skilja sig lite mellan dem, därför behöver vi ändra värdet på RD något (storleksordning 10 ohm typ) för att strömmen genom RD och strömmen genom RB ska bli lika stora och spänningen på utgången och ingången ska bli noll.

## Strömspegling
Man skalar upp och ned strömmarna från strömspeglingen med resistorerna. I formlerna han skrev upp sätter man alltså in vilken ström $I_{1}$ eller $I_{2}$ man vill ha, och får ut värdet som resistansen måste ha för att man ska få den strömmen genom strömspeglingen.


ltspice more realstic simulation of components, we don’t neglect parasitic caps, we also have [[Biasering\|bias]] circuit. In the ideal case matlab and ltspice simulations are the same. The order of the system of equations is higher in ltspice than in matlab, therefore more accurate.

measure open loop gain by placing 10k resistor in parallell with input and output and remove feedback resistor.

if you compare closedloop response in matlab with ltspice and measurements and they’re quite comparable, then probably the [[Fasmarginal\|phase margin]] measured in matlab is applicable. 

if we make sure that feedforward doesn’t make a phase difference of 180 degrees then we can guarantee that the circuit won’t oscillate. That’s why we use open loop gain to measure [[Fasmarginal\|phase margin]]. There is only feedforward and no feedback. 

input impedance 3.3k , should work with .1mA gives a voltage of .33V which should be our maximum input voltage. But we should start with smaller amplitudes like 0.1V. Measure output voltage and sweep the frequency. Take point measurements and note it down in a spreadsheet. Looking for the ratio so note down both input and output. Measure [[Fasmarginal\|phase margin]] with cursors, from 0-crossing of input to 0-crossing of output. Do both before and after compensation.


# report
explain the methods and why we use them
for [[Phantom Zero\|phantom zero]] implementation we should explain why we chose the implementation we did and why there are two

matlab results
ltspice results
measurement results

put matlab in appendix. 


# plugin 
ltspice till latex plugin??? fråga vincent vad fan han menade