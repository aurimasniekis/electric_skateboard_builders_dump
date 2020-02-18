# Torqueboards 12s esc question

### Replies: 16 Views: 3443

## \#1 Posted by: cmatson Posted at: 2015-07-23T02:31:03.200Z Reads: 176

```
does anyone (maybe torqueboards himself?) know how many watts the sensored 12s esc is pulling continuous, and how many it bursts? odd question, but Onloop and I are trying to figure out what killed my battery...
```

---
## \#2 Posted by: onloop Posted at: 2015-07-23T03:40:31.972Z Reads: 176

```
The watts it is pulling is related to the load, High Load = More Watts. Minimal Load = Less Watts. So it is not a set amount that is always on it is a variable amount. This variable amount is determined by the efficiency of the ESC, The motor design itself & the load on the motor. Which is also determined by gearing ratio and wheels size, rider weight & incline etc.

So for it to blow that BMS it would of had to be pulling over 2400W for more then 10 Seconds. Which is not impossible. But without a watt meter attached we won't know what your system is pulling. Also this is all speculation, need to do more testing on the fault to know more.

From my testing with a watt meter an average of 1000W (probably less) is about the normal continuous current of a dual drive eboard.


***NOTE: All SPACE cells will be coming with a built in 60A fuse from now on to protect it from sustained high discharges over 2400W.***

The ESC's I have been using for the last 12 months all have had Current limiting. So I thought I really don't need a fuse. But when the man himself Ben Vedder say this:

> ***QUOTE FROM BENJAMIN VEDDER***
> *I would still recommend a fuse. If you happen to short two motor wires for an instant (the motor could even short internally from mechanical damage), the current limit will not keep up because the motor inductance disappears. When that short happens, the two FETs that are ON will fail with a short circuit. When the opposing FETs to them switch on, they will also short out and you get a low-impedance connection between plus and minus - that will lead to a small fire:*
> *If you have the fuse in a situation like that, you will kill one or two FETs and maybe the DRV, but they can be replaced and the VESC will work again. Without the fuse, there is no way you can repair the VESC after a short. You also save other components from the fire. Therefore I always recommend adding a fuse, even if you use a hobby ESC.*


The sepcs on that 12S TorqueBoards ESC are:
Continuous Current – 120A
Burst Current – 180A up to 10 seconds
Input Voltage – 5-12 cells Lithium Battery or 15-36 cells NiMH Battery
BEC – No, you will need a separate BEC aka UBEC, SBEC, etc.
Refresh rate of throttle signal – 50Hz to 432Hz
Size – 92mm L x 55mm W x 15mm H
Weight – 133g 

**So with a 12S battery in theory it can peak at 8000W for up to 10 seconds.. or continuous for 5300 watts without burning up. IT'S A BEAST!**

with a 10S battery it could peak at 6660W for 10 seconds... or continuous for 4440 without burning up.
```

---
## \#3 Posted by: torqueboards Posted at: 2015-07-23T15:14:07.503Z Reads: 147

```
Your best bet would be to put a watt meter through your setup. You can then actually see what wattage and amps you are pulling. There are certain watt meters which log.

Typically, it's about 10-30 amps cont and 60 amps peak. Not usually, do we ever pull higher then that. I've tested going up some steep hills and perhaps maybe 70-80 amps peak but haven't been able to reach higher.

It is capable of pulling 120amps cont and is tested before being shipped. I haven't had much of a failure rate with these ESCs. Also 1080A burst up to 10 seconds.

The BMS should stop the battery from pulling based on it's own specs, I would assume?

I still don't see how you would even get close to 120amps cont.
```

---
## \#4 Posted by: cmatson Posted at: 2015-07-23T16:24:26.367Z Reads: 135

```
Thanks all for the help: maybe I'll do some testing after getting another space cell.
```

---
## \#5 Posted by: onloop Posted at: 2015-07-23T23:30:48.046Z Reads: 134

```
Yeah it still a bit of a mystery what happened.

Anyway under warranty you get a brand new one shipped to your door.

Only problem is there has been a world wide shake-up with all carriers who handle li-ion batteries just recently.... http://www.electric-skateboard.builders/t/boeing-warns-about-flying-lithium-batteries-consignments/73
so your delivery is going to be a bit slower then before... will ship out next week.
```

---
## \#6 Posted by: cmatson Posted at: 2015-08-01T21:48:05.958Z Reads: 131

```
So I was pleasantly surprised when my replacement space cell showed up yesterday, and went right to work on my board. I went through all the esc’s programable functions, and made a couple changes: lowed acceleration from “high” to medium, and changed the overall max power to 80% down from 100%. Everything else I just made sure was in Torqueboard’s recommended settings range. I first tested it with normal abec 11 83mm flywheels, and rode it around for maybe a kilometer with no problems. So, I threw on the 5 inch pneumatics, and then rode it for maybe 3 or 4 kilometers, before being satisfied and coming home. Then, my dad wanted to take a ride with the pneumatics, and thats when I blew the space cell’s fuse. He gave it a pushing start, and didn’t even start to pull the trigger until he was going 6 or 7kph. The motor started to push him from there just fine, for about 3 seconds, and then, he tried to give it more power to accelerate, and it just cut out. After looking at the fuse, you can easily see that it is blown… My dad weighs about 95kg, while I only weigh 65kg, but still, Someone of his size should still be able to ride the board. So at this point is it just safe to say I can't use this esc with a space cell?
```

---
## \#7 Posted by: torqueboards Posted at: 2015-08-02T00:40:38.248Z Reads: 120

```
So I actually just spoke with another customer of mine who is using a single TorqueBoards 12S ESC with the Enertion SPACE Cell he is also here in SF uphill/downhill. He recommended to use the lower settings as to not allow the amperage to reach higher limits which makes sense. So far he's not have had any problems.

You can adjust the motor timing and motor acceleration much lower to not allow the setup to go completely at full power upon throttle. This should keep the amperage on your setup lower. I suggest trying that first.

Problem with BMS systems is once you hit peak. They'll literally shut off so I'd say test it and go easy on it first and be aware because if it cuts off it will slow the board down too.

Please report back on your findings :smile:
```

---
## \#8 Posted by: cmatson Posted at: 2015-08-02T01:15:45.855Z Reads: 117

```
Ok sounds good so here's the plan- lower motor timing, and acceleration, then try again. I will still keep the max power at 80%, and leave everything else unchanged. It is really re-assuring to know someone else has this combo, and that it is working in San Francisco of all places. Down here in florida, you'd be lucky to to even see a hill...
```

---
## \#9 Posted by: onloop Posted at: 2015-08-02T03:57:51.353Z Reads: 117

```
The other thing I used to do to help protect my electronics, this was when I used flier esc, was to set "exponential" acceleration curves. It prevents the system pulling high amps when there is high loads. I.e. when you are starting it uses very gradual acceleration.

Not sure if the torqueboards ESC has throttle curve control but it's worth trying if it does have it.
```

---
## \#10 Posted by: cmatson Posted at: 2015-08-03T01:52:15.355Z Reads: 117

```
Update: esc acceleration turned to low, although I couldn't tell much of a difference from medium... also, motor timing turned from very high to normal. Result: worked flawlessly with the pneumatics when I rode it around for about a mile, and it also worked with my dad riding it for about half a mile. I also had my dad do some hard acceleration tests (well, as fast as he could accelerate without falling off..) and it never blew a fuse! One more thing though: onloop said the fuse was 60 amps, but it says 30 on the top. Also I bought a 10 pack of fuses from autozone, and they were 30 amps. The fuses were all color coded so I got green ones (green ones came with the space cell) that looked near-identicle to the stock fuses. Also, even if I wanted to get 60 amp fuses, they didn't have any in that size: the highest that size went was 30, and for 40-60amps, the fuses nearly doubled in size and would clearly not fit. On a side note, I did the tests today on an autozone purchased fuse, and it was fine. Here's a pic of the fuses- the lightly colored one in the middle came with the space cell, and the darker ones were purchased<img src="/uploads/db1493/original/1X/549608cf1f72d8ff0c2ed5d9423c6f9312e2d3be.jpg" width="690" height="388">
```

---
## \#11 Posted by: onloop Posted at: 2015-08-03T02:27:16.666Z Reads: 108

```
It is great news that changing the setting worked well! So it seems that the TorqueBoards ESC has built in current limiting. That's really good! Also it seems that it doesn't adversely effect your performance! Which is also great news!

**Regarding the Fuse:** 
Yes, I did say it was a 60A fuse, but I was wrong! I just checked with the battery engineers, they said a 60A fuse is not suitable as it can actually allow 90-100A for a few seconds. This is too much for the 60A BMS Which will shut down.

A 30A Fuse will allow 60A peak for about 5 Secs then it will blow which is perfect as it will protect the BMS.
```

---
## \#12 Posted by: torqueboards Posted at: 2015-08-03T02:32:57.971Z Reads: 107

```
Great news!!! I was referring to current limiting by the "amperage number" similar to VESC. That's really great news. Now you can enjoy your space cell :smile:

If you add a fuse, doesn't that stop the regen since a fuse is only one way directional.
```

---
## \#13 Posted by: cmatson Posted at: 2015-08-03T03:18:50.020Z Reads: 109

```
Yep, everything is looking good now, and if its working great with 5 inch pneumatics, it'll definitely be fine on 83mm flywheels.

My next test (tomorrow) will be to decrease the motor timing even further (I really don't care about speed for the pneumatics, and more torque is always beneficial) but bring the power back up from 80% to 100%. This might end up preforming not that differently than the 80% power + higher motor timing that I am using now, but I'd still like to do some more testing... 

Is there anything else you guys think I should adjust, even if its just something to test for kicks? this goes for either 83mm flywheels, or 5 inch pneumatics, because I will be running both from time to time, and will obviously switch settings when going between them.
```

---
## \#14 Posted by: onloop Posted at: 2015-08-03T03:27:05.444Z Reads: 106

```
Fuses are not one way. you can install it any way and they still function
```

---
## \#15 Posted by: torqueboards Posted at: 2015-08-03T04:21:24.753Z Reads: 103

```
[quote="onloop, post:14, topic:69, full:true"]
Fuses are not one way. you can install it any way and they still function
[/quote]

Oh cool. That's good to know. :smile:
```

---
## \#16 Posted by: onloop Posted at: 2015-08-03T04:56:38.798Z Reads: 103

```
As you have a few fuses in stock now, I would recommend riding up a step hill as fast as possible, wearing a pack with 10kg inside & slowing increasing the settings for power output (and acceleration) of the ESC, before each run, until your fuse blows. Then drop it back just enough to stop the fuse blowing..

This should have you in a good zone of max power and safety for the electronics.
```

---
