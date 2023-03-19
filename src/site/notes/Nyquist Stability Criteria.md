---
{"dg-publish":true,"permalink":"/nyquist-stability-criteria/","tags":["reglerteknik"]}
---


[[Nyquist plot\|Nyquist plot]]
Tells us wether or not our [[System (matematisk definition)\|System (matematisk definition)]] will be [[Stabila och Instabila System\|stable]] when we close the loop.

It is a little more general because we might not have a [[Överföringsfunktion\|transfer function]] model, only measurements of a [[System (matematisk definition)\|System (matematisk definition)]].

We draw a [[Nyquist plot\|nyquist plot]] and get an easy yes or no to wether or not the [[System (matematisk definition)\|System (matematisk definition)]] is [[Stabila och Instabila System\|stable]]. 

It gives a notion of [[Robustness\|robustness]], since we can see if we are close to being unstable or not.

The nyquist criterion regards the point $- \frac{1}{K}$. If that point is to the left of the [[Nyquist plot\|nyquist plot]] the [[System (matematisk definition)\|System (matematisk definition)]] is [[Stabila och Instabila System\|stable]]. 

If you draw a circle around the nyquist criterion point, it's size is a measure of how [[Robustness\|robust]] the [[System (matematisk definition)\|System (matematisk definition)]] is.

This is the simple version that needs the [[Överföringsfunktion\|transfer function]] to be [[Stabila och Instabila System\|stable]].

The nyquist criterion gives us two measurements regarding the [[Stabila och Instabila System\|stability]] of the [[System (matematisk definition)\|System (matematisk definition)]] [[Gain margin\|Gain Margin]] and [[Fasmarginal\|Phase Margin]]

# Användningsområden
Punkten $- \frac{1}{K}$ ska ligga till vänster om nyquist kurvan. När kurvan är i vänster halvplan får man värdet som punkten måste vara till vänster om vid vinkeln $-\pi$. Sätt in den vinkeln i funktionen för fasen för att få fram vilken frekvens det är vid. Sätt in frekvensen i funktionen för [[Förstärkning\|gain]] för att få fram vilket värde $K$ har vid skiftet från [[Stabila och Instabila System\|instabilt]] till [[Stabila och Instabila System\|stabilt]].