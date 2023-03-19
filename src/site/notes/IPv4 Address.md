---
{"dg-publish":true,"permalink":"/i-pv4-address/","tags":["kommunikationssystem"]}
---


![Pasted image 20230214164030.png](/img/user/images/Pasted%20image%2020230214164030.png)
The [[IPv4\|IPv4]] address contains the network-ID and the host-ID. In order to know which is which you can use an address with a mask or write the address on [[Classless Addressing\|CIDR]] form.

The mask is the same length as the address and has a one if that bit is part of the network id and a zero if it's a part of the host id.
[[Classless Addressing\|CIDR]] form is on the form IP/"bit-number where the host id starts".