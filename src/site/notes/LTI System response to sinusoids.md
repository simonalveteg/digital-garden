---
{"dg-publish":true,"permalink":"/lti-system-response-to-sinusoids/","tags":["digitalsignalbehandling"]}
---

Input $x(n)=Ae^{j \omega n}$ gives (through [[Faltning\|convolution]] with [[Impulssvar\|impulse response]]) $$y(n)=\sum\limits_{k=-\infty}^{\infty}h(k)Ae^{j \omega(n-k)}=\left(\sum\limits_{k=-\infty}^{\infty}h(k)e^{-j \omega k} \right)Ae^{j \omega n}$$
which is the [[Discrete-time Fourier transform\|DTFT]] of $h(n)$ times the input signal.
$$=H(\omega)Ae^{j \omega n}=H(\omega)x(n)$$
We say that $H(\omega)$ is the frequency response of the [[Linjära och Tidsinvarianta System\|LTI system]]. Complex sinusoids are eigenfunctions of [[Linjära och Tidsinvarianta System\|LTI systems]], with eigenvalue $H(\omega)$!

$cos(\omega n)$ and $sin(\omega n)$ is an eigenfunction of [[Linjära och Tidsinvarianta System\|LTI systems]] with real-valued [[Impulssvar\|impulse response]] with eigenvalue $H(\omega)=H*(-\omega)$.

Can also be described in terms of the magnitude and phase of $H(\omega)$
$$y(n)=H(\omega)Ae^{j \omega n}= |H(\omega)|e^{j\angle H(\omega)}Ae^{j \omega n}$$
$$=|H(\omega)|Acos(\omega(n-\Delta(\omega)))$$
where $\Delta(\omega)=-\angle H(\omega)/\omega$ is the delay in number of samples (which isn't necessarily an integer).


> When you plot $X(\omega)$ the magnitude and the phase are plotted seperately because you usually want to see how the amplitude is affected seperately from the phase.

The delay of the [[Signal\|signal]] is typically frequency dependent and negative phase shifts give positive delays. 
