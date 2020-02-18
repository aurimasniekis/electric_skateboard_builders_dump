# HAL sensor wire pin-out

### Replies: 12 Views: 1167

## \#1 Posted by: mmaner Posted at: 2017-06-03T21:48:44.219Z Reads: 133

```
I've got x2 DIY/TB VESC's and x2 Polar 6354 190kv sealed motors.  Im trying to make HAL sensor cables to to run hybrid mode.  I have the JST PH 2.0mm 6 pin cables, but I don't know what header to use to connect on the motor side nor do I know the wire order.  

I've searched here, endless sphere and googled my ass off...all I achieved is now I'm more confused then when I started.  Can someone diagram the HAL sensor cable and identify the motor side header?  Thanks
```

---
## \#2 Posted by: mccloed Posted at: 2017-06-03T22:37:01.009Z Reads: 130

```
Does this help?

<img src="/uploads/db1493/original/3X/f/4/f403c693cde51b8c59f23ef55522789962e94895.PNG" width="281" height="500">
```

---
## \#3 Posted by: mmaner Posted at: 2017-06-03T22:38:36.619Z Reads: 116

```
Kind of, JUST ZH is the header for the motor side, as I understand it, but I need the female​ header that will couple to it...also the wire pin-out.  Thanks
```

---
## \#4 Posted by: Surfer Posted at: 2017-06-03T22:57:30.239Z Reads: 109

```
I hope doesn't sound too stupid, but I use the adaptor from maytech to connect the polar 6355 sealed to the vesc, and just is plug and play. If it helps a picture let me know.
```

---
## \#5 Posted by: mmaner Posted at: 2017-06-03T23:03:34.834Z Reads: 106

```
Yes please, and a link if you have one.  I'd rather make it but I'll just buy them to get it done 😀.
```

---
## \#6 Posted by: Surfer Posted at: 2017-06-03T23:12:58.653Z Reads: 103

```
<img src="/uploads/db1493/original/3X/7/d/7d1695ec9bd8ca663f7b2e358fcab78840060214.jpg" width="690" height="388"> If it's not clearly enough I do another disassembling more.
Sorry no link, it was included with the maytech drv cooker
```

---
## \#7 Posted by: mmaner Posted at: 2017-06-03T23:16:01.439Z Reads: 97

```
That'll work. Thanks.

Still looking g for a pin-out if anyone has it.
```

---
## \#8 Posted by: Surfer Posted at: 2017-06-03T23:20:58.212Z Reads: 104

```
I think drv cooker autodetect the sensors order, then I think it's only important + -. Please don't believe me, confirm it before. :smiley:
```

---
## \#9 Posted by: Jinra Posted at: 2017-06-03T23:33:34.964Z Reads: 104

```
red = 5v
white = temp
black = GND

The rest are hall 1/2/3, order doesn't matter but you **must** do motor detection to get the hall positions.

You can see from my Carbonated build that I simply soldered the bare wires from the JST-PH 2.0mm 6pin header to the leads on the Polar motor

<img src="/uploads/db1493/original/3X/5/0/50429702ea742d482000d9457d9b57202380c0d3.png" width="668" height="500">
```

---
## \#10 Posted by: mmaner Posted at: 2017-06-04T01:25:31.137Z Reads: 101

```
Great, ty sir.
```

---
## \#11 Posted by: mmaner Posted at: 2017-06-14T20:08:54.912Z Reads: 85

```
Does anyone have any JST-ZH 6pin 1.5mm pitch headers they would sell cheap.  I would like x4 but I just need x2 right now.  Thanks
```

---
## \#12 Posted by: Acido Posted at: 2018-10-26T14:03:09.709Z Reads: 36

```
Those are for vesc?
If you don't find any lmk

damn why dont i read the dates
```

---
