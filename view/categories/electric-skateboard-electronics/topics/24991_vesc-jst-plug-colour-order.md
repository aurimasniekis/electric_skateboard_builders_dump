# Vesc JST plug colour order

### Replies: 8 Views: 757

## \#1 Posted by: bigben Posted at: 2017-06-09T19:30:59.077Z Reads: 72

```
I'm wondering if anyone can help me with the arrangement of coloured wires into the 6 place jst lead on vesc 4?
I have got a new larger jst plug which now fits the vesc but unsure of the arrangement of colours.
I have red, black, white,yellow,blue and green. (group  buy 6374)
A nudge in the right direction would be appreciated.
I have both DIY and Enertion vescs.
```

---
## \#2 Posted by: bigben Posted at: 2017-06-09T19:36:01.283Z Reads: 70

```
Would it be in the same order as the vesc 6?
<img src="/uploads/db1493/original/3X/5/d/5dbab088931ceee7d2ef3a4804aa70a31984cad7.png" width="531" height="500">
```

---
## \#3 Posted by: Jinra Posted at: 2017-06-09T20:00:02.503Z Reads: 58

```
red = 5v
black = GND
white = temp
the others are hall 1/2/3
```

---
## \#4 Posted by: bigben Posted at: 2017-06-09T20:06:22.901Z Reads: 55

```
Thanks @Jinra. 
I can't see any markings on the vesc I have to tell which way they should go into the plugs though. 
Would they be the same as vesc 6?
```

---
## \#5 Posted by: Jinra Posted at: 2017-06-09T20:12:28.138Z Reads: 52

```
I dont know about the VESC 6 but the VESC 4 has markings on the pcb.

If you orient with the mosfets facing down the order from left to right is

GND,
HALL3
HALL2
HALL1
TEMP
5V
```

---
## \#6 Posted by: bigben Posted at: 2017-06-09T20:26:52.405Z Reads: 49

```
Thanks again @Jinra.
Something like this then. 
<img src="/uploads/db1493/original/3X/6/5/65df1f9006b334188736fedd638803ccc6fec247.JPG" width="375" height="500">
```

---
## \#7 Posted by: Jinra Posted at: 2017-06-09T20:27:44.973Z Reads: 46

```
Yep :thumbsup:
```

---
## \#8 Posted by: hexakopter Posted at: 2017-06-09T21:58:13.022Z Reads: 40

```
I hope you read the message that the labeling on the new BETA VESC 6.4 is mirrored. Please read in the five pages long PDF for the right pin assignment. 
I think it should be the same assignment like on your HW4.XX, so you dont need to swap wires, but please double check.
When you connecting it wrong you will short 3.3V/5V (what you have chosen with the switch) to ground.
```

---
