# VESC Problem (5V Rail)

### Replies: 7 Views: 300

## \#1 Posted by: RyuX Posted at: 2018-05-25T12:17:06.360Z Reads: 85

```
Hey guys.

I replaced a broken DRV8302 after a fail of my VESC.
However even though I soldered the bottom GND PAD Properly (i put solder paste on it and reflowed everything and pressed it down firmly) I have some issues.

I changed the DRV8302 3x already to different new parts.. made sure the bottom GND is soldered.. I also replaced the STM32F405 and flashed it again with STLink.
But I still only measure 1.8V on the 5V Rail from the DRV Chip.

Anyone please have a hint ?

Also I tested the PCB with a 18V Lab Supply.. it will draw around 0.9A and when I use the 18V Supply the 5V Rail will show 7.5V - however when using the 44V LiPo it will show only 1.8V.
It's very strange.. The V_SENSE resistors and all the pins connections seem correct :(
What could be the problem ?

Thanks for the help
```

---
## \#2 Posted by: Acido Posted at: 2018-05-25T12:48:35.113Z Reads: 70

```
did you check for shorted 3 and 5v pins?
```

---
## \#3 Posted by: JohnnyMeduse Posted at: 2018-05-25T12:59:46.925Z Reads: 67

```
Make sure the tvs diode is alright (d5)
```

---
## \#4 Posted by: RyuX Posted at: 2018-05-25T15:42:40.465Z Reads: 51

```
Hey.. well actually my D5 was broken before so I just did not replace it yet.. D5 part is not assembled on my PCB - I thought this was only as a protection - not for the regulation. You think this might be my problem ?

I ordered one should arrive in a week or so..

Thanks
```

---
## \#5 Posted by: Blasto Posted at: 2018-05-25T15:52:21.964Z Reads: 46

```
D5 is a catch diode to give an alternative current path when the switch is off, if not present you will get the results you are seeing <2.5V
```

---
## \#6 Posted by: RyuX Posted at: 2018-05-25T17:32:17.021Z Reads: 35

```
Ok.. I will wait till it arrives and try again.
```

---
## \#7 Posted by: RyuX Posted at: 2018-05-29T17:20:19.693Z Reads: 13

```
So i received D5 Diode now and soldered it in.. Again with the 18V Lab Supply the 5V Rail will have 6.82V but 3.3V will show 3.25V.
Any hints how to proceed from here ? It seems the DRV8302 still produces too high voltage (even though replaced three times and the bottom bad sufficiently covered in soldering paste and pressed firmly against the board while reflowing).
Thanks for any help
```

---
