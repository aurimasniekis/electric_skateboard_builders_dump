# What fuse do you use?

### Replies: 48 Views: 6051

## \#1 Posted by: Stevemk14ebr Posted at: 2016-07-22T01:57:30.049Z Reads: 575

```
I'm looking into picking a fuse for my build. I run 12s lipos with dual TB 230kv motors (rated at 80amps) and dual TB 120a Esc's. I'm thinking of looking into some 58V 80A fuses, does this sound alright, should it be higher/lower? What do you guys use on your builds and what would you recommend.
```

---
## \#2 Posted by: barajabali Posted at: 2016-07-22T02:06:30.948Z Reads: 572

```
Tbh I don't use a fuse and have never had a problem
```

---
## \#3 Posted by: Pantologist Posted at: 2016-07-22T02:39:52.738Z Reads: 564

```
That should be fine. Just make sure you use easily replaceable ones. You might want to look into getting a circuit breaker rated at your spec instead. You can easily reset it if you trip it.

At 12S though, I doubt you will reach the 80A. You might hit max, 60A going up a hill or something.
```

---
## \#4 Posted by: Stevemk14ebr Posted at: 2016-07-22T02:44:55.512Z Reads: 561

```
Well the goal is to not blow the fuse while riding and instead protect against shorts stuff.

I was more looking for links and stuff as there are ALOT of options and i'd like to go with wjat is proven
```

---
## \#5 Posted by: barajabali Posted at: 2016-07-22T02:52:30.837Z Reads: 537

```
Let us know what you end up with :) maybe ill integrate in my packs in the future.
```

---
## \#6 Posted by: Namasaki Posted at: 2016-07-22T03:02:11.122Z Reads: 533

```
I was running exactly the same setup as you and with an inline watt/amp meter going uphill the peak amp draw on my battery was only 18.4a @ 12s
37.38a @ 6s
```

---
## \#7 Posted by: Stevemk14ebr Posted at: 2016-07-22T03:11:22.480Z Reads: 529

```
Awesome info, thank you. I wanted to put in a watteter but i decided against it. I know ive seen people post that they use fuses. Anyone?
```

---
## \#8 Posted by: Namasaki Posted at: 2016-07-22T03:32:03.562Z Reads: 520

```
A fuse is good insurance in case one of your esc's shorts out or you get a short in your wiring.
a fuse will save your batteries.
You can get regular size ATC/ATO fuses in 40,50 and 60 amp on Amazon
```

---
## \#9 Posted by: mason Posted at: 2016-08-06T01:37:28.586Z Reads: 485

```
most I see are rated for 36v, but I've also heard people using 60v systems on them.

What is true? I'm looking at fuses for my 50v lipo.
```

---
## \#10 Posted by: Namasaki Posted at: 2016-08-06T02:21:39.158Z Reads: 487

```
They should work  ok for 12s or you can get a maxi fuse. There bigger and have heavier guage wire
```

---
## \#11 Posted by: Stevemk14ebr Posted at: 2016-08-06T04:08:06.466Z Reads: 485

```
I never found a proper fuse. I did alot of research though. Never underspec your fuse, if it says 36v do not use it on a 50v system. The voltage ratings are very important for dc systems because they define if the fuse will actually stop current from flowing if it gets blown. Dc voltage likes to arc much more than ac due to the fact it's "constant", which means fuses need to then have more arc suppressing material in them to counter that. If you do under spec your fuse what may happen is that the fuse blows at whatever current it is rated at and then an arc forms between the two fuse terminals, thus completing the circuit and nullifying a fuse in the first place.

You CAN use fuses that have ac only voltage ratings but you need to AT LEAST double what your are running. Example, if you run a 50v Dc system you'd need a 100v ac fuse at absolute minimum.

Tldr; dont underspec your fuse or it wont work as expected if and when it is blown.
```

---
## \#12 Posted by: Namasaki Posted at: 2016-08-06T12:07:58.614Z Reads: 461

```
Good point, 
I'm actually not using a fuse on my new setup but my bms has short protection
```

---
## \#13 Posted by: flatsp0t Posted at: 2016-08-06T13:19:18.446Z Reads: 452

```
I use mini-ANL type fuses, they have very low resistance and a large contact patch.
The onla problem is the relatively large holder (slightly larger than one 18650 cell).
As a bonus, they are available up to 120A.
```

---
## \#14 Posted by: Randyc1 Posted at: 2016-08-06T13:33:44.094Z Reads: 446

```
Only 18A going uphill ??,  ... some people here have reported taking up to 60 A going uphill ?
```

---
## \#15 Posted by: Namasaki Posted at: 2016-08-06T14:24:23.605Z Reads: 445

```
That is what the inline meter showed at 12s
Going up a 10% hill. 
Don't know how some are pulling 60a. 
Maybe on a 30-40% hill
```

---
## \#16 Posted by: Bender Posted at: 2016-09-14T01:47:59.950Z Reads: 434

```
[quote="Namasaki, post:8, topic:6457, full:true"]
A fuse is good insurance in case one of your esc's shorts out or you get a short in your wiring.a fuse will save your batteries.You can get regular size ATC/ATO fuses in 40,50 and 60 amp on Amazon
[/quote]
@Namasaki could you help me find the regular size fuses?
All I can find above 40a are the maxi fuses.
Thank you!
```

---
## \#17 Posted by: Jinra Posted at: 2016-09-14T02:00:39.067Z Reads: 440

```
Small blade fuses only go to 40a max. You need to use the fat blade fuses if you want to go larger. I have thought about getting something like this for a more robust, compact fuse

https://www.amazon.com/gp/aw/d/B007WX0NMS/ref=mp_s_a_1_6?ie=UTF8&qid=1473818376&sr=8-6&pi=AC_SX236_SY340_FMwebp_QL65&keywords=fuse+holder
```

---
## \#18 Posted by: Bender Posted at: 2016-09-14T02:12:08.665Z Reads: 442

```
Thanks Jinra
ok, so im not crazy, couldn't find small blade fuses above 40 anywhere. 
I was looking at the ones you pointed out and the mini anl that flatspot mentioned.
Let us know if you try it out.
```

---
## \#19 Posted by: Namasaki Posted at: 2016-09-14T03:15:13.999Z Reads: 444

```
I'm afraid @Jinra is correct, the 50a and 60a fuses that I saw on Amazon where miss identified as regular ATO/ATC fuses.
When I checked closer the size is large like maxi fuses.
https://www.amazon.com/Teal-60A-Standard-Blade-Fuse/dp/B00W8WHLE6/ref=sr_1_2?ie=UTF8&qid=1473822881&sr=8-2&keywords=60a+ATO+fuses
```

---
## \#20 Posted by: Namasaki Posted at: 2016-09-14T03:17:05.279Z Reads: 456

```
If your discharging through a good BMS then you could skip the fuse because BMS should have short protection.
I'm actually not using a fuse.
```

---
## \#21 Posted by: DeathCookies Posted at: 2016-09-14T07:34:53.984Z Reads: 440

```
@Chaka has showed me [this fuse](http://www.littelfuse.com/products/fuses/automotive-passenger-car/high-current-fuses/bf1-58v.aspx#). Only problem will be to solder it on the switch that it does not take that much space....

I still do need a simple car fuse which is rated to 60V....

Many people are using a normal car fuse (it seems so) which is underrated? Is this true?
```

---
## \#22 Posted by: DeathCookies Posted at: 2016-09-14T11:03:01.739Z Reads: 428

```
The best fuse i got so far ( and i will stick to it) was suggested by @elkick
http://de.farnell.com/littelfuse/142-6185-5402/flachsicherung-flink-40a-58v/dp/2508398

I hope this will help everyone. For me it does!
```

---
## \#23 Posted by: Jinra Posted at: 2016-09-14T11:08:29.659Z Reads: 420

```
That's the standard mini blade fuses that only has 40a max. it'd be great to get a fuse of this size in 60A+, but I've never seen them. 

A 40a fuse like this is what caused me to eat it while racing (ie massive acceleration), and cut it out of my pack altogether.
```

---
## \#24 Posted by: DeathCookies Posted at: 2016-09-14T11:15:53.751Z Reads: 409

```
You had the problem that this fuse broke because you pulled to much for too long?

elkick (esk8.de) is selling the vedder switch and none of his costumers reported that this fuse broke. you can pull up to [80a for 5 seconds](http://www.farnell.com/datasheets/2000040.pdf?_ga=1.103693447.60925051.1473251809). I think 80a continous for 5 seconds is really much! I do think too that this fuse is probably the best because you want it to break at some point. Otherwise a fuse is unnecessary ;)
```

---
## \#25 Posted by: DeathCookies Posted at: 2016-09-14T11:27:23.381Z Reads: 390

```
Just to get an idea how much ampere you will pull in real life.
I dont know the setup from @Ackmaniac but the numbers speak for themselves: 

[quote="devin, post:51, topic:9525"]
interestingly with 50% throttle / 40V

5km/h - 65 watts "available" - 1.6 battery amps
10km/h - 370 watts "available" - 9.25 battery amps
15km/h - 545 watts "available" - 13.62 battery amps
20km/h - 687 watts "available" - 17.17 battery amps
25km/h - 835 watts "available" - 20.87 battery amps
30km/h - 985 watts "available" - 24.62 battery amps
35km/h - 1155 watts "available" - 28.87 battery amps
40km/h - 1208 watts "available" - 30.2 battery amps
45km/h - 1154 watts "available" - 28.85 battery amps
49km/h - 909 watts "available" - 22.72 battery amps
[/quote]
```

---
## \#26 Posted by: Jinra Posted at: 2016-09-14T11:31:28.878Z Reads: 369

```
I don't take anything Devin says seriously. And no, i wasn't pulling too much for too long. I was hard accelerating for like 2 seconds after a bit of riding so I'm sure the fuse was already a little warm, and the fuse blew. 40a is too small of a fuse to use imo. 60-80a would be better. A long uphill session can draw more than 40a continuous, especially at lower voltages, and your board may die going up.
```

---
## \#27 Posted by: DeathCookies Posted at: 2016-09-14T11:44:56.496Z Reads: 365

```
Yeah devin is devin :smiley:
but ackmaniac has posted a video of his data logging. So this are real numbers from a vesc!

Could you make a long uphill session and quickly connect a laptop to see how much you have pulled?
```

---
## \#28 Posted by: elkick Posted at: 2016-09-14T11:51:22.116Z Reads: 367

```
[quote="Jinra, post:26, topic:6457"]
especially at lower voltages, and your board may die going up
[/quote]

That's true, for 10s and 12s a 40A fuse is absolutely sufficient, for <8s I'd also go for a higher value. 

I'm even using 40A on the eMTB setup with 2x6374 with 10s and 12s.
```

---
## \#29 Posted by: Jinra Posted at: 2016-09-14T12:00:27.140Z Reads: 352

```
fwiw i rode on dual VESCs 5065 200kv motors and a 10s4p pack with 40 battery max and 50 motor max on both VESCs and rode fine for weeks. I even went up a long and steep hill that made my motors pretty toasty. It was only when i punched it full throttle from slow speeds racing @evoheyax, that i blew the fuse.

@DeathCookies not sure what you mean, his video drew 30a max at 10s
```

---
## \#30 Posted by: DeathCookies Posted at: 2016-09-14T12:33:01.597Z Reads: 347

```
[quote="Jinra, post:29, topic:6457"]
@DeathCookies not sure what you mean, his video drew 30a max at 10s
[/quote]

I wanted to show you that you normally dont pull that much ampere even if you were going up to 50kmh! Thus i do not think we need such a high rated fuse. But i would appreciate if someone proves me wrong with some vesc logging data. :)
```

---
## \#31 Posted by: Bender Posted at: 2016-09-14T12:53:08.662Z Reads: 337

```
[quote="Jinra, post:29, topic:6457"]
fwiw i rode on dual VESCs 5065 200kv motors and a 10s4p pack with 40 battery max and 50 motor max on both VESCs and rode fine for weeks. I even went up a long and steep hill that made my motors pretty toasty. It was only when i punched it full throttle from slow speeds racing @evoheyax, that i blew the fuse
[/quote]

A blown fuse in a real world situation with the relevant data is all the proof I need :grinning:
I'm going 60a
```

---
## \#32 Posted by: DeathCookies Posted at: 2016-09-14T13:00:10.023Z Reads: 330

```
[quote="elkick, post:28, topic:6457"]
I'm even using 40A on the eMTB setup with 2x6374 with 10s and 12s.
[/quote]

40A on each VESC or 20A on each VESC?
```

---
## \#33 Posted by: elkick Posted at: 2016-09-14T13:01:28.566Z Reads: 329

```
Just one fuse within the anti spark switch between batteries and VESCs.
```

---
## \#34 Posted by: Jinra Posted at: 2016-09-14T14:04:00.786Z Reads: 331

```
yea.. I'm still recovering from the scrape that got infected. Worst part is I'm on vacation! I might throw a 60-80a inline fuse later, or just risk it and run fuse-less.
```

---
## \#35 Posted by: devin Posted at: 2016-09-14T14:28:30.479Z Reads: 328

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#36 Posted by: Jinra Posted at: 2016-09-14T14:36:17.540Z Reads: 322

```
I didn't say you were wrong, half the time you post it's wildly off topic and only tries to further your own aimless agenda. If you want to test your theories, get your own VESCs and board and test them, then report back. I'm not even sure what you're trying to do by continuing to spew all these words about motor and battery currents.
```

---
## \#37 Posted by: devin Posted at: 2016-09-14T14:38:00.814Z Reads: 314

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#38 Posted by: Jinra Posted at: 2016-09-14T14:52:38.451Z Reads: 307

```
If you want to talk about your theories, @elkick already proved you wrong about why the bursts of speed happen. It's not because of some asinine reason as "wrong motor/battery current ratio", it was because of the limitations of having 2 shunts.
```

---
## \#39 Posted by: devin Posted at: 2016-09-14T14:56:03.185Z Reads: 308

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#40 Posted by: sash Posted at: 2017-08-16T18:54:38.620Z Reads: 263

```
[quote="Jinra, post:29, topic:6457"]
ESCs 5065 200kv motors and a 10s4p pack with 40 battery max and 50 motor max on both VESCs and rode fine for weeks. I even went up a long and steep hill that made my motors pretty toasty. It was only when i punched it full
[/quote]

Thinking about adding a fuse to my setup.  So what is the final consensus about fuses?    

I have 10S4P battery + 2 VESC-X + dual 6355 190kv motors.  Will 40 amp ATC fuse be enough?   Spacecells use with exact fuses.   But this kind of fuses are rated for 32 Volts, which gives me some doubts about it.   

I am not riding at super crazy speeds (at least for now), but I might need to go uphill occasionally.   I set 20 Amp motors limit in each VESC, so 40 Amp fuse looks like a good match.   But I am worried that voltage rating of ATC fuses is not enough for 10S setup.
```

---
## \#41 Posted by: Jinra Posted at: 2017-08-16T19:02:04.371Z Reads: 258

```
For 10s I'd recommend at least a 60A fuse. Mine blew and got me injured pretty bad. Personally, I don't run a fuse anymore.
```

---
## \#42 Posted by: sash Posted at: 2017-08-16T19:16:57.772Z Reads: 256

```
Thanks, Jinra.  Then I'll keep riding without a fuse.  Later I might add a 60A strip fuse to my XT90S anti-spark key, like discussed here

http://www.electric-skateboard.builders/t/how-to-fused-xt90-s-anti-spark-loop-key/16912
```

---
## \#43 Posted by: sash Posted at: 2017-08-16T19:55:31.266Z Reads: 248

```
Something like this 

https://hc-cargo.co.uk/catalog/p/191187--strip-fuse

or 

https://hc-cargo.co.uk/catalog/p/192319--strip-fuse
```

---
## \#44 Posted by: RiGo Posted at: 2017-10-12T21:04:03.839Z Reads: 224

```
Just adding my question here... I've read through the thread but still not quite sure.

I have a 10s3p battery with 190kv 6355 motors (like the enertion r-spec ones) and I'm running 50A batt max. I've bought a 60A maxi fuse and want to make sure this is enough?

Will hard acceleration from standstill or acceleration uphill spike the current enough to potentially blow a 60A fuse?

Should I be using a 80A fuse?
```

---
## \#45 Posted by: Nordle Posted at: 2017-10-12T21:14:53.201Z Reads: 211

```
nice rhyme
```

---
## \#46 Posted by: MysticalDork Posted at: 2017-10-12T22:08:46.218Z Reads: 203

```
If your battery max is 50, and the pack is good for 60, I'd get a 60a fuse. No use having a fuse that won't trip until the batteries are pushing so much current that they're damaging themselves.
```

---
## \#47 Posted by: RiGo Posted at: 2017-10-13T04:31:14.535Z Reads: 197

```
[quote="MysticalDork, post:46, topic:6457, full:true"]
If your battery max is 50, and the pack is good for 60, I'd get a 60a fuse. No use having a fuse that won't trip until the batteries are pushing so much current that they're damaging themselves.
[/quote]

I'm more worried about current spikes. Will there be spikes that will blow a 60A fuse with my setup?
```

---
## \#48 Posted by: michaelcpg Posted at: 2017-10-13T08:09:22.482Z Reads: 190

```
My previous board (with a 10s3p Space Cell) had a 40A fuse and my VESC battery max was set to 40A and I live in a city surrounded by long, steep hills and the fuse never blew. 

Different fuses will tolerate different periods of time at their rated current before they blow though so there's no real definitive number you can stick to if unless the manufacturer provides this. 

If you're using a 10S3P pack then I definitely wouldn't recommend going any higher than 50A in your settings if you want the battery to have a decent life. A 60A fuse should probably be fine for your settings
```

---
