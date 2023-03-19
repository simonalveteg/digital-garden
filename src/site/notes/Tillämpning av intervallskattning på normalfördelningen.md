---
{"dg-publish":true,"permalink":"/tillaempning-av-intervallskattning-pa-normalfoerdelningen/","tags":["matematiskstatistik"]}
---

Det är vanligt att man på grundval av insamlade data önskar göra en [[Intervallskattning\|intervallskattning]] av någon okänd parameter och att [[Normalfördelning\|normalfördelning]] kan förutstättas i den använda modellen.

# [[Konfidensintervall\|Konfidensintervall]] för [[Väntevärde\|väntevärdet]]
Låt $x_{1},\dots,x_n$ vara et [[Slumpmässigt Stickprov\|slumpmässigt stickprov]] från $N(\mu,\sigma)$ där $\mu$ är okänt. Då är 
$$
I_\mu=(\overline x-\lambda_{\alpha/2}D,\overline x+\lambda_{\alpha/2}D)
$$
om $\sigma$ är känt ($D=\frac{\sigma}{\sqrt{ n }}$), samt
$$
I_\mu=(\overline x-t_{\alpha/2}(f)d,\overline x+t_{\alpha/2}(f)d)
$$
om $\sigma$ är okänt ($d=s/\sqrt{ n }$ , $f=n-1$)
ett tvåsidigt [[Konfidensintervall\|konfidensintervall]] för $\mu$ med [[Konfidensgrad\|konfidensgraden]] $1-\alpha$.

Det viktiga när man använder en sats som ovan, är att tänka på om ens data har samlats in på ett sätt så att förutsättningarna för satsen är uppfylld.

# [[Konfidensintervall\|Konfidensintervall]] för [[Standardavvikelse\|standardavvikelsen]]
Låt $x_{1},\dots,x_n$ vara ett [[Slumpmässigt Stickprov\|slumpmässigt stickprov]] från $N(\mu,\sigma)$ där $\sigma$ är okänt. Då är
$$
I_\sigma=(k_{1}s,k_{2}s)
$$
där $k_{1}=\sqrt{ f/\mathcal{X}_{\alpha/2}^{2}(f) }$ och $k_{2}=\sqrt{ f/\mathcal{X}_{1-\alpha/2}^{2}(f) }$. ($f=n-1$)
ettkonfidensintervall fö r$\sigma$ med [[Konfidensgrad\|konfidensgraden]] $1-\alpha$.

# [[Konfidensintervall\|Konfidensintervall]] för differens mellan [[Väntevärde\|väntevärden]]

Låt $x_{1},\dots,x_{n_{1}}$ och $y_{1},\dots,y_{n_{1}}$ vara [[Slumpmässigt Stickprov\|slumpmässiga]], av varandra oberoende stickprov från $N(\mu_1,\sigma_1)$ respektive $N(\mu_{2},\sigma_{2})$. Om $\sigma_{1}$ och $\sigma_{2}$ är kända så är 
$$
I_{\mu_{1}-\mu_{2}}=(\overline x-\overline y-\lambda_{\alpha/2}D,\overline x-\overline y+\lambda_{\alpha/2}D)
$$
ett [[Tvåsidigt Konfidensintervall\|tvåsidigt konfidensintervall]] för $\mu_{1}-\mu_{2}$ med [[Konfidensgrad\|konfidensgraden]] $1-\alpha$; här är $D=\sqrt{ \sigma_{1}^{2}/n_{1}+\sigma_{2}^{2}/n_{2} }$.

Om $\sigma_{1}=\sigma_{2}=\sigma$ där $\sigma$ är okänt så är
$$
I_{\mu_{1}-\mu_{2}}=(\overline x-\overline y-t_{\alpha/2}d,\overline x-\overline y+t_{\alpha/2}d)
$$
ett [[Tvåsidigt Konfidensintervall\|tvåsidigt konfidensintervall]] för $\mu_{1}-\mu_{2}$ med konfdensgraden $1-\alpha$; här är $d=s\sqrt{ 1/n_{1}+1/n_{2} }$ där $s=\sqrt{ \frac{Q_{1}+Q_{2}}{(n_{1}-1)+(n_{2}-1)} }$ och $f=(n_{1}-1)+(n_{2}-1)$.


