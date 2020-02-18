# VESC Programming Problems

### Replies: 16 Views: 2317

## \#1 Posted by: Jack Posted at: 2016-02-07T14:58:11.009Z Reads: 98

```
Hi guys,

I finished a couple VESCs about a month ago and the first one wouldn't program but the second worked fine until the positive lipo power cable shorted out i suspect. After looking at @chaka VESC repair thread I replaced both the DRV and ST micro but I can't seam to program it or upload a bootloader now! I just get the error shown in the screenshot. 

Error: read version failed
in procedure 'transport'
** OpenOCD init Failed **

<img src="/uploads/db1493/original/2X/3/36a98ddc4ae884f481c8a4b1128b9864b3c71d83.png" width="690" height="441">

<img src="/uploads/db1493/original/2X/1/186b341e0c4501c21b32dfe0cd727b48f42756a6.JPG" width="666" height="500">

This is what i get with both boards, I've tried a different ST Link V2 programmer and its exactly the same. Would anyone be able to help me out?!

Cheers, Jack
```

---
## \#2 Posted by: chaka Posted at: 2016-02-07T15:22:07.940Z Reads: 96

```
Your pin order is a little off. Change the black wire from GND to SWIM on your stlink and you should be able to flash the VESC.

 From the photo the clk and gnd pins look like they may be shorted with a bit of solder too. Hard to tell from a photo.
```

---
## \#3 Posted by: Jack Posted at: 2016-02-07T21:30:22.277Z Reads: 90

```
@chaka Hey thanks for the tip however Ive just tried it and its no different :(

Im running Ubuntu 14.04 through parallels on a mac, would that affect anything, it strange as it worked previously with the same setup.

Cheers, Jack
```

---
## \#4 Posted by: onloop Posted at: 2016-02-07T22:14:24.487Z Reads: 88

```
I haven't read about many people using parallels. Try a VM for Ubuntu I have seen that work. Maybe @jacobbloy can shed some light.
```

---
## \#5 Posted by: jacobbloy Posted at: 2016-02-07T22:36:58.963Z Reads: 83

```
i personally use a vmware fusion but it should work the same. it would be more some thing like you haven't connected your usb device though the vm correctly as some time its set that your mac is preference.

but i don't remember ever seeing this error, if you can't get it sorted vedder has his own forum connected to vedder.se he would be the best to look at this one. http://vedder.se/forums/
```

---
## \#6 Posted by: Blasto Posted at: 2016-02-07T22:43:40.770Z Reads: 78

```
I programmed the fw and bootloader of my vesc on a mac w parallels and no problem at all. 

When i had that error message, it would usually be hw related

Verify that your wires aren't shorting through the solder mask, by the picture they seem to be lying directly on the pcb
```

---
## \#7 Posted by: Jack Posted at: 2016-02-07T22:45:34.290Z Reads: 76

```
yeah its strange because it worked for me before, I have replaced both chips on the board and the solder joints look fine. However would anything else have been damaged/things to look for on the hardware side? 

Thanks for everyones help so far! Cheers
```

---
## \#8 Posted by: chaka Posted at: 2016-02-07T23:31:45.420Z Reads: 72

```
Do you get a blue light when you connect the stlink? If not then you have a hw problem.
```

---
## \#9 Posted by: Jack Posted at: 2016-02-07T23:33:49.747Z Reads: 72

```
Yes Blue light comes on when plugging in although on the other board (which previously worked fine) it doesn't but i think thats because i soldered the LED backwards. I was in a rush, don't judge!

If the blue light is on does that mean its defiantly a software problem then?

Cheers
```

---
## \#10 Posted by: torqueboards Posted at: 2016-02-07T23:53:06.170Z Reads: 69

```
Make sure you are on USB 2.0 and not a USB 3.0 port. 3.0 seems to have issues.
```

---
## \#11 Posted by: chaka Posted at: 2016-02-08T00:06:57.178Z Reads: 71

```
Unfortunatly the answer is no, you could still have hardware issues. sometimes it is because of a microscopic bridge hardly visible with 5x magnification. Check the processor thoroughly, if you were able to flash a vesc with the same setup previously then you most likely have a hardware issue.
```

---
## \#12 Posted by: Jack Posted at: 2016-02-08T12:33:44.086Z Reads: 69

```
Haha what a nightmare! I just want to start riding again! I was getting some errors when I reinstalled Ubuntu about OpenOSD not being found, and my MacBook Pro does have USB 3.0 which might be a problem according to @torqueboards although I still can't forget about the fact that it did work before. So thats telling me its hardware as well as @chaka 

I know a few other people are having this issue but I think it may be caused by different scenarios. Hopefully ill get there soon, my new motors should be arriving this week!

Thanks for the help guys :smile:
```

---
## \#13 Posted by: trbt555 Posted at: 2016-02-09T20:20:24.927Z Reads: 62

```
@Jack, if it's any consolation, I just finished two VESCS on the PCB's I got from you and I have exactly the same problem.
I have the same ST-LINK V2 as well.

I don't understand why you're connecting pin 6, this is an unused pin:
<img src="/uploads/db1493/original/2X/1/1ddbc192956b36e91deb6501e67ac7694b5ace7b.jpg" width="199" height="199">

Should I be getting any of the LEDS on the VESC to light up when I connect the programmer ? 
(I may have a short somewhere because the programmer conks out when I connect the 3.3V pin. No LEDS.)
```

---
## \#14 Posted by: Jack Posted at: 2016-02-10T00:16:01.501Z Reads: 60

```
@trbt555

Yeah I had that issue on one of the boards I soldered. You've got a short somewhere on the 3.3v line. Test the regulator with a multimeter to be sure. 

I'm not really sure what's up because I had it working fine on my boards before. I think my hand soldering techniques could do with some work!
```

---
## \#15 Posted by: trbt555 Posted at: 2016-02-10T12:29:31.860Z Reads: 59

```
A few lessons learned: after soldering a whole bunch of ceramic capacitors it's very easy to forget that the two Tantalum capacitors have a polarity. Same thing for the LEDs.
```

---
## \#16 Posted by: chaka Posted at: 2016-02-10T14:45:28.451Z Reads: 57

```
The schottky and tvs diode are also polarized.
```

---
