---
{"dg-publish":true,"permalink":"/operativsystem/","tags":["datorteknik"]}
---

Ett operativsystem är ett program som exekveras på datorn, med mål att hantera hårdvaruresurser i datorsystemet, samt erhålla tjnster för exekvering av applikationsprogram.
![Pasted image 20230120143020.png](/img/user/images/Pasted%20image%2020230120143020.png)
Applikationen får tillgång till hårdvaran via operativsystemet, men operativsystemet har fortfarande kontroll. Det finns en extern klocka som säger till med jämna mellanrum att "hallå nu är det slut för dig, det finns andra som vill göra saker". Då sparas allt som finns i processorns [[Register\|register]] till [[Process Control Block\|Process Control Block]] innan nästa program börjar exekvera. Det kallas kontextbyte.

Operativsystemet har [[Scheduler\|Schemaläggare]] som bestämmer vilka program som ska få exekveras.

[[Processer och trådar\|Processer och trådar]]

# Vad gör ett OS?
* Processhantering
* [[Minneshantering\|Minneshantering]]
* Filsystem
* Drivrutiner
* Nätverk
* Säkerhet
* In och utmatning
