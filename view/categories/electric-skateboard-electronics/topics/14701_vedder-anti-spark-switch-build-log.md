# Vedder Anti-Spark Switch (BUILD LOG)

### Replies: 38 Views: 3325

## \#1 Posted by: lox897 Posted at: 2016-12-15T04:17:15.056Z Reads: 337

```
The Melbourne ESK8 group are building 6 vedder anti spark switches. I will be documenting the progress as we gather parts and start to solder the switches. Hopefully this helps other people to build their own. If you think a video would be good please tell me.

So far we have the PCBs on order from OshPark (thanks @chaka for sharing the files) and our Mouser order has arrived.
<img src="/uploads/db1493/original/3X/c/6/c6f1ad0436ead174d8fe6cd3dd3d5f0a02f72889.JPG" width="500" height="500"> 

The parts we are using are:
<img src="/uploads/db1493/original/3X/8/5/85a61968bc30a6ae1f1fe4f7c30c5b51c19e11b2.jpg" width="375" height="500">
```

---
## \#2 Posted by: sl33py Posted at: 2016-12-15T05:33:36.888Z Reads: 312

```
Nice Lox.  How are you going to solder them - hot air or reflow/toaster over or skillet?
```

---
## \#3 Posted by: lox897 Posted at: 2016-12-15T05:46:24.384Z Reads: 309

```
@sl33py I will be using a hot air station.

EDIT: What type of switch do I need to use? Thanks
```

---
## \#4 Posted by: DeathCookies Posted at: 2016-12-15T08:21:43.738Z Reads: 290

```
SPDT
SinglePoleDualThrow

if i am not mistaken
```

---
## \#5 Posted by: Maxid Posted at: 2016-12-15T09:05:47.233Z Reads: 283

```
Can also be a DPDT - the double throw is the important part. The poles don't really matter as you can always just connect the three pins that you need even if there are more.
```

---
## \#6 Posted by: lox897 Posted at: 2016-12-22T01:07:57.675Z Reads: 256

```
UPDATE: OshPark PCBs have shipped. We should be able to build these soon. I may have to drag-solder and hand solder as I am having issues with my hot air station. I'll report back how I go.
```

---
## \#7 Posted by: sl33py Posted at: 2016-12-23T06:38:57.092Z Reads: 239

```
That will work for the small components, but it'll be really tough on the FETs (if you exceed their temp when soldering you can damage them and they will fail prematurely).  The entire underside/base of the FET is a huge solder joint perforated through the PCB to flow the amps...  This is where a skillet might be best if you can't get your hot air working...
```

---
## \#8 Posted by: lox897 Posted at: 2016-12-23T06:50:34.293Z Reads: 233

```
Well, I got my hot air station working the other day, so I should be alright.
```

---
## \#9 Posted by: lox897 Posted at: 2017-01-16T01:45:13.184Z Reads: 225

```
PCBs arrived today. Bearing for size, the PCBs are smaller than I thought. And they send FREE JELLY BELLIES!!! Gotta love OshPark
<img src="/uploads/db1493/original/3X/b/9/b91a689f16f9e1a6b228e89e110352b35aeb151e.jpg" width="375" height="500">
```

---
## \#10 Posted by: lox897 Posted at: 2017-01-18T04:21:54.080Z Reads: 220

```
Anyone able to comment on the soldering? @sl33py @chaka <img src="/uploads/db1493/original/3X/0/6/06a9078bfc42c84aa031d9abe26f1b2b82778246.JPG" width="690" height="388"><img src="/uploads/db1493/original/3X/6/8/68d412f7fc504055558c0b9739f05e3755d9bae0.JPG" width="281" height="500"><img src="/uploads/db1493/original/3X/5/9/59662a8a8b13ea0718ac02a52df0b542452d477f.JPG" width="281" height="500"><img src="/uploads/db1493/original/3X/6/3/6310ef3db2e6b8597b113e2aea54ec837e6c0d96.JPG" width="690" height="388"><img src="/uploads/db1493/original/3X/f/9/f9773a647c213018cc48a87b32f98d5a6a026c1b.JPG" width="281" height="500"><img src="/uploads/db1493/original/3X/d/a/dafb24786c6abcf9113dd8014ad41d77e4ee8d98.JPG" width="281" height="500"><img src="/uploads/db1493/original/3X/c/1/c1c7ff44c6322f8b8f9fadf0c7bab8d25c127bb7.JPG" width="500" height="500">
```

---
## \#11 Posted by: lrdesigns Posted at: 2017-01-18T05:06:07.690Z Reads: 206

```
[quote="lox897, post:10, topic:14701"]
Anyone able to comment on the soldering?
[/quote]

I wont comment on the small ones but the power wires it looks like you need more heat, a bigger tip or a more powerful iron. This may work fine but its not ideal or pretty. It should looks like a smooth bubble. 

I find with these large wires they absorb a lot of heat so I will pre heat them as much as possible before bringing them into contact with the PCB for final soldering. It helps a lot. They need to be held with a tool though as they will get really hot even through the insulation.
```

---
## \#12 Posted by: lox897 Posted at: 2017-01-18T05:20:23.072Z Reads: 202

```
Thanks. I will try them again
```

---
## \#13 Posted by: NickTheDude Posted at: 2017-01-18T05:34:48.415Z Reads: 193

```
Yeah, you want to get the wire hot enough that the solder basically disappears inside it and binds all the strands together.
```

---
## \#14 Posted by: sl33py Posted at: 2017-01-19T19:25:22.247Z Reads: 189

```
@lox897 - agree with @lrdesigns on the power wires.

On the smaller components - couple suggestions (i'm by no means an expert and defer to @chaka and similar).

FETs - dry?  Did you put flux on them before flowing with air or oven?  Perhaps you just cleaned it off before pic?  It helps transfer heat and can help protect them when heating (over heating can damage them).

the small components - looks like you could use a slightly bigger dollop of solder paste, but looks good otherwise.

I usually go back afterwards and hand solder some additional solder on the legs of the fets - leaving the far left leg clear and free, but burying the rest.  

Looks good man!
```

---
## \#15 Posted by: lox897 Posted at: 2017-01-19T20:04:30.659Z Reads: 180

```
I'll be hand soldering more on the fets. I didn't use any flux at all actually, didn't have any. Should I have used it? @sl33py
```

---
## \#16 Posted by: sl33py Posted at: 2017-01-19T21:38:44.143Z Reads: 179

```
I was told it helped - especially with hot air (directional) reflow.  More heat transfer and less heat into just the FET.  

Relaying what i was told...  I know the spec sheet for the FETs has a temp threshold and timelimit - that's the concern for damage if overheated for too long.

It cannot hurt, i have it, so i use it even when reflow oven.  less needed for sure in a gradual heat up from all sides in an oven.  only a dab or two of the flux on ea FET.  cheap insurance vs a $3-5 FET.

How did you heat - hot air or reflow oven?
```

---
## \#17 Posted by: lox897 Posted at: 2017-01-19T21:46:23.071Z Reads: 166

```
Hot air. For like 10 seconds on the pins. FET was only warm afterwards. But the first one I heated for longer so I hope it hasn't died.
```

---
## \#18 Posted by: sl33py Posted at: 2017-01-19T21:51:28.923Z Reads: 178

```
i think you'll be fine.  

You just don't want to cook them too long w/ too much heat.  If you look at the spec sheet for the FET (on mouser is where i grab mine) - it'll give you the threshold temps and time.  

It's little things like preheating the PCB and gradually heating it all even w/ hot air that help, then just hit the FET itself at the end to get the base to flow (under the FET being the hard part to do w/o hot air or reflow oven).

If your hot air was set and 1 _GABILLION_ degrees :wink: - i'd worry.  If you were slow heating it all and just the FET at the end for 10 sec - you're fine.
```

---
## \#19 Posted by: OskarCastrone Posted at: 2017-01-19T21:53:46.653Z Reads: 177

```
Thank you for sharing! This looks great! I am sure this is going to help a lot of DIY'ers. 
I think a video would be very nice. I personally learn better watching a video instead of reading about it.
```

---
## \#20 Posted by: lox897 Posted at: 2017-01-19T21:57:46.014Z Reads: 173

```
Can't really do a video of the process now... but I can sum up how I did it and stuff
```

---
## \#21 Posted by: lox897 Posted at: 2017-01-19T21:58:35.266Z Reads: 150

```
I was using 275C-300C so I think I should be good
```

---
## \#22 Posted by: lox897 Posted at: 2017-01-19T21:59:30.540Z Reads: 156

```
And if I do a video I'll probably get bashed for my cringe 14 year old voice 😂
```

---
## \#23 Posted by: sl33py Posted at: 2017-01-19T22:12:00.171Z Reads: 159

```
you may be *only* 14, but you are a rockstar who's building his own Anti-spark switches!  Kudos man!!

Plenty of folks don't even try or ham fist it (i killed a couple FETs...).
```

---
## \#24 Posted by: lox897 Posted at: 2017-01-19T22:27:20.596Z Reads: 164

```
Thanks man! I'll try and shoot a video today if I have time. I'm almost finished my Bro's board so that's first priority.
```

---
## \#25 Posted by: lox897 Posted at: 2017-01-19T23:56:56.747Z Reads: 164

```
According to some pictures, the bottom switch pad is GND, middle is VCC and top is the switch one? Is this correct? @chaka @sl33py @DeathCookies
```

---
## \#26 Posted by: DeathCookies Posted at: 2017-01-20T01:31:23.305Z Reads: 164

```
http://www.electric-skateboard.builders/uploads/db1493/optimized/3X/e/5/e594848ed3834bdb62218a6d301a8aadfd2dc95a_1_624x500.jpg
```

---
## \#27 Posted by: lox897 Posted at: 2017-01-20T02:51:40.254Z Reads: 155

```
That doesn't really help me. What do they stand for?
```

---
## \#28 Posted by: CRABOLSKY Posted at: 2017-01-20T04:40:16.062Z Reads: 159

```
Great work Lox, for your sake and mine I hope these work out 😁
```

---
## \#29 Posted by: sl33py Posted at: 2017-01-20T07:10:40.679Z Reads: 162

```
a 3 position switch - as i understand it:

NO - normally open.  So if you push the switch it will turn off.  It's common state is on.
C - common?
NC - normally closed.  So if you flip the switch it will turn on.  Normal state is off.

my .02 and possibly close but not quite right...  

i think i got it right - watched this same vid a while back.  just a few minutes long and hope it helps:

https://www.youtube.com/watch?v=YN_kV2h-a04

GL!
```

---
## \#30 Posted by: Maxid Posted at: 2017-01-20T07:15:14.654Z Reads: 159

```
There is nor VCC or GND on these pads. They are for a STDP switch which has a channel that is normally closed and one that is normally open (just like @sl33py said. The backside should also have a schematic showing this.
```

---
## \#31 Posted by: lox897 Posted at: 2017-01-20T07:26:30.179Z Reads: 149

```
Nevermind, I just guessed and it worked first try 😎
```

---
## \#32 Posted by: lox897 Posted at: 2017-01-20T11:00:02.628Z Reads: 143

```
Zener Diode started smoking. It looked burnt even before I powered it on. I'll try the other ones tomorrow. Xt90 loop key for now 😐
```

---
## \#33 Posted by: Maxid Posted at: 2017-01-20T11:02:10.976Z Reads: 146

```
That is why you should not just guess and assume it worked. The labels are there for a reason...
```

---
## \#34 Posted by: chaka Posted at: 2017-01-20T15:14:43.379Z Reads: 143

```
What sleepy said, :grin:

Strange that you got a smoking diode?
```

---
## \#35 Posted by: goldenHusky Posted at: 2017-01-20T15:37:00.085Z Reads: 142

```
[quote="chaka, post:34, topic:14701"]
Strange that you got a smoking diode?
[/quote]

Yea, because even if you reversed the polarity of the Z diode, the current gets limited by the 1Mohm resistor in serial.
Very strange
```

---
## \#36 Posted by: sl33py Posted at: 2017-01-20T16:41:13.732Z Reads: 135

```
Agreed.  I would definitely make sure your other switches have the zenner setup correctly - the perpendicular/horizontal line is at the top iirc.  (just see the surrounding layer mask/ink showing the small double line = at the top).

Anything else burnt or swapping the diode fixed?
```

---
## \#37 Posted by: lox897 Posted at: 2017-01-20T17:43:42.961Z Reads: 143

```
[quote="Maxid, post:33, topic:14701, full:true"]
That is why you should not just guess and assume it worked. The labels are there for a reason...
[/quote]

Well, I'm sorry. It was working fine with my 3s battery and nothing was smoking. As soon as I did the 12s battery, boom.

I'm not 100% sure it was the diode, I unplugged it and guessed where the smoke was coming from. Don't want to plug it back in. @sl33py @chaka @goldenHusky I can provide pictures if needed. I'm probably just shit at SMD soldering and screwed something up
```

---
## \#38 Posted by: lox897 Posted at: 2017-01-20T17:44:48.462Z Reads: 141

```
Polarity was right on the Zener diodes. Diode Line on the silkscreen line
```

---
