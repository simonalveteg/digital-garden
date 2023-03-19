---
{"dg-publish":true,"permalink":"/hidden-terminal-problem/","tags":["kommunikationssystem"]}
---


Hidden Terminal Problem kallas det när två terminaler A och B pratar med en basstation C. A och B kan inte se varandra så Collision Detection fungerar inte. Därför kan båda försöka prata med C samtidigt utan att veta om att det blir en kollision. Lösningen är att använda en handshaking mekanism med Request To Send, Clear To Send och Ack, som alla terminaler som kan höra basstationen kan lyssna på, och hålla käften när det inte är deras tur att prata.