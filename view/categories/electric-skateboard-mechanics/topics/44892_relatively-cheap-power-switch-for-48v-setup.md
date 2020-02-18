# Relatively cheap power switch for 48V setup

### Replies: 9 Views: 765

## \#1 Posted by: swagimir Posted at: 2018-01-28T21:48:12.209Z Reads: 152

```
Hi guys,
some weeks ago I made a decision to change motor and voltage used by my skateboard (24V previously and 48V currently). I have new motor, 4x 3S LiPo packs in series, 12S BMS, VESC, Charger for 48V battery. Everything is almost finished, but I wonder how to make a power switch. Previously I used car relay and it worked generally fine. Do you know any cheap solution for 48V setup? I haven't found any 48V relays with size of car relay. I don't want to spend to much money for dedicated switch specially for VESC.
I suppose that XT90 "loop key" is one of the cheapest for sure, but I would prefer to have button if I may :) 

BTW. Previously i used car relay (12V on 'connectors' propably and 24V coil) for 24V setup. Could it cause restarting skateboard after some minutes of driving? I had a problem like that before and why it was happening. Temperatures on VESC maybe were ok, but this relay was a weak point.


Thank you really for any help ;) 
Marcin
```

---
## \#2 Posted by: krloz Posted at: 2018-01-28T22:05:26.597Z Reads: 140

```
I will always recommend xt90s.
Simple, easy, cheapo, fail proof, not very aesthetic
```

---
## \#3 Posted by: krloz Posted at: 2018-01-28T22:06:23.051Z Reads: 136

```
If you still haven't invested in the bms maybe you can look for I've with switch.
```

---
## \#4 Posted by: swagimir Posted at: 2018-01-28T22:57:45.098Z Reads: 116

```
Thank you for answer. I have a BMS already (same like that for LiPos: https://pl.aliexpress.com/item/High-quality-36V-12S-43-8V-Lifepo4-battery-BMS-and-lifepo4-18650-or-Lipo-battery-with/32455728066.html ) :) 

If there won't be any choices for me so I will use XT90 Antispark as you said. Power switch looked and worked awesome for now :P
```

---
## \#5 Posted by: scepterr Posted at: 2018-01-28T23:02:10.981Z Reads: 110

```
It's not just about voltage,it's about amperage and wattage, if let's say you use 100A discharge at 12S you're looking at 5000+watts you need to put through the switch. I don't know of any reliable enough switch to do that other than using a loopkey
```

---
## \#6 Posted by: Eboosted Posted at: 2018-01-28T23:05:07.376Z Reads: 107

```
Get the ones from @goldenHusky they are good, I has those on all my builds
```

---
## \#7 Posted by: swagimir Posted at: 2018-01-28T23:25:47.455Z Reads: 100

```
@scepterr, there was 50A (limited using BLDC Tool) on 24V maximally earlier. A car relay I used was 'high-current ready' (on the box was 80A) :P 
Now I want to limit to 30A on 48V.

No doubt it is hard to find cheap solution. 

@Eboosted, thank you for recommendation. I will look at this in a moment and think about it ;)
```

---
## \#8 Posted by: scepterr Posted at: 2018-01-28T23:47:18.759Z Reads: 96

```
Oh my bad I thought you were doing dual motors for some reason, yeah for 1, 50A batt
```

---
## \#9 Posted by: swagimir Posted at: 2018-01-29T09:31:28.940Z Reads: 76

```
@scepterr Yes, I use just 1 motor ;) This one previously: https://hobbyking.com/en_us/turnigy-aerodrive-sk3-5055-430kv-brushless-outrunner-motor.html , and now I have that one: https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-168kv-brushless-outrunner-motor.html . Dual motor construction requires 2 escs, so that solution seems to be cheaper and powerful enough :P
```

---
