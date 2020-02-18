# Regenerative breaking over charging LiPo&rsquo;s?

### Replies: 23 Views: 1624

## \#1 Posted by: BadleyBoarding Posted at: 2018-01-15T12:48:42.894Z Reads: 225

```
I've activated regenerative breaking on my VESC (hw v4.10) and will mainly be using my board to get to and from campus. To get to campus I have to go out my door and immediately down a hill, since the batteries will already be fully charged when I leave the house I'm concerned regenerative breaking will overcharge the batteries, is there any way to limit this happening in VESC settings or otherwise?
```

---
## \#2 Posted by: aigenic Posted at: 2018-01-15T12:55:24.313Z Reads: 220

```
Correct me if I am not right, but in the BLDC tool you can set up max voltage...if the battery reaches this voltage, the VESC should turn off and you will be left without brakes but without fire underneath your deck ;) BMS does the same thing...

You would ahve to not charge your LiPos fully...

Some eboards like mellow and InBoard use heat resistor to allow you to brake when the battery is fully charged ;) but I dont think it is doable with VESC...
```

---
## \#3 Posted by: GrecoMan Posted at: 2018-01-15T12:56:19.003Z Reads: 212

```
don’t fully charge your batteries.
```

---
## \#4 Posted by: BadleyBoarding Posted at: 2018-01-15T12:59:05.375Z Reads: 209

```
I only normally charge my batteries to 4.14v per cell (4.2 recommended max) but I don't know how quickly regenerative will charge them
```

---
## \#5 Posted by: GrecoMan Posted at: 2018-01-15T13:02:52.668Z Reads: 199

```
if your brakes cut out going down the hill, you charged too much.  if not, your golden
```

---
## \#6 Posted by: ARetardedPillow Posted at: 2018-01-15T13:11:23.948Z Reads: 194

```
I charge mine to 41.15V
```

---
## \#7 Posted by: BadleyBoarding Posted at: 2018-01-15T13:28:43.612Z Reads: 194

```
Yeah I'll try setting the max voltage limit on the VESC and hope my brakes don't stop working half way down haha, thanks guys
```

---
## \#8 Posted by: aigenic Posted at: 2018-01-15T13:58:51.992Z Reads: 188

```
Hope you can stop without electric brakes :) it might be useful :D Hope you dont kill yourself ;)
```

---
## \#9 Posted by: ARetardedPillow Posted at: 2018-01-15T14:04:52.539Z Reads: 183

```
I always prepare to foot brake when I'm going down a hill that leads to an intersection just in case if anything fails I don't get hit by a car and die
```

---
## \#10 Posted by: Namasaki Posted at: 2018-01-15T17:45:32.869Z Reads: 170

```
I’m running Lipos and discharging through a Bestech  bms. 
I have gone down steep hills braking all the way with a full battery while monitoring battery voltage. 
The bms prevented overcharging past the overcharge detection voltage that was set on the bms. 
It did this without shutting down the system. 
The only problem with this is that if the hill was excessively long, the bms might overheat and shut down. 
This is the hill I tested on. Going up the in this video
https://www.youtube.com/watch?v=3F-QcfUBrAs&feature=share

Your only other option is to charge below full. 
DO NOT Lower the max voltage setting on your Vesc. You could loose your brakes even with your battery not full. Leave max voltage at 57v
```

---
## \#11 Posted by: Colydog Posted at: 2018-01-15T21:57:56.871Z Reads: 138

```
I thought it would work like this. When you put the brakes on, part of the breaking force is used to charge the battery, at what ever regen level you set to, and the rest is dissipated as heat in the motors and VESC. When the batt is full then all the force is dissipated as heat. Otherwise you could only break as hard as your batteries can take charge.
```

---
## \#12 Posted by: ducktaperules Posted at: 2018-01-15T22:55:49.301Z Reads: 128

```
Can you just charge on campus rather than at home?
```

---
## \#13 Posted by: Ackmaniac Posted at: 2018-01-16T00:00:38.719Z Reads: 120

```
The vesc can't do that. All the energy is going into the battery. But if your way down that hill is as short as shown in the video then simply don't care about it (if the bms is not shutting down)
That hill isn't enough to harm your battery.
```

---
## \#14 Posted by: BadleyBoarding Posted at: 2018-01-16T16:30:59.199Z Reads: 109

```
Think i'll leave the batteries slightly below full for now and try to be careful. @Namasaki I had never considered running LiPo's through a BMS, could I get a link to the one you're using?
```

---
## \#15 Posted by: Ackmaniac Posted at: 2018-01-16T17:44:12.434Z Reads: 97

```
Do not add a BMS in the discharge cycle. Only use it for charging via a power supply.
```

---
## \#16 Posted by: Namasaki Posted at: 2018-01-17T00:24:44.485Z Reads: 89

```
http://bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html

This is the one I use and discharge through. It will handle 80a continuous and 200a peaks.
It seems to do well in protecting the battery from overcharging by regen braking although I have not tested it on really long hills with a full battery.
```

---
## \#17 Posted by: Juiced Posted at: 2018-01-17T02:29:04.824Z Reads: 84

```
I thought it was discontinued no?
```

---
## \#18 Posted by: Namasaki Posted at: 2018-01-17T04:21:51.826Z Reads: 79

```
We thought so but apparently not. Some people have been able to buy them still.
```

---
## \#19 Posted by: Mathias Posted at: 2018-01-17T06:12:42.026Z Reads: 77

```
And here "protecting" means it will cut off your battery,  and shutting down your vesc with an overvoltage error (no breaks, no nothing for a while). I don't think it's a good idea to have a bms like that... I'd rather risk my battery's life span than my own... 

[quote="BadleyBoarding, post:4, topic:43782, full:true"]
I only normally charge my batteries to 4.14v per cell (4.2 recommended max) but I don’t know how quickly regenerative will charge them
[/quote]

I'm in the same situation, living on a hill. It's easy to estimate how much energy you can actually gain from riding down your hill:

E = rider weight * g * height of the hill

For a 20 m hill and a 90 kg rider that's 
90 * 10 * 20 J = 18 kJ = 5 Wh

Realistically it's gonna be less because of friction and motor efficiency < 1. Probably rather 2-3 Wh depending on how steep the hill is. But this tells you if you're in the same ballpark of the charge that still "fits" into your battery. You can find out if this is "charging your batteries too fast" by looking at the discharge curve. If you e.g. have a 100 Wh pack, look at the discharge curve for your battery and find out what voltage you got at ~95% (5 Wh missing). That's roughly the voltage you should charge to. Then you're on the safe side for this example. 
I guess it's almost difficult to overcharge your pack so much by braking that it catches fire, but if it's your daily commute it will certainly not do your pack any good to slightly overcharge it every day...
```

---
## \#20 Posted by: BadleyBoarding Posted at: 2018-01-18T16:35:07.330Z Reads: 62

```
Thanks @Mathias, by the looks of it I should be fine (assuming my distance estimates are correct)
```

---
## \#21 Posted by: BadleyBoarding Posted at: 2018-01-18T16:36:00.112Z Reads: 59

```
Doesn't look like I can buy it :(
```

---
## \#22 Posted by: Mathias Posted at: 2018-01-18T16:43:23.068Z Reads: 60

```
Google maps works well to estimate it! It has a decent height map. Look up the directions of your route/hill and set it to bike. Then the details will show a height map! I use it all the time to plan longer rides. I like to avoid long, steep downhill sections...
```

---
## \#23 Posted by: Namasaki Posted at: 2018-01-19T00:13:16.217Z Reads: 54

```
You have to email sales and request to purchase it. The min order qty is 2
```

---
