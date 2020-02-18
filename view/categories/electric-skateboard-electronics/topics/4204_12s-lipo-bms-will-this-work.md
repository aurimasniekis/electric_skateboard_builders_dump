# 12s LiPo BMS: Will this work?

### Replies: 32 Views: 4975

## \#1 Posted by: mason Posted at: 2016-06-03T21:00:11.948Z Reads: 450

```
I'm going to have 4x 5000mah 3s batteries in series for 12s. I want an easy way to charge my board, so I looked into BMS. I'm new so bear with me:
- Will [this](http://www.batterysupports.com/44v-48v-504v-12s-60a-12x-36v-lithium-ion-lipolymer-battery-bms-p-270.html) BMS along with [this](http://www.batterysupports.com/36v-438v-5a-lifepo4-battery-charger-12s-12x-32v-life-charger-p-161.html) power supply be compatible?
- Where do I plug in the power supply?
- Is 60A enough for VESC/170kv motor?
Sorry for the stupid questions
```

---
## \#2 Posted by: Michaelinvegas Posted at: 2016-06-03T21:08:13.322Z Reads: 451

```
Humm...dont they charge and discharge from the same point on the board?
```

---
## \#3 Posted by: Michaelinvegas Posted at: 2016-06-03T21:09:26.618Z Reads: 442

```
I'd hit up the guys that did the battery and bms group by for assistance....

@longhairedboy can you put ur two cents in ?
```

---
## \#4 Posted by: Michaelinvegas Posted at: 2016-06-03T21:18:20.511Z Reads: 430

```
This[quote="barajabali, post:12, topic:4203, full:true"]
Wel I'm using 100amp bms because this is goin on a mountain board which is going to produce higher than average amps. 

I think you can get away with a 60-80 amp bms on a regular board depending if it's dual drive or single. 

And good question about the on off switch. Not sure
[/quote]

 is what @barajabali said in a different thread
```

---
## \#5 Posted by: mason Posted at: 2016-06-03T21:24:16.068Z Reads: 400

```
alright so [this](http://www.batterysupports.com/44v-48v-504v-12s-80a-12x-36v-lithium-ion-lipolymer-battery-bms-p-392.html) bms
```

---
## \#6 Posted by: Jinra Posted at: 2016-06-03T21:42:49.123Z Reads: 391

```
You'll have to do a bit of rewiring
```

---
## \#7 Posted by: mccloed Posted at: 2016-06-03T21:51:56.802Z Reads: 385

```
The charger you listed is for  LiFePo4.
```

---
## \#8 Posted by: Michaelinvegas Posted at: 2016-06-03T22:40:03.377Z Reads: 380

```
As @mccloed said
[quote="mccloed, post:7, topic:4204"]
The charger you listed is for  LiFeP
[/quote]

Gotta be diligent ... All voltage is not equal... They differ between battery chemistry 

Also the amps rating can't be under what flows through the bms...because it will fry the bms 

Like I said gotta hit the guys that are making them now...the info is still fresh in their heads ...lol

I don't want to give you a 👍🏻 because I'm not 100% sure myself ... I've been reading and watching you guys muscle through these dilemmas
```

---
## \#9 Posted by: lox897 Posted at: 2016-06-03T22:42:00.786Z Reads: 351

```
What is the discharge rate on your batteries? If you are going at least 25c then get an 80-100amp BMS so you have more room if you need it. And you should only be charging your batteries at 1c so a 5amp charger will be quickest.
```

---
## \#10 Posted by: Jinra Posted at: 2016-06-03T22:43:01.204Z Reads: 345

```
[quote="Michaelinvegas, post:8, topic:4204"]
Also the amps rating can't be under what flows through the bms...because it will fry the bms
[/quote]

What do you mean by this?
```

---
## \#11 Posted by: lox897 Posted at: 2016-06-03T22:47:35.216Z Reads: 322

```
I think he said it the wrong way around. If your motor is drawing 80 amps and you have a 60 amp BMS then the BMS will cut out. You want a BMS that has the amps you think you will need. 80 amps is the sweet spot IMO and most packs I am going to make will have at least 80amp discharge continuous.
```

---
## \#12 Posted by: Jinra Posted at: 2016-06-03T22:48:22.600Z Reads: 315

```
Just not sure what he meant burning the BMS out. BMS's are there to prevent exactly that.
```

---
## \#13 Posted by: lox897 Posted at: 2016-06-03T22:49:46.762Z Reads: 310

```
I don't think it burns them out. They just cut the power, and if you are going down a hill and there is to many amps, you definitely don't want your power cut.
```

---
## \#14 Posted by: mason Posted at: 2016-06-03T23:08:19.567Z Reads: 302

```
20c

10 characters
```

---
## \#15 Posted by: Michaelinvegas Posted at: 2016-06-03T23:08:48.938Z Reads: 301

```
Ahhhh .... @lox897 to the rescue ... Thanks
```

---
## \#16 Posted by: lox897 Posted at: 2016-06-03T23:10:22.929Z Reads: 301

```
5ah x 20c = 100amp continuous. Get an 100amp BMS.
```

---
## \#17 Posted by: Jinra Posted at: 2016-06-03T23:11:16.674Z Reads: 297

```
I think you mean 100A :P
```

---
## \#18 Posted by: lox897 Posted at: 2016-06-03T23:12:42.867Z Reads: 292

```
Lol. I wasn't even thinking. I'm in bed. My bad.
```

---
## \#19 Posted by: mason Posted at: 2016-06-03T23:38:35.246Z Reads: 301

```
it has 30c burst, so how about [this?](http://www.batterysupports.com/44v-48v-504v-12s-150a-12x36v-lithium-ion-lipolymer-battery-bms-p-394.html)
```

---
## \#20 Posted by: lox897 Posted at: 2016-06-04T00:50:01.080Z Reads: 300

```
100amps should be plenty. You want a bms with the amount your batteries can do continuously.
```

---
## \#21 Posted by: massy Posted at: 2016-06-04T15:47:18.442Z Reads: 293

```
I run a BMS on my 10s LiPO board. Bypassing the BMS while discharging and charging with the BMS. Works like clockwork so far and no worries about maximum discharge. However you don't get the same security while discharging but I measure my batteries regularly and VESC has the voltage drop off so I won't discharge too much.

Also, I don't get all the fuzz about "don't use a BMS with LiPO". It's essentially a balance charger and you also get some security measures while discharging(if you do not bypass it). Can't be worse than running the LiPO's without one at all. If so, I don't see how.
```

---
## \#22 Posted by: longhairedboy Posted at: 2016-06-06T13:04:09.405Z Reads: 285

```
That BMS will work fine, but that charger will not. You need a lithium-ion/lithium polymer charger. This one will do it for you. 

http://www.batterysupports.com/36v-42v-5a-lithium-ion-battery-charger-10s-10x-36v-lion-lipo-p-166.html

@massy yeah i don't get it either. having a BMS and dedicated charger is EXACTLY like having a balance charger. Except the balnacer is in the board and the charger is outside, and all you do is plug it into the wall and go away for a bit instead of babysitting a programmable and finicky piece of equipment that stops every 30 minutes for no reason.
```

---
## \#23 Posted by: lox897 Posted at: 2016-06-06T22:49:51.324Z Reads: 274

```
I thought he wanted a 12s charger? That is a 10S charger. Unless we are talking about someone else.
```

---
## \#24 Posted by: mason Posted at: 2016-07-03T04:26:04.003Z Reads: 248

```
If you were pulling 100a continuous, your battery would die quickly.
```

---
## \#25 Posted by: lox897 Posted at: 2016-07-03T04:34:45.371Z Reads: 240

```
I never said anything about pulling 100 amp continuous... I said 100amp would be plenty.
```

---
## \#26 Posted by: mason Posted at: 2016-07-03T04:43:02.892Z Reads: 236

```
but why say continuous if it's not continuous?
```

---
## \#27 Posted by: lox897 Posted at: 2016-07-03T05:08:54.234Z Reads: 225

```
Well if 20c is what your battery can do continuously and you have 5ah then why not get a 100amp continuous bms? It is highly unlikely you will ever draw 100amps continuously so a 60amp BMS would be fine.
```

---
## \#28 Posted by: lox897 Posted at: 2016-07-03T05:14:40.925Z Reads: 224

```
@link5505 are you Aussie?
```

---
## \#29 Posted by: mason Posted at: 2016-07-03T05:18:50.346Z Reads: 226

```
American. I ended up buying a 60a BMS. I guess it's just my English that makes it confusing
```

---
## \#30 Posted by: mason Posted at: 2016-07-03T05:19:45.270Z Reads: 223

```
Also it didn't seem practical to me to use 20c continuous lol
```

---
## \#31 Posted by: Tusko Posted at: 2016-07-03T05:32:24.577Z Reads: 220

```
Im sorry this sounds EXTREMELY noobish and out of place, But wheres the button to make a new topic or thread :neutral_face: help please...
```

---
## \#32 Posted by: lox897 Posted at: 2016-07-03T05:59:52.686Z Reads: 217

```
On the left hand side. Above the topics. You may not be able to create a thread until you have read for at least 30 minutes and commented on a few topics.
```

---
