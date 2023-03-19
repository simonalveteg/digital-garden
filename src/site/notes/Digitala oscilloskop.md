---
{"dg-publish":true,"permalink":"/digitala-oscilloskop/","tags":["mätteknik"]}
---

Minnet i ett digitalt [[Oscilloskop\|oscilloskop]] används för olika ändamål, ex:
- Inspelningsminne (Acquisition Memory)
- Bildskärmsminne (Display Memory)
- Vågformsminne (Waveform Memory)
- Inställningsminne (Setting Memory)

Inspelningsmnnet utnyttjas vid varje inspelning, och överförs direkt efter inspelningen till bildskärmsminnet som lagrar punkterna som visas på skärmen. Inspelningsminnet delas upp mellan de använda kanalerna, så ju fler kanaler man använder desto mindre inspelningsminne har varje [[Signal\|kanal]].


## Dötid
En DSO (Digital Storage Oscilloscope) spelar in mätpunkter i inspelningsminnet och kopierar det därefter till bildskärmsminnet (se [[Effektiv Samplingshastighet\|Effektiv Samplingshastighet]]), vissa DSO:er har flera mikroprocessorer som kan arbeta parallellt men det är vanligast att en sköter allt, och då måste den ta en paus från att spela in för att överföra det till bildskärmen. Ju högre inspelningsminne desto längre sammanhängande partier får man.
![inspelningstid och dötid oscilloskop.png](/img/user/images/inspelningstid%20och%20d%C3%B6tid%20oscilloskop.png)

# Effektiv [[Bandbredd\|Bandbredd]]
Den effektiva [[Bandbredd\|bandbredden]] i ett digitalt [[Oscilloskop\|oscilloskop]] påverkas av den analoga [[Bandbredd\|bandbredden]] och samplingshastigheten
## [[Bandbredd\|Bandbredd]]
Bildskärmen spelar ingen roll för [[Bandbredd\|bandbredden]], allt beror på själva inspelningen, och då är det endast ingånsförstärkaren och [[Sampling\|samplingfrekvensen]] som har betydelse för [[Bandbredd\|bandbredden]].

Den analoga [[Bandbredd\|bandbredden]] i ingångssteget sätter en övre gräns för vilka frekvenser som kan återges.

Om ett digitalt [[Oscilloskop\|oscilloskop]] har [[Bandbredd\|bandbredden]] 100MHz kan det inte användas för noggranna tid- och spänningsmätningar på pulser med frekvensen 100MHz. Pulser är sammansättningar av ofantligt många olika (höga) frekvenser, vilka då kommer dämpas väldigt mycket vid ingången. 

> [[Oscilloskop\|Oscilloskop]] är inte användbara för noggranna mätningar över hela analoga [[Bandbredd\|bandbredden]].

Oscilloskopets [[Bandbredd\|bandbredd]] bör överstiga frekvensen av en ansluten sinussignal med en faktor 5 vid amplitudmätning
Oscilloskopets [[Stigtid\|stigtid]] bör understiga stigtiden av en ansluten pulssignal med en faktor 5 vid tidmätning.

## Samplingshastighet
För att få någorlunda realistiska bildskärmsåtervigningar av insignalen bör man ha en viss marginal till [[Nyquists Samplingskriterium\|Nyquist-frekvensen]]

## FFT (Fast Fourier Transform)
FFT är en algoritm som transformerar den insamplade [[Signal\|signalen]] från DSO:ns normala tidsdomän till frekvensdomänen (spänning över frekvens) via en Foriertransformation. Med FFT kan vi se signalens frekvensinnehåll på skärmen.