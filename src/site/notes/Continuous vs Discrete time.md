---
{"dg-publish":true,"permalink":"/continuous-vs-discrete-time/","tags":["digitalsignalbehandling"]}
---


* Analog systems are continuous, but not very flexible
* Digital systems are discrete, and can be very flexible
* [[Sampling\|Sampling]] and [[Reconstruction\|reconstruction]] is needed for a digital system to interact with the real world.

You can’t do everything with analog circuits, sometimes they are difficult to realise. They don’t have the possibility to store signals and they aren’t very flexible. There are few instances irl where you get discrete signals in a natural way. Discrete signals are mostly man made. Using only discrete time singals we can essentially not interact with the real world, but they can be very flexible and programmable.

The best of both worlds:
input signal → [[Sampling\|sampling]] (analog to digital) → digital processing → [[Reconstruction\|reconstruction]] (digital to analog) → output signal
A mixture of continous and discrete signals with digital signal processing in the middle.


The fundamental difference between continuous-time and [[Discrete-time signals\|discrete-time signals]] is in their range of values for $F$ and $\Omega$ or $f$ and $\omega$. 

[[Relations among frequency variables\|Relations among frequency variables]]