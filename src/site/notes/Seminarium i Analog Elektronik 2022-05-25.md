---
{"dg-publish":true,"permalink":"/seminarium-i-analog-elektronik-2022-05-25/","tags":["seminarium","analogelektronik"]}
---


gain bandwidth / unity gain bandwidth is the frequency at which loop gain reaches 0dB, and is equal to $w_{3dB}$ as long as p1 is dominant and p2 is much larger.


## Formler att memorisera

$$A=\frac{Q_{c}}{Q_{i}}=\frac{i_{c}}{v_{i}}$$
$$\beta=\left.\frac{Q_{i}}{Q_{c}}\right|_{Q_{s}=0}$$
$$A_{t\infty}=A_{t}=\left.\frac{Q_{L}}{Q_{s}}\right|_{A\rightarrow\infty,Q_{i}\rightarrow0}$$
$$A_{t}=A_{t\infty}\frac{-A\beta(s)}{1-A\beta(s)}$$
$$A_{t}(0)=A_{t\infty}\frac{-A\beta(0)}{1-A\beta(0)}$$
$$\text{Gain error}=|A_{t}-A_{t\infty}|$$
$$\text{Normalized gain error}=\frac{|A_{t}-A_{t\infty}|}{A_{t}}$$
$$p_{1},p_{2}.. = \text{loop gain poles}$$
$$p_{1}',p_{2}'..=\text{system poles}$$
$$w_{0}=LP^{\frac{1}{n}}=(|1-A\beta(0)|p_{1}p_{2}..p_{n})^{\frac{1}{n}}$$
$$\sum\limits p' \leq \sum\limits p$$
$$\text{for 2 pole MFM system: } \begin{cases}\sum\limits p'=-\sqrt{2}w_{0}\\p_{1,2}'=\frac{\sqrt{2}}{2}w_{0}(-1\pm j)\end{cases}$$
$$\text{for 3 pole MFM system: }\begin{cases}\sum\limits p'=-2w_{0}\\p_{1}'=-w_{0}\\p_{2,3}'=-\frac{w_{0}}{2}(1\pm\sqrt{3}j)\end{cases}$$
$$\text{phantom zero for 2 pole system: } n_{ph}=\frac{w_{0}^{2}}{\sqrt{2}w_{0}+\sum\limits p}\approx \frac{w_{0}}{\sqrt{2}} \text{ if } \sum\limits p'<<\sum\limits p $$
when you do capacitive narrowbanding you make a dominant pole, in that case you can use this equation, and #question inherently dominant pole when? (hörde inte vad han sa men det var något fall när den är inherently dominant typ?)
$$GB=\frac{UGB}{A_{t\infty}} \text{ for a system with a dominant pole}$$

$$\text{for current mirroring: } \frac{I_{A}}{I_{B}}=\frac{R_{B}}{R_{A}}$$

$$I_{C}=I_{S}e^\frac{V_{BE}}{V_{T}}\left(1+\frac{V_{CE}}{V_{A}}\right)$$
$$r_{\pi}=\frac{\beta_{f}V_{T}}{I_{C}}$$
$$g_{m}=\frac{I_{C}}{V_{T}}$$
$$r_{\pi}=\frac{\beta_{f}}{g_{m}}$$
$$I_{C}=\beta_{f}I_{B}$$
$$I_{E}=(\beta_{f}+1)I_{B}$$
$$\omega_{T}\approx \frac{g_{m}}{c_{\pi}}\Rightarrow \frac{1}{r_{\pi}c_{\pi}}=\frac{\omega_{T}}{\beta_{f}}$$
if you are aske to calculate input or output impedance of a [[Feedback System\|Feedback System]], you can open the feedback path and then you can calculate input/ouput impedance with for example thevenin model by replacing source with test source and divinging voltage by current. But then you need to correct r_i or r_out with a factor of 1+AB or 1/1+AB depending on the type of amplifier. Tänk dig vad som är idealt, faktorn ska göra det mer idealt. Om det är ström ut så vill vi ha så stor utimpedans som möjligt, och därmed vill vi göra resistansen större med en faktor 1+AB.


## Subject
[[Analog Elektronik\|Analog Elektronik]]
