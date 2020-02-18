# How reliable has the focbox shown to be so far?

### Replies: 28 Views: 1671

## \#1 Posted by: Hummie Posted at: 2017-11-25T04:13:09.846Z Reads: 251

```
I'm wondering more about it breaking then it hitting an overtemp limit but wondering how its shown there too.

In foc how's it shown to last is what Im mostly wondering


I heard something about them being made in different places..where are they made now and how are those showing?


and when it does fail has it even launched people?

whose had one the longest?
```

---
## \#2 Posted by: mmaner Posted at: 2017-11-25T04:21:48.291Z Reads: 250

```
I have my dual focbox's setup in hybrid mode.  I was practicing drifting yesterday for an hour or so, from a stand still to full throttle while pushing the back of the board outside. I did this prolly a hundred times, hitting around 50 to 60 amps everytime, no issues. .
```

---
## \#3 Posted by: louwii Posted at: 2017-11-25T04:23:58.168Z Reads: 250

```
Given its original price, and its sale price on Cyber Monday, you should just go for one. At that price, I'd say it's unbeatable.
```

---
## \#4 Posted by: Hummie Posted at: 2017-11-25T04:24:02.369Z Reads: 244

```
....so we have one hour, one hour with drifting, one hour with drifting anything more anyone?  how bout 6 months?
```

---
## \#5 Posted by: JLabs Posted at: 2017-11-25T04:25:13.117Z Reads: 245

```
They haven’t FOCed me yet.. I push them hard as well climbing long steep hills... if it were only $97 all the time :thinking:
```

---
## \#6 Posted by: Hummie Posted at: 2017-11-25T04:25:53.051Z Reads: 245

```
if it shows reliable maybe I would be after the insurance its practically the same price as the only two vendors who seem at all legit, axle and ollin,(diy wish it was more reliable but seems not yet)  and those two come with assumed assurance.   but they're slow to get from if even available I think.  ollin slow?  axle I think is out for so long


still waiting for cheap and reliable to happen but more so reliable.  Ive had them break and even with insurance Id rather not break.  Or has it become assumed they will break at this point with these things
```

---
## \#7 Posted by: E1Allen Posted at: 2017-11-25T07:54:05.884Z Reads: 217

```
I've been trying to push dual FOCBOX on 6374s.  So far I've been able to pull 35a max each by mashing the throttle sitting on the board. I'd just get tossed standing. I tried some uphill tests but the bumpy road to the big hill loosened my motor mounts so I just had belt slip trying to accelerate hard. Honestly if I broke one I'd just buy another? I've seen some complaints on the forum but it's a good ESC for the price.
```

---
## \#8 Posted by: Hummie Posted at: 2017-11-25T08:11:39.554Z Reads: 212

```
that brings up a longstanding question:
on current control you set the battery amp max, how come it doesn't necessarily hit that current at full throttle?
```

---
## \#9 Posted by: chuttney1 Posted at: 2017-11-25T09:08:33.592Z Reads: 203

```
How reliable is it at 12S voltage?
```

---
## \#10 Posted by: chuttney1 Posted at: 2017-11-25T09:12:11.605Z Reads: 204

```
With any electronic device, it will only use up the current it needs to work. The best way to make any ESC reach max amperage is to put a resistive load on the driven end.
```

---
## \#11 Posted by: Hummie Posted at: 2017-11-25T15:06:15.613Z Reads: 194

```
but the throttle is creating the resistive load to a large degree, yet not all of it, no?.  I can hit max throttle and the vesc will put out a much increased current because of that.
```

---
## \#12 Posted by: E1Allen Posted at: 2017-11-25T17:23:03.160Z Reads: 182

```
Plenty of people running 12s with FocBox
```

---
## \#13 Posted by: barajabali Posted at: 2017-11-25T17:25:16.605Z Reads: 180

```
I run 12s with the focbox in FOC single drive 6374 sensored.  Pull 60 amps most rides since I weigh 230lbs on one motor. 

6 months In so far no issues
```

---
## \#14 Posted by: chuttney1 Posted at: 2017-11-25T18:50:28.388Z Reads: 171

```
This was discussed here why for some when the throttle went full, the current draw from the battery was not at peak. Yes, you should get the total amount of current draw since a throttle press all the way to 100% should be a value of 1 or 100% on the duty cycle. I know the VESC itself has no problem. The issue is how torque is delivered from the motor over time, and that has been shown in the BLDC test curve of the unloaded motor. And then someone brought up a post when they went to hit the report command for the kV value on the VESC it was reported less than the stated value stickered on the motor. I'm not about to turn this post into a technical post since this is a reliability post about the focbox. Most discussion here never seems to stay focus on the topic here.
```

---
## \#15 Posted by: mmaner Posted at: 2017-11-25T21:24:05.017Z Reads: 154

```
I usually don't keep data regularly, only collect data when I'm looking for some specific data points.
```

---
## \#16 Posted by: PXSS Posted at: 2017-11-25T21:51:48.890Z Reads: 148

```
[quote="Hummie, post:8, topic:39217"]
on current control you set the battery amp max, how come it doesn't necessarily hit that current at full throttle?
[/quote]

Physics!

Place your skateboard upside down, Remove the belt and wheels off the motor and hit full throttle. 

The motor will spin at max rpm. Correct?

How much power does the motor need to spin at max RPM? Not much, since there is no load. 

This is called the no load power condition. This is equal to your battery voltage x your no load current. The no load current is proportional to the torque required to spin the motor.

Ideally this would be zero but in the real world there are losses. Your bearings, copper and magnets; they all have losses. Therefore you need some torque to keep the motor spinning. 

**I expect you to answer this:**
**Lets say you only need 5A to spin the motor at no load. Why would your ESC draw 80A? Better yet, where would all that extra power go?**

---
It is weird that you make motors, but don't really know the basics of how an ESC works...
```

---
## \#17 Posted by: SORRENTINO Posted at: 2017-11-25T22:16:22.423Z Reads: 138

```
60amp battery or 60 amp motor?
```

---
## \#18 Posted by: longhairedboy Posted at: 2017-11-25T22:17:57.595Z Reads: 138

```
We're running them at 12S in dual configs Keeping the settings to about half of their advertised rated current, they last a very long time. Zero issues so far. And they feel great.
```

---
## \#19 Posted by: Hummie Posted at: 2017-11-26T02:42:45.559Z Reads: 116

```


Expecting might be too much

The speed a motor is spinning will change its no load current draw so with 12s vs 10 or whatever it changes.  but whatever and lets assume in youre scenario we're not all of a sudden with a 20s battery and this 80amps isn't partially being lost iron losses.  So 80amps gone out of the battery I'd assume it ends up in a hill conquered and a hot bunch of wire in the motor.  

but your question and talk of no-load current doesn't help me understand my question and how with what is known as "current control" I can program the vesc to have 50 battery amps and yet not get 50 to happen with 100% throttle regardless of the terrain I'm on.
```

---
## \#20 Posted by: PXSS Posted at: 2017-11-26T13:43:45.250Z Reads: 103

```
I'll clear up the scenario:
**Your board is sitting upside down in your living room with no wheels or belts, just a motor attached to your truck**
You have the following:
10S100P battery at 36V (assume there is zero voltage sag)
ESC is in current control mode, and limits are set to 80A for battery and 120A for motor. 
100kV motor. 
Assume that at this voltage, no load current is 5A. 

What happens when you hit full throttle? 

What speed does your motor spin at?

Does the ESC command 5A, 80A or 120A to the motor?

Why?

---
I'll answer these questions later for 3 different scenarios and hopefully you will understand how ESCs work
```

---
## \#21 Posted by: Hummie Posted at: 2017-11-26T16:13:32.373Z Reads: 96

```


What happens when you hit full throttle just on the table is the new scenario then.  It'll do very close to 3600 rpm and 5amps.  Why such a speed?  the motor has little mechanical resistance and is able to get its applied effective voltage and the back emf very close, as the motor always is trying to do.   If the motor experienced a load, such as a very steep hill, or as I'd assumed cranking the throttle as hard as possible from a standstill, it is applying a higher effective voltage to the motor and there becomes a greater contrast between the back emf and applied voltage and the motor struggles to balance the two and current flows.  The difference between the applied effective voltage and the back emf, and the resistance of the winding, determines the current flow as determined by ohms law and I assumed the limit as to what current could then be applied by the esc would be set by the  current limits on the vesc.
```

---
## \#22 Posted by: PXSS Posted at: 2017-11-26T16:30:37.296Z Reads: 92

```
[quote="Hummie, post:21, topic:39217"]
The difference between the two voltages and the resistance of the winding determines the current flow
[/quote]

There is your answer. 

Your current flow is determined by the needs of your motor and not your ESC. If your motor needs more power than your ESC limits allow, you will peg the limit. In any other scenario, you will not.
```

---
## \#23 Posted by: Hummie Posted at: 2017-11-26T17:01:50.127Z Reads: 83

```
which comes back to my question:
i'm not hitting the esc amp limit amp when applying full throttle
```

---
## \#24 Posted by: PXSS Posted at: 2017-11-26T17:02:42.679Z Reads: 83

```
[quote="PXSS, post:22, topic:39217"]
Your current flow is determined by the needs of your motor
[/quote]

Your motor doesn't need it...

Lower the battery amp limit to 10 and see if you don't hit it
```

---
## \#25 Posted by: Hummie Posted at: 2017-11-26T17:08:59.987Z Reads: 82

```
Id think the current flow would be determined by the contrast between the applied voltage and back emf and if I hit full throttle it would be possible to apply a high enough voltage to hit whatever the amp limit set on the esc is regardless of if I'm an 8lbs baby on a downhill.  I feel the motor only needs what I say it needs... I'm saying it needs more and not getting it.
```

---
## \#26 Posted by: PXSS Posted at: 2017-11-26T17:15:32.523Z Reads: 80

```
[quote="Hummie, post:25, topic:39217"]
regardless of if I'm an 8lbs baby on a downhill
[/quote]

Or a board upside down on your bench???

[quote="Hummie, post:25, topic:39217"]
the motor only needs what I say it needs..
[/quote]

So fuck physics essentially...
```

---
## \#27 Posted by: Hummie Posted at: 2017-11-26T17:19:27.906Z Reads: 76

```
I said a downhill but there should be a moment before the motor gets up to speed where a lot more current would be able to flow before the motor spins up even on a bench.
it is logical that if the throttle is determining the effective voltage then full throttle would be able to hit the full pack voltage if need be and the esc should be able to apply whatever current limits are set at any moment regardless of hill or not...until it gets up to speed.
```

---
## \#28 Posted by: E1Allen Posted at: 2017-11-26T17:55:13.096Z Reads: 68

```
I know punching the throttle at low speeds spikes the motor amps and ESC amps are well behind.  Cruise speed is about even. But I assume everyone with telemetry can see this as well.<img src="/uploads/db1493/original/3X/f/4/f4c7c5136f8c00ea92f07f2b5f8301acc24e6267.PNG" width="281" height="500"><img src="/uploads/db1493/original/3X/2/8/28e44d09db8c1a4a26493d3103a48cd1d7d19792.PNG" width="281" height="500">

I have motor amps at to 65 Max because that's what the manufacturer says is Max.  Looks like it's not quite reaching it yet.
```

---
