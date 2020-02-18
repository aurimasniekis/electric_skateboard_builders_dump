# Board got stuck on full throttle with no brakes! What could cause this? (Related story: Slid my e-skate for the first time!)

### Replies: 29 Views: 2476

## \#1 Posted by: jmasta Posted at: 2017-06-28T04:22:02.268Z Reads: 335

```
I had just finished charging up a steep hill at over 20mph on my daily commute to campus.  Nothing out of the ordinary; I have done this probably close to 100 times.  But as I approached the crest of the hill, suddenly my board got a mind of its own and went into full turbo mode.  **100% throttle and no brakes**.  The acceleration was intense to say the least...

So there I am, speeding towards a red light with two lanes of cars waiting.  Luckily I was right by campus near a major pedestrian crossing. The walk signal was ticking down "7...6...5..."  My timing could not have been any more perfect, because it happened to be within the few seconds when traffic is stopped both ways for pedestrians.

I flew past the cars, narrowly speeding by in the bike lane.  Once in the intersection where I had more space, I threw a **heelside shutdown slide** with a dozen cars watching.  I safely killed my speed, but  my board was still stuck on full throttle.  With me on my butt, the board took off like a bat out of hell back across the intersection, hit a curb, and then ended up upside down in the grass, still raging at 100% throttle.

**_Result:_**  I turned off the e-switch, turned it back on, and it was as if nothing happened. Continued riding without issues.  I had bluetooth telemetry running through Metr, but the data is not very helpful.  All the values seem to flatline when the anomaly took place, and then the recording stopped a few seconds later

So.........
--> **What could have caused this issue?**
--> **Does this seem to be a VESC issue or an issue with the GT2B?**
--> **Any ideas on how to prevent this in the future?**


.
_**Setup**:_ (still haven't posted my build thread....)

* VESC v4.12 (2.18 firmware)
* FS-GT2B Remote (stock)
* SK3-6374 149kV @ 12S
* 18:34 gearing on 83mm wheels (27mph max weighted speed + tons of torque)

_Freshly scrubbed 75a Flywheels:_
**<img src="/uploads/db1493/original/3X/8/7/87d42bc27d49e5f15262629282ebfcc3e158b97d.JPG" width="375" height="500">**
.
.

**_Conclusion:_**

This could have been a very serious accident.  Learn how to stop... without your brakes!  This was my first time needing to slide an electric board (on super soft 75a Flywheels no less), but definitely not my first time sliding.  I have over a decade of experience downhill skateboarding, and so when things like this happen, muscle memory just kicks in.  When you've practiced something 1000s of times, you aren't overcome with fear... you just react.  I say this not to boast but to reiterate how dangerous skateboards (especially skateboards with powerful motors) can be.  

Be safe out there!
```

---
## \#2 Posted by: sl33py Posted at: 2017-06-28T04:52:21.148Z Reads: 315

```
WOW - glad you are OK!  Great read and chuckle, but glad it ended so well given the ways it could've ended poorly...

Kudos on the slide skill too - i will follow to see what it might've been.
```

---
## \#3 Posted by: Titoxd10001 Posted at: 2017-06-28T04:54:17.837Z Reads: 313

```
Do you have failsafe setup properly?
```

---
## \#4 Posted by: Namasaki Posted at: 2017-06-28T05:12:08.846Z Reads: 306

```
@Titoxd10001 Thats what I'm thinking as well, Fail Safe not engaged.
Happened to me once with the nano remote.  I tried to run my board a about 20ft without a passenger and my remote lost connection and the board took off with me running down the street after it. 
Luckily it hit a curb and flipped over.
```

---
## \#5 Posted by: wafflejock Posted at: 2017-06-28T05:14:39.357Z Reads: 305

```
Frightening have had a similar situation with a full throttle board with a mind of it's own but in my case wasn't too hard to figure out what went wrong (also it was from a stop so I got off before the board was up to speed but it still took to the streets on it's own until it met a wall).

After disassembling the electronics from my broken board and bringing them home I retouched all the solder points on my homemade receiver and it fixed the issue in the short term.  I went through after that and tested disconnecting each pin and seeing what the output was from my homemade receiver and it turns out the signals from the library I was using would report 255 in the data stream when one of the pins was disconnected between the radio and microcontroller (would think the library would show the radio as disconnected but apparently not)

I was able to fix that with code (just ignores 255 values only 1-254 are "valid" 0 or 255 can happen when things get disconnected) since fixing it I haven't had my VESC by itself ever go crazy... take it for what it's worth, one data point of no error yet on the VESCs part for me.
```

---
## \#6 Posted by: Jinra Posted at: 2017-06-28T05:21:03.731Z Reads: 284

```
Try this, turn your board and remote on and verify it works. Then turn off the remote and leave the board on, see if it either constantly accelerates or brakes.
```

---
## \#7 Posted by: Michaelinvegas Posted at: 2017-06-28T05:25:24.028Z Reads: 275

```
Wow that was exciting! Loved the play by play. Glad you're ok.
```

---
## \#8 Posted by: jbruce Posted at: 2017-06-28T05:36:36.546Z Reads: 277

```
This is why it's quite valuable to have your switch or loop key in a place you can reach it while riding. For me I could just bend down and cut power to my board if something like this begins to happen. Glad to hear you're ok though.
```

---
## \#9 Posted by: wafflejock Posted at: 2017-06-28T05:44:43.943Z Reads: 282

```
I also have that setup.... now
```

---
## \#10 Posted by: jmasta Posted at: 2017-06-28T05:51:49.133Z Reads: 283

```
[quote="Titoxd10001, post:3, topic:26314, full:true"]
Do you have failsafe setup properly?
[/quote]

Does this count as a failsafe?

<img src="/uploads/db1493/original/3X/c/8/c81477be7c2882b214f64cda019d215b44e83149.JPG" width="420" height="420">

Haha. But no, I did not program a failsafe. Would you be referring to the GT2B's failsafe or one programmed in the VESC?  I remember reading/see both but used neither.  Which method is preferred?
```

---
## \#11 Posted by: psychotiller Posted at: 2017-06-28T05:59:14.659Z Reads: 277

```
Exactly why it's mandatory to learn some longboard skills. Glad to hear you're alright. The difference of a couple of seconds and it may have been a different story.  Set up that receiver fail-safe.
```

---
## \#12 Posted by: Titoxd10001 Posted at: 2017-06-28T06:02:56.385Z Reads: 272

```
With gt2b it's simple. First you want to setup ppm tab correctly. Make sure pulsewidth values correspond to 0% 50% 100%. Most important being 50% at neutral. You can adjust this with throttle trim on remote.

When you have that setup properly all you need to do to set failsafe is press and hold a little button on the receiver that is marked and look lights should flash. To test it worked you can check in the ppm tab the green bar (check box "display") should stay at 50% when remote is turned off. You can turn on/off controller before rides to make sure failsafe is working also.
```

---
## \#13 Posted by: jbruce Posted at: 2017-06-28T06:44:20.736Z Reads: 260

```
Hah i see, live and learn
```

---
## \#14 Posted by: memesupreme Posted at: 2017-06-28T13:47:48.941Z Reads: 245

```
surely teach us how to slide 75a wheels! jk. I don't think I have a fail safe so when my remote ran out of battery I kept going, but due to lack of skill and great amount of crashing experience I went off road and flew into the bush. now I always charge my remote.
```

---
## \#15 Posted by: Mikeomania12 Posted at: 2017-06-28T15:36:11.122Z Reads: 238

```
Yes please tell us how u slide such wheels
```

---
## \#16 Posted by: jmasta Posted at: 2017-06-28T23:06:37.050Z Reads: 234

```
[quote="Mikeomania12, post:15, topic:26314, full:true"]
Yes please tell us how u slide such wheels
[/quote]

**Go fast and commit.**  Any wheel will slide at 20mph+.  _(Having a runaway electric board will solve both these problems!)_

The heelside shutdown slide is very easy to learn, since its only half of the Coleman slide (aka heelside pendulum).  [Note: There are countless Youtube videos available for this slide.  Many years ago I wrote up a very thorough "how-to" for a technical writing class; maybe i'll share it when I have time]

I recommend this slide for e-skate because it's simple, safe, and you only need one slide glove.  Wear a slide puck on your front glove and hold the remote in your rear hand.  Even if you screw up this slide, it still puts you in a very safe position to fall; it lowers your center of gravity (no impact) and you'll just end up sliding to a stop on your hands/feet if you lose your board

Flywheels slide very well once properly broken in.  81a is ideal, but 75a is very doable... it just kills your wheels faster and has a stronger hookup.  Don't attempt to slide fresh Flywheels (especially on smooth grippy pavement) without breaking them in, or they are prone to chunking.  Note that sliding your wheels inherently makes them much less grippy (which is why I only slide my e-skate during an emergency)

I recommend learning the basics on harder wheels, perhaps even on a doublekick setup.  You'd be better off using something other than your nice e-skate wheels because you are almost guaranteed to flatspot your wheels when learning (pro tip: don't lock your board at 90°. You need to keep the wheels moving throughout the slide).  Once you've got the body mechanics down, the skills are transferrable to any board
```

---
## \#17 Posted by: jmasta Posted at: 2017-06-28T23:28:54.472Z Reads: 213

```
[quote="Titoxd10001, post:12, topic:26314, full:true"]
With gt2b it's simple. First you want to setup ppm tab correctly. Make sure pulsewidth values correspond to 0% 50% 100%. Most important being 50% at neutral. You can adjust this with throttle trim on remote.

When you have that setup properly all you need to do to set failsafe is press and hold a little button on the receiver that is marked and look lights should flash. To test it worked you can check in the ppm tab the green bar (check box "display") should stay at 50% when remote is turned off. You can turn on/off controller before rides to make sure failsafe is working also.
[/quote]

Thank you for this!

Can you explain more how the GT2B failsafe works?  Does it define a set value if connection is lost (i.e., 50%=neutral)?  Or does it apply a braking current of some sort?

I never set up the failsafe because I didn't want the board to apply brakes if the remote is shutoff.  I sometimes ride with the board powered on and the remote off. I also tow my board around by the front truck (once again, while powered on to prevent blowing the VESC)

.
.
.
.


[quote="jbruce, post:8, topic:26314, full:true"]
This is why it's quite valuable to have your switch or loop key in a place you can reach it while riding. For me I could just bend down and cut power to my board if something like this begins to happen. Glad to hear you're ok though.
[/quote]
This is a good idea.  You'd want the button to be in a place where it doesn't break your stance and compromise stability.  On the heelside rail behind the front foot would be an ideal location

Though in the few seconds while stuck on "insano mode" speeding toward the red light, the last thing I thought about was turning off the board or receiver. Maybe that's just old DH habits kicking in...
```

---
## \#18 Posted by: Titoxd10001 Posted at: 2017-06-28T23:50:13.002Z Reads: 198

```
Failsafe means that when signal is lost it will return to neutral/50%.  

Turn on your board and remote. Then turn off remote to see if there is any movement. You can also check in ppm tab
```

---
## \#19 Posted by: lrdesigns Posted at: 2017-06-29T04:30:56.253Z Reads: 203

```
The fail safe will give the esc what ever signal your remote was giving when you set the fail safe. Say you press the fail safe button at 100% throttle for some crazy reason, then if you loose connection the board will go to 100% throttle.  Its recommended to set it at neutral for obvious reasons.  

-  If you make any adjustments in the PPM tab then you have to reset your fail safe or it wont be at neutral anymore.

- Another thing I have found with the GT2B if I turn on my board but not the remote after a minute or so it goes to full throttle. Not sure why. But if I turn on my remote, then turn it off again it sets the fail safe correctly and I can leave my board on and remote off without any strange throttling.  So now I always turn the remote on first before the board just to be sure. 

- Keeping the remote fully charged is also important. When the battery gets low it still works but the trims move around which can make the board act strangely. 

**A correctly set and tested fail safe is one of the most critical safety measures.** I have had the GT2B drop out going over tram tracks but due to the fail safe being neutral it just cut the power temporarily, and the connection comes back quickly on GT2B so it was all good.
```

---
## \#20 Posted by: Martinsp Posted at: 2017-06-29T07:51:50.261Z Reads: 198

```
@jmasta Im not sure if soap and gloves count :D :D
```

---
## \#21 Posted by: WARMAN Posted at: 2017-06-29T09:36:09.293Z Reads: 200

```
Had the same "full throttle" thing happen to me! Was a bad connection, the reciever to vesc cable..just replaced it.
Also as mentioned adjust your throttle trim to the correct point, iv found if you have it set at too much throttle and not enough brake even the slightest movement on throttle turns in to way too much throttle and just continues to gain speed.
There's a sweet spot your know when you've found it.
On my master cho moded gt2b it's with the arrow pointed between 12 and 1o'clock.
<img src="/uploads/db1493/original/3X/4/4/44786531c4092e9c2487e79ae78010a56378ad6c.jpg" width="281" height="500">
```

---
## \#22 Posted by: treenutter Posted at: 2017-06-29T13:50:50.503Z Reads: 189

```
[quote="jmasta, post:1, topic:26314"]
threw a heelside shutdown slide
[/quote]

@jmasta great write up and story! Makes me want to improve my slide skills. I'm not sure I would have reacted as well. I think I would have tried foot braking and then rolled off to a knee slide (I wear knee pads). 

In all my esk8 riding I've never had a signal drop or error w GT2B. I set failsafe, so I wonder if I've ever had a drop and not noticed.
```

---
## \#23 Posted by: jmasta Posted at: 2017-06-29T23:54:09.342Z Reads: 176

```
[quote="Martinsp, post:20, topic:26314, full:true"]
@jmasta Im not sure if soap and gloves count :D :D
[/quote]

Haha they may slide like soap, but that is UHMW-PE. Vintage 2009. :joy:  Lightweight, low coefficient of friction, and nearly bulletproof.  That's not even an exaggeration... NASA uses the same material for radiation shielding

[quote="treenutter, post:22, topic:26314"]
@jmasta great write up and story! Makes me want to improve my slide skills. I'm not sure I would have reacted as well. I think I would have tried foot braking and then rolled off to a knee slide (I wear knee pads). 
[/quote]

Thanks!  To be honest, at speeds above ~20mph, I am much more confident sliding.  That may be because when footbraking, I always pivot my front foot so it's parallel with the board.  The guys I know that footbrake at 50mph tend to keep their front foot in position

And now that I think about it... I don't know if I could overpower that SK3-6374 motor stuck at max throttle, with just the sole of my shoe. That motor is powerful
```

---
## \#24 Posted by: lrdesigns Posted at: 2017-07-02T05:44:26.873Z Reads: 152

```
"Loopkey acessible from topside" I liked this idea so I added one to my board. With this design I can access from both sides. <img src="/uploads/db1493/original/3X/a/e/ae3661ac05197a01de8a82f4562b66195c1f14df.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/8/2/821aaf4d97d6a83378902d6d1bb7f3ef3eb78a78.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/6/1/613a5dbc1951ec3aaad2269a25d7c6f5b72f1314.JPG" width="666" height="500">
```

---
## \#25 Posted by: do_a_kickflip Posted at: 2017-07-02T13:19:06.386Z Reads: 143

```
Great thinking. I'm going on/off switch and planned to mount it on the side of my enclosure towards the back for easy accessibility in a pinch. I think I'll add some sort of marking on my grip tape so I'll know exactly where to reach for if I ever need to.
```

---
## \#26 Posted by: Stef Posted at: 2017-07-12T18:10:03.260Z Reads: 128

```
I set up the fail safe on my gt2b to coast when connection is lost with the remote, this works fine as when I turn off the remote whilst holding the throttle, the motors stop spinning after 1 second. However, if I leave the remote off and the board on for some time (im guessing 1-2 minutes) all of a sudden the motors will start to spin again?! This almost caught me off guard one time on a dock, luckily the board was upside down (phew).

Has anyone experienced the same issue? Is there a way to fix this?
```

---
## \#27 Posted by: Mathias03 Posted at: 2017-08-27T18:03:38.832Z Reads: 101

```
tip eat a potato
```

---
## \#28 Posted by: Clonkex Posted at: 2017-08-28T04:48:18.271Z Reads: 98

```
Daaang, that's some scary stuff! That's why I intend to be very careful with the failsafe code on my custom Arduino-based receiver. I want it to cut to neutral throttle if anything at all disconnects. After reading this thread I realise it'll be a good idea to also have a manual safety switch or loopkey (that physically disconnects the battery) on the side of the board as a backup to the software failsafe. I'm no stranger to speed (I rollerblade at some pretty high speeds sometimes and thoroughly enjoy it) but I see no reason to make that speed any more dangerous than it already is. I'm happy to go flying through a rough gravel patch or bounce off a speed bump at high speed on my blades but if I can't see if a car is about to appear from around a corner there's no way in hell I'm going down that hill.

But I guess most people would have a similar opinion.
```

---
## \#29 Posted by: Pafrican Posted at: 2017-09-08T17:49:53.589Z Reads: 73

```
Very similar thing happened to me with an identical set-up:

VESC v4.12 (2.18 firmware)
FS-GT2B Remote (stock)
SK3-6374 149kV @ 12S
14:27 gearing on 69mm wheels

I inevitably rode over a metal plate that was spanning across a bridge. The impact (similar to riding over a larger crack in the ground) caused my board to stop responding to my transmitter. I turned it off then back on; board was riding fine again. I approached a second bridge with another metal plate spanning across it. This time I rode over it at a lower speed to minimize the impact. The board reacted the opposite way... it went full throttle and wouldn't stop.

I did have the timeout feature on my VESC set to 1 second, but that didn't seem to kick in. I was unaware of a "fail safe" feature on the GT2B. Good to know!

People on this site have been telling me that the cable between the VESC and receiver got loose which caused my board to go rogue. 

Glad to know you're okay!
```

---
