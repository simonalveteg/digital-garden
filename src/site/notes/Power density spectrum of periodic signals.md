---
{"dg-publish":true,"permalink":"/power-density-spectrum-of-periodic-signals/","tags":["digitalsignalbehandling"]}
---

For a continuous signal the average power of a periodic signal is 
$$P_{x}=\frac{1}{T_{P}} \int_{T_{P}}|x(t)|^{2}dt = \sum\limits_{k=-\infty}^{\infty}|c_{k}|^{2}$$
where $|c_{k}|^{2}$ is the average power of the kth term in the series, located at frequency $kF_{0}$. With which you can draw a [[Power Density Spectrum\|Power Density Spectrum]].
![Pasted image 20220912135730.png](/img/user/images/Pasted%20image%2020220912135730.png)

For discrete-time periodic signals the average power is 
$$P_{x}=\frac{1}{N}\sum\limits_{n=0}^{N-1}|x(n)|^{2}=\sum\limits_{k=0}^{N-1}|c_{k}|^{2}$$
where $|c_{k}|^{2}$ is the average power of the kth term in the series, located at frequency $kf_{0}$. 
