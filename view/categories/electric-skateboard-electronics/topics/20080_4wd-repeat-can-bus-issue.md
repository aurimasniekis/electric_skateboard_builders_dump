# 4wd repeat CAN bus issue

### Replies: 14 Views: 1653

## \#1 Posted by: BigBoyToys Posted at: 2017-03-31T19:27:34.017Z Reads: 148

```
Hey VESC guru's. I decided to switch my 4WD hub motor board from split servo PPM control to 4wd CAN bus control last night and lost 2 of the 4 VESC-X's I was using. I'm pretty sure the CAN tranceivers are toast. Both VESC's are lights out and the C25 CAP is getting hot. This same issue happened when I used CAN to control my TB VESC's. I thought I was over using CAN bus after the first incident but making adjustments to all 4 VESC's is so time consuming and I have a micro USB extension from the Master VESC that would allow me to adjust all 4 through the side of my enclosure had this worked. 

I've never had issues running two VESC's via CAN bus but running four seems to be problematic. Anyone else have any insight on this issue?

FYI I already triple checked my CAN bus harness there are no issues with it. I'm confident its Vesc hardware or firmware related.

Thanks
```

---
## \#2 Posted by: flatsp0t Posted at: 2017-03-31T20:12:53.901Z Reads: 141

```
Just to be sure, did you just connect RT/TX or also power?
```

---
## \#3 Posted by: BigBoyToys Posted at: 2017-03-31T20:22:35.247Z Reads: 130

```
Only the two center wires, no power was connected.
```

---
## \#4 Posted by: flatsp0t Posted at: 2017-03-31T20:32:02.872Z Reads: 122

```
Well, so that is not the reason. Seems odd that anything burned, when there is no power connected.
Seems like an odd bug.
Did you connect them as star or in series?
```

---
## \#5 Posted by: Jebe Posted at: 2017-03-31T22:44:02.349Z Reads: 109

```
feel your pain. Been through this myself. Have you emailed enertion?
```

---
## \#6 Posted by: Jebe Posted at: 2017-03-31T23:00:36.402Z Reads: 106

```
http://www.electric-skateboard.builders/t/need-help-dead-vescx-and-3-dead-vesc/18666/15
```

---
## \#7 Posted by: BigBoyToys Posted at: 2017-04-01T01:59:03.061Z Reads: 92

```
I used a length of wire and then soldered an extra piece at each end. Not sure that really qualifies as series though it's more of a parallel connection.
```

---
## \#8 Posted by: BigBoyToys Posted at: 2017-04-01T02:09:01.547Z Reads: 91

```
I have, running 4 VESC's on CAN isn't something I seen done much on the forum if at all though so I think I'm in no man's land with this setup. 

It's been suggested that the bias resistor resistance may be too low for 4 VESC's connected via can bus. I'm investigating this and will report back.
```

---
## \#9 Posted by: flatsp0t Posted at: 2017-04-01T07:15:35.624Z Reads: 92

```
I think @evoheyax has done it. But not 100%sure.
```

---
## \#10 Posted by: BigBoyToys Posted at: 2017-04-01T07:36:02.432Z Reads: 89

```
His rocket 4wd uses a servo splitter from what Ive seen.
```

---
## \#11 Posted by: evoheyax Posted at: 2017-04-01T07:53:45.117Z Reads: 85

```
I had chaka build a custom quad vesc. He has made atleast one other one from what I know. It uses canbus and splits them 4 ways. I id them 0, 1, 2 and 3. One master, 3 slaves. It works with no issues.

I use the vesc modules and iOS app system I have developed on the master, which is configured to uart + ppm. I use the 2.4 ghz trigger that torque boards made famous.

System works flawlessly. I'm just working on battery technology right now and developing a dummy proof battery system.

If you have any questions, feel free to ask.
```

---
## \#12 Posted by: BigBoyToys Posted at: 2017-04-01T08:28:10.218Z Reads: 80

```
When u say he made a quad vesc do you mean the vesc has been modified to support 4 Vescs or did he just build the harness for you?

Thanks for sharing. I'd like one of you modules!
```

---
## \#13 Posted by: flatsp0t Posted at: 2017-04-01T10:17:55.522Z Reads: 79

```
http://www.electric-skateboard.builders/t/ollinboardcos-quad-vesc-module/869
```

---
## \#14 Posted by: BigBoyToys Posted at: 2017-04-01T15:24:29.427Z Reads: 76

```
Literally a QUAD VESC how have I never seen that lol.
```

---
