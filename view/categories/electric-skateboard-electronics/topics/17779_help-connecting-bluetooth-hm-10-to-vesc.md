# Help connecting bluetooth HM-10 to VESC

### Replies: 6 Views: 2614

## \#1 Posted by: Eboosted Posted at: 2017-02-16T04:47:56.117Z Reads: 338

```
I've connected VCC, GND, TX and RX from the UARP port to the Bluetooth HM-10.

This is the one I bought:
https://www.amazon.com/gp/product/B015R3IJ4I/ref=oh_aui_search_detailpage?ie=UTF8&psc=1

I've installed VESC Connect for Android and I was able to connect to the module, it has a solid red led. The baud rate was left at the 9600 by default and app to use was set to PPM and UART, but I can't datalog or read config from VESC, no information is received by the phone.

What else could I try?
```

---
## \#2 Posted by: Blasto Posted at: 2017-02-16T04:58:51.278Z Reads: 334

```
did you connect like this?

BLE           VESC
VCC          3.3V
GND         GND
RX             TX
TX              RX
```

---
## \#3 Posted by: Eboosted Posted at: 2017-02-16T05:01:50.358Z Reads: 324

```
No, I connected:

RX RX
TX TX

should I switch it?
```

---
## \#4 Posted by: Blasto Posted at: 2017-02-16T05:02:36.685Z Reads: 316

```
[quote="Eboosted, post:3, topic:17779"]
should I switch it?
[/quote]

yep, don't worry, nothing damaged
```

---
## \#5 Posted by: Eboosted Posted at: 2017-02-16T05:06:34.007Z Reads: 313

```
Wow thanks a lot Blasto! There should a step by step somewhere. I've been battling for hours. It's connected now!
```

---
## \#6 Posted by: Blasto Posted at: 2017-02-16T05:26:16.475Z Reads: 312

```
did somewhat of a write up on the vedder forum and I think there's some info buried in a nunchuck thread (fuck knows where that is)

http://vedder.se/forums/viewtopic.php?f=15&t=75
```

---
