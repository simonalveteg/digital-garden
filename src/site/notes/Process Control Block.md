---
{"dg-publish":true,"permalink":"/process-control-block/","tags":["datorteknik"]}
---

PCB är en datastruktur som innehåller information om processen som är associerad med den. Istället för att ha en PCB per process delas dem upp i flera mindre process control blocks. Det görs för att förhindra [[Fragmentering\|fragmentation]] - dvs när det finns lediga PCBs att lagra information i, fast det man vill spara tar för stor plats.