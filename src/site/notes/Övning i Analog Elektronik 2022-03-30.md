---
{"dg-publish":true,"permalink":"/oevning-i-analog-elektronik-2022-03-30/","tags":["övning","analogelektronik"]}
---


[[Frekvenskompensering\|frekvenskompensering]]
- hur vi kan manipulera en krets beteende 

[[Maximal Flat Frekvensgång\|Butterworthsystem]] - [[Maximal Flat Frekvensgång\|MFM system]] 

1. [[Bandbreddsuppskattning\|Bandwidth estimation]]
we can come up with a value for maximum achievable [[Bandbredd\|bandwidth]] if we would have a [[Maximal Flat Frekvensgång\|MFM system]] with these poles, or if we would compensate our [[System (matematisk definition)\|System (matematisk definition)]] as an [[Maximal Flat Frekvensgång\|MFM system]]. [[Bandbreddsuppskattning\|Bandwidth estimation]] gives us the maximum achievable [[Bandbredd\|bandwidth]] when we compensate a [[System (matematisk definition)\|System (matematisk definition)]] with some [[Slingpoler och Slingnollställen\|loop-poles]]. [[Bandbreddsuppskattning\|Bandwidth estimation]] is done using LP: [[LP-produkten\|Loop-gain pole product]] $= | 1-AB(0) |p_1p_2p_3…p_n$(n [[Dominanta och Icke-dominanta poler\|dominanta poler]]).
$$BW=\omega_0=LP_{n}^\frac{1}{n}$$
2. Find [[Systempoler\|system poles]] of [[Maximal Flat Frekvensgång\|MFM system]]
If we convert our [[System (matematisk definition)\|System (matematisk definition)]] to [[Maximal Flat Frekvensgång\|butterworthsystem]], we can find the [[Systempoler\|system poles]].

If our [[System (matematisk definition)\|System (matematisk definition)]] is a second order [[System (matematisk definition)\|System (matematisk definition)]]:
$$p_{1,2}'=-\frac{\omega_{0}}{\sqrt{2}}(1\pm j) \Rightarrow \sum\limits p'=-\sqrt{2}\omega_{0}$$
![2nd order mfm system.png|350](/img/user/images/2nd%20order%20mfm%20system.png)

If our [[System (matematisk definition)\|System (matematisk definition)]] is a third order [[System (matematisk definition)\|System (matematisk definition)]]:
$$\begin{cases} p_{1}'= -\omega_{0}   \\ p_{2,3}'=-\omega_{0}\left( \frac{1}{2}\pm j\frac{\sqrt{3}}{2} \right)
\end{cases}\space\space\space \Rightarrow \sum\limits p'=-2\omega_{0}
$$
![3rd order mfm system.png](/img/user/images/3rd%20order%20mfm%20system.png)
3. Validity check!
it ( #question  it as in the compensation? The [[System (matematisk definition)\|System (matematisk definition)]] after compensation?) is valid if the sum of [[Systempoler\|system poles]] is $\leq$ the sum of loop poles. Otherwise we included a non-dominant pole in our calculations, in that case we start over form step one and remove the smallest pole

Vi vill sätta [[Systempoler\|systempolerna]] på cirkeln med radien av [[LP-produkten\|LP-produkten]]! När man flyttar [[Poler\|polerna]] på cirkeln förändras inte systemets [[Bandbredd\|bandbredd]]. 

för två [[Poler\|poler]] är det unconditionally [[Stabila och Instabila System\|stable]], men man kanske vill designa den på ett specifikt sätt (ex [[Maximal Flat Frekvensgång\|MFM]]). Även om den är [[Stabila och Instabila System\|stabil]] vill man ibland [[Frekvenskompensering\|frekvenskompensera]] för att öka [[Fasmarginal\|fasmarginalen]]. 




## Subject
[[Analog Elektronik\|Analog Elektronik]]
