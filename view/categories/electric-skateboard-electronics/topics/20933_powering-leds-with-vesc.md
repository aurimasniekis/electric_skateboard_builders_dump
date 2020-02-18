# Powering leds with vesc

### Replies: 10 Views: 881

## \#1 Posted by: Gabriel_Robinson Posted at: 2017-04-13T15:24:40.032Z Reads: 151

```
Can I power led strips using the vesc? With a servo spliter powering the reciever and leds?
```

---
## \#2 Posted by: mmaner Posted at: 2017-04-13T16:28:32.447Z Reads: 137

```
Don't kill your VESC, just get one of these...
https://www.amazon.com/gp/product/B01MT81GO1/ref=oh_aui_detailpage_o02_s01?ie=UTF8&psc=1
```

---
## \#3 Posted by: ReeCorDs Posted at: 2017-11-26T19:02:46.672Z Reads: 80

```
How to wire this up?
```

---
## \#4 Posted by: DevinG Posted at: 2018-04-11T22:28:34.997Z Reads: 57

```
Link is now 404
```

---
## \#5 Posted by: b264 Posted at: 2018-04-11T22:29:32.697Z Reads: 54

```
[DROK DC-DC Buck Converter 3A Adapter Power Supply Module Step Down Regulator 12V/24V/36V to 5V with USB+Micro USB](https://www.amazon.com/gp/product/B016XI9CZQ/ref=oh_aui_detailpage_o00_s00?ie=UTF8&psc=1)
```

---
## \#6 Posted by: DevinG Posted at: 2018-04-11T22:32:49.119Z Reads: 52

```
I appreciate the quick link! Im asking because my led strip had pin holes similar to receiver...im also trying to decern whether or not my focbox can handle this.
```

---
## \#7 Posted by: b264 Posted at: 2018-04-11T22:48:21.315Z Reads: 47

```
You can pull a maximum of 1A from the 5V line on your FOCBOX aside from what the RF receiver uses.  That's 5 watts.  Otherwise, use the buck converter.  If you pull too much it will cook the DRV8302 IC.
```

---
## \#8 Posted by: DevinG Posted at: 2018-04-11T23:11:14.515Z Reads: 43

```
Thanks thats good to know, however it sounds like the later is the safer bet.
```

---
## \#9 Posted by: evoheyax Posted at: 2018-04-11T23:15:09.759Z Reads: 42

```
I am power 8 led's per vesc without any issues, via the uart port. I use 1 vesc uart for bluetooth, 1 for my speedometer, and 2 to power the front and back leds, No issues so far...
```

---
## \#10 Posted by: b264 Posted at: 2018-04-11T23:57:50.638Z Reads: 37

```
It only matters how much current you are drawing, not where it goes.  LEDs can be anywhere from 0.005A to 36A
```

---
