# VESC dead? DRV8302 contact problems?

### Replies: 11 Views: 185

## \#1 Posted by: zenobios Posted at: 2019-09-12T15:26:28.370Z Reads: 55

```
Hi guys,

I was riding at the beach, everything was working fine. I then charged my batteries two days later, switched on my board but nothing happened after pushing the remote control. 

I think one of my VESCs got damaged due to salt 😥.

![20190912_171554|375x500](upload://gfJGsCjDzrnxlhJVAIhb7JOauOk.jpeg)

I can communicate with the VESC normally using the BLDC tool but as soon as I run the motor detection the motor doesn't spin and I get a bad detection result (the same motor works properly with my other VESC). 

So, any ideas (beside the obvious one of buying a new VESC 🙄)? 

Thanks 
Andreas
```

---
## \#2 Posted by: AlanZhou Posted at: 2019-09-12T16:20:28.335Z Reads: 50

```
Trying cleaning the vesc with alcohol
```

---
## \#3 Posted by: zenobios Posted at: 2019-09-14T20:47:48.613Z Reads: 39

```
Cleaned it with Isopropanol but it didn't work 🤨
```

---
## \#4 Posted by: Santino Posted at: 2019-09-15T06:15:08.178Z Reads: 36

```
Try to run again the firmware on that vesc alone, and do motor detection wi only one motor...canbus disconnected...also ask @trampa...good luck...
```

---
## \#5 Posted by: zenobios Posted at: 2019-09-15T08:36:32.816Z Reads: 32

```
Already did that, except asking @trampa.
```

---
## \#6 Posted by: trampa Posted at: 2019-09-15T16:15:21.281Z Reads: 29

```
That's a clone, VESC compatible. What model, manufacturer is that? Split PPM or CAN Bus used?
```

---
## \#7 Posted by: zenobios Posted at: 2019-09-17T08:55:57.188Z Reads: 25

```
I'm using CAN.

![20190917_105355|690x388](upload://bMnEPRqERQbvUwST03EnaQDijaH.jpeg) ![20190917_105343|690x388](upload://vjbsG43bi4ms17WsDF48FY0UEGd.jpeg)

Not sure which manufacturer it is. I attached pics, perhaps that helps.
```

---
## \#8 Posted by: trampa Posted at: 2019-09-17T09:18:27.016Z Reads: 25

```
No official release. They put Benjamin's name on and vedder.se, or didn't remove the branding from the PCB files that Benjamin Vedder published years back. It is an old 4.12 design. 

Install VESC-Tool, update the FW. Select the **FW 4.10,4.11,4.12**
Try to run motor detection., If that does not work, get a new device. 

If you use CAN BUS on a V4.12, be sure to always switch them on simultaneous (e.g. connect them to a single battery/switch). If you switch them on one after another the CAN transceiver will blow up.
```

---
## \#9 Posted by: AlanZhou Posted at: 2019-09-17T12:17:33.007Z Reads: 16

```
That's a TB vesc
```

---
## \#10 Posted by: Ben.Nexus Posted at: 2019-09-17T12:57:40.576Z Reads: 15

```
Give all your bullet connectors a tug, check for a bad solder under the shrink wrap.
```

---
## \#11 Posted by: zenobios Posted at: 2019-09-17T13:08:17.312Z Reads: 12

```
Oh yes. I'm sorry. Thought I had already written that 🙄
```

---
