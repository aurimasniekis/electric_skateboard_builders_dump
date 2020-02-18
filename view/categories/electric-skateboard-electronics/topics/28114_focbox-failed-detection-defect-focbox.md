# FOCBOX, failed detection - defect focbox?

### Replies: 23 Views: 1519

## \#1 Posted by: TranxFu Posted at: 2017-07-20T15:15:12.347Z Reads: 249

```
Hey guys,

I’ve encountered a problem with my focboxe. it was running fine in FOC For the last few weeks. The last days it was running, it would detect a bit higher values for the foc motor detection. But still would run fine.

I took down the board to redo the battery pack and switch wheels. Now after connecting everything again it constantly fails motor detection. The motor is just stuttering and hardly turning. 
What I‘ve done so far:

- Reflash Firmware, motor detection in BLDC & FOC both failed. I tried the original firmware as well as akmaniacs.
- Changing phase wires, tried each combination. Failing as well.
- I don’t use the hall sensors. But I still tried Sensored and sensorless. No difference.
- I checked the motor cables for continuity and they all seem fine. 

Would this point to a defect FOCBOX? Is there anything I can check on the board/measure ?
I will make sure to upload a video later next you guys can see what I mean by stuttering.

@yummyblobs
```

---
## \#2 Posted by: Blasto Posted at: 2017-07-20T15:19:54.751Z Reads: 236

```
Do you get a error msg in the terminal after the detection?

Terminal tab, type "faults"
```

---
## \#3 Posted by: TranxFu Posted at: 2017-07-20T15:31:54.244Z Reads: 224

```
No fault codes detected :confused:  I’m pretty sure settings are all correct. I’ll show a pic of the real-time graph when I do motor detection later when I’m home.
```

---
## \#4 Posted by: psychotiller Posted at: 2017-07-20T15:35:53.560Z Reads: 214

```
Whenever you disconnect your sensor/phase wires you often have to run motor detection again.
```

---
## \#5 Posted by: Blasto Posted at: 2017-07-20T15:36:06.512Z Reads: 207

```
Ok thats a good sign, probably some parameter is throtteling the motor detection or a broken phase wire
```

---
## \#6 Posted by: TranxFu Posted at: 2017-07-20T15:40:59.183Z Reads: 202

```
I’ve done around 10-15 motor detections for now. With all possible phase wire combinations and firmware reflash and and and... can I conclude that the phase wires are fine if I get continuity on all of them ?
```

---
## \#7 Posted by: psychotiller Posted at: 2017-07-20T15:42:52.005Z Reads: 189

```
Have you tried doing motor detection without the sensor wire plugged in on bldc? Do that, if it works then do motor detection again with sensor wires plugged in. Apply. Then do FOC detection.
```

---
## \#8 Posted by: Blasto Posted at: 2017-07-20T15:46:51.146Z Reads: 191

```
[quote="TranxFu, post:6, topic:28114"]
can I conclude that the phase wires are fine if I get continuity on all of them ?
[/quote]

Well not really, if you have a bad solder on a connector, no mater what combination you'll have the same result.

What motor are you using and what is your battery?

A pic of your setup would help
```

---
## \#9 Posted by: TranxFu Posted at: 2017-07-20T16:02:54.721Z Reads: 177

```
AH Okay, I’ll resolder connectors first of all when I’m home then. The setup is a 190kv aps 6374 on a 10s4p and focbox. Photos and videos when I’m home
```

---
## \#10 Posted by: Blasto Posted at: 2017-07-20T16:07:06.589Z Reads: 173

```
Well don't necessarily need to resolder them, i'm just giving hints to where to look for a problem.

Could be worth checking your input voltage also
```

---
## \#11 Posted by: yummyblobs Posted at: 2017-07-20T16:47:11.395Z Reads: 173

```
Did you try motor detection on a different motor? Have you checked the board for burnt parts?
```

---
## \#12 Posted by: TranxFu Posted at: 2017-07-20T21:19:25.615Z Reads: 173

```
Ok guys, have made a video. You can see the failed bldc motor detection and the stuttering. Changing cables do not make a difference in the behavior. I also can't move the motor properly with the arrow keys. FOC is behaving the same way. 
**!WARNING! turn down the volume**
https://youtu.be/mzmA8O0MmJY

<img src="/uploads/db1493/original/3X/6/8/6821d664284421702bf0f4880daee0bda1d3444e.png" width="690" height="420"><img src="/uploads/db1493/original/3X/c/3/c3fc68182601a6950eb0cd388f40b149c8cc8b12.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/0/d/0deef2dc06b0e52b6e68311134890fd50012bcac.JPG" width="375" height="500">
```

---
## \#13 Posted by: JohnnyMeduse Posted at: 2017-07-20T21:23:53.307Z Reads: 154

```
Do you have any picture of the Mosfet side...
```

---
## \#14 Posted by: TranxFu Posted at: 2017-07-20T21:58:07.554Z Reads: 152

```
They look fine to me :confused:  **R2 looks weird but I just checked its just the glue**
<img src="/uploads/db1493/original/3X/4/f/4f84cfd7a4671e3be42afbe1046482af1a21930f.JPG" width="375" height="500">
```

---
## \#15 Posted by: psychotiller Posted at: 2017-07-20T22:18:04.234Z Reads: 148

```
Did you try what I suggested???
```

---
## \#16 Posted by: TranxFu Posted at: 2017-07-20T22:30:32.345Z Reads: 147

```
Yes, tried that before :) The sensor never worked for me, even before that. Still no difference though.
```

---
## \#17 Posted by: TarzanHBK Posted at: 2017-07-21T09:28:42.570Z Reads: 141

```
Someone pointed out a failed detection and rised the detection current from 6A to 8A and that worked.
```

---
## \#18 Posted by: TranxFu Posted at: 2017-07-21T09:43:53.357Z Reads: 143

```
I've read that somewhere too and tried that. Motor just stutters harder at detection :sweat_smile:...
Anyway, @Blasto has messaged me and offered me to take care of it. Apparently some of the FETs/gates are soldered on really bad. And I'll get a new unit in return ! Real class act :smile:
```

---
## \#19 Posted by: TranxFu Posted at: 2017-07-21T10:11:53.309Z Reads: 137

```
I just took a closer look at the FOCBOX and noticed that R6 is missing. Can anyone confirm that there should be a resistor there ? Its right next to the USB plug.
```

---
## \#20 Posted by: Maxid Posted at: 2017-07-21T10:22:27.933Z Reads: 134

```
Did you do the correct orientation of the sensor wires? The label on the focbox is wrong
```

---
## \#21 Posted by: TranxFu Posted at: 2017-07-21T10:24:12.533Z Reads: 130

```
Yes, I've seen that thread. Tried all kinds of orientations. Could never get it to work. Maybe the hall sensor problem is on the motor side. Is there a way I can check the sensor wires with a multimeter ?
```

---
## \#22 Posted by: cesargrimmelprez Posted at: 2018-04-19T17:48:56.564Z Reads: 53

```
Some problem, how did you fix it? Or did you get a new one?
```

---
## \#23 Posted by: onepunchboard Posted at: 2018-04-19T18:00:10.171Z Reads: 52

```
try up the D value by .01 and find the vaule until detection is sucessful
```

---
