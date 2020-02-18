# Learning to use uart with vesc and arduino

### Replies: 3 Views: 300

## \#1 Posted by: asaf123098 Posted at: 2019-06-19T20:38:48.008Z Reads: 51

```
Hi i wish to make my own arduino TX (with NRF24 module, and another arduino and nrf as receiver) that communicates with the vesc to run the motor, and i want to use the reverse button option from app settings -> ADC, is it possible with uart?
basically, im trying to copy the functions of a bought tx by myself because i want to learn how it works.

https://github.com/RollingGecko/VescUartControl/blob/master/VescUart.cpp
I found this repository but i couldn't under stand how am i supposed to wire the vesc to the arduino to the vesc, or how to use the methods in this repository

Will i need these connectors?
https://www.ebay.com/itm/Micro-JST-PH-2-0mm-7-Pin-Connector-plug-with-Wires-Cables-10-Sets/272566229599?epid=20008518661&hash=item3f76369a5f:g:snwAAOSwA3dYT7-i

Can i brick the vesc by mistake when trying to use the uart?
If so, how would i be able to fix it?

Any help on how to make my own uart tx and rx would be awesome, thanks!!
```

---
## \#2 Posted by: Pimousse Posted at: 2019-06-19T22:19:52.158Z Reads: 37

```
Rollinggecko's library is an old one.
Give @solidgeek 's one a try.

[quote="asaf123098, post:1, topic:96954"]
Can i brick the vesc by mistake when trying to use the uart? If so, how would i be able to fix it?
[/quote]
You can't really brick the VESC just using UART. Or maybe if you send config write commands, maybe.
If bricked, get a ST-Link and follow one of the tutorials you may find here and there.
```

---
## \#3 Posted by: asaf123098 Posted at: 2019-06-20T04:53:02.420Z Reads: 27

```
Ok, i will try to look at solidgeek's library,
The only part im missing now is the wiring, in solid geeks receiver scheme he only shows to wire the Arduino's rx tx pins to uart, but he wont show where to connect to the vesc

I found [this](http://vedder.se/wp-content/uploads/2015/01/PCB_Front.png) picture that show where s the uart port on the vesc, but not the pinout of the port,

And [this](http://vedder.se/wp-content/uploads/2015/01/Schematic-1.png) picture, in which P3 - PWR_COMM connector looks like it the uart port, but it has only 6 pins and uart has 7, so i cant identify the pins myself

Would [this](https://rover.ebay.com/rover/0/0/0?mpre=https%3A%2F%2Fwww.ebay.ca%2Fulk%2Fitm%2F382975017845) st link do the job in case of a bricked vesc?
```

---
