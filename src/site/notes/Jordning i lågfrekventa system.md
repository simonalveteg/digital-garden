---
{"dg-publish":true,"permalink":"/jordning-i-lagfrekventa-system/","tags":["mätteknik"]}
---

För [[Jordning\|jordning]] av [[System (matematisk definition)\|System (matematisk definition)]] vid låga frekvenser behöver man undvika jordslingor, eller åtminstone minimera dess area. Annars kan externa magnetfält lätt inducera strömmar. Då är det lämpligt att använda **enpunktsjordning** (single point ground).
![enpunktsjordning.png](/img/user/images/enpunktsjordning.png)
![flerpunkt_vs_enpunkt.png|400](/img/user/images/flerpunkt_vs_enpunkt.png)

Problemet är [[System (matematisk definition)\|System (matematisk definition)]] som arbetar med både höga och låga frekvenser, men man kan jorda med jordledning i ena änden av [[System (matematisk definition)\|systemet]] och i andra änden koppla en [[Kapacitans\|kondensator]] mellan [[System (matematisk definition)\|systemet]] och jordpunkten. [[Kapacitans\|Kondensatorn]] fungerar som ett avbrott vid låga frekvenser, dvs fungerar endast som jordledare vid höga frekvenser (och ger en kort jordledning). En ström kan inte induceras då kretsen inte är sluten. Kallas **hybridjord**.