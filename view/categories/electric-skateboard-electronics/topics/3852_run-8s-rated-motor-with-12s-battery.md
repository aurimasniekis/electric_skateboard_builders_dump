# Run 8s rated motor with 12s battery

### Replies: 28 Views: 2987

## \#1 Posted by: tor Posted at: 2016-05-26T08:15:28.656Z Reads: 185

```
I bought a motor from Alienpowersystems.com, the motor is rated to 8s (30v) and 2200w max.

I want to run the motor with 12s (45v) for better efficiency and lower temps. Will the motor run fine if I use 12s and limit the current draw in the vesc to 45A so the maximum output doesn't exceed 2200w?
2200w/45v=48A

I cannot see why it shouldn't be possible because higher voltage equals to less current, and that equals to thinner wires since the heat generation gets lower.﻿
```

---
## \#2 Posted by: Michaelinvegas Posted at: 2016-05-26T08:20:47.770Z Reads: 187

```
May not be wise to over volt the motor...have you asked Alien?
```

---
## \#3 Posted by: Haimindo Posted at: 2016-05-26T08:25:48.505Z Reads: 181

```
Yeah I would recommend asking Bruno (APS-guy) by email
```

---
## \#4 Posted by: tor Posted at: 2016-05-26T08:35:07.258Z Reads: 173

```
Yhea, this is the reply I got: "They are 8s max rated. i know people use them on 10s, but honestly i can not say to use on 12s. you can try but it is on your own risk."

What is it that determines the max voltatage? My perception is that the manufacturer sets a maximun voltage to prevent user to draw more than the maximum output from the motor, in this case 2200w. With a VESC I'm able to strangle the current and the output won't exceed 2200w.
```

---
## \#5 Posted by: Michaelinvegas Posted at: 2016-05-26T08:43:38.861Z Reads: 165

```
Not sure what factors limit voltage but I would assume putting up to 12s would put a huge strain on its wiring ...it's a big jump from 8s...10s I can see ....but 12s is gonna fry something
```

---
## \#6 Posted by: tor Posted at: 2016-05-26T08:50:58.431Z Reads: 159

```
Hmm alright, thanks for your response. I haven't got any theoretical answer to this question why it's not possible so I'll stick with my theory and try it. I will post my results here, in the future!
```

---
## \#7 Posted by: Michaelinvegas Posted at: 2016-05-26T09:03:10.302Z Reads: 150

```
Lol yeah it's late ... Someone my see this an chime in...

Any thoughts @Hummie?
```

---
## \#8 Posted by: Michaelinvegas Posted at: 2016-05-26T10:37:45.403Z Reads: 144

```
http://www.rcgroups.com/forums/showthread.php?t=1329612
```

---
## \#9 Posted by: tor Posted at: 2016-05-26T11:01:49.138Z Reads: 139

```
Thank you! 

"More Watts means more heat in the windings too lf course and the final determinant is that you have to limit either the current or duration to avoid overheating."

"Conventional wisdom suggests that high voltage, low amps should be marginally better than the reverse....waste heat comes from I^R"

"If you increase voltage and decrease the current (given power) generally you could be closer to peakeff running. (but there is an optimum couple)"

Nothing says it shouldn't be possible.
```

---
## \#10 Posted by: longhairedboy Posted at: 2016-05-26T11:57:33.571Z Reads: 129

```
I say burn up the motor for science.
```

---
## \#11 Posted by: tor Posted at: 2016-05-26T12:04:25.880Z Reads: 128

```
Haha.. But I think(and hopes) that the motor won't burn up! :joy:
```

---
## \#12 Posted by: lowGuido Posted at: 2016-05-26T12:49:57.992Z Reads: 123

```
be careful about this "high voltage equals low current" thing because it is not that simple. if you just up the voltage it will draw more current!
the high voltage low current "rule" if you can call it that, only applies if you also change the motor to a lower kv motor.
```

---
## \#13 Posted by: tor Posted at: 2016-05-26T13:03:03.746Z Reads: 116

```
As I said, one of the ingrediens is to make this work is to **limit the current draw in the vesc to 45A**. The motor will actually draw less current for the same wattage. It can be calculated with this formula: P=UxI. 

But you are right, if the current wasn't possible to limit, the wattage would exceed 2200w and the motor would burn.
```

---
## \#14 Posted by: Hummie Posted at: 2016-05-26T14:13:38.602Z Reads: 111

```
I read that the real motor max voltage is related to both the winding enamel and the bearing max rpm.   The enamel likely can do much can more.  The high kv of a little motor will mean high rpm so the bearings are a limit.  Really the max voltage is more so there to limit the amps which are much more available with the high voltage.  With the amp limit you should be fine.  Maybe see what rpm the bearings can spin
```

---
## \#15 Posted by: Michaelinvegas Posted at: 2016-05-27T05:37:44.858Z Reads: 98

```
I'm thinking that there may be some physical constraints that will keep it from running 12s at an extended period of time...and as you mentioned, bearings may not hold up to higher rpm...

Will be interesting to see what can be concluded from testing an 8s motor at 12s.
```

---
## \#16 Posted by: Namasaki Posted at: 2016-05-27T06:00:40.767Z Reads: 94

```
I agree with LHB, Just do it for Science, then let us know what happened.
```

---
## \#17 Posted by: longhairedboy Posted at: 2016-05-27T17:23:09.093Z Reads: 87

```
Trial and Error is the purest form of Science!

Hail Skatan, may his bearings deliver us from eternal road rashiness.
```

---
## \#18 Posted by: tor Posted at: 2016-05-27T18:08:31.350Z Reads: 84

```
So I have read quite a bit in the subject. **What's creating the magnetic field is the current, not the voltage.** Of course, the voltage must be there becuase 0v =0A. The higher the voltage is the higher the current gets. It can be calculated with Ohms Law U=IxR.

As mentioned before; If the motor has higher voltage it needs lower current for the same wattage. **But if the current is lower, the magnetic field must be lower becuase the current is lower, right?** And if the magnetic field is weaker the motor will have less torque but it will be possible to reach higher RPM:s. That's why high voltage motors has lower kv, the high voltage doesn't create much torque as the ones running on lower current, so they need to have lower RPM per volt to compensate.

This is just a theory by me, but I think it seems legit. **I could run the motor with 12s but it would weaker (slower acceleration) but the top speed would be higher.** Some of you mentions that the bearing will not hold up at higher RPM:s, and you are surely right. But it's not hard to replace bearings on brushless motors if it breaks.

@longhairedboy @Namasaki @Michaelinvegas @Hummie @lowGuido @Haimindo
```

---
## \#19 Posted by: Hummie Posted at: 2016-05-27T18:20:19.457Z Reads: 77

```
I've been endlessly trying to get to the bottom of voltsge in a motor as well

Given the same motor with the same winding it makes sense that it would have less torque running more volts because wattage is amps and volts multiplied and amps make inductance.  But I've heard it different ways and on here, forget his name but he's just a half a head avatar, he wrote some formula which I forget explaining a decrease in temp with voltage in the motor.   I'm still questioning if amps alone create inductance or if an amp is not simply and amp and if it's pushed with voltage it's different
```

---
## \#20 Posted by: Michaelinvegas Posted at: 2016-05-27T18:23:21.034Z Reads: 81

```
@tor totally get what your saying...bearings are an obvious choice for failure point because of the higher rpm, and yes you can replace them with high spec bearings...but that's just one point of possible failure of course ... Windings...epoxy not being able to take the heat and increase speed...Gees what else is in a motor? 
IMO anything that gets hot on 8s will get hotter on 12s weather is electrical resistance or physical resistance...which will shorten the lifespan of the motor...so will agree that it will work...but not as long as it would at 8s

We just don't want you to squeeze the "magic smoke" (like @longhairedboy likes to call it) out of a perfectly good motor 😉
```

---
## \#21 Posted by: longhairedboy Posted at: 2016-05-27T18:34:22.256Z Reads: 72

```
you really can't let the magic smoke out. i mean its fucking impossible to get it back in there, i've tried everything, including multi-phasic polarized electron traps, magnetically contained plasma inductors, and even tried bypassing the primary power conduits on the heisenberg compensators to create a phase warp bubble that would slow down time and thus prevent the smoke from moving out while i found a solution, but nothing. The only thing you can do is fully reverse the time stream and travel to the point before it was released and kill your other self before you can burn up the motor and ruin your day.
```

---
## \#22 Posted by: tor Posted at: 2016-05-27T19:30:29.135Z Reads: 70

```
Hahaah... @longhairedboy

I think I'll stick with 8s, maybe in the future I'll try this. Acceleration on my board now is insane and top speed is around 20 mph(30km/h) and that speed is enough.

@Hummie @Michaelinvegas
```

---
## \#23 Posted by: Hummie Posted at: 2016-05-27T19:59:07.489Z Reads: 70

```
From researching again I still don't know who to believe about overall results but it does seem an amp is an amp and it alone is the source of inductance and the electromagnetic side of the motor.  With more voltsge u can simply push more through quicker and you'll have a higher top speed.  For motor efficiency I've read anything from running at half to 80 percent of max no-load rpm as defined by volts times kv is most efficient.  On a board the rpm is all over the place and I keep it simple and turn up the voltsge as high as possible and watch the max motor temp.  
I bet ur motor would be fine on 12s if u reterminated it to a wye wind to further lower the kv but otherwise I think the bearings might go too fast (think they'd get hot).  Other than the bearings the enamel is very likely is the same as on their 12s motor and ...there's nothing else in there.  There is the risk with the high voltsge blasting the motor into magnetic saturation quicker, like on a super steep hill, and the motor more quickly will throw amps at the windings and then...the smoke.  But as long as u keep aware and check temps on the steepest things I think you're safe.  Me for example, I'm running two 54mm motors (rare size) and 90kv and am always looking for the most voltsge I can get as it just means more speed to me
```

---
## \#24 Posted by: brentsinger Posted at: 2017-03-05T02:25:55.184Z Reads: 52

```
Hi, sorry to weigh in late but I think I can help if you are still intersted in solving the question. I'm an EE and a student of motor drive, disclaimer I don't do motor drive for living and could be wrong, i'm not offering advice, just providing you help to make your own decision.

Please correct me if I'm wrong. Caution: rambling answer with little proofing. 

So voltage is good but possibly not for the reasons you've stated. Yes, lower current is needed for same power and this is mostly a relief to the battery system and power input, less heating of wires, connectors which really does matter at higher power levels. High current wires and connectors are HUGE to be low ESR (resistance), resistance being death to current. High voltage gives smaller and cheaper soln there. At the motor not it's not so easy.

What makes a motor turn is current through the winding. This makes a magnetic field, simple enough. Each of the three phases is a just big inductor, a coil of wire where magnetic fields are built and super-impose. Pump in more current, get more field. The more voltage you have, the FASTER the field builds up and the BIGGER the current gets, MORE POWER more fun more torque. Also the max current can be higher, voltage being the driver of current. 

A net effect is that for the same power output, higher voltage gives you a lower duty cycle. But the same peak currents in the motor are still required; they are built up faster though, and there's less 'sag' when the load is driven because more voltage, more potential, more grunt. Paracitic resistance in the system is overcome because average current is lower and there's more voltage to work with anyhow, so the drop on parasitics is lower % of total. Remember that the drive is cut up into portions of on and off, very binary as you'd expect. So for the period that motor is on, the faster current growth is a bit more stressful on the gear. This is compensated by the off time when there is no stress, kind of makes it ok. One issue is that you may throw a magnet, literally pulled off the wall, and it could happen when the motor ages. 

Everything is fine until you hit Saturation. Things are great as long as the current is able to keep growing. Saturation is the worst thing in the world. An inductor can only hold so much field/flux/energy before real world effects fuck you day and it stops building up. It'ls like the inductor stops 'pushing back', effectively slowing the build up of current, when it stops pushing back the current will FALL OF A CLIFF. At that point the inductor winding becomes a fat short circuit and current rages through the wire making a shit ton of heat and suffering. Short circuits like this are death to your batteries, motor drives, and motors. The MOSFETs will pop, the wires will burn (I've burnt through a lot of good wire this way), the batteries will be fatally wounded (ditto) and the ice caps will melt we all drown. 

An 8S motor SHOULD be designed to stand up to an 8S source being short circuited through the windings for long enough that your ESC detects the fault and stops the fire from starting. Just need fat wires to make it 8S safe, then no fire, no law suit. Naturally 12S voltage on an 8S safe motor will be incinerated. This stuff is hard to protect against because a short circuit can appear like a normal use at high power, you need to tune to it. Underwriters laboratory care about this sort of stuff and engineers can technically end up in jail, but you won't sue yourself and will be careful right?. 

So I'm saying the 8S rating is probably just a safety thing to stop fires. 

The things that will cause saturation are a) asking too much power (which you can handle). b) if you are stalling, and the motor doesn't commutate at the right speed you'll stay driving the same winding for ages and it'll saturate. total stalling = massive current.

What really limits the max voltage to the motor is the amount of flux the winding can support before saturation happens, i.e. how big is the winding = weight in your hand. You can make an algorithm to hit them harder as they go faster, because the motor commutates faster, you have a shorter window to hit it so do so with more gusto. Just DON"T drive it extra hard when it starts to slow down and stall, limit duty cycle at lower rpm, etc. A higher frequency drive helps I think, but this moves problems elsewhere too. 

How much do you trust your ESC? I say use the 12s on the 8s motor if you can power limit the system and you trust the ESC will do it fast enough, and design the system not to stall easily or at all, and respect the motor max RPM so your bearing dont' melt. i.e. use the 8S motor in the 8S motor envelope, but enjoy the better acceleration and torque of the 12S drive. 

By the way: 
1) high high rpm speed doesn't require high power/current, that's a function of balance, inertia/weight and bearing quality. LOAD & torque drives up current. 

2) 2200W from an 8S battery system? I'm calling bullshit on that. I have a 10S setup on a big heavy 65mm 12S motor and an esc of my own design (for 2KW) and I'm struggling to get past 750W of real power ~ about 1HP. In my experience batteries just don't provide that sort of juice. As soon as you ask for more they sag out, voltage goes down, motor starts to slip. Yes, I know I need more expensive batteries and more of them... that aside, even with 'the batteries of the gods' 2.2KW = 3HP = NOT likely to happen from an 8S in my experience and you should ask them to tell you how they rate and test the motors to that rating. 

Do you do it? Was there a fire?
```

---
## \#25 Posted by: Hummie Posted at: 2017-03-05T02:56:19.372Z Reads: 42

```
an inductor won't saturate but the core within it will.
```

---
## \#26 Posted by: brentsinger Posted at: 2017-03-05T04:31:25.243Z Reads: 44

```
Now we're splitting hairs, but you are correct. 

I don't even  know what the material is inside my motor. Probably just a laminated iron that's good for magnetisation. Know is probabably a good thing since that tells you how long you can pump the thing until you saturation. I wonder if they make motors with Ferrite or similar material. The trade offs would be interesting.
```

---
## \#27 Posted by: Hummie Posted at: 2017-03-05T15:29:34.998Z Reads: 38

```
Ferrite is more efficient but need be larger
http://m.powerelectronics.com/passive-components/ferrite-out-better-core-materials-your-pol-design
```

---
## \#28 Posted by: lrdesigns Posted at: 2017-03-08T06:30:06.987Z Reads: 33

```
I just want to put my two cents in. I'm not an EE but I have many years of experience with small brushless motors from being in RC models hobby. 

From my experience over voltage does not kill motors, heat from over loading the motor will kill it every time irrespective of voltage or RPM. More voltage will increase RPM, but you will reach the ERPM limit of the vesc way before the physical RPM limit of the motor. 

If you increase the voltage over spec you have to compensate by reducing the load on the motor, in our case this means reducing the gear ratio. Then check your not getting over heating during initial testing. 

I am currently running a 270kv 6s rated motor on 12s, it just means I need a 4:1 gear ratio to keep the motor happy and not over load it. If I ran a 2:1 ratio it would definitely over heat.
```

---
