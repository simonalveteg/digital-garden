---
{"dg-publish":true,"permalink":"/quick-start-guide-to-vhdl/","tags":["digitalteknik"]}
---

#digitalteknik 
**chapter 1 and section 2.2 (and 2.1 cursively)** 

## Chapter 1 
Moderna digital-design flöden använder CAE och CAD för att hantera komplexiteten hos moderna digitala system 

[[Hardware Description Language\|HDL]] språk som [[VHDL\|VHDL]] tillåter att denna funktionalitet kan realiseras med hjälp av text. Språken kan moddelera digitala system på många olika [[Abstraktionsnivåer\|abstraktions-modeller]]  vilket gör att komplexa system kan designas på olika nivåer utan att oroa sig om detaljer av implementationen. 

## Chapter 2 
- Varje [[Signal\|Signal]] och port måste kopplas till en datatyp 
- Datatypen definierar värden som en [[Signal\|Signal]] eller port kan hantera
- [[VHDL\|VHDL]] innehåller 3 huvudsektioner 
	- Package _inkludera funktionalitet_ 
	- Entity _definiera gränssnitt, inputs/outputs_ 
	- Architecture _beteende (här beskrivs hela funktionen)_ 
- **Port** _input/output deklarerad i Entity_ 
-  **[[Signal\|Signal]]** *intern koppling deklarerar i Architecture. Syns ej utanför 

[[VHDL\|VHDL]] supporter en hierarisk design. Olika subsystem kan designas och kopplas ihop för att bygga flera [[Abstraktionsnivåer\|abstraktionsnivåer]]. Inom dessa subsystem kan Port och [[Signal\|Signal]] ha samma namn då de inte är synliga till andra subsystem