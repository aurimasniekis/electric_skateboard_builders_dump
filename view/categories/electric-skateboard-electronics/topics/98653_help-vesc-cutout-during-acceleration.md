# \[HELP\] VESC Cutout During Acceleration

### Replies: 12 Views: 339

## \#1 Posted by: RedLiquid Posted at: 2019-07-17T16:12:22.072Z Reads: 64

```
Hey guys, I'm looking for some help!  First of all I'd like to mention that I've analyzed MANY previous threads regarding this issue to no avail.  Anyways, here is the problem:

When accelerating from a standstill with high throttle, the motor will begin to "shake" (or clunk?) when reaching a certain RPM.  Luckily I have been able to isolate the problem to this setting:

![cap|624x500,75%](upload://yD83hDR3mnl7mWn0QrjQWozjwvU.jpeg)

When the "sensorless ERPM" has been reached, the motor essentially becomes stupid and starts clunking for a few seconds.  At this moment, if I hold the throttle above like 70% or so, the VESC just shuts down and throws an ABS_OVER_CURRENT fault.  (strange thing is my abs. max is set to 130A, and the terminal does not even show >130A?) However if I ease back on the throttle and gently accelerate past the sensorless ERPM, the motor will eventually regain control.  

![cap2|662x304,75%](upload://bigG1S6205iWfGavf7c20xFZBdn.jpeg) 

I verified this is the issue by adjusting the sensorless ERPM.  If I set it to 1000, the clunking/fault code will occur at around 1000erpm.  If I set it to 15000, the same will occur at approx. 15000erpm,etc etc.  For testing's sake I set it to 999999erpm so it is never reached, and the clunking is gone for good.  Unfortunately this means it will be running in sensored FOC mode at high rpms, which is quite noisy and very inefficient (I noticed a significant decrease in power). 

To reiterate simply:

IF throttle > ~70%

AND I am riding the bike (motor has a load)

AND sensorless ERPM is reached

THEN motor will clunk/lag/shake

THEN vesc will throw 
 ABS_OVER_CURRENT fault

I am running 12s5p with a bestech BMS, 
VESC is Flipsky's FSESC6.6 single,
Motor is Maytech 6374 190kv.

Any advice is appreciated!
```

---
## \#2 Posted by: Deodand Posted at: 2019-07-17T17:02:00.677Z Reads: 54

```
This might mean the detection of your FOC motor parameters is inaccurate (Resistance, Inductance and Flux Linkage). Is it a beefy motor? If so I would try upping some of the values in the detection routine. One way to do this is to up your max motor/battery amps before running detection. The detection routine will automatically step up the current and duty cycle up to 50% of the max settings when running detection until it finds a suitable load to run detection on the motor.
```

---
## \#3 Posted by: RedLiquid Posted at: 2019-07-17T18:34:31.499Z Reads: 50

```
Thanks, I will try this when I get home later today!
The motor is just a typical 6374 outrunner
```

---
## \#4 Posted by: RedLiquid Posted at: 2019-07-18T04:39:13.671Z Reads: 43

```
That did the trick. Rode about 5 miles today without seeing any more hiccups.  Thanks so much!

Now that the issue is fixed, I discovered another (unrelated) behavior.  When going on a steep uphill+full throttle, the VESC will sometimes cut off.  Is this normal? or is there a way to optimize my settings so that this does not happen?  Some of my settings include:

Motor max/min = 65A/-65A

Battery max/min = 30A/-12A

Abs Current Max = 130A ->changed to 140A but it still occurs

If this behavior cannot be fixed, that is fine with me; I will just learn not to go full throttle on steep hills.  However if there is an easy way to address the cutoff then I'm all for it.  Thanks!
```

---
## \#5 Posted by: Deodand Posted at: 2019-07-18T17:02:53.827Z Reads: 32

```
At the end of a ride when you experience a cutoff connect to your vesc with a computer without power cycling and in the terminal type "faults". This will provide some information into what is causing the cutouts hopefully.
```

---
## \#6 Posted by: RedLiquid Posted at: 2019-07-18T19:51:02.878Z Reads: 23

```
That was the first thing I tried to do yesterday.  Strangely enough, the VESC reported "No faults logged since startup".  Tried multiple times and it still did not show any faults.  

Perhaps the BMS is cutting out rather than the VESC, causing it to reboot and lose any stored codes?
This seems unlikely because my BMS overcurrent protection is set to 220A, which is higher than the vesc absolute max.

Maybe one of my solder connections is too weak, causing a momentary connection cut in sustained acceleration. <-- I think this may be the most likely... can this damage my vesc or other components if left unfixed?
```

---
## \#7 Posted by: Deodand Posted at: 2019-07-18T19:52:26.629Z Reads: 18

```
You definitely want to get a poor solder joint addressed, left unchecked it will fatigue during vibration and worsen. Who made the vesc you are using?
```

---
## \#8 Posted by: RedLiquid Posted at: 2019-07-18T20:05:34.870Z Reads: 18

```
I'm currently using a single Flipsky FSESC 6.6.  But I don't believe the vesc is the issue because I had the same cutout problems in my setup previously, while using a FOCbox.

I'll check my motor phase wires and see if there are any cold solders there.

Additional question.. is it unusual for my battery voltage to sag visibly?  When I am on medium to high throttle, my battery indicator slowly trickles down anywhere from 5-15 percent depending on how long I hold it.  Then when I release the throttle, the voltage will climb back up to normal.  I'm hoping the battery is not the cause because it'll take a while to disassemble and diagnose solder joints. Dx
```

---
## \#9 Posted by: MysticalDork Posted at: 2019-07-18T20:09:42.837Z Reads: 17

```
Voltage sag is totally normal under sustained heavy load. What's your BMS maximum continuous current?
```

---
## \#10 Posted by: RedLiquid Posted at: 2019-07-18T20:18:59.978Z Reads: 17

```
Ah I see.  My BMS is rated at 80A continuous which is is well above the rest of my setup.

So I will the motor phase wires for a cold solder then.  I have a fairly strong suspicion about the motor because I dropped it once before all the symptoms started happening. : ^ )
```

---
## \#11 Posted by: RedLiquid Posted at: 2019-07-18T20:27:03.188Z Reads: 15

```
Looking at the recent posts, I bumped into this..
According to [Schtekarsten](https://www.electric-skateboard.builders/u/Schtekarsten) a resistor swap might help, possibly this applies to Flipsky 6.6 as well?
https://www.electric-skateboard.builders/t/flipsky-4-20-a-explanation-to-the-mystery-and-how-to-stop-the-cutouts-entirely/87824
```

---
## \#12 Posted by: Schtekarsten Posted at: 2019-07-18T20:30:34.237Z Reads: 15

```
yeah nah shouldn't be the case.
```

---
