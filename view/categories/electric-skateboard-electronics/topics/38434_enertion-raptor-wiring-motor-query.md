# Enertion Raptor wiring / motor query

### Replies: 33 Views: 1875

## \#1 Posted by: Hatman30 Posted at: 2017-11-15T19:13:49.526Z Reads: 146

```
I’ve just got hold of a Raptor from a friend and am giving it some long over due maintenance. The first thing I noticed is that the vesc are not linked via can bus but have the receiver input split. 
The first pic is mine, the 2nd pic another Raptor
<img src="/uploads/db1493/original/3X/6/5/65a6a5d76d5fbc6b30a7f40893677535eec3b475.jpeg" width="666" height="500"><img src="/uploads/db1493/original/3X/a/6/a61fbc5cc4bc44dc0c4034cc26580dedb408dd20.jpeg" width="281" height="500">
Also, I noticed this.
One motor spools up first at low revs and then the 2nd one kicks in. Dya reckon this is related? Many thx 
Ps I would upload the video but it’s not letting me
```

---
## \#2 Posted by: Mikenopolis Posted at: 2017-11-15T19:24:35.366Z Reads: 138

```
videos need to be uploaded to youtube and linked here that's the only way to get videos here.

I was told that with no load, it's common to have one motor turn before the other? maybe it is a split PPM thing. I would love some more input on this phenomenon as well

In this video I have two "Raptors" that I rebuilt. The belt one on the left is canbus, the CarOn direct drive on the right is split ppm, you can see that one wheel lags behind in startup, but works perfectly fine with load.
https://www.youtube.com/watch?v=R4bzwgxUMDQ
```

---
## \#3 Posted by: longhairedboy Posted at: 2017-11-15T19:28:03.371Z Reads: 131

```
make sure both VESCs have the same settings, link the can busses, and tell them both to use it. Bob's your uncle. 

makes me want to get this busted up raptor 1 shell i have running.
```

---
## \#4 Posted by: Hatman30 Posted at: 2017-11-15T19:37:46.539Z Reads: 127

```
I would but the can bus on the 2nd vesc’s pins are bent and covered in solder for some reason?! 
<img src="/uploads/db1493/original/3X/0/a/0a3f1909e1e0335eabc247f2d3eb6bfa14a15566.jpeg" width="375" height="500">
Ps here’s a link to the vid.
https://vimeo.com/242987420
```

---
## \#5 Posted by: Skitzor Posted at: 2017-11-15T19:45:16.289Z Reads: 113

```
I would also suggest hooking up the canbus again. 2 middle contacts should be bridged...
but the remaining solder makes me suspect that there was an error in the circuit and split PPM was the only other option.
If you're familiar with soldering I would try to remove the remaining solder inside the holes with a solder pump and try with breadboard leads if the CAN is still alive. If good, solder them.

https://statics3.seeedstudio.com/images/product/new75pcs1.JPG 

In both cases, it's still recommended that the settings on Master and Slave are exactly the same.
```

---
## \#6 Posted by: Hatman30 Posted at: 2017-11-15T23:48:39.345Z Reads: 104

```
I think I’m gonna leave it split ppm for now and see if it bothers me. The solder residue and burn mark to the edge of the can bus plug has me slightly concerned and I don’t have any spare leads to hand
```

---
## \#7 Posted by: Battosaii Posted at: 2017-11-16T00:54:49.854Z Reads: 104

```
My original vescs in my Raptor used split ppm but I used canbus for my Focboxs
```

---
## \#8 Posted by: Mikenopolis Posted at: 2017-11-16T00:59:26.488Z Reads: 104

```
hmmm didn't know that Enertion did split ppm. The broken raptor I bought was canbus, Jason must've changed at some point. I rather like split just because of potential vesc issues, so far I've had two vesc fault but I was left with one working vesc and motor and didn't get stranded.
```

---
## \#9 Posted by: Skitzor Posted at: 2017-11-16T12:44:31.423Z Reads: 90

```
Even with Canbus, let's say you have a problem with your master, you just switch the PPM signal to your slave and run on one motor home.
```

---
## \#10 Posted by: longhairedboy Posted at: 2017-11-16T13:01:55.658Z Reads: 86

```
[quote="Hatman30, post:4, topic:38434"]
I would but the can bus on the 2nd vesc’s pins are bent and covered in solder for some reason?!
[/quote]

Oh good. That means you won't have to tin them. Just flux the wires and let the solder on the pins do all the work.
```

---
## \#11 Posted by: longhairedboy Posted at: 2017-11-16T13:02:49.604Z Reads: 87

```
[quote="Mikenopolis, post:8, topic:38434"]
hmmm didn't know that Enertion did split ppm.
[/quote]

they don't usually. Could be a sign something was wrong. Couldn't be major thoguh because a shorted or malfunctioning can bus usually means nothing else is working either.
```

---
## \#12 Posted by: Hatman30 Posted at: 2017-11-16T14:15:07.760Z Reads: 96

```
Just taken it for a spin, all seems ok apart from occasionally cutting out under heavy braking. I’m gonna switch over to the Nano x remote and see if that remedy’s it <img src="/uploads/db1493/original/3X/d/6/d6fa06a760262dacbfd92a6f371c11e3c8e1a2b1.jpg" width="375" height="500">
```

---
## \#13 Posted by: Hatman30 Posted at: 2017-11-16T15:01:10.821Z Reads: 93

```
Ok, sorry to hi jack my own thread but when the Nano x remote is connected and the throttle is in the neutral position - the wheels are under torque ie don’t move but are hard to move by hand(no free wheeling, like having a gear engaged) 
With the old school remote they just free wheel as normal/ like having the clutch depressed on a stick shift)
Can anyone explain please? 
Many thx
This is a vid with just the Nano X receiver plugged in.
https://vimeo.com/243137813
```

---
## \#14 Posted by: WARMAN Posted at: 2017-11-16T16:22:35.260Z Reads: 79

```
Does the Nano x remote have throttle trim? I had this problem once with my gt2b,just needed to center the trim.
```

---
## \#15 Posted by: b264 Posted at: 2017-11-16T16:34:24.455Z Reads: 81

```
[quote="Skitzor, post:9, topic:38434, full:true"]
Even with Canbus, let's say you have a problem with your master, you just switch the PPM signal to your slave and run on one motor home.
[/quote]

Taking a board apart on the side of the road is an extremely solid FAIL in my rulebook.  That's assuming I have the tools or time at that moment to do so.
```

---
## \#16 Posted by: WARMAN Posted at: 2017-11-16T16:36:11.444Z Reads: 82

```
http://www.electric-skateboard.builders/t/raptor-1-brake-locked-after-upgrading-to-nano-x/37271?u=warman
```

---
## \#17 Posted by: Skitzor Posted at: 2017-11-16T16:54:10.502Z Reads: 74

```
I do agree on your point. But have you ever been forced pushing it home for 5km (a bit over 3 miles) ?
Well, I have, zero fun in it though. Since then I have spare belts and basic tools with me to make sure one motor can carry me home.
```

---
## \#18 Posted by: Hatman30 Posted at: 2017-11-16T16:58:57.460Z Reads: 68

```
This happens even before the remote has been turned on/ paired
```

---
## \#19 Posted by: b264 Posted at: 2017-11-16T17:00:15.327Z Reads: 68

```
Dude, I'd get a Lyft before I pushed 5km home.  f dat
```

---
## \#20 Posted by: Skitzor Posted at: 2017-11-16T17:11:36.559Z Reads: 72

```
I also replied in that topic. Waiting to hear back from his Vesc settings. I simply believe, because of the new controller, he didn't change the PPM thresholds in the tool to the new ones. So he has to move his throttle a bit up to be in the middle...
```

---
## \#21 Posted by: Hatman30 Posted at: 2017-11-16T17:37:56.198Z Reads: 72

```
Plugged it into bldc, however current firmware is 2.18 and my version only reads 2.54 onwards.
Any issues with updating to 2.54 using split ppm and also does anybody have a link for the firmware if poss? 
Many thx
```

---
## \#22 Posted by: WARMAN Posted at: 2017-11-16T18:00:33.731Z Reads: 69

```
@Ackmaniac the man you wana talk to about firmware.
```

---
## \#23 Posted by: CarlCollins Posted at: 2017-11-17T05:51:09.552Z Reads: 65

```
Hi Hatman 

Have you tried using different version of BLDC tool?
Also please tell us about your Operating system.
Is your board showing limited connectivity?
```

---
## \#24 Posted by: Hatman30 Posted at: 2017-11-17T11:43:10.422Z Reads: 56

```
About to download the Enertion version now. 
I’d just like to have the option of running can bus, however it looks like the vesc that was replaced also has damage to the canbus pins 😢<img src="/uploads/db1493/original/3X/a/b/ab8cf063a55e262fa2a08e4778f6f958f31d85a3.jpg" width="375" height="500">
```

---
## \#25 Posted by: Hatman30 Posted at: 2017-11-17T12:51:16.188Z Reads: 55

```
Also, it appears that with this split ppm set up that the receiver is getting power from both vesc??
Ps tried the nano x and every time I turn off and on the board it just resets connection until I disconnect/ reconnect the receiver wire.
```

---
## \#26 Posted by: Skitzor Posted at: 2017-11-17T13:20:01.415Z Reads: 57

```
I would shoot for your PPM wiring to be done this way :slight_smile:

https://image.ibb.co/bSJYzF/image1.jpg

Then the receiver is only powered by your chosen "master" vesc.

If you have time in the next couple hours and can hook it up to your computer, I can help you out with a teamviewer session to doublecheck the settings. Up to you...
```

---
## \#27 Posted by: CarlCollins Posted at: 2017-11-17T13:35:50.696Z Reads: 51

```
I agree with Skitzor, arrange a teamviewer session with him. If it works fine, Report back.
If issue is still there, Let me help you with it :slight_smile:
```

---
## \#28 Posted by: Hatman30 Posted at: 2017-11-18T00:08:16.302Z Reads: 42

```
Disconnected the 5v and ground feed from the 2nd vesc and all seems to be working A ok. Confused as to why it was wired that way in the first place but at least that seems to have fixed it for now.
Had a go at canbus earlier but no joy .
That could be why it was changed to split ppm
```

---
## \#29 Posted by: CarlCollins Posted at: 2017-11-18T02:55:21.174Z Reads: 38

```
I'm glad that your issue is resolved. :slight_smile:
```

---
## \#30 Posted by: Skitzor Posted at: 2017-11-18T10:23:13.970Z Reads: 30

```
Good news, enjoy the board !
```

---
## \#32 Posted by: Skitzor Posted at: 2017-11-20T16:56:10.790Z Reads: 24

```
Posting an issue again and then deleting it, I'm confused...
```

---
## \#33 Posted by: Hatman30 Posted at: 2017-11-20T17:06:45.757Z Reads: 26

```
I'm now having an issue when going full throttle and the motors cutting out. I thought I'd remedied it (thus deleted post) but just took it for a spin and it keeps doing it under full load. The motors are set to 40 amp max and batt max is at 25.
```

---
## \#34 Posted by: Hatman30 Posted at: 2017-11-20T19:22:14.525Z Reads: 22

```
also discovered this, which is pretty useful
https://vimeo.com/243708857
```

---
