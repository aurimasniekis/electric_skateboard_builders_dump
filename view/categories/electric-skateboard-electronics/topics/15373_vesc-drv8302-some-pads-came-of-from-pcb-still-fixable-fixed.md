# VESC DRV8302 some pads came of from pcb, still fixable? \[fixed\]

### Replies: 5 Views: 1574

## \#1 Posted by: mclightning Posted at: 2016-12-29T23:02:10.244Z Reads: 88

```
Hi,

In an effort to replace fried DRV8303 on my VESC. I disassembled the fried 8302.
But while doing that, some of the pin solder areas on the pcb came off and some bent.
Here is a photo of it (sorry for uncleaned board, dont have solder wick & isopropyl yet):
[http://imgur.com/a/1Ytwc](http://imgur.com/a/1Ytwc)


You can see the pin areas on top left corner are gone.
But these pins (4 & 5) look unused. Am I correct?
https://raw.githubusercontent.com/vedderb/bldc-hardware/master/design/PNGs/Schematic-7.png

Do you think this is still fixable or ruined?
```

---
## \#2 Posted by: Blasto Posted at: 2016-12-29T23:41:23.393Z Reads: 71

```
Still good, clean it up with some solder wick
```

---
## \#3 Posted by: mclightning Posted at: 2016-12-30T13:08:22.617Z Reads: 44

```
Some of the solder pads are bent but I believe they are fixable. 
http://imgur.com/a/EJOn6
```

---
## \#4 Posted by: mclightning Posted at: 2016-12-30T18:43:37.574Z Reads: 37

```
result : it is completely dead.

soldered new drv8302. checked all pins to secure they are not touching each other. check all pins reaching to end of lines on the pcb.

1st test : leds come on and off immediately at start, then also on power off.

2nd test : while trying to secure connections more. Fault pin pad came off. Now it is not turning on even the leds.

A sad day for my hobby. I dont know what to do with this board now. I also spend extra on fixing equipment + new drv8302 chip.
```

---
## \#5 Posted by: mclightning Posted at: 2016-12-30T21:12:15.551Z Reads: 28

```
Hi everyone!

Great news! I managed to fix it. It is working. Although many pads came off on the pcb, they were mostly unused pins. And I made bridge for 1 pin.
https://www.instagram.com/p/BOp-QMWDTST/

Are there any steps I should take to verify it is working safely?
```

---
