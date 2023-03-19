---
{"dg-publish":true,"permalink":"/termisk-modell-av-fysisk-kropp/","tags":["elenergiteknik"]}
---


Fysiska kroppar kan både lagra och leda [[Värme\|värme]], och olika ämnen och aggregationstillstånd är olika bra på detta. 

[[Termisk Resistans\|Termisk Resistans]] beskriver förmågan att leda [[Värme\|värme]]. *Ledningsförmågan* beskrivs av begreppet [[Termisk Konduktivitet\|Termisk Konduktivitet]] ur vilken den termiska resistansen kan beräknas, på samma sätt som [[Resistans\|Elektrisk Resistans]] kan härledas ur den [[Conductivity\|Elektriska Konduktiviteten]]. *Lagringsförmågan* beskrivs med begreppet [[Termisk Kapacivitet\|Termisk Kapacivitet]]. 

Med den termiska resistansen och [[Termisk Kapacivitet\|termiska kapacitansen]] kan man beräkna temperaturutvecklingen om den tillförda och bortförda effekten är kända.
$$
\frac{dT}{dt}=\frac{P_t-P_b}{C_t}
$$
där $T$ är temperaturen, $P_t$ är tillförd [[Effekt\|effekt]], $P_b$ är bortförd [[Effekt\|effekt]] samt $C_t$ är den [[Termisk Kapacivitet\|termiska kapacitansen]].

Den bortförda effekten beror på flera storheter, framförallt temperaturskillnaden och den termiska resistansen mellan objektet och omgivningen. Om kylningen sker genom värmeavgivning till luften spelar även luftens hastighet roll. Om man inte har en fläkt måste luften som är närmast förflyttas genom konvektion (varm luft stiger uppåt), vilket går sakta => bortförd [[Effekt\|effekt]] minskar. Objektets färg är också viktig, pga [[Svartkroppsstrålare\|svartkroppsstrålning]]. Det är dock rimligt att anta att den bortförda effekten endast beror av temperaturskillnad och [[Resistans\|resistans]],
$$
P_b=\frac{T-T_a}{R_t}
$$
där $T_a$ är omgivningens temperatur och $R_t$ är den termiska resistansen mellan objektet och omgivningen. Färg och forcerad ventilation är oftast inräknade i den termiska resistansen!

Den *dynamiska termiska ekvationen* för ett objekt som tillförs effekten $P_t$, befiner sig i en ogmivning med temperaturen $T_a$, har den [[Termisk Kapacivitet\|termiska kapacitansen]] $C_t$ och den termiska resistansen $R_t$ är


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/den-dynamiska-termiska-ekvationen/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">





$
\frac{dT}{dt}=\frac{P_t}{C_t}-\frac{T-T_a}{R_t\cdot C_t}=- \frac{T}{R_t\cdot C_t}+\frac{P_t}{C_t}+\frac{T_a}{R_t\cdot C_t}
$

</div></div>


Den termiska kretsen har [[Tidskonstant\|tidskonstanten]] $R_tC_t$. Ett välisolerat föremål som kan lagra mycket [[Värme\|värme]] får en lång [[Tidskonstant\|tidskonstant]] så att dess temperatur förändras långsamt (högt $R_t$ och $C_t$).


See also -> [[Modell av temperaturdynamik\|Modell av temperaturdynamik]]