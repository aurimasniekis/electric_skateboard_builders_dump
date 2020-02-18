# Using esk8 to sk8 kite

### Replies: 23 Views: 1183

## \#1 Posted by: ekitesurfer Posted at: 2016-07-11T15:09:21.776Z Reads: 153

```
If you are not familiar with sk8 kiting, it is basically kite surfing using a longboard. Buy a 4m ozone access and a harness of some sort, or use a rock climbing harness, some pads and you are in. Be careful because kiting is highly addictive and once you learn it on land you are going to be spending some cash on water/snow kites:)

Anyway my question is this. I don't have my esk8-yet so I am wondering:

Would it be bad to turn the board off and kite around for a while? Could it be bad to leave the board on and kite around for a while? Maybe I could rig something that only lets me hit the brakes, or I just carry a wrench and take the belt off?  How susceptible to dust are esk8s? Could I ride a satellite motor on the playa?
```

---
## \#2 Posted by: Jinra Posted at: 2016-07-11T16:01:43.413Z Reads: 139

```
Not bad at all. In fact if you leave the board on and brake while kiting you can charge your battery!
```

---
## \#3 Posted by: Michaelinvegas Posted at: 2016-07-11T16:04:09.012Z Reads: 136

```
[quote="ekitesurfer, post:1, topic:5912"]
Would it be bad to turn the board off and kite around for a while?
[/quote]

Even with the board turned off...as the motor spins it will create electricity...I'm not sure if this s good thing
```

---
## \#4 Posted by: ekitesurfer Posted at: 2016-07-11T16:22:34.530Z Reads: 126

```
Yeah, on I can see it being ok, just need to rig some device that prevents me from hitting the gas....
```

---
## \#5 Posted by: ekitesurfer Posted at: 2016-07-11T16:25:01.315Z Reads: 118

```
That's what I was wondering. I would probably never ride it like that but where does the e power go if you do?
```

---
## \#6 Posted by: Jinra Posted at: 2016-07-11T16:26:46.208Z Reads: 110

```
i don't think it'll generate electricity unless the phase wires are shorted/brakes are applied, at least not any significant amount.
```

---
## \#7 Posted by: Michaelinvegas Posted at: 2016-07-11T16:35:38.138Z Reads: 103

```
The power needs to go someplace ...

And that's back in to the ESC...and that will def blow something eventually
```

---
## \#8 Posted by: ekitesurfer Posted at: 2016-07-11T16:38:01.714Z Reads: 101

```
This is the debate I wanted to start :)
```

---
## \#9 Posted by: Michaelinvegas Posted at: 2016-07-11T16:50:02.337Z Reads: 97

```
Do you have a vesc or and esc?
```

---
## \#10 Posted by: Michaelinvegas Posted at: 2016-07-11T16:51:47.757Z Reads: 93

```
@onloop @chaka @torqueboards

You guys have any input on this subject?

Also @lowGuido @longhairedboy you guys have thoughts on this?
```

---
## \#11 Posted by: ekitesurfer Posted at: 2016-07-11T17:01:41.823Z Reads: 84

```
Have a vesc, waiting on a motor now that I decided I need pulleys for my hills
```

---
## \#12 Posted by: sl33py Posted at: 2016-07-11T17:14:52.606Z Reads: 81

```
It definitely generates electricity - spin your motor and look at your VESC.  Even with batteries disconnected you will see the LEDs on the VESC light up.  Can do this by hand easily - now imagine gear ratio and wheel force spinning it!

Without somewhere for the voltage to go, i'd be worried about damaging the VESC (or similar ESC's which regen brake).  I would either keep the batteries connected (but not fully charged - overcharge batteries possibly?), or unplug the phase wires from motor to ESC.
```

---
## \#13 Posted by: ekitesurfer Posted at: 2016-07-11T17:21:44.963Z Reads: 77

```
Lets keep this debate going. We need an electrical engineer here:p What does a motor do when it is just spinning?
```

---
## \#14 Posted by: Jinra Posted at: 2016-07-11T17:30:47.972Z Reads: 76

```
So the question now is if it generates any significant amount that would cause harm to the ESC/VESC. My guess is no, otherwise one of the main draws of hub motors (resistance-less kicking and coasting) would be made impractical to use if it's just going to blow your controller on a downhill slope.
```

---
## \#15 Posted by: sl33py Posted at: 2016-07-11T17:38:28.447Z Reads: 77

```
understood.  I will ask in Vedder's forum and see what they say.  I'm guessing there will be a threshold of voltage and amperage it can handle and dissipate (likely as heat - has to go somewhere right!?).

If i get a moment i can pull out my multimeter at home or even the watt meter (small inline) to see what sort of voltage/amps it's generating.

Good question @ekitesurfer.  I don't usually worry about it, but i do know that one of the (possibly fixed) issues with boosted was loss of brakes with full battery and trying to brake.  With nowhere to go you'd simply lose brakes - where other boards just dissipate as heat.
```

---
## \#16 Posted by: barajabali Posted at: 2016-07-11T17:44:09.126Z Reads: 72

```
I would use a 'dumb switch'  actually break the positive connection using a loop key. You won't charge your pack but you'll save your electronics
```

---
## \#17 Posted by: sl33py Posted at: 2016-07-11T17:49:48.120Z Reads: 73

```
agreed.  Doing a quick search on VEdder.se forum i saw a response from "rew" (knows his stuff that is for sure) on a similar question - basically on a bike w/o batteries connected:
[quote]the capacitor(s) will get some voltage from the motor, maybe the software can "hold out" when you stop for a few seconds. But you can't power anything.... And braking is completely out of the question: You'll charge the capacitor until either the capacitor, the fets or the DRV chip blows. Whichever comes first.... 
[/quote]

With batteries connected (and everything powered on) you'll have your wireless remote and be able to brake.  Without batteries i doubt your controller will connect, and without anywhere for the voltage to go it seems like you may blow something.

Now that i've searched for it, i'll post a quick question - both this and what happens when batteries are full?
```

---
## \#18 Posted by: lowGuido Posted at: 2016-07-11T18:38:21.341Z Reads: 70

```
in my experience you can do it, however you need to have the ESC powered on and have low charge batteries attached.

if you don't have the ESC powered up I have found that once you generate enough power to boot up it does weird things like locking a wheel up randomly
```

---
## \#19 Posted by: sismeiro Posted at: 2016-07-11T21:21:58.891Z Reads: 57

```
[quote="lowGuido, post:18, topic:5912"]
if you don't have the ESC powered up I have found that once you generate enough power to boot up it does weird things like locking a wheel up randomly
[/quote]

Hum... I was reading this thread and asking myself if this was what happened to me. The battery was almost empty and I decided to turn off the longboard and push until I arrive to the car. When I was gathering speed I heard the ESC noise and felt like the brakes were being applied.

So It seems it's better to continue and push with the longboard turned on.
```

---
## \#20 Posted by: Michaelinvegas Posted at: 2016-07-11T22:46:15.157Z Reads: 50

```
[quote="Michaelinvegas, post:7, topic:5912"]
The power needs to go someplace ...
[/quote]

And back to my original statement 👆🏻
```

---
## \#21 Posted by: Nordle Posted at: 2016-07-11T23:12:41.470Z Reads: 48

```

Did you ever mention things getting warm, thats all wasted power. And if you have a esc that supports regen you can charge your battery while braking (a bit). I would say you're totally fine if you go riding your board when it's on (just don't charge your battery totally full before you do that).
```

---
## \#22 Posted by: sl33py Posted at: 2016-07-12T17:44:18.767Z Reads: 42

```
i feel like this is a great definitive outline from rew on vedder.se:
[quote="rew"]There simply isn't hardware to "dissipate heat". So that won't happen. 

I have a 4700uF capacitor on the input. At 50V it holds: 0.5 . C . U^2 = .5 * 4.7mF * 2500V^2 = 5.8J of energy. That would be when going from 0 to 50V, it is a little less if say you go from 12V to 50V. 12V is about the minimum operating voltage for the VESC. 

Anyway, braking at 300W, would give you the ability to brake for about 20ms before the capacitor exceeds 50V. If you've set a "battery max" the VESC will stop trying to brake, but the back-EMF back-feeding into the capacitor cannot be prevented. This is a "no-op" as long as your speed is below the 50V theoretical max speed. So for example, my bike goes 1 km/h for every volt of battery voltage. So if I join the tour-de-france going down a mountain, the VESC will stop trying to brake at say the max voltage of my battery say 30V. This can happen at 20km/h. Then when I hit 30km/h the motor will feed the bus voltage without the VESC's consent. If there is no battery and just a cap it the speed will rise to 60km/h and the bus voltage will be pushed over the 60V-and-more limits of various components on the VESC. At less than 70V, the mosfets will start to conduct even when driven "OFF". Once there is a path, significant power from the mechanical system will be put into the mosfets. These mosfets are very sturdy and the manufacturer has specified how long this can go on... The taken energy can be a maximum of 0.5 to 1J ("Single pulse"). This will last you less than a milisecond at those speeds. 

So: If the battery voltage goes above max, the VESC will stop helping with braking. If your speed then goes above the theoretical speed for 60V batteries, the VESC will die without warning. 

When scaling mountains, start with a full battery at the bottom, ride the thing to the top. That guarantees "space" in the battery for the regenerated energy. Do not go faster than the theoretical speed for 60V batteries. Have a mechanical brake to dissipate energy if you want to.[/quote]

So, i read this as "don't brake fully charged" - there is almost no leeway (a few ms) and after that your brakes will stop and your VESC will fry.  And definitely don't ride w/ no batteries, or powered off.

HTH!
```

---
## \#23 Posted by: electroncuddler Posted at: 2016-08-19T06:13:27.196Z Reads: 27

```
This:
[quote="barajabali, post:16, topic:5912"]
I would use a 'dumb switch'
[/quote]

I would put a switch on the positive leg going from the esc to the motor. this will mean that the motor will generate a prety high voltage, but no current. (do not touch! more info: http://www.windynation.com/jzv/inf/open-circuit-voltage-and-short-circuit-current) Just turn the switch off when you want to ride in passive mode and back on when you want some assistance.
```

---
