---
{"dg-publish":true,"permalink":"/dimensionering-av-ad-omvandlare/","tags":["kommunikationssystem"]}
---

Hur man dimensionerar en AD omvandlare beror på vilka frekvenser som finns med i den analoga signalen, samt var den digitala signalen ska användas. Om man exempelvis vill spela in stadsmiljö vill man få med hela det hörbara spektrumet, dvs ca 20kHz. Det leder till en [[Sampling\|samplingfrekvens]] på 40kHz ([[Nyquists Samplingskriterium\|Nyquists Samplingskriterium]]). [[Quantization\|Kvantisering]] kan exempelvis vara 8-bitar (telefoni) eller 16-bitar (CD). CD är bättre, men om ljudkvaliten inte spelar så stor roll kan man välja 8-bitar. För att kunna återge ljudet i stereo behövs två kanaler. *Överföringshastigheten* i detta exemplet blir $40000\text{samples/s}\cdot16\text{bits/sample}\cdot2=1.28\text{Mbps}$.
