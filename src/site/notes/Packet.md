---
{"dg-publish":true,"permalink":"/packet/","tags":["kommunikationssystem"]}
---

När information ska skickas bukar den delas upp i mindre delar, så kallade paket. Det kan bestå av upp till tre delar: huvud (header), data och svans (trailer).Det är upp till varje protokoll att bestämma hur dess datapaket skall se ut.

Payload är den delen av datapaketet som mottagaren har nytta av och overhead är den del som behövs för att nyttolasten ska kunna komma fram korrekt - header och trailer. Ju fler [[Störningar\|störningar]] desto mer overhead behövs.