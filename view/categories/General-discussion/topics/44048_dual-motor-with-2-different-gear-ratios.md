# Dual motor with 2 different gear ratios?

### Replies: 20 Views: 1316

## \#1 Posted by: Acklavidian Posted at: 2018-01-18T23:04:15.436Z Reads: 205

```
Has anyone tried having a dual motor board where each wheel has different gear ratios. Where one motor is geared for torque while the other it's geared for top end. Could this broaden the acceleration curve of a dual motor board?
```

---
## \#2 Posted by: GrecoMan Posted at: 2018-01-18T23:05:28.056Z Reads: 213

```
yes. many people have. most notable is @lowGuido
well actually, @lowGuido used 2 different kV’s. would accomplish the same thing as what you’re talking about. think the biggest problem with different gear ratios is that when going full speed, one motor would just become a generator and all it would do is increase drag.

nice enough @Sender?
was tempted to just say use the search button 😉
```

---
## \#3 Posted by: mmaner Posted at: 2018-01-18T23:05:50.385Z Reads: 202

```
http://www.electric-skateboard.builders/t/different-motor-kvs/2964
http://www.electric-skateboard.builders/t/same-motor-different-kv-and-different-torque-nm/37832
http://www.electric-skateboard.builders/t/uneven-dual-rear-drive/113/5
http://www.electric-skateboard.builders/t/dual-diagonal-uneven-setup/7810
http://www.electric-skateboard.builders/t/ways-to-configure-the-motor-layout/679/2
```

---
## \#4 Posted by: Mathias Posted at: 2018-01-18T23:22:51.408Z Reads: 166

```
I wouldn't do it. The "trick" behind this is that you use one of your two motors in an operation mode that has high power output but a crappy efficiency. The motor will get hot, and you waste a hughe amout of energy. The max speed of your board shoud be ~90% of the no load speed. Then you have the highest torque and the highest efficiency. If your board can't reach the theoretical speed, your problem is too little power, not too low KV. Get a bigger motor, or more motors.
```

---
## \#5 Posted by: Acklavidian Posted at: 2018-01-18T23:34:55.666Z Reads: 157

```
What about using a hub gear from a bike? Has anyone tried that?
```

---
## \#6 Posted by: ATLesk8 Posted at: 2018-01-18T23:35:51.198Z Reads: 153

```
I think it would be cool to run a 170kv 16/40 and 190kv 16/36 or any other differing kv/gearing.
```

---
## \#7 Posted by: squishy654 Posted at: 2018-01-18T23:37:13.229Z Reads: 151

```
If the firmware would take it into account it could be a viable option for more versatility and efficiency...
```

---
## \#8 Posted by: Mathias Posted at: 2018-01-18T23:45:18.967Z Reads: 138

```
I don't believe that you can increase efficiency. As I said. The maximum efficiency is at KV as low as possible. The closer BOTH of your motors run to the 90% of the no load speed (before the efficiency drops again) the better. There is an optimum for a certain max speed. Having one motor to higher: you lose (too high torque load). Having one motor lower: even worse! You have NEGATIVE power output from that one...
```

---
## \#9 Posted by: squishy654 Posted at: 2018-01-18T23:47:11.055Z Reads: 124

```
But the firmware can transfer power from one to the other, when it becomes more efficient and the other not so much, you see? I understand the problem you are outlining, I'm proposing the firmware solve it dynamically..
```

---
## \#10 Posted by: Mathias Posted at: 2018-01-18T23:57:13.327Z Reads: 120

```
What problem? My point is that the highes torque and the highest efficiency is bot there for the lowest possible KV. Adding one motor with higher KV both is worse. Nothing to gain there except for output power at crappy efficiency. "Transferring" the power from one motor running above no load speed happens automatically but is also nothing you can gain from. In best case if you had 100% efficiency you lose nothing, but that's not the case. I don't see how there's anything to gain here. 

You need a motor that delivers enough power at low torque load. Uneven drive is a workaround for motors that are operating beyond their capabilities.
```

---
## \#11 Posted by: pennyboard Posted at: 2018-01-19T08:02:50.620Z Reads: 89

```
I've done it. Like @GrecoMan says, at high speed, one just acts as a generator and slows the other one down. So it doesn't really work as intended, not to mention you risk blowing your vesc by forcing the lower geared one over the ERPM limit. 

That's not to say it doesn't "work". My gearing was set-up 13/36 on one motor and 16/36 on the other motor. The theoretical top speed when using only 13/36 gearing was 32 mph. I was able to achieve 35 mph using on 13T and one 16T gear. So in that sense it works.

However, due to the generator effect, the board could barely reach 35mph and took forever to get there, making the improved top speed essentially useless unless you're drag racing on an airstrip. 
Basically it doesn't really make sense, because you never use the top speed and risk damaging your electronics/motors
```

---
## \#12 Posted by: PredatorBoards Posted at: 2018-01-19T08:36:27.764Z Reads: 82

```
Why not run a one-way bearing on the lower rated motor?
```

---
## \#13 Posted by: pennyboard Posted at: 2018-01-19T08:39:44.196Z Reads: 79

```
I suppose you could, although then you wouldn't get the braking benefit of both motors. 
although then you'd have to figure out a way to mount the bearing within the motor pulley, which could get complex
```

---
## \#14 Posted by: squishy654 Posted at: 2018-01-19T17:14:24.586Z Reads: 69

```
I have a chain drive with freewheels...done..lol
```

---
## \#15 Posted by: ugothakd Posted at: 2018-01-19T18:32:00.624Z Reads: 60

```
Although there are no conclusive results, some think that uneven drive is actually quicker than same geared. Some people prefer a high kv high gear ratio because it's sort of like a "running" start, the motor is already turning quickly. And then the lowest kv motor provides the torque needed. All of this is discussed in the threads linked above
```

---
## \#16 Posted by: b264 Posted at: 2018-01-19T21:53:41.968Z Reads: 56

```
[quote="squishy654, post:7, topic:44048, full:true"]
If the firmware would take it into account it could be a viable option for more versatility and efficiency…
[/quote]

:arrow_up:

This.  If you adjust the firmware to turn off one motor when it becomes inefficient then everything should be fine.  Hope you know calculus and C99
```

---
## \#17 Posted by: pennyboard Posted at: 2018-01-19T22:53:24.246Z Reads: 43

```
I don't know that you can just "turn off" a motor. Maybe open all the FETs on the Vesc so the phase wires are all open-circuit, but the motor is till going to turn and generate a back EMF. And there's a good chance that the back EMF will eventually build up to the point where it'll jump and potentially short out the VESC.

This is part of the reason why you shouldn't push-ride or down-hill with the board turned off.
```

---
## \#18 Posted by: b264 Posted at: 2018-01-19T23:21:24.985Z Reads: 40

```
If that was the case, you could spin the motor with the wires unhooked and if you spun it long enough, the wires would arc through the air

I think the main reason for that is because MOSFETs typically have a lower Gate-to-Source voltage limit than they do for Drain-to-Source.  But I could be wrong.

Opening the FETs is exactly what I meant when I said "turn off"
```

---
## \#19 Posted by: pennyboard Posted at: 2018-01-19T23:28:22.358Z Reads: 35

```
I think it is the case that the voltage will arc eventually. However the air acts as a dielectric, and it takes a lot of voltage for it to experience dielectric breakdown, somewhere like 1 million volts/meter. So until that happens, basically now current flows, since the resistance is too high. Also, it would be basically impossible to generate 1 million volts/meter by spinning the motor. But if a certain component on the vesc has a lower dielectric breakdown, like PCB might (I'm not really sure if it does or not), you could risk shorting it.
```

---
## \#20 Posted by: b264 Posted at: 2018-01-19T23:30:19.919Z Reads: 37

```
I don't think it does that
```

---
