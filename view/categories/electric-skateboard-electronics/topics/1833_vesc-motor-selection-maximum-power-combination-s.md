# VESC/Motor Selection- maximum power combination(s)?

### Replies: 18 Views: 5895

## \#1 Posted by: Qwiksand Posted at: 2016-03-15T21:15:10.878Z Reads: 434

```
I've only just begun dabbling with the VESC and RC motors in general, but I already see where the small size/high-power output really fits with my general use scenarios- ebike, esk8, light PEV, etc.

It seems to me that in order to maximize power output, the VESC and motor should be a good match with both units able to output approximately equal power levels. Am I right in assuming that the best combo would then be VESC on 12 series lipo mated to an approximate 190kv motor like a SK3 6374 or the R-spec 6372?

If that's the case, where do you feel the maximums should be set on the VESC? Or do you have a better motor in mind?

I've also wondered about how the VESC would drive the newer c80-100 that lunacycle sells.
http://lunacycle.com/motors-and-esc/c80-100-kv130-high-power-brushless-rc-motor/

This motor is only 130kv, so you would be giving  up quite a bit of RPM if it's limited to 12s. Something that is outside my capabilities at the moment, but may be interesting for ebike/light PEV use, would be to rewind this motor as a six phase and run dual VESCs. Again, pipe dreams at the moment, not even sure if this is possible, but that would be one power dense little unit!

Real world experience would be awesome, but speculation is most certainly welcome :sunglasses:
```

---
## \#2 Posted by: mattdig Posted at: 2016-03-15T21:48:15.198Z Reads: 420

```
I've got a Turnigy SK3 6364 245kv. It says 10S in the specs but I'm running it on 6S and it's a little champion of speed and torque.
http://www.hobbyking.com/hobbyking/store/__35029__Turnigy_Aerodrive_SK3_6364_245kv_Brushless_Outrunner_Motor_US_Warehouse_.html
```

---
## \#3 Posted by: Qwiksand Posted at: 2016-03-16T14:16:06.236Z Reads: 412

```
I'm sure it works, but it is far from maxed/optimized, right? 

A VESC on 6s is only at 50% of its potential peak power output and that motor is likely running a bit slower than it would like for max efficiency- peak rpm on on 6s for a 245kv is (theoretically) 6174rpm where most reports on these little motors seem to say optimum rpm is between 8k and 9k.
```

---
## \#4 Posted by: onloop Posted at: 2016-03-17T21:51:18.134Z Reads: 395

```
VESC designer has said that optimum RPM for these type of brushless outrunners is 8600RPM.

That why i built my system with 10S & 190KV motors. 

11S battery would be perfect but just not practical to build at 3P for a flat battery. Even cell numbers is better.

11S at 4P would be nice. This also keeps you in a safe zone in terms of VESC voltage limit (60V max) Some people have reported issues using 12S and motors over 190KV.
```

---
## \#5 Posted by: Qwiksand Posted at: 2016-03-20T16:10:05.074Z Reads: 371

```
@onloop, have you had any issues running the big r-spec (190 kv 6372 version) with a VESC on 12s?

For reference:
http://vedder.se/2014/10/chosing-the-right-bldc-motor-and-battery-setup-for-an-electric-skateboard

Using the above article as our manual, maximum rpm for a 190kv motor on 12s (50.4v max voltage @4.2v/cell) is 9576 rpm (67,032 erpm). If we use vedder's suggested "moderate charge level" of 3.8v/cell (45.6v total for 12s), we get a perfect 8664 rpm (60,648 erpm). This, in theory, should be an optimal VESC/motor pairing.

So my question to you is does this theory hold up in practice? Or is 12s pushing too close to the limits for reliable operation at 190kv?

Also, what are you recommending for max amp settings in BLDC-tool for the big r-spec?
```

---
## \#6 Posted by: Hummie Posted at: 2016-03-20T18:32:10.823Z Reads: 346

```
8600rpm is decided as the most efficient electrically but maybe it's not a good number to shoot for in the real world where we have hills, stop signs, wind resistance, multiple accelerations and braking.   If you set-up your gearing for  an averag of 8600rpm maybe you would be limited in top speed, or at the other end of the spectrum you could become inefficient going up hills.  I bet these real-world challenges would be more of an influence on over-all efficiency and battery range than keeping at 8600

I read 12s is ok only for motors 100kv and lower.  Maybe if u don't ever hit an electrical speed that's too high it'd be ok to do even more voltage..such as a really low kv on a bike hub motor or even just not pushe the throttle as high
```

---
## \#7 Posted by: Qwiksand Posted at: 2016-03-20T23:46:17.627Z Reads: 320

```
@Hummie, you raise valid concerns regarding gearing considerations, however, this is a separate issue entirely to the topic at hand.

As to the maximum of 100kv on 12s, I highly suggest you read the link I posted above. Here it is again in case you missed it:

http://vedder.se/2014/10/chosing-the-right-bldc-motor-and-battery-setup-for-an-electric-skateboard
```

---
## \#8 Posted by: Hummie Posted at: 2016-03-21T06:43:47.008Z Reads: 306

```
You're right this thread's title is "maximum power combinations".   It just seems people aren't really looking for max power in the true sense...the max power would be at full speed and people don't hang at that speed often.  

The 8600 number is ideal for efficiency of the esc and not the max power of the motor/vesc anyway. 

Voltage max:
"I have discovered that a good trade-off is at around 60V (quite safe for 10s or 12s lipos), where the efficiency is good and the voltage is not too problematic to handle. "

But only if the commutation speed isn't too high as with a kv that is...id read 100kv but maybe it's 190, and above that the motor will act up at high voltage.  

This is what I've read somewhere and maybe forgotten and could be wrong
```

---
## \#9 Posted by: onloop Posted at: 2016-03-21T10:34:14.787Z Reads: 287

```
[quote="Qwiksand, post:5, topic:1833"]
have you had any issues running the big r-spec (190 kv 6372 version) with a VESC on 12s?
[/quote]

I don't run 12S, never have so cant comment. 10S is good for my use case i don't see any reason to go higher. for VESC it might prove better to keep the voltage under 12S

For the big R-SEPC 6374 you could try gradually increasing to 4kw for very quick runs and see how it goes heat wise. the power increase might not be useable and therefore not noticeable. wether your battery can do that much output safely/continuously or not is another question, What are you trying to build exactly? 

I really doubt there are many situations on a skateboard where you would need to run that much power or use bigger motors.

The R-SPEC 6374 with 2.1kw peak is enough to drop you on your arse. I suppose if you are a big guy and want to climb the steepest hills at top speed and accelerate as fast as a tesla more power might be needed, is this build for race purpose?
```

---
## \#10 Posted by: Qwiksand Posted at: 2016-03-21T22:34:30.176Z Reads: 264

```
@Hummie, I don't know what the maximum eRPM for the VESC actually is- I'm not sure if I've seen this listed or discussed. Vedder states that "these losses" become significant at 60k eRPM, but I don't know what the actual eRPM max limit is where the VESC can't keep up.
```

---
## \#11 Posted by: Qwiksand Posted at: 2016-03-21T22:47:12.516Z Reads: 259

```
@onloop, 

What would you recommend as your maximum's for the 6374 r-spec on a vesc? Is 10s the limit or do you feel pushing to 12s might be ok? Where would you be comfortable setting max motor current? 

I agree, we're not likely to make full use of this hypothetical "maximum power combo" on a stand-up board, but I'm mainly looking to use a pair of these little motors/controllers in a 2-speed gearbox mid-drive I'm working on for an ebike.
```

---
## \#12 Posted by: onloop Posted at: 2016-03-21T23:17:29.507Z Reads: 259

```
[quote="Qwiksand, post:11, topic:1833"]
Is 10s the limit or do you feel pushing to 12s might be ok?
[/quote]

12S will be fine.

The max current is maybe 100AMP peak..

you really just need to test it & report back.

Honestly, I have never used these motors at MAX & I never will.

My aim was to get a really good powerful motor that can handle big power, But never ever run it at max because there is a really thin line between MAX & BOOM.

Running your motor at max is a very bad idea and it will fail. You should probably just buy a bigger motor that can handle twice the power you plan to run through it.

If I have learned anything from building electric skateboards, most importantly is over engineer everything and run your system at 60-70% of its max potential.
```

---
## \#13 Posted by: Nowind Posted at: 2016-05-18T19:35:00.279Z Reads: 235

```
Hey.

I´m running the SK3-6374-192KV as a Dual Rear Drive on 12S with the VESC on Trampa Mountainboard.
The Gearing is 1:7 and good for 47kmh on that 8inch pneumatic tires.
Its a really nice setup which runs very good since about 4 month.

The Vesc set to:
 MAX CURRENT 100A,
 START UP BOOST 0.1

Tryed many other setups and vesc setting, but i doubt that you get a more powerfull combination then this one.

Greetz
Jenso
```

---
## \#14 Posted by: Kwaad Posted at: 2017-03-03T09:26:37.794Z Reads: 146

```
Hi, I am new in VESC.
Could you please help me.
I want to use 16s lifepo4 with VESC (with heat sink) and with 190kv 6374 motor.
And set max current 40 - 50amp and max volt 50 in VESC for motor.
Will be work fine?

Thanks.
```

---
## \#15 Posted by: kavkac Posted at: 2017-06-03T14:37:22.842Z Reads: 128

```
Hi, 

I have an e-longboard and have some problems with my current ESC, so I decided to buy a VESC.. 

Please help me:
Is VESC powerful enough to be used in configuration with 6S battery and this motor: http://alienpowersystem.com/shop/brushless-motors/alien-6355-outrunner-brushless-motor-190kv-2200w/
What would be the limits?

Regards, Jaka
```

---
## \#16 Posted by: Hummie Posted at: 2017-06-03T18:14:47.492Z Reads: 124

```
from what i remember of past people trying 6s it was too many amps for the vesc to get decent power and it would over-temp shut off.   the motor isn't the issue.
```

---
## \#17 Posted by: kavkac Posted at: 2017-06-04T23:25:10.610Z Reads: 107

```
Would it still hurt the VESC if I set the max Amps to a reasonable value?
```

---
## \#18 Posted by: Nedtrampz Posted at: 2019-01-03T03:32:06.613Z Reads: 22

```
Itll be 190 bro. Youll want above 100 for sure running smaller wheels. 

I have the 136kv motors from trampa for my mountainboard (8 inch tires) 

They reccomend their 112kv any lower would be way to slow. Youd have to gear it stupidly
```

---
