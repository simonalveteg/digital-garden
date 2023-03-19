---
{"dg-publish":true,"permalink":"/i-pv6-address/","tags":["kommunikationssystem"]}
---

En IPv6 adress består av 16 byte (128 bitar). För lättläslighet brukar den skrivas i hexadecimalt format med kolon emellan (*hexadecimal colon notation*). De 128 bitarna är uppdelade i 8 delar där varje del består av 2 byte. Eftersom att många bitar i en IPv6-adress kommer vara 0 kan man skriva den i ett förkortat format där hela följder av nollor kan ersättas med dubbla kolon.

Ex:
DA27:0255:0000:0000:0000:000D:1E2C:D200 på lång form
DA27:255::D:1E2C:D200 på kort form.

Om man har flera följder av nollor brukar man sätta en enskild nolla mellan de dubbla kolonen på de ställen där det är minst nollor. Ex
ED22:0000:0000:04D2:0000:0000:0000:000D blir ED22:0:0:4D2::D på kort form.