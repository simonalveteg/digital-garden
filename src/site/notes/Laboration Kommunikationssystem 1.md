---
{"dg-publish":true,"permalink":"/laboration-kommunikationssystem-1/","tags":["laboration","kommunikationssystem"]}
---


# A
## 1
You should sample the pulse signal at it's midpoint, which gives the maximum protection against drifting.
## 2
A pulse signal is what is sent in the physical medium (air) between the two nodes, and the pulses corresponds to bits.  A symbol is a collection of bits.
## 3
A preamble is a collection of symbols or bits that is used to inform the receiver of what the signal is. The receiver can use the preamble to align it's sampling rate with the signal.
## 4
The maximum drift is half of the pulsewidth. More than that and the sampled value will be wrong.
## 5
The objective of the SFD is to signal the start and end of a frame. The preamble is not enough, since there would be no way of differentiating the preamble from the data. 
## 6
The channel bit rate is $\frac{1}{T_s}=\frac{1}{0.1}=10$ bits/s.
## 7
The effective bit rate relates to the bits that are used for data. The data bits divided by the total number of bits, multiplied by the bit rate gives the effective bit rate. In this case it is $10\cdot \frac{8}{48}=1.67$ bits/s.
## 8
The total amount of bits that need to be sent is $48\cdot2=96$ which means it will take $9.6$ seconds, due to the bit rate of 10 bits/s.
# B
## 1
```C
int readBit(int i) {
	int tbit = ((tx.frame << i) & 0x8000 ) == 0 ? 0x0 : 0x1;
	return tbit;
}

```
## 2
```C
void sendPreamble() {
	byte preamble = PREAMBLE_SEQ;
	int msb;
	for(int i = 0; LEN_PREAMBLE; i++) {
		preamble <<= i;
		msb = (preamble & 0x80) == 0 ? 0 : 1;
		digitalWrite(PIN_TX, msb);
		delay(T_S);
	}
}
```
## 3
```C
void putBit(int i, int rbit) {
	temp = rbit << (LEN_FRAME - i - 1);
	rx.frame = rx.frame | temp;
} 
```
## 4
```C
void setSelectedLED() {
	tx.frame_payload = sh.selected_led();
	tx.frame_generation();
}
```
# C
## 1
![Pasted image 20230126133337.png](/img/user/images/Pasted%20image%2020230126133337.png)
## 2
![Pasted image 20230126133329.png](/img/user/images/Pasted%20image%2020230126133329.png)
## 3
In L1_SEND, which belongs to the physical layer, a tx.frame is transmitted to the other node. L1_RECEIVE awaits a message from the other node. When the preamble is found it synchronizes with it, looks for the SFD and stores the incoming message. L2_FRAME_REC processes the received frame on the data layer. L2_DATA_SEND also belongs to the data layer, and processes a frame to be sent. L2_ACK_REC processes the reception of an ACK frame and L2_ACK_SEND processes the sending of an ACK frame. L2_RETRANSMIT handles [[Automatic Repeat Request algorithm\|ARQ]] logic. 
The APP_PRODUCE state belongs to the [[Application Layer\|application layer]] and takes input from the user.
![Pasted image 20230127164002.png](/img/user/images/Pasted%20image%2020230127164002.png)