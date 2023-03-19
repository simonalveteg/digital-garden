---
{"dg-publish":true,"permalink":"/signal-transmission/","tags":["kommunikationssystem"]}
---

Det finns flera sätt att överföra data, genom olika kodningar och moduleringar.

## On-off keying
Send one bit during $T_b$ seconds and use two signal levels, "on" and "off", for 1 and 0.

## Bipolar signalling
En etta skickas med A och en nolla med -A.
![Pasted image 20230117163558.png|400](/img/user/images/Pasted%20image%2020230117163558.png)

## NRZ and RZ
On-off keying och bipolar signalling är exempel på NRZ (non-return to zero) där pulsen håller ut, dvs om det är fem ettor i rad kommer signalen ha samma värde tills nästa nolla kommer. Return to zero (RZ) återvänder istället till noll efter lika lång tid varje gång, vilket gör att mottagaren inte kan räkna fel.
![Pasted image 20230117164321.png](/img/user/images/Pasted%20image%2020230117164321.png)

## Manchester Coding
To get a zero passing in each signal time, split the pulse shape in two parts and use +/- as amplitude.

Manchester Coding consists of both data and a clock pulse?

Varje uppåtflank är en etta och varje nedåtflak är noll.
![Pasted image 20230117164307.png](/img/user/images/Pasted%20image%2020230117164307.png)

## Differential Manchester Coding
Samma princip som Manchester Coding, men om samma signal skickas som den förra så är det en nolla. Om den förra inverteras är det en etta.
![Pasted image 20230117164510.png](/img/user/images/Pasted%20image%2020230117164510.png)
Varje bit innehåller även information om föregående bit, vilket kan vara till nytta om det finns mycket [[Noise\|brus]] på länken.

## Pulse Amplitude Modulation
The data is stored in the amplitude and transmitted with a pulse shape.
Bipolar signaling is a form of binary PAM - 2-PAM.
![2PAM.png](/img/user/images/2PAM.png)

M-PAM uses M amplitude levels to represent $k=\log_2(M)$ bits.
2-PAM:
![Pasted image 20230117165253.png](/img/user/images/Pasted%20image%2020230117165253.png)
![Pasted image 20230117165311.png](/img/user/images/Pasted%20image%2020230117165311.png)
