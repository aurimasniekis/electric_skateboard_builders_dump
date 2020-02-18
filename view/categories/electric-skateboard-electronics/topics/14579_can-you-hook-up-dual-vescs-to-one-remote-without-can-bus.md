# Can you hook up dual VESCs to one remote without can bus?

### Replies: 42 Views: 2351

## \#1 Posted by: Skateman Posted at: 2016-12-13T01:39:14.791Z Reads: 182

```
Anyone know how to hook up 2 VESCs to one remote without using the can bus cable. My VESCs are separated from each other. Appreciate the help.
```

---
## \#2 Posted by: caustin Posted at: 2016-12-13T01:52:57.312Z Reads: 184

```
Servo ppm y-splitter is one way. Another way is some remotes have dual signal so second channel is dup signal  I think benchwheel is one like that?
```

---
## \#3 Posted by: Skateman Posted at: 2016-12-13T02:12:44.516Z Reads: 182

```
I'm not familiar with ppm y-splitter. How does it work?
```

---
## \#4 Posted by: caustin Posted at: 2016-12-13T02:32:00.719Z Reads: 175

```
How are your VESCs physically separated as that probably bounds the solution better. If truly isolated, no wires can span, then may need 2 receivers.
```

---
## \#5 Posted by: Skateman Posted at: 2016-12-13T02:43:00.365Z Reads: 162

```
@Caustin Well, it's more like two transmitters. O, like you said a Benchwheel. My VESCs are being used for roller skates, so hence the separation. On my skateboard I can use can bus. Only thing I don't have is the procedure to bind transmitters and receivers for the Benchwheel remote. I looked everywhere and haven't found it yet. That's what I need. Because, like you say, the Benchwheel has two channels.
```

---
## \#6 Posted by: saul Posted at: 2016-12-13T02:46:20.077Z Reads: 161

```
OH I haven't seen anyone trying eblades in a while! They are blades right? lol

I don't think a regular rc remote with work with 2 rx at the same time.
You could do one remote for each foot?
```

---
## \#7 Posted by: Skateman Posted at: 2016-12-13T02:55:42.370Z Reads: 150

```
Actually they're quad roller skates, lol  Yes, two remotes will probably be the answer. It seems like I read that the VESCs could do that but, may be complicated. Don't know. For what it's worth, here's the "skate" lol

<img src="/uploads/db1493/original/3X/a/3/a316a89c7f80aac899499f7ff804553ce781999f.JPG" width="666" height="500">
```

---
## \#8 Posted by: saul Posted at: 2016-12-13T03:01:01.709Z Reads: 143

```
There could be ways of doing it with one remote but i think separate systems would be much simpler! 
Looks cool! I see carbon fiber baseplate, Snowboard bindings and sharkwheels! Wheres the motor?
```

---
## \#9 Posted by: Skateman Posted at: 2016-12-13T03:06:20.659Z Reads: 145

```
Oh, it's on the other side. It's a Hummie Steel Hub motor. Works great!  Got it running on FOC and it's as smooth as ever.


<img src="/uploads/db1493/original/3X/c/e/ced2c8f2b9570f131704ca9a7d95e881f23a35f6.JPG" width="666" height="500">
```

---
## \#10 Posted by: caustin Posted at: 2016-12-13T03:12:03.005Z Reads: 140

```
Haha, wow that clarifies things...and looks awesome!  Let's see how others chime in, would be much better if did not need 2 remote tx and 2 rx. The benchwheel can easily use the second channel for dup signal but to same single binded rx. Perhaps one of the forum vesc or binding wizards can enlighten us.
```

---
## \#11 Posted by: Skateman Posted at: 2016-12-13T03:19:21.634Z Reads: 137

```
Thanks much! @Caustin. I have two Benchwheel remotes and two rxs, so if someone does know how to bind to the two rxs, to one remote, that be good.
```

---
## \#12 Posted by: caustin Posted at: 2016-12-13T03:46:46.567Z Reads: 138

```
Yeah, having seen the benchwheel documentation it will not answer your question!!
```

---
## \#13 Posted by: Skateman Posted at: 2016-12-13T04:00:59.148Z Reads: 137

```
All I have is this paper that came with the remote and tx. My buddy translated it from Chinese. It's only about the rx. One cool thing though, is the blank box next to 5V on the right doesn't go anywhere, so I connected the LEFT 5V on the back of the board to that pin and was able to plug my fan in and it worked! What luck! lol


<img src="/uploads/db1493/original/3X/9/2/92c35c0538073be0678cc30729c75f13281fbe2e.JPG" width="375" height="500">
```

---
## \#14 Posted by: caustin Posted at: 2016-12-13T04:06:20.998Z Reads: 126

```
Haha, nice luck on the phantom 5V lol 

Rest of docs are even less enlightening 

https://www.electro-sport.de/WebRoot/Store7/Shops/78292882/570F/A27D/164A/565D/F41B/C0A8/2ABA/B24F/Benchwheel.pdf
```

---
## \#15 Posted by: Skateman Posted at: 2016-12-13T04:19:14.050Z Reads: 128

```
Yea, great manual but lacks the binding. Guess your not suppose to do that
```

---
## \#16 Posted by: Skateman Posted at: 2016-12-13T04:33:21.780Z Reads: 126

```
@Saul. Thanks for the info.
```

---
## \#17 Posted by: Aggdaddy Posted at: 2016-12-13T05:25:58.847Z Reads: 127

```
Is this a DIY project?  I see the battery on the back of the skate and I am wondering why not make a back pack out of it?  Put the battery, receiver and vescs using a servo Y splitter (cut the 5v lead from one of the servo leads to the vescs) in a back pack and run the motor cables to the motors in the shoes.  Some wire loom would be necessary for this as well.

I am just wondering if the length of the cable would have any effect on the power.  But your shoes would be a lot lighter.
```

---
## \#18 Posted by: Skateman Posted at: 2016-12-13T12:56:55.511Z Reads: 128

```
Yea, its a DIY. These skates evolved over time. Took me about a year. Mainly waiting on parts and Machinist. I did try having all the parts you said, but on a waist belt. It actually worked pretty good. They were definitely lighter. It's an idea I may go back to. The extra weight doesn't seem to effect riding them too much. They're somewhat difficult to ride at first. Helps to be a good quad roller skater already,  (I'm doing better).  I have a pair of practice skates. Just gotta ride both of them regularly. Gonna post a video when I can.

If someone could tell me how the Y-splitter works, sure would appreciate it. The length didn't seem to bother my other pair, but they were made from a production made skateboard I bought and cut up. Just wonder how that would work with the VESCs?


<img src="/uploads/db1493/original/3X/0/5/050c1d5231e60f28fb7f2d0137c730ed9c384449.JPG" width="666" height="500">
```

---
## \#19 Posted by: Ackmaniac Posted at: 2016-12-13T19:01:01.930Z Reads: 105

```
With a lot of programming and testing it would be possible to connect them via UART and Bluetooth or WIFI modules. WIFI with UDP would be better because it is the fastest. But then the VESC needs to send the signal via UART and not via CAN. So it would be tricky but possible.
```

---
## \#20 Posted by: Aggdaddy Posted at: 2016-12-13T22:05:43.297Z Reads: 98

```
The y-splitter goes into your throttle channel on the receiver, then each end of the cable goes into the vesc.  Just make sure to cut the +5 volt (middle wire) of one of the vesc's receiver cable.

The receiver only needs power from one vesc.  I had problems with my build and this is one of the details I discovered, running dual vescs.

I always liked the idea of roller skates or wheels on my feet, but I really suck at it.  I have blades that I bought years ago and rode maybe two or three times.   They haven't been on my feet since.

But with that little experience and the power of these motors, how do you keep your feet on the ground?  Do you have to put your feet in a line before acceleration?
```

---
## \#21 Posted by: Skateman Posted at: 2016-12-14T01:11:52.258Z Reads: 88

```
@Ackmaniac, that's really good info. I'm just now using VESC for the first time. A lot of help came from here. I did set it up on BLDC first,  then went to FOC and it worked well. My buddy told me about current control so I would have reverse and that worked pretty good too. I would like to try your methods, so I'll start reading up on what you said. It does need to be wireless cause of the two separate skates.

@Aggdaddy I haven't skated in 13 years and I lost it all. I actually could skate backward back then. I'm doing better now but it's coming slow. Sure don't remember it being this hard to skate again. 13 years and my age have a lot to do with it. lol  Right now I'm only skating with one skate as the other is under construction and near completion. I need a drone battery and finish the wiring. Then figure out the dual VESC control. Skating the electric skate is actually easier than my practice skates right now. Haven't done to much yet, but I did ride them. I did keep the skates side by side and just kinda stand there. Surprising, it was easier than I expected. All of the torque has to go through one leg and it starts hurting quick. Could get use to that though. Two would be better. It' been a long time coming and I'm really happy with things so far.
```

---
## \#22 Posted by: Aggdaddy Posted at: 2016-12-14T02:41:59.180Z Reads: 78

```
Post the video when you complete it.  Seems like you are close to completing the project.
```

---
## \#23 Posted by: Skateman Posted at: 2016-12-14T02:48:04.622Z Reads: 75

```
I sure @Aggdaddy. Also maybe catch up with as I live in Santa Fe, Tx., 25 mi. south of Houston.
```

---
## \#24 Posted by: oripaamoni Posted at: 2016-12-14T02:58:30.715Z Reads: 73

```
also if the GT2b is like all the other FRSKY systems I have for my drones you can bind multiple receivers to one tx. I have about 14 on my taranis on one model and if 2 receivers are on at the same time they both just mirror each other.
```

---
## \#25 Posted by: Skateman Posted at: 2016-12-14T03:14:06.794Z Reads: 71

```
A mini trigger would be GT2B? I also have a micro remote. Would that work too?
```

---
## \#26 Posted by: Aggdaddy Posted at: 2016-12-14T04:42:32.446Z Reads: 67

```
I have never tried multiple receivers, but if you don't have another receiver that is similar, wouldn't the servo Y-splitter solution be cheaper and achieve the same goal?
```

---
## \#27 Posted by: Skateman Posted at: 2016-12-14T04:46:23.915Z Reads: 74

```
Not sure how that set up looks but with two separate skates I'm not sure. Can you explain the configuration to me?
```

---
## \#28 Posted by: caustin Posted at: 2016-12-14T05:06:45.159Z Reads: 79

```
I imagine the only way the servo y-splitter method works is to run a long 2-wire servo extension cable (leave out red power wire) up one leg then back down the other, lol. That would at least work rock solid if you wanted to test it out, just not the most graceful solution (and you could do that with a canbus extension wire as well) !
```

---
## \#29 Posted by: Aggdaddy Posted at: 2016-12-14T05:11:44.356Z Reads: 85

```
<img src="/uploads/db1493/original/3X/1/7/1717f5e7b4ba21ea2d8a72698912712d830e0bc8.jpg" width="302" height="500">

That is best I can do with pencil and paper.  That is what I would think would be a nice set up for powered skates.   It would all be in the back pack. The motor wires would go all the way to the feet and needs to be secured with wire loom from the back pack to the skates.   Probably be best to use bullet connectors near the feet when getting ready to skate.  Then unplug when your are removing the backpack.
```

---
## \#30 Posted by: Skateman Posted at: 2016-12-14T05:14:14.068Z Reads: 77

```
That would surely work. And yea, can bus at that. For testing, why not. That's probably what I'll do.  I like to figure out Ackmaniac' s wireless proposal, but that's over my head on VESCs right now.
```

---
## \#31 Posted by: Skateman Posted at: 2016-12-14T05:18:41.418Z Reads: 73

```
@Aggdaddy I like that idea too. How would long motor wires effect things?
```

---
## \#32 Posted by: SeanHacker Posted at: 2016-12-14T05:19:17.603Z Reads: 68

```
@Ackmaniac Has the best ideas. He know's what he's talking about too.
```

---
## \#33 Posted by: Skateman Posted at: 2016-12-14T05:21:59.205Z Reads: 66

```
Maybe he'll work on it for me and I'll "hook him up" lol
```

---
## \#34 Posted by: Skateman Posted at: 2016-12-14T05:24:29.607Z Reads: 65

```
I did try a waist belt and it worked. Similar to Aggdaddy. But not with VESCs.
```

---
## \#35 Posted by: caustin Posted at: 2016-12-14T05:26:05.373Z Reads: 61

```
I also like @Aggdaddy method.  Forum (VESC) experience has been length in battery cables no good, motor phase cables ok. That said I have not seen 3foot phase cables tried so would out that out there as a question to the wiring wizards here lol.
```

---
## \#36 Posted by: Skateman Posted at: 2016-12-14T05:30:06.282Z Reads: 63

```
That sounds good. Anybody got any input on long motor phase cables. Larger cables or/and finer strands maybe?
```

---
## \#37 Posted by: caustin Posted at: 2016-12-14T05:34:32.479Z Reads: 63

```
Haha, put that in a new thread with title 3 foot motor phase cable issues and you will get some responses faster lol
```

---
## \#38 Posted by: Skateman Posted at: 2016-12-14T05:35:45.692Z Reads: 64

```
Oh yea that's right. You can tell I'm new here. lol
```

---
## \#39 Posted by: Aggdaddy Posted at: 2016-12-14T05:41:07.106Z Reads: 66

```
My motor cables are about two to three feet on my mountainboard, going from the box in the center of the board to the back.  I would say they are 12 to 10 gauge in size.   I didn't build it, but I did a lot of mods to the electronics.
```

---
## \#40 Posted by: Skateman Posted at: 2016-12-14T05:43:08.080Z Reads: 65

```
If that works fine then that's probably long enough and will work.
```

---
## \#41 Posted by: caustin Posted at: 2016-12-14T05:53:15.958Z Reads: 66

```
https://www.rcgroups.com/forums/showthread.php?952523-too-long-battery-wires-will-kill-ESC-over-time-precautions-solutions-workarounds
```

---
## \#42 Posted by: Skateman Posted at: 2016-12-15T03:53:29.194Z Reads: 59

```
Thanks @Cuastin! That's some really informative info on long motor and battery wires. If I decide to go that route, I should be able to make up cables with capacitors that will do the job.
```

---
