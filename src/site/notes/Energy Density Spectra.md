---
{"dg-publish":true,"permalink":"/energy-density-spectra/","tags":["digitalsignalbehandling"]}
---

By squaring both sides of the magnitude relation we get $$|Y(\omega)|^{2}=|H(\omega)|^{2}|X(\omega)|^{2}$$ which tells us that the energy density spectra of the input and output signals of the filter are related as 
$$S_{yy}(\omega)=|H(\omega)|^{2}S_{xx}(\omega)$$
Since [[Energi\|energy]] is related to magnitude squared we can illustrate the magnitude relation 
![Pasted image 20220919140054.png](/img/user/images/Pasted%20image%2020220919140054.png)
leading to corresponding energy spectra relation 
![Pasted image 20220919140112.png](/img/user/images/Pasted%20image%2020220919140112.png)
Integration of $S_{yy}(\omega)$ tells us that the [[Energi\|energy]] of the output signal is $$E_{y}=\frac{1}{2 \pi} \int_{-\pi}^{\pi}|H(\omega)|^{2}S_{xx}(\omega)d {\omega}$$



> Energy spectra are very important for many applications, like wireless communications where there are strict regulation son how large it can be, both inside and outside our "own" frequency band.
