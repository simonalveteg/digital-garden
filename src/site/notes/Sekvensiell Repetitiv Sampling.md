---
{"dg-publish":true,"permalink":"/sekvensiell-repetitiv-sampling/","tags":["mätteknik"]}
---

Om [[Signal\|signalen]] är repititiv finns det fler samplingsmetoder än [[Realtidssampling\|realtidssampling]] att välja på. De bygger på *repetitiv [[Sampling\|sampling]]*, dvs att signalens mätpunkter inte samplas i ett enda pass utan i flera cykler. 

Vid sekvensiell repetitiv [[Sampling\|sampling]] tas varje nytt sample på kurvan i olika cykler. För varje sample är sampletidpunkten förskjuten med ett kort tidsintervall.

![sequential sampling.png](/img/user/images/sequential%20sampling.png)
Tidsupplösningen beror endast på fördröjningstiden (dvs hur mycket samplingen förskjuts mellan cykler). Det tar dock relativt lång tid jämfört med [[Realtidssampling\|realtidssampling]]. Man måste köra lika många pass som man vill ha mätpunkter.

## Se också:
[[Slumpmässig Repetitiv Sampling\|Slumpmässig Repetitiv Sampling]]