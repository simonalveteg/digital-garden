---
{"dg-publish":true,"permalink":"/slumpmaessig-repetitiv-sampling/","tags":["mätteknik"]}
---

Precis som vid [[Sekvensiell Repetitiv Sampling\|Sekvensiell Repetitiv Sampling]] samplar man [[Signal\|signalen]] i flera pass. Skillnaden är att man vid slumpmässig repetitiv [[Sampling\|sampling]] tar en grupp av samples i varje pass, inte bara ett enstaka. Varje grupp startar vid en slumpmässig tidpunkt oberoende av triggertidpunkten. 

Inom varje grupp bestäms tiden mellan varje sample av den normala realtidssamplingsklockan. För att kunna bestämma samplens fasläge på vågformen mäts tiden mellan första samplet och en triggertidpunkt.


![slumpmässig repetitiv sampling.png](/img/user/images/slumpm%C3%A4ssig%20repetitiv%20sampling.png)