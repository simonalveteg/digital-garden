---
{"dg-publish":true,"permalink":"/fpga-design-flow/","tags":["digitalteknik"]}
---

# [[Field Pogrammable Gate Array\|FPGA]] Design Flow
![Pasted image 20211101114135.png](/img/user/images/Pasted%20image%2020211101114135.png)
1. Design entry: man börjar med sin design, antingen med Hardware Descrption Languages ([[Hardware Description Language\|HDL]]), kretsscheman eller High Level Synthesis (HLS). Nackdelen med kretsscheman är att de oftast är bundna till vilken tillverkares komponenter man använder. Man sätter oftast constraints på sin desing, ex klockfrekvens, signalfördröjning, energikonsumtion, antal pins osv. 
2. Register Transfer Level Simulation (RTL simulation): verifiera att designen funkar som man tänkt sig
3. Syntes: när man översätter/mappar en design till resurser
	1. Look-up tables (LUTs)
	2. Flip-flops
	3. latches
	4. adders
	5. multipliers
	6. memory
4. Implementering: placering av komponenter osv.
5. Simulera igen, dessa simuleringar tar längre tid men är mer exakta
6. Timing analysis: går det att klocka den i tänkt frekvens?
7. Programmera! De flesta [[Field Pogrammable Gate Array\|FPGA]] använder SRAM för att lagra konfigurationen, dvs konfigureringen försvinner varje gång man startar om FPGAn. Löses genom att lagra konfigurationen på ett minne som man kopplar till FPGAn.
8. Testing: Verifiera att allt funkade som tänkt :)


