---
{"dg-publish":true,"permalink":"/maximum-transfer-unit/","tags":["kommunikationssystem"]}
---


Olika [[Data Link Layer\|länkprotokoll]] har olika maxlängd på sina [[Framing\|ramar]]. Denna kallas för Maximum Transfer Unit eller MTU. När ett [[Internet Protocol\|IP]]-datagram skall kapslas in i länkprotokollets ram får datagrammets längd inte vara större än länkprotokollets MTU. Om det är det måste det  [[Fragmentering\|fragmenteras]].

MTU är alltså inte den maximala längden av det som skickas på en länk, utan den maximala längden av det datagram man vill skicka via länken. Skillnaden är att det kommer tillkomma overhead ovanpå datagrammet innan det skickas. Storleksbegränsningen ligger rimligtvis på datagrammet man vill skicka.