# Problem connect to vesc built in nrf

### Replies: 10 Views: 440

## \#1 Posted by: m.kicker Posted at: 2018-07-04T07:59:04.829Z Reads: 79

```
Hi!

I would like to communicate directly to the vesc built in nrf. I want to send data to the vesc with an arduino+nrf chip.
So first I thought to etablish a simple connection like receive the alive packets on an arduino+nrf. But it is not working.

If I keep the default firmware on the vesc and configure the nrf ( speed 1MBPS, channel 76 ,  etc), what should I do on the arduino ? A simple nrf receiver on arduino with the same configuration is not working .

PLease help!

Thanks!
M
```

---
## \#2 Posted by: Wentworth Posted at: 2018-07-04T09:29:22.958Z Reads: 72

```
https://www.electric-skateboard.builders/t/nunchuk-problem/60402/2
This is a post I sent, I am doing this, I do not know if it is similar to yours. This does not use Arduino, you can follow this to make the same.
```

---
## \#3 Posted by: Wentworth Posted at: 2018-07-04T09:48:38.599Z Reads: 60

```
I seem to have found what you want. You confirm it.
https://endless-sphere.com/forums/viewtopic.php?f=35&t=73812
```

---
## \#4 Posted by: m.kicker Posted at: 2018-07-04T10:04:52.460Z Reads: 57

```
The arduBoardControl uses 2 arduino : one for the remote and another on vesc. I don't have the same configuration : one arduino+nrf and vesc (built-in nrf). So no arduino to receive on vesc. I don't think this project will help me a lot.

I looked at the nunchuck code of Vedder but it is not simple to translate it to arduino. So I wanted to configure an arduino+nrf just to receive the alive packets first.
```

---
## \#5 Posted by: Wentworth Posted at: 2018-07-05T01:06:54.299Z Reads: 47

```
If you have any news or progress, please let me know. I'm studying this thing too
```

---
## \#6 Posted by: m.kicker Posted at: 2018-07-10T14:30:29.356Z Reads: 39

```
Hi! 
 I did it! Connect to the nrf with an arduino+nrf

I wrote a custom app which turn off the nrf driver. Then it configures the nrf and start listening.

Configuration : no retries, no auto ack, no dynamic payload, no CRC, no feature

Here are the registers
SETUP AW 0x3
RX PW P0 0x20
RX_PW_P1  0x20
EN_AA 0
EN_RXADDR 0x3
RF-CH 0x4c
RF_SETUP 0x47
CONFIG 0x3
DYNPD 0
FEATURE 0
SETUP_RETRY 0

I receive " hello world" from arduino
```

---
## \#7 Posted by: Wentworth Posted at: 2018-07-15T07:38:18.557Z Reads: 26

```
Congratulations! Looking forward to your further information！
```

---
## \#8 Posted by: Wentworth Posted at: 2018-08-01T07:08:25.584Z Reads: 14

```
Hey friend. Is there any new progress?
```

---
## \#9 Posted by: m.kicker Posted at: 2018-08-02T08:20:33.450Z Reads: 10

```
For Now I can send a data structure to the VESC. I planned to enable auto ack or retries. 
WHat I don't understand is  : with CRC enabled on VESC , the receiver FIFO is empty. When I disable CRC on VESC I can receive ( even with CRC on transmitter ).

Does the chip compute CRC itself and reject packets if not wrong CRC ?
```

---
## \#10 Posted by: Wentworth Posted at: 2018-08-02T08:50:59.809Z Reads: 9

```
I haven't studied the data structure, so I can't help you. It seems that you have to have a hard time. Looking forward to your new news
```

---
