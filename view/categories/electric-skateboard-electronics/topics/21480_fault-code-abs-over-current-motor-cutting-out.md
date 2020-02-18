# FAULT_CODE_ABS_OVER_CURRENT (Motor cutting out)

### Replies: 30 Views: 1621

## \#1 Posted by: kptheinventor Posted at: 2017-04-21T02:30:51.094Z Reads: 191

```
Hi there. I've been having a problem with my board when I am accelerating or braking the motor cuts off which is somewhat scary. Apparently I am getting a FAULT_CODE_ABS_OVER_CURRENT error. My setup is:
Sk3 6364
8s lipo
Vesc-x  
83mm wheels
15t/36t

Can anyone see anything wrong with my settings or setup? Or any other troubleshooting?

<img src="/uploads/db1493/original/3X/b/2/b2fcf5f8acbcff0f1e7aa59e416603bb5c442510.png" width="690" height="382"><img src="/uploads/db1493/original/3X/5/4/546409888bf5cd91e5e7af5e218108c6dc1b074e.png" width="690" height="382"><img src="/uploads/db1493/original/3X/5/e/5e32fe6b4a8564510742f281b310cbd5719c5f14.png" width="690" height="382">
```

---
## \#2 Posted by: Blasto Posted at: 2017-04-21T03:14:18.495Z Reads: 176

```
Your settings seem ok, personnaly i would put motor max 60A and batt max 30A. But that is just some tweaks.

What situation are you getting this fault?

If on the bench, no load and jamming the trigger full speed, up your motor max to 70-80A. Could also up your abs max to 150A...

If your getting this from a dead stop and jamming the trigger, maybe you should consider going dual 6355 or give yourself a kick start
```

---
## \#3 Posted by: kptheinventor Posted at: 2017-04-21T03:24:02.983Z Reads: 174

```
Various situations. Some times when accelerating both from dead start and push start. Sometimes when cruising along the brakes won't work or the accelerate will brake instead of accelerate. 

When on the bench applying full acceleration most of the times the motor stutters and continues to stutter until I take off the acceleration.
```

---
## \#4 Posted by: Blasto Posted at: 2017-04-21T03:53:30.308Z Reads: 169

```
Well, at 8S i would crank up the abs max to 150-160A...
```

---
## \#5 Posted by: Eboosted Posted at: 2017-04-21T04:06:33.299Z Reads: 167

```
Would you suggest this to a dual 6355 build as well? I'm having the same issue once in a while
```

---
## \#6 Posted by: kptheinventor Posted at: 2017-04-21T04:48:26.835Z Reads: 163

```
I tried this unfortunately it did not solve this :confused: thanks for the suggestion
```

---
## \#7 Posted by: kptheinventor Posted at: 2017-04-21T04:49:08.466Z Reads: 156

```
I'm trying to avoid switching to dual motor because of the cost :confused:
```

---
## \#8 Posted by: Eboosted Posted at: 2017-04-21T04:53:48.434Z Reads: 153

```
If you can do a single, you can do a double, just save a bit more, it is really worth it
```

---
## \#9 Posted by: kptheinventor Posted at: 2017-04-21T05:10:21.727Z Reads: 153

```
As a uni student it was hard enough to justify the original purchase, but I guess I'll have to have a think about the future of my builds
```

---
## \#10 Posted by: JohnnyMeduse Posted at: 2017-04-21T17:28:56.142Z Reads: 142

```
[quote="kptheinventor, post:3, topic:21480"]
Sometimes when cruising along the brakes won't work or the accelerate will brake instead of accelerate.
[/quote]

Sound like a bad motor or remote... what remote do you use ?
```

---
## \#11 Posted by: kptheinventor Posted at: 2017-04-21T23:20:47.253Z Reads: 138

```
Benchwheel remote. Would the remote give off an over current fault?
```

---
## \#12 Posted by: Ackmaniac Posted at: 2017-04-21T23:46:24.410Z Reads: 135

```
Did you run a motor detection or do you use the default parameters from the firmware. Be aware that you have to press the apply button after the motor detection.
```

---
## \#13 Posted by: kptheinventor Posted at: 2017-04-21T23:51:11.000Z Reads: 136

```
I ran a motor detection then changed some of the motor settings to suit my build. Yeah I press write configuration to apply the settings. Also I've had this build since mid January and it has been working fine but then 2 months ago these problems started occuring.
```

---
## \#14 Posted by: Ackmaniac Posted at: 2017-04-21T23:54:59.396Z Reads: 136

```
You have to press the apply button below the motor detection button and then hit the write button. Because the values you have there are not coming from the normal process. You either typed them in manually or used the default parameters form your firmware. Maybe that stressed the motor over time and this can be the error now. Or maybe the VESC has issues or got stressed by the motor configuration.
And the information that it worked once and now not anymore is very important. Because that proves that something broke. Sadly many people tell the important information after a lot of posts.
```

---
## \#15 Posted by: kptheinventor Posted at: 2017-04-22T00:05:40.445Z Reads: 132

```
The first vesc set up I did @Luke set everything up and I assume he did it correctly and pressed apply. When would you have to do more motor detection's? Like when you change the settings or just the first time?
```

---
## \#16 Posted by: Ackmaniac Posted at: 2017-04-22T00:09:05.655Z Reads: 129

```
Just press the buttons in this order and show a screenshot how the screen looks like afterwards.
<img src="/uploads/db1493/original/3X/c/3/c3b61b5237b6372fb9e2d7eaa22a16653eb6e336.png" width="690" height="381">
And you have to do the detection only one time. Only when you have Hall sensors and you change the order of the phase wires then you have to do it again. But that isn't the case for you.
```

---
## \#17 Posted by: kptheinventor Posted at: 2017-04-22T00:32:03.178Z Reads: 124

```
<img src="/uploads/db1493/original/3X/6/4/6450db987fd31505ed2e75ee7853b733f90436d9.png" width="690" height="382">
```

---
## \#18 Posted by: Ackmaniac Posted at: 2017-04-22T01:36:09.769Z Reads: 117

```
So the BEMF coupling was a bit off. 720 before and now 900. Maybe that can kill the motor or the VESC over time. Don't really thinks so but i also never tried wrong settings over a longer period.
Just test if you still get the errors.
```

---
## \#19 Posted by: kptheinventor Posted at: 2017-04-22T01:47:24.125Z Reads: 117

```
I still had errors after that. However I decided to change the remote rx wires that are connected to the vesc and I took it for a ride without any issues whatsoever. Which is strange as I changed them yesterday when I upgraded the aesthetics. Would these wires cause the fault in anyway?
```

---
## \#20 Posted by: JohnnyMeduse Posted at: 2017-04-22T01:53:11.840Z Reads: 116

```
[quote="kptheinventor, post:19, topic:21480"]
Would these wires cause the fault in anyway?
[/quote]

maybe... if the ppm wire is badly connect it might send wrong command to the vesc.
```

---
## \#21 Posted by: kptheinventor Posted at: 2017-04-22T02:00:24.108Z Reads: 110

```
Ahh alright fair enough. While you are here is there anything I can do to increase my braking force? (I'm on holiday and there is tons of steep hills here) I researched and I believe I'm close to the max braking I could have with my current set up.
```

---
## \#22 Posted by: JohnnyMeduse Posted at: 2017-04-22T02:04:15.898Z Reads: 107

```
you can put your batt min  (this parameter control the braking force) at -8 or -10 and if it still not enough -12
```

---
## \#23 Posted by: kptheinventor Posted at: 2017-04-22T02:08:50.902Z Reads: 107

```
On lipo 8s (2 x 4s 5000mah)? Isn't that not really that safe/ will ruin the batteries?
```

---
## \#24 Posted by: Blasto Posted at: 2017-04-22T02:12:33.484Z Reads: 107

```
Your batt is 5Ah, you can charge lipos generally at 3C, in your case 15A, so up to batt min at -15A is safe
```

---
## \#25 Posted by: kptheinventor Posted at: 2017-04-22T02:34:59.629Z Reads: 105

```
The website says the battery has a max 5c charge. Which seems high for a lipo?
 https://hobbyking.com/en_us/turnigy-5000mah-4s1p-14-8v-20c-hardcase-pack.html
```

---
## \#26 Posted by: Blasto Posted at: 2017-04-22T03:16:50.642Z Reads: 103

```
So there you go, your batt is good to -25A, or -12.5 on a dual. (-25A your wheel will just lock up)
```

---
## \#27 Posted by: Bataleon Posted at: 2017-04-23T11:29:05.502Z Reads: 97

```
Did you solve the issue? I had the exact problem which was fixed by setting my "motor max" and "batt max" to both the same value, or very close. In my case, both 40A.
```

---
## \#28 Posted by: kptheinventor Posted at: 2017-04-23T12:17:32.587Z Reads: 93

```
It was the jumper cables. They must have been fatigued or broken in the wires somewhere.
```

---
## \#29 Posted by: Bataleon Posted at: 2017-04-23T12:22:06.845Z Reads: 91

```
Ah, which jumper cables? To the receiver?
```

---
## \#30 Posted by: kptheinventor Posted at: 2017-04-23T21:38:27.916Z Reads: 89

```
Sorry yeah the ones from the vesc to the receiver (I'm no sure if that's what they are actually called haha).
```

---
