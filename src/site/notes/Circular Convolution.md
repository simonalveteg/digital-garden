---
{"dg-publish":true,"permalink":"/circular-convolution/","tags":["digitalsignalbehandling"]}
---

When performing circular [[Faltning\|convolution]] of length $N$ between two signals we also time-reverse one of them, shift it relative to the other one, and sum the product of individual elements for each shift with the difference that we calculate indices mod $N$ and get a resulting sequence of length $N$ #question wtf står det ens här??

$$\circledast$$
The N-point [[Discrete Fourier Transform\|DFT]] of $y(n)$ is the product (for $k=0,1\dots N-1$)
$$
Y(k)=X_{1}(k)X_{2}(k)
$$
where 
$$
X_{1}(k)=X_{1}(z)\vert_{z=e^{j 2\pi k/N}}
$$


[[Circular to linear convolution\|Circular to linear convolution]]
[[Linear to circular convolution\|Linear to circular convolution]]