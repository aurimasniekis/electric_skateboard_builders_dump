# Rewiring ESC capacitors

### Replies: 15 Views: 1769

## \#1 Posted by: jakobnator Posted at: 2016-05-20T02:19:27.661Z Reads: 133

```
I am working on a 3d printed enclosure using my FVT  ESC. From the past I have learned that this ESC must be vented so I built a little hole in the top of the enclosure, and took the fan off for airflow to cross the heat sink when riding. While the clearance looks fine I am really worried about the Caps being the farthest sticking out thing of this board. Can I desolder them and give them about 2 inches of wire so I can tuck them underneath? I remember in school learning about the importance of the proximity of large capacitors in power supplies due to the inductance of the wire or something. Is this going to be a problem?

https://dl2.pushbulletusercontent.com/aKERFCQdSovJwtrNhstaGvLIu10n85Lf/IMG_20160519_221233.jpg

https://dl2.pushbulletusercontent.com/ZAXNU1DcHd9rPGbem1fMPZRsxLB03Ws7/IMG_20160519_221306.jpg
```

---
## \#2 Posted by: paragon Posted at: 2016-05-20T02:27:35.876Z Reads: 127

```
If anything, add another cap if you are extending the wires by 2 inches.

Edit: a newer version of that esc that I have comes with 3 caps instead of 2, so adding 2 extra (for a total of 4) may be better.
```

---
## \#3 Posted by: jakobnator Posted at: 2016-05-20T02:30:28.207Z Reads: 123

```
But does the distance between the rest of the pcb to the capacitors matter?
```

---
## \#4 Posted by: paragon Posted at: 2016-05-20T02:31:00.715Z Reads: 122

```
As far as I know, it's the length of the wire that matters.
```

---
## \#5 Posted by: paragon Posted at: 2016-05-20T02:31:53.379Z Reads: 115

```
Here's some relevant info: http://www.rcgroups.com/forums/showthread.php?s=1069a01f6c4d61f2ff5e090fb71bd961&t=952523&page=1
```

---
## \#6 Posted by: jakobnator Posted at: 2016-05-20T02:32:37.732Z Reads: 115

```
Right thats what I am saying would a few inches make a difference?

EDIT: Thanks will look at that
```

---
## \#7 Posted by: paragon Posted at: 2016-05-20T02:37:14.125Z Reads: 115

```
I think you should add one more cap as a precaution.
```

---
## \#8 Posted by: jakobnator Posted at: 2016-05-20T02:39:28.306Z Reads: 118

```
So two are on top wired into the PCB, one is wired out to about an inch of lead wire. Are all of these in parallel to the power supply? Adding another sounds like a good idea after lengthening the distance from the pcb to the capacitors.
```

---
## \#9 Posted by: paragon Posted at: 2016-05-20T02:51:03.676Z Reads: 113

```
From the first post in the thread I gave you:
[quote]Solution II & rules of thumb, calculation spreadsheet
If you have to lengthen the battery wires, for whatever reason, add extra electrolytic capacitors in parallel with ESC, never in series with ESC. As a rule of thumb, for every 4inch/10cm extra length/distance between battery and ESC, add an 220uF extra capacitance near the controller (electrolytic condensators, voltage the same as the capacitors already installed, low ESR type) (Ludwich Retzbach, German e-flight author&editor, the 'R' in LRK).[/quote]
Please read up some more next time.
```

---
## \#10 Posted by: jakobnator Posted at: 2016-05-20T03:06:43.393Z Reads: 107

```
Correct I read that whole post. I am not asking about the distance from the ESC to the batteries I am talking about the distance from the ESC to the capacitors. Why would two of them be integrated into the PCB and one of them kept off a few inches, unless the other has some other purpose (not being connected for regulating voltage spikes).
```

---
## \#11 Posted by: Hummie Posted at: 2016-05-20T03:16:09.657Z Reads: 101

```
If there's wires between the caps and esc the inductance can build there.  You want the shortest distance possible.  How short and how many caps you want...depends if you're into Rc planes or electric bikes.
```

---
## \#12 Posted by: jakobnator Posted at: 2016-05-20T17:46:12.667Z Reads: 88

```
Well I am stumped, after testing my new connections before desoldering the capacitors my motor won't turn on. I get the LED saying its a sensor-less motor, however even with the motor unplugged I get the same LED pattern. 

Things I have checked/know:
Batteries are fully charged and balanced
Voltage to the ESC is 25.12 Volts
Connection from ESC to Batteries is good
Connection from ESC to motor connectors is good
All of the wires from the motor seem to have the same resistance
cooling fan is working
Receiver has solid LED indicating it is bound to the transmitter (Channel 3)
Transmitter is on
USB Link recognizes ESC and I was able to reflash firmware and it gave the OK status when done.

Motor doesn't make any beeps and is completely limp as if it weren't plugged in, ESC manual states that if the LED is on and motor doesn't power up there is an incorrect power range from the battery however they are freshly charged 6s batteries. 

Any help is appreciated

https://dl2.pushbulletusercontent.com/psJNiYb93CpMuL98i86luIk3tn1EF7wN/IMG_20160520_133805.jpg
```

---
## \#13 Posted by: Hummie Posted at: 2016-05-20T18:02:28.829Z Reads: 77

```
i dont know much electronics and i might be wrong...i heard you always want to be on channel 2.  ?  id like to know if this is correct.

spinning the motor as it is in your pic looks like it will cause a table tornado.
```

---
## \#14 Posted by: jakobnator Posted at: 2016-05-20T20:57:04.555Z Reads: 71

```
Haha yea I don't plan to activate the motor just get it to beep. I am pretty sure I tried all the channels but I might be a dumbass and not tried channel 2, however I think the motor would at least beep even if it's in the wrong channel. Will test channel 2 when I get home

Alright the problem was that the ESC is sort of two layers that are stacked together connected by header pins (Think arduino shield) When I took it apart I guess I didn't push it in all the way or something but it is indeed working now. and yes channel two is the throttle, but motor responds to controllers channel 1 as well. Now I am relocating the capacitors, will update with pictures when done for those curious
```

---
## \#15 Posted by: jakobnator Posted at: 2016-05-21T04:57:28.740Z Reads: 59

```
If you are reading this do not attempt to move 3rd capacitor from ESC, removed the board caps and everything worked fine, attempted to move the third cap and an inductor in my esc exploded totaling the ESC. :cry:

Will be saving up for VESC.......
```

---
