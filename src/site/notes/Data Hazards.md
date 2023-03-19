---
{"dg-publish":true,"permalink":"/data-hazards/","tags":["datorteknik"]}
---

Om en instruktion vill använda data som inte är färdigprocesserad än uppkommer en data hazard. Låt säga att en är ADD och nästa är ADD med resultatet av den första, en konflikt där är en data-hazard. Det kan man lösa med hjälp av delays. För att minska "straffet" (i slösad tid) kan man använda forwarding/bypassing. Direkt plocka värdet från ALUn och se till att det kommer tillbaka till ALUn igen.
