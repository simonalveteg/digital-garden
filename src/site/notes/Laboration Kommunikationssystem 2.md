---
{"dg-publish":true,"permalink":"/laboration-kommunikationssystem-2/","tags":["laboration","kommunikationssystem"]}
---


# A
## 1
a) The development node's own adress is set in code using sh.my_adress
b) The master node's adress is set using the DIP switches 1 and 2. If both are off addressing is inactive, and otherwise it follows the binary convention. S1S2=01 gives adress 1 and so on.
c) The same way as the masters node.
## 2
If the development node doesn't receive an ack within a certain timeframe it should resend the frame.
## 3
If the ACK isn't received it will send out a new frame, which will prompt the master node to send a new ACK. This continues until the ACK is received.
## 4
The frame is resent until the correct ACK is received.
# B
![Pasted image 20230216143701.png](/img/user/images/Pasted%20image%2020230216143701.png)
![Pasted image 20230215185210.png](/img/user/images/Pasted%20image%2020230215185210.png)
# C
![Pasted image 20230127164002.png](/img/user/images/Pasted%20image%2020230127164002.png)

# D
## 1
![Pasted image 20230215134858.png](/img/user/images/Pasted%20image%2020230215134858.png)
## 2
![Pasted image 20230215111407.png](/img/user/images/Pasted%20image%2020230215111407.png)
