---
{"dg-publish":true,"permalink":"/periodic-sampling/","tags":["mätteknik","digitalsignalbehandling"]}
---


Periodic [[Sampling\|sampling]] (or uniform [[Sampling\|sampling]]) is the type of [[Sampling\|sampling]] used most often in practice. This is described by the relation
$$x(n)=x_{a}(nT)$$
where $x(n)$ is the [[Discrete-time signals\|discrete-time signal]] obtained by taking samples of the analog signal $x_{a}(t)$ every $T$ seconds ([[Sampling Period\|sampling period]]/[[Sampling Period\|sampling interval]]). 
$$F_{s}=\frac{1}{T}$$
is called the *[[Sampling Period\|sampling rate]]*, or the [[Sampling Period\|sampling frequency]].

Periodic sampling establishes a relationship between the time variables $t$ of continuous-time signals $n$ of [[Discrete-time signals\|discrete-time signals]],
$$t=nT=\frac{n}{F_{s}}$$

The frequency variables $f$ (discrete-time) and $F$ (continuous-time) are linearly related as 


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/frequency-variable-relations/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




$f=\frac{F}{F_{s}}$


</div></div>


which is equivalent to 
$$\omega=\Omega T$$


## Repetitiva samplingsmetoder
Den *horisontella* uplösningen av en [[Signal\|signal]] beror bland annat på den använda samplingsmetoden. Man brukar skilja mellan [[Realtidssampling\|Realtidssampling]], [[Sekvensiell Repetitiv Sampling\|Sekvensiell Repetitiv Sampling]], och [[Slumpmässig Repetitiv Sampling\|Slumpmässig Repetitiv Sampling]].