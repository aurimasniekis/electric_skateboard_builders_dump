# Switchable Dual or Single drive boards

### Replies: 23 Views: 3492

## \#1 Posted by: lowGuido Posted at: 2015-09-05T05:56:20.302Z Reads: 203

```
So I was cruising around the lake at lunch today on my single, there were a couple of little hills that I went up and felt my little single start to bog down a bit.  
Not enough to stop me, but just enough to make me think would be nice to have a bit of extra power.

But then I thought I really Do also like not having to stop and change batteries very often

so how could I have the power of a dual with the range of a single?

then it hit me (bear with me I'm just thinking out loud here) If I wired up a dual motor board with a switch on it so that I could switch between single and dual drive? I thought about it and its totally do able. i'll have to conduct some testing, but Im thinking that If you cut the PWM signal wire to one of the ESC's you could just have a switch on it to turn on the second motor. sure you will lose a little bit of power running the second ESC for no reason, but it would be negligible and It would stop the ESC from having to boot up allowing you to switch on the 2nd motor on the fly.

It obviously wouldn't be as good as a pure single, because you would have the drag of a dual and a loss on the 2nd ESC..
But It could be an interesting compromise.
just thought I'd throw it out there in case anyone has experimented with this kind of thing before.
```

---
## \#2 Posted by: torqueboards Posted at: 2015-09-05T06:48:48.631Z Reads: 202

```
I didn't notice much difference in the distance with a single vs a dual.

You wouldn't be able to switch between the two because you'd have to have one motor pull both motors. It would work if you disconnected the belt but if you don't it will cause drag which would make your motor work harder and get hot sooner.

Dual's a great investment.
```

---
## \#3 Posted by: lowGuido Posted at: 2015-09-05T06:58:10.948Z Reads: 202

```
the distance difference between single and dual for me is about 30% more from a single.

I cant really comment for sure because I haven't done it yet, but I have kick pushed an electric board several Km with belt attached and the motor just freewheels, I assume the unused motor would do the same. I'll do some real world tests in the weeks to come.
```

---
## \#4 Posted by: onloop Posted at: 2015-09-05T06:58:26.649Z Reads: 196

```
[quote="lowGuido, post:1, topic:177"]
so how could I have the power of a dual with the range of a single 
[/quote]

Firstly I would want to see some data on this, I agree that in some cases single may be more efficient. But there is also some chance that it is less effecient.

For instance... if you go up hills a lot with just a single, on average, it might actually be pulling more (or at least the same) amps then a dual drive board.

A motor keeps drawing more and more current until the load goes away or the motor goes into meltdown.

So now consider during your journey if there is rarely any load peaks because you maintain a constant speed and don't climb steep hills maybe the power consumed running two motors is not actually much more then a single motor...

I think dual motor definitely has the potential to use up more power if you are just gunning it around on the flats accelerating hard and fast... 

My gut feeling is that if you feel like you want more power just get dual drive & it probably won't use a lot more power... you can easily add more watt hours.

If you really just want to get up hills and don't want the cost/weight disadvantages of DD design a two speed gear box and the just gear down.

I have thought about it before. You could actually have an automatic transmission.  When the rpm increased high enough a clutch engages with a lower gear reduction. If rpm slows, like at the bottom of a hill the high gear reduction slips back on and you get the  extra torque.

There is only one way to find out.... test it!
```

---
## \#5 Posted by: lowGuido Posted at: 2015-09-05T07:05:03.800Z Reads: 177

```
I have built 5 boards, 
one with a 5000mah battery and single motor
another with a 5000mah battery and dual motor
(really those are the only 2 that matter for this example)
the single motor will Consistently get me 30% further on the same routes.

I like your transmission Idea. that's good.
```

---
## \#6 Posted by: onloop Posted at: 2015-09-05T08:50:03.010Z Reads: 177

```
whenever i get crazy ideas i always say to myself "keep it simple stupid" this might mean that i am not innovating with lots of new ideas but it also means i can really focus on the stuff that works really well. 

when i'm rich and have several mechanical engineers working for me with plenty of time and resources i would definitely experiment with a two stage gearing / automatic transmission for a single motor.... until then two big motors & a bigger battery do the job, they probably do it better and probably cost less...

generally speaking, if you want more power - you need to add more power. power in = power out. 

I don't think there is a way to get everything you want using tricks. Your build will become very complex & expensive with lots of extra electrickery and at the end of the day you probably just need bigger motor & bigger batteries.
```

---
## \#7 Posted by: lowGuido Posted at: 2015-09-05T08:57:56.209Z Reads: 167

```
Yeah but I have done single, Dual Diag, Dual rear, and Uneven Dual rear. I have contemplated 4X4 but not gone there yet..
I agree with K.I.S.S. But I'm bored of the norm. I want to try new things. 
I have a pile of motors and boards lying around I can play with. if I want dual motors I'll just ride a dual motor board.
although history has shown me that more often than not I choose not to ride a Dual board because I prefer my single 8000mAh board for long trips.
```

---
## \#8 Posted by: torqueboards Posted at: 2015-09-05T18:59:11.110Z Reads: 172

```
Makes sense I would say for a single on complete flat ground to get 30% more range.

For myself, I ride uphill about 30-40% of the time so my single will have to put out the same power with a single or dual.

They seem pretty much the same for me.
```

---
## \#9 Posted by: MonsterCoatings Posted at: 2016-01-12T07:24:41.464Z Reads: 196

```
Hey @chaka, (or anyone else that can answer this) I posted this question in another thread but wondering if you could answer me this? Since @Wanderer 's "The Heavyweight" is an AWD board with hub motors (I'm considering similar set up, I'm Godzilla sized) I was wondering. What is the possibility of going from AWD to 2WD or 1WD to extend ones range when lots of torque is not needed (on the flats).
```

---
## \#10 Posted by: psychotiller Posted at: 2016-01-13T03:29:57.376Z Reads: 190

```
You'll be "generating" current in all of the unpowered motors. I've had a semi bad experience coasting down hill on a dead board with the switch off. 
Maybe you could figure out how to really charge your battery with those wheels while you're conserving  power
```

---
## \#11 Posted by: lowGuido Posted at: 2016-01-13T05:33:35.606Z Reads: 184

```
you could do it by taking the signal wire off the PWM input but keeping the ESC powered on couldn't you?
that way the motors are never getting the signal to drive, but still generating small amounts of power from coasting.

(this theory is untested however I have kick pushed a dead battery board for several kms with the ESC powered on and PWM disconnected)
```

---
## \#12 Posted by: chaka Posted at: 2016-01-13T15:06:15.192Z Reads: 182

```
[quote="MonsterCoatings, post:61, topic:103, full:true"]
Hey @chaka, (or anyone else that can answer this) I posted this question in another thread but wondering if you could answer me this? Since @Wanderer 's "The Heavyweight" is an AWD board with hub motors (I'm considering similar set up, I'm Godzilla sized) I was wondering. What is the possibility of going from AWD to 2WD or 1WD to extend ones range when lots of torque is not needed (on the flats).
[/quote]

In my opinion you would run more efficiently with all motors engaged. Less energy wasted as heat.

[quote="onloop, post:62, topic:103, full:true"]
BEAST MODE... this is very cool.
[/quote]

Who would have thought we would work so well together!

@Wanderer I can sleep well now knowing it fits!
```

---
## \#13 Posted by: trbt555 Posted at: 2016-01-14T12:41:21.746Z Reads: 177

```
Interesting topic, cutting motors to conserve power.
I think the question is : on flat terrain, does the increased drag of an unpowered motor negate the energy conserved by turning it off or not ? Could certainly be tested. I think there might be a benefit.
I don't think there's an out-of-the-box solution to shut off motors but a decent hobbyist would probably be able to come up with a workable solution. If I had the time, I'd be all over this.

For example, on a 2.4Ghz GT2B TX/RX combo there are 3 channels of which only one is used for throttle. One of those spare channels could be used to manually switch off one or more motors. Remote switches that plug into your RX are available at hobby stores. You could use such a switch to interrupt the PPM signal going to the VESC's you want to turn off. Absence of an input signal would cause those VESC's to time out. If you don't have brake current associated with the time out for those VESC's, they will just coast along. But interrupting the PPM signal while on the throttle might give unexpected results. Cheap and easy to test nevertheless.

In another scenario you could have all 4 VESCs on CANbus and interrupt the bus to one or more slaves. I don't know how a slave VESC behaves when separated from it's master. Can be easily tested.

You could also connect one of those solid state anti-spark switches onto a remote switch operated by the spare channel and interrupt the power to the VESC, but I don't know how these switches handle switching under load.

Finally, for an automated solution, you could have an Arduino hooked up to an accelerometer decide you are on flat enough ground and switch motors off for you, in any of the above ways.
```

---
## \#14 Posted by: Wanderer Posted at: 2016-01-14T19:05:35.107Z Reads: 161

```
Good ideas here, but think this discussion would be suited to a new thread.
```

---
## \#15 Posted by: treenutter Posted at: 2016-01-14T22:09:36.696Z Reads: 156

```
@trbt555 I love your ingenuity! I always ride with a skate tool, and if I need to kick-push home I just take the belt off. Although I'm still pushing the weight of the electronic components, there's no resistance on the drive wheel and it feels like a normal longboard.
```

---
## \#16 Posted by: lowGuido Posted at: 2016-01-15T22:07:43.688Z Reads: 127

```
moved to existing thread. in the interest of neatness.
```

---
## \#17 Posted by: MonsterCoatings Posted at: 2016-01-20T06:41:28.059Z Reads: 127

```
Has anyone seen a device like a slipper clutch in a Moto GP bike or bicycle freewheel available for a E skateboard wheel or part of the drivetrain (only for one of the two wheels this way you can still have brakes, just not as strong as dual brakes). This would permit  single drive with brakes and when power is applied dual drive and when not needed freewheel with negligible drag.
```

---
## \#18 Posted by: lowGuido Posted at: 2016-01-20T06:55:19.630Z Reads: 131

```
nope. I have thought about these sorts of things but never seen anything fesable.
```

---
## \#19 Posted by: WrinklyWink Posted at: 2016-05-27T07:04:33.766Z Reads: 109

```
would you care to elaborate? I like regenerative braking but if there is a situation where it could backfire please let us know what happened so that we might avoid this.
```

---
## \#20 Posted by: psychotiller Posted at: 2016-05-27T10:44:31.372Z Reads: 105

```
Our motors are generators. When they spin they create electricity. If that electricity builds up, sometimes things melt. It can be wiring, fets, caps or even batteries. My point is, you can't just switch your board off and bomb a 2 mile hill.
```

---
## \#21 Posted by: Michaelinvegas Posted at: 2016-05-27T10:53:45.695Z Reads: 102

```
The power made by the motors while connected but not on could damage ur stuff .... The only way really safe is to disconnect your phase wires

So you can't turn off one motor unless you disconnect it
```

---
## \#22 Posted by: longhairedboy Posted at: 2016-05-27T18:50:54.278Z Reads: 102

```
the way i run my wire channels allows to to drop a mount, motor, and belt in the field with a hex key and skate tool. 

I have also just unplugged it and tucked the phase leads in so that they don't drag or get caught in anything. 

I have consistently seen better range on flats with a single motor when running at a reasonalbe fun speed (15-18mph), but i have not tested this yet while burying the trigger. 

There was a post here somewhere about space cell range and i did a test on a single 6355 vs a dual 6355 and i was able to go further on the same charge level with just one motor. I think it was the thread about space cell range. Anyway i got more range on one motor than two. but hills were steeper, if you know what i mean.
```

---
## \#23 Posted by: claudiofiore88 Posted at: 2016-05-27T19:09:46.586Z Reads: 90

```
What if you used the vesc to control 3 relays to physically disconnect the phase wires from one of the motors although there's still the drag problem with the second belt.
```

---
