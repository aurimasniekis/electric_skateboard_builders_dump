# VESC - does regenerative braking require a BMS?

### Replies: 17 Views: 2070

## \#1 Posted by: slick Posted at: 2018-05-30T21:22:50.629Z Reads: 280

```
Hey guys,

My first VESC (HK/Turnigy Sk8 ESC) finally arrived and I´ve managed to configure it with the VESC Tool after a frustrating start (VESC Tool could´nt detect VESC,,,then VESC Tool crashed while trying to update firmware...you know, that kind of stuff). 

Anyway, I´m running a SK3 5065 236KV in FOC and it seems to work fine after the motor setup wizard (well at least on my desk). After that I ran the input setup wizard and everything was fine too. I disconnected the VESC from the PC and gave it a try - YAAAAY! it´s alive! :relaxed:

I have two 4S 5000mah LiPos in series and  I had to think about regenerative braking and how the VESC charges LiPos or cells in general. :face_with_raised_eyebrow:

Here are my questions 
**does regenerative braking require a BMS?.**
**can I turn regenerative braking off?**

I´m just trying to make sure everything is safe before I install things and go on the road, 
Any help is appreciated! :grinning:

Thanks,
chris
```

---
## \#2 Posted by: squishy654 Posted at: 2018-05-30T21:26:38.064Z Reads: 268

```
it doesn't require a BMS but a BMS is much healthier for your batteries.. and yes you can turn it off by setting the breaking amps to zero, but then you would lose your breaking ability..
```

---
## \#3 Posted by: slick Posted at: 2018-05-30T21:34:02.682Z Reads: 258

```
huh...seems like I´ll have to leave regenerative braking "on" if I want a brake. 
thanks for the quick answer ! @squishy654
```

---
## \#4 Posted by: linsus Posted at: 2018-05-31T07:34:52.098Z Reads: 220

```
The only sufficient way to break a BLDC motor (without a physical discbreak) is to use regenerative breaking. To turn the motor into a generator you basically phase shift the sinwaves(180 degrees if im not wrong). Instead of the magnetic field propelling the motor forward it applies retardation to the rotor and generates a current. Sure you could let that energy burn up in a load somewhere but since the currents are quite fast and not continuous it wont be dangerous for the battery to soak them. Only time you should be cautious is if you have a absolutly fully charged battery and break down a long ass hill. That could potentially set a fire.
```

---
## \#5 Posted by: slick Posted at: 2018-05-31T08:58:23.339Z Reads: 199

```
Thanks for the detailed answer @linsus. Fire hazard was one of the things that came into my mind when I thought about it - thanks for reassuring my thoughts. Though I don´t have huge hills to worry about, I´m still trying  to be very careful with what I´m doing as an inexperienced / first time VESC user.

I read a bit in the forum before going to sleep and my concentration was failing me. I think I read something about the **VESC not applying regenerative currents while coasting (?)** so it´s really just feeding current back when I actively use brakes. In some cases I just let the board slow down itself - so it´s relatively safe, right ? And I also checked in the VESC Tool again. Under the "Current" tab I can set the "Battery Current Max" (max. amp drawn from battery) and "Battery Current Max Regen"  (max regen current that flows back to battery)

So i could in theory set the "Battery Current Max Regen" to 0 and no current will flow back into the cells - which could/will generate heat (?) thus might cause the VESC to kick in the Temp Cutoff (the energy needs to go somewhere, right ?).
```

---
## \#6 Posted by: SimosMCmuffin Posted at: 2018-05-31T12:34:56.187Z Reads: 168

```
[quote="slick, post:5, topic:57304"]
VESC not applying regenerative currents while coasting
[/quote]
 If you're not applying throttle or brake, then the VESC will let the motor just freeroll. Although if you go very fast for example downhill without motor power, if the motor reaches high enough speed it might start pushing energy back into the battery without brakes being applied.

[quote="slick, post:1, topic:57304"]
does regenerative braking require a BMS?.
[/quote]
In theory yes, but not really in practice, except for a particular scenario.

When you're braking and energy is pumped back to the battery it's voltage will raise, how much the voltage raises is dependent on the braking current, motor speed and the battery's ability to absorb the incoming energy (this depends on battery's current rating and capacity).

What you want to avoid is any of your cells in your battery going over 4.2V, but this isn't really a problem during a ride and you have discharged the battery already so it's cells are not near the 4.2V, how much lower will they be depends on how much energy you have used, but generally the cells will be able to absorb the energy without their voltage raising too much.

The only scenario where this really might happen, is that you have charged your battery to the top and you immediately have a long downhill on the start of your ride, which you need to use brakes on. With the battery being full, it's cells are very near that 4.2V full point and anymore energy into the battery will raise the cell voltages over that limit. This might drastically shorten the life of the battery or if it's even more, then the cell might experience a thermal runaway (aka, burst into flames).

I would recommend having _some_ brakes on the board, if you're not sure, just set the negative braking currents to something low. So knowing these rules and you knowing your riding route, if you charge full, avoid strong braking in the beginning or alternatively, don't charge completely full, but leave a little "breathing room".
```

---
## \#7 Posted by: slick Posted at: 2018-05-31T13:50:27.004Z Reads: 132

```
thanks SimosMcmuffin. I set the "Battery Current Max Regen" to 10 amps for now and see...I hope I can get things running soon. I can´t wait to try out the VESC.

EDIT : I changed it to -25A....read why i the post below...
```

---
## \#8 Posted by: squishy654 Posted at: 2018-05-31T14:16:55.251Z Reads: 130

```
My current setting are at 10amps, it's like half assed breaks but keep my battery healthy
```

---
## \#9 Posted by: SimosMCmuffin Posted at: 2018-05-31T14:43:22.263Z Reads: 127

```
What's your "Motor current max regen"?
```

---
## \#10 Posted by: slick Posted at: 2018-05-31T15:19:53.171Z Reads: 129

```
Motor
Motor Current Max : 60A
Motor Current Max Brake : -60A
Absolute Maximum Current : 130A
Slow ABS Current Limit : True

Battery
Battery Current Max : 50A
**Battery Current Max Regen : -25A**

DRV8301
DRV8301 OC Mode : Current Limit
DRV8301 OC Adjustment : 16

I have 2 4S1P LiPo 5000 mah packs wired to a 8S1P 5000 mah LiPo pack. 40C continious 50C burst. 

The way I understand it is that the VESC
will feed back 25A (max.) to my packs. If I understood and calculated correctly : 25A divided by 8 Lipo cells = 3,125A. So the VESC will charge at a max. current of 3,125A per cell which is under 1C charge current. Makes sense to me or am I missing something?
```

---
## \#11 Posted by: SimosMCmuffin Posted at: 2018-05-31T17:18:38.443Z Reads: 113

```
The -60 motor brake current is pretty darn high. At higher speeds the braking power is limited by the battery current regen max, but as your speed slows down it can ramp up the motor brake current.

IMO start with:
Motor current regen max: 30A
and battery current regen max: 20A

Then as you get used to the feel and you want more braking power, increase them.
```

---
## \#12 Posted by: slick Posted at: 2018-05-31T17:23:53.505Z Reads: 106

```
I'll try out your suggestion. Thanks for the help!
```

---
## \#13 Posted by: Jalapeno Posted at: 2018-07-27T22:18:15.574Z Reads: 96

```
How are you connecting those 2x 4S1P batteries to the 8S1P?

And your reasoning is off.
With your example of a 8S1P if you set a limit of 25A recharge current, then each cell will be charged at 25A which is well above 1C for most cells. Just think about it, if the cells are wired in series where does the current go to? The current that goes in the positive voltage cable must come out in the ground cable of the battery.
But at 8S and 25A you have about 8x3.7x25=740W worth of braking power (rough math, disregarding battery voltage increase when charging).
If your battery was 4S you would have half the braking power, 370W (for the same brake current).

Lets say your pack is made up of 2500mAh cells in a 8S1P configuration. To charge the pack at 1C is exactly the same as charging each cell at 1C which is 2.5A.
You would need a pack to be 8S10P in order to have 1C flowing across each cell. That is 25A divided by 10 cells in parallel = 2.5A. But that is just guessing, as cells are not created equally and imbalances (internal resistance) can occur throughout the life of the pack, some cells in a given parallel array might be charged at more than 1C and others less.

You should be fairly safe, but keep in mind that if the pack is full, braking is not good as it may tip the cells over 4.2V which will reduce their lifespan. Charging at currents more than recommended by the manufacturer will also reduce their lifespan.
Both these situations may turn in to puffed batteries or fires if taken to extremes.
```

---
## \#14 Posted by: slick Posted at: 2018-07-28T07:06:57.432Z Reads: 78

```
I'm running on 2x 4s LiPo packs 5000mah wired in series to a single 8s pack. So  1C charge current = 5 amps. 

So with -25amps regen current, am I now feeding back 3.125 amps per cell (which is below 1C) or are the cells getting 25amps individually? 

I have'nt encountered any problems so far and the LiPo packs are fine as far as I can tell. Then again, it might just be Fortuna protecting a fool  (me just being lucky).

I wish i had stronger brakes but I dare not go beyond my current settings. It gets a bit sketchy when Im riding at higher speeds and something unexpected happens. So I ride accordingly to avoid dangerous situations.

So what do you think? 
Did I wrap my head around this correctly?
```

---
## \#16 Posted by: Jalapeno Posted at: 2018-07-28T23:51:25.672Z Reads: 72

```
[quote="slick, post:14, topic:57304"]
So with -25amps regen current, am I now feeding back 3.125 amps per cell (which is below 1C) or are the cells getting 25amps individually?
[/quote]

If I understood correctly you have two 4S Lipos wired in series to make a 8S battery?
If you regen at 25A, then you are putting -25A through your posive and ground battery leads.
Since your cells are wired in series each one of them has -25A of current flowing through them.

Just picture current as water and cells as water tanks. If the tanks are in series and you have 25 liters/second flowing through them then you have to have 25 liters/second flowing through each one. You can use this analogy for the parallel, series and parallel battery arrangements.

I'm just letting you know that you are in fact charging your battery at more than 1C.
If you read around people use fairly high regen currents compared to 1C.
```

---
## \#17 Posted by: slick Posted at: 2018-07-29T08:58:43.877Z Reads: 61

```
Yes,packs are wired to 8s1p when riding. Btw, thanks for taking the time and explaining. One  thought just came to mind:

The regen-amp is not always, in this case -25amps, constant correct? I mean the amps generated by the motor depends on your speed = motor rpm. So if my motor is not rotating fast enough to generate 25 amps the current being fed back to the LiPo should be smaller, correct?
```

---
## \#18 Posted by: Jalapeno Posted at: 2018-07-29T22:41:26.241Z Reads: 58

```
I would also say so, yes.
```

---
