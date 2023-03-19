---
{"dg-publish":true,"permalink":"/go-back-n-arq/","tags":["kommunikationssystem"]}
---


![Pasted image 20230123163844.png](/img/user/images/Pasted%20image%2020230123163844.png)
![Pasted image 20230123164030.png](/img/user/images/Pasted%20image%2020230123164030.png)
Använder [[Sliding Window\|Sliding Window]]. Om man använder fel fönsterstorlek kan ram nummer 3 exempelvis uppfattas som en ny ram 3 av mottagaren. Bra att ha en liten buffer mellan användbara och icke användbara [[Framing\|ramar]].

Om sändaren får en ACK för ett tidigare sekvensnummer kommer den skicka om alla [[Framing\|ramar]] från det numret och framåt, om den int ehar fått nästa ACK innan nästa timeout.

Alla ACK måste inte komma fram, om ACK 4 och ACK 5 tappas bort på vägen, men ACK 6 kommer fram så vet man ändå att de tidigare ACK:en har skickats.

Mottagaren skickar ACK med sekvensnummer för nästa [[Packet\|paket]] den vill få.

If the wrong window size is selected, duplicate frames can be accepted as new?