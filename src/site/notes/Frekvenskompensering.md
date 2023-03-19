---
{"dg-publish":true,"permalink":"/frekvenskompensering/","tags":["analogelektronik"]}
---


## Varför frekvenskompensera?
När man designar en [[Förstärkare\|förstärkare]] har man oftast några önskemål om dess funktion. Det kan vara att man vill att [[Förstärkning\|förstärkningen]] ska vara lika stor för alla frekvenser, att frequency roll-off ska vara så skarp som möjligt, att [[Stegsvar\|stegsvaret]] ska vara så snabbt som möjligt m.m. För att uppnå önskad prestanda behöver man oftast använda sig av frekvenskompensering.

## Vad innebär frekvenskompensering?
För att få önskad prestanda vill vi att [[Systempoler\|systempolerna]] ska befinna sig på en specifik position. Positionen beror på vad det är vi vill uppnå. Om vi vill ha jämn [[Förstärkning\|förstärkning]] för alla frekvenser inom [[Bandbredd\|bandbredden]] ([[Maximal Flat Frekvensgång\|MFM]]) vill vi att [[Systempoler\|systempolerna]] ska vara i [[Butterworthposition\|Butterworthposition]]. Detta gör man med olika [[Frekvenskompenseringsmetoder\|Frekvenskompenseringsmetoder]].

[[Hur frekvenskompensering kan påverka rotorten - MFM system\|Hur frekvenskompensering kan påverka rotorten - MFM system]]



#question why do our amplifiers behave like filters? 

När man flyttar [[Systempoler\|systempolerna]] förändras systemets karaktäristiska polynom #question vad är det
* frekvenskompensering tillämpas bara på [[Dominanta och Icke-dominanta poler\|dominanta poler]]
* Idealt ska kompensering ej påverka [[LP-produkten\|LP-produkten]] eller $A \beta(0)$.
