---
{"dg-publish":true,"permalink":"/triggerprinciper/","tags":["mätteknik"]}
---

[[Digitala oscilloskop\|Digitala oscilloskop]] har oftast fler möjligheter till [[Triggning\|triggning]] än analoga [[Oscilloskop\|oscilloskop]].

## Flanktriggning (Edge Triggering)
Den normala triggningsmetoden för att starta en inspelning. Man inväntar en bestämd signalflank på en bestämd triggernivå på insignalen. 

## Pulslängdstriggning (Glitch Trigger)
Om man ska visa ett pulståg där vissa pulser har betydligt kortare pulslängd jämför med de normala pulserna. Vid pulslängdstriggning kan oscilloskopet använda två triggerpunkter (flank till flank) för att mäta upp en pulslängd som jämförs med ett förinställt värde. Om det uppmätta värdet är mindre än det förinställda värdet så startas inspelningen. Kombinerat med förtriggning kan man fånga smala pulser på skärmen och se vad som hände före triggertillfället.

## Logiktriggning (Pattern Triggning)
Om man övervakar flera logiksignaler samtidigt kan man ange en kombination av deras logiska nivåer som triggernivåer, basically [[Digitalteknik\|Digitalteknik]]. Alternativen kan vara High, Low eller Don’t Care. 

## Tidsfördröjd Triggning (Time Delay Trigger)
Man ställer in en [[Förflyttningsfunktionen\|tidsfördröjning]]. Används i kombination med ett huvud-triggervillkor för att starta en inspelning en viss tid efter att huvudtriggervillkoret har inträffat. Lämplig för att spela in den stabila delen av [[Signal\|signaler]] med ett visst insvängningsförlopp.

## Händelsefördröjd triggning (Event Delay Trigger)
Vid händelsefördröjd [[Triggning\|triggning]] används en av ingångssignalerna för att fördröja själva triggertid punkten. Man har precis som i tidsfördröjd [[Triggning\|triggning]] ett huvudtriggervillkor. När det har inträffat räknas antalet triggerhändelser på fördröjningssignalen. När det inställa antalet triggerhändelser har nåtts startar inspelningen. Lämplig för att fånga seriella data som inträffar N klockpulser efter start.