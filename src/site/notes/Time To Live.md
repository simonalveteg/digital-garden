---
{"dg-publish":true,"permalink":"/time-to-live/","tags":["kommunikationssystem"]}
---


När en dator skickar ut ett [[Internet Protocol\|IP]]-datagram sätter den TTL på paketet (vanligtvis 128). Varje [[Router\|router]] som datagram passerar måste räkna ned TTL med 1. När TTL är 0 måste det kastas. Routern som kastar datagrammet skickar ett [[Internet Control Message Protocol\|ICMP]] meddelande till datagrammets avsändare om att datagrammet kastas.

Traceroute använder sig av datagram där TTL-fältet är manipulerat så att varenda [[Router\|router]] längs sträckan kommer skicka tillbaka ett Time Exceeded [[Internet Control Message Protocol\|ICMP]] meddelande. Genom att sätta fel port kommer även den slutgiltiga destinationen att svara med Destination Uncreachable.