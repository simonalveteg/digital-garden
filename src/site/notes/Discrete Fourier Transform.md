---
{"dg-publish":true,"permalink":"/discrete-fourier-transform/","tags":["digitalsignalbehandling"]}
---

The discrete [[Fouriertransformationer\|Fourier transform]] is suitable for efficient digital implementations since it results in functions of a discrete variable.

We define the N-point DFT as
$$X(k)=\sum\limits_{n=0}^{N-1}x(n)e^{-\frac{j2 \pi kn}{N}}$$
where $N$ is the number of samples

the corresponding inverse transform is 
$$x(n)=\frac{1}{N}\sum\limits_{k=0}^{N-1}X(k)e^{j2\pi k\frac{n}{N}}$$

We avoid [[Aliasing\|aliasing]] if the [[Signal\|signal]] $x(n)$ is time-limited to the period $N$, and the DFT also uniquely defines $h\omega e_{2}$ which means we can recover $x(n)$ from $X(k)$.

The frequency samples of the [[Discrete-time Fourier transform\|DTFT]] $X(f)$ corresponds to $X(k)$ ? #question 

If our $N$ is larger than the [[Signal\|signal]] length $L$ we have [[Zero-Padding\|zero-padding]] with $N-L$ additional zeros.

[[Computational complexity of DFT\|Computational complexity of DFT]]
[[The DFT as a linear transformation\|The DFT as a linear transformation]]
[[Relationship between DFT and other transforms\|Relationship between DFT and other transforms]]
[[Essential properties of the DFT\|Essential properties of the DFT]]
[[DFT for filtering long signals\|DFT for filtering long signals]]
