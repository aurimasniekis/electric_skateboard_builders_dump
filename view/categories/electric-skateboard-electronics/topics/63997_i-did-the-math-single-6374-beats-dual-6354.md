# I did the math: single 6374 beats dual 6354

### Replies: 55 Views: 1880

## \#1 Posted by: Jmding Posted at: 2018-08-06T05:09:12.228Z Reads: 548

```
Sorry for the clickbait title, but I did the math, and it suggests that single 6374 basically just as powerful as dual 6354s.  Obviously this seems wrong and I'm still pretty new here and learning a ton, but I can't find the mistake and I'd REALLY like to get some feedback.  Let me know what you think.

Comparing a few setups:
1) single 6374, ~200 Kv (lets assume SK3)
2) dual 5045, ~200 Kv (only suitable Kv motor I found were Racestar's, everything else seems to be Kv 500+)
3) dual 90mm hub, ~85 Kv (essential dual 6364 motors, seem to be popular hub motors with brands like Meepo, WowGo, etc)
4) dual 6354, ~200 Kv (several suppliers have these)

At any given time:
Power_in = Power_out - Power_lost

Power_in is basically what your battery and ESC can put out, so something like 36V * 50A ish

A "powerful" motor setup is the one that converts as much of the electrical power from the battery into mechanical power at the wheels as possible, i.e. we need to maximize Power_out

That means we need to minimize Power_lost, which comes from air-resistance, rolling resistance, belt-drag, and copper losses (resistance * current^2).  There's nothing we can do about air-resistance and rolling resistance, so ignore those.  Lets also ignore belt-drag for now since that 3 of the 4 setups use belts, and looking at some manufacturer numbers belt drives should be on the order of 95% efficient anyway.  The only thing left to try to minimize is the copper losses.  So lets estimate the copper losses for each setup, starting with the motors' internal resistances.

1) SK3 6374 has a internal resistance of 0.016 ohm according to HK
2) Estimating the Racestar 5045 200 Kv internal resistance is tricky since its not quoted anywhere.  But we can guess based on the SK3 5045, 450 Kv motor, which has an internal resistance of 0.025 ohm according to HK.  Kv goes down when wire turns go up, and if you increase wire turns you have to use thinner wire, so basically a motor's internal resistance scales as the square of the inverse of Kv.  So roughly speaking, a 200 Kv Sk3 should have an internal resistance of 0.025 ohm * (450 Kv / 200 Kv)^2 = 0.127 ohm, roughly 8x that of the 6374
3) Again we have to estimate the internal resistance of these hub motors, but basing it off of SK3 6364 190 Kv motors gives us an estimate of 0.028 ohm * (190 Kv / 85 Kv)^2 = 0.14 ohm, roughly 9x that of the 6374
4) Estimated internal resistance based on SK3 6354 260Kv motors gives us 0.023 ohm * (260 Kv / 200 Kv)^2 = 0.039 ohm, or roughly 2.5x

1) the single 6374 will suck all of the current from the battery (I_6374), so it's copper losses are I_6374^2 * R_6374, where R is it's internal resistance
2) each motor in a dual 5045 setup will only consume half of the current, and R_5045 = 8 * R_6374, so the total copper losses across both motors is basically 2 * I_5045^2 * R_5045, 2 * (0.5 * I_6374)^2 * 8 * R_6374 = 4 * I_6374^2 * R_6374.  You're losing four times as much power to copper-losses compared to a single 6374
3) 2 * I_hub^2 * R_hub = 4.5 * I_6374^2 * R_6374, 4.5x the power losses
4) 2 * I_6354^2 * R_6354 = 1.25 * I_6374^2 * R_6374, 1.25x the power losses

So basically, single 6374 is within error of equivalent to dual 6354 in power, and 4x more powerful than dual 5045 or dual 90mm hubs.

Durability wise, dual 6354 is better than single 6374 since the heat is easier to dissipate over two separate motors.  And traction is way easier to manage on dual 6354s.  But consider that adding a second 63XX motor costs $20 truck mount + $40 belts and pulleys + $80 motor + $100 VESC = $240, not to mention weight and complexity, it seems to me that budget or light-weight builds should seriously consider the single 6374 as an extremely compelling alternative.
```

---
## \#2 Posted by: Maxid Posted at: 2018-08-06T05:32:20.381Z Reads: 522

```
Read up on belt slippage - case closed.
```

---
## \#3 Posted by: Michaelinvegas Posted at: 2018-08-06T05:37:23.032Z Reads: 523

```
Sure looks complicated...is Esk8 that complicated?
```

---
## \#4 Posted by: Michaelinvegas Posted at: 2018-08-06T05:40:15.019Z Reads: 516

```
Just be dumb like us and use this thing http://calc.esk8.it/ and start building all those decimals are giving me a headache
```

---
## \#5 Posted by: Jmding Posted at: 2018-08-06T05:40:31.611Z Reads: 514

```
Maxid, that's a great point with conventional drivetrains.  If we bump up to 8mm tooth pitch and 15mm belt width though, it wouldn't cost much in weight or $$, and I think it would solve that problem.

Michaelinvegas, haha no it doesnt need to be at all!  But there are plenty of people trying to build light weight or inexpensive boards, who I hope might find this kind of stuff useful.
```

---
## \#6 Posted by: chuttney1 Posted at: 2018-08-06T05:50:12.599Z Reads: 489

```
Here's a paper someone did on eksates for their Master's Thesis from Massey University in New Zealand.

https://mro.massey.ac.nz/bitstream/handle/10179/10977/02_whole.pdf
```

---
## \#7 Posted by: thisguyhere Posted at: 2018-08-06T05:57:22.258Z Reads: 467

```
holy fkn shit, did they get their thesis approved?

210 pages, wow
```

---
## \#8 Posted by: pat.speed Posted at: 2018-08-06T06:00:53.457Z Reads: 457

```
What about in terms of traction? IMO two smaller motors will always beat one bigger motor
```

---
## \#9 Posted by: chuttney1 Posted at: 2018-08-06T06:16:43.070Z Reads: 451

```
[quote="thisguyhere, post:7, topic:63997"]
holy fkn shit, did they get their thesis approved?
[/quote]

Can't be published if it is not approved.
```

---
## \#10 Posted by: Maxid Posted at: 2018-08-06T07:11:14.951Z Reads: 434

```
It's 108 pages - everything past the bibliography is basically unnecessary.
Can't believe people get a masters degree for this type of work in 2016 - "An electric powered skateboard was designed and built for testing and development of an innovative hub motor propulsion system and motor controller."
@jacobbloy should have gotten a PhD then.

PS: Yes I am salty and yes I am still reading this thing.
```

---
## \#11 Posted by: sami Posted at: 2018-08-06T07:26:24.286Z Reads: 413

```
If you can TL;DR it for us that would be awesome
```

---
## \#12 Posted by: Maxid Posted at: 2018-08-06T07:34:33.451Z Reads: 407

```
well he also designed his own motor controller to do FOC tests so the work feels adequate - but he probably could have just used a VESC and do the tests this way. Without the time frame it took to finish the thesis it is hard to judge.
The code comments say 2013 so I am not sure if it took him 3 years to finish (which seems really long for a Masters thesis)
```

---
## \#13 Posted by: dareno Posted at: 2018-08-06T07:38:43.396Z Reads: 398

```
Its not rocket science really it isn't.  Driving both rear wheels is a lot better than driving one.  Stop doing math and build it and ride it and see.
```

---
## \#14 Posted by: PatRocks Posted at: 2018-08-06T08:23:01.327Z Reads: 392

```
I'm gonna agree with the above, you're overthinking the motor efficiency. On the relevant scale of battery capacity in esk8, one motor vs dual motor efficiency is not a "make or break" decision point. I mean, in terms of watt hr/mile (Km, sorry), the range of "x" battery running single vs dual motor is not a deciding factor. 

What _is a deciding factor_ is the cost of another motor and esc, belt, and gears. The feels of a single vs dual are similar, in that they're both an electric-fucking-miracle-vehicle, but in the scope of "EFMV'S", Dual motor is worth the extra money for most of us here at miracle vehicle builders dot forum. 

Back on topic, if you're NOT limited by money, dual drive is going to be a better experience for the rider, and the cost/benefit is only really measurable in dollars or pesos. If you aren't stranded in the desert, don't waste time comparing efficiency, it's about what you want to ride!!!

Tldr: practically speaking, you're gonna use similar amounts of energy either way. Mechanically speaking, dual drive wears out half as fast (and there's other pros&cons) has better brakes and makes your friends precisely 2.25 times more jealous
```

---
## \#15 Posted by: Maxid Posted at: 2018-08-06T08:26:49.408Z Reads: 366

```
[quote="PatRocks, post:14, topic:63997, full:true"]
What _is a deciding factor_ is the cost of another motor and esc, belt, and gears.
[/quote]

Sometimes I feel like that esk8s are still comparatively cheap. I mean even a full blown 4WD Trampa ATB setup for like 3000$ is still "just" the price people pay for their in-car-radio or non-standard car paint. It's crazy...
```

---
## \#16 Posted by: PatRocks Posted at: 2018-08-06T09:18:49.745Z Reads: 345

```
Agreed! If what a human being wants is a means of transportation, it's a "sky's the limit" sort of thing as far as what you can spend. Or you can walk for free. @Jmding you have many things to consider in the long run, and with enough research and cost benefit analysis, you may find exactly what you hope for. My opinion is that overkill is relatively similar in cost to "mediocre" and building for performance is the more rewarding (albeit more expensive) approach. But again, I'm a shameless hardware junkie
```

---
## \#17 Posted by: Okami Posted at: 2018-08-06T11:24:06.714Z Reads: 304

```
I think one of the drawbacks is braking power and acceleration when using only one motor.

If u design a transmission / use differential to drive 2 wheels at once with one motor, then maybe it is a different story but u would probably lose some effienciency in this drive train
```

---
## \#18 Posted by: amazingdave Posted at: 2018-08-06T12:42:23.849Z Reads: 289

```
Grip.... on my single dark matter powered board I have all the power I need for any hill, until it’s rough or damp then I lose all that torque into wheel spin. Same goes with knobs on for braking. 

It wasn’t that big a deal for the first 100 miles but now I hit my max speed every ride for most of the ride and at 30mph the braking with one wheel drive is too sketchy!

Dual 6374 is the way forward! (Why limit yourself to dual 6354!)
```

---
## \#20 Posted by: professor_shartsis Posted at: 2018-08-06T14:27:11.775Z Reads: 286

```
[quote="Jmding, post:1, topic:63997"]
SK3 6374 has a internal resistance of 0.016 ohm according to HK
[/quote]

[quote="Jmding, post:1, topic:63997"]
* Estimated internal resistance based on SK3 6354 260Kv motors gives us 0.023 ohm * (260 Kv / 200 Kv)^2 = 0.039 ohm, or roughly 2.5x
[/quote]

[quote="Jmding, post:1, topic:63997"]
So basically, single 6374 is within error of equivalent to dual 6354 in power, and 4x more powerful than dual 5045 or dual 90mm hubs.
[/quote]

Here's the comparison between (2) 200kv motors with 0.039ohm vs (1) 200kv motor with 0.016ohm...

During acceleration at full throttle, the single motor with lower resistance has higher electrical to mechanical conversion efficiency (green line, top left chart), but half as many pounds of thrust as the dual motor with higher resistance (yellow and green lines, bottom left chart). Ohmic heating per motor is roughly 2.5 times greater with the dual motor with 0.039ohm resistance.

Both systems are assumed to have 50v battery, 200kv, 90mm tire, 2.55:1 gear ratio, 100% throttle, 95% max duty cycle, 60a motor amp limit and 30a battery amp limit.

https://image.ibb.co/gxEhGK/2_vs_1.gif
```

---
## \#21 Posted by: Jmding Posted at: 2018-08-06T15:07:47.650Z Reads: 251

```
Professor, why is that? Single and dual are both consuming the same total current at the same Kt, so shouldn't the torque be the same?
```

---
## \#22 Posted by: professor_shartsis Posted at: 2018-08-06T15:13:39.497Z Reads: 244

```
[quote="Jmding, post:21, topic:63997, full:true"]
Professor, why is that? Single and dual are both consuming the same total current at the same Kt, so shouldn’t the torque be the same?
[/quote]

torque **per motor** is the same with both as seen with blue line, top right chart, but the dual has twice as many motors, so at full throttle during acceleration the thrust in pounds is doubled with the dual setup, as seen with the yellow and green lines, bottom left chart.
```

---
## \#23 Posted by: Jmding Posted at: 2018-08-06T15:15:55.249Z Reads: 234

```
 ah it looks like you’re assuming 2x electrical watts in a dual motor setup. But isn’t the electrical watts capped at your battery system anyway, so single or dual motors, it’s capped at cellCount3.6V30A (unless of course your battery is capable of more than 1x the current draw of the motor, which seems to be rare except in extremely long-range builds)

Said another way, you don't have the current from the battery to actually draw the 2x torque potential of the dual motors
```

---
## \#24 Posted by: professor_shartsis Posted at: 2018-08-06T15:17:12.904Z Reads: 232

```
[quote="Jmding, post:23, topic:63997, full:true"]
Edit: ah it looks like you’re assuming 2x electrical watts in a dual motor setup. But isn’t the electrical watts capped at your battery system anyway, so single or dual motors, it’s capped at cellCount3.6V30A (unless of course your battery is capable of more than 1x the current draw of the motor, which seems to be rare except in extremely long-range builds)
[/quote]

yes with the assumed 60a motor amp limit and 30a battery amp limit settings, above the speed that the battery amp limit is reached, each vesc is drawing 30a battery amps, so total 60a battery amps with the dual setup vs 30a battery amps with the single setup.
```

---
## \#25 Posted by: Jmding Posted at: 2018-08-06T15:18:36.489Z Reads: 220

```
I see, the battery amp limit is quoted per VESC instead of for the battery pack. Isn't the apples to apples comparison then to do 60a battery amp limit in the single motor setup vs 30 for dual?
```

---
## \#26 Posted by: professor_shartsis Posted at: 2018-08-06T15:29:17.151Z Reads: 221

```
[quote="Jmding, post:25, topic:63997"]
Isn’t the apples to apples comparison then to do 60a battery amp limit in the single motor setup vs 30 for dual?
[/quote]

Here's a comparison of the dual setup with 30a battery amp limit per motor vs single setup with lower resistance and 60a battery amp limit per motor...

The dual still has roughly double the thrust throughout most of the acceleration profile because, due to the 60a motor amp limit, you can't draw anything close to 60a battery amps with the single setup throughout most of the acceleration profile as seen with the red line, bottom right chart....

Once you get to about 35mph, thrust is nearly equal with both setups, but still a bit higher with the dual (yellow and green lines, bottom left chart).

https://image.ibb.co/eWMnYz/2_30a_1_60a.gif
```

---
## \#27 Posted by: Jmding Posted at: 2018-08-06T15:56:56.795Z Reads: 204

```
Any chance I could get a copy of the spreadsheet?  I dont understand where the battery amps calculation is coming from.  I would have thought that the maximum current the motor could draw at a given board-speed would be:
motorRPM / (Kv * motorInternalResistance)

which even at 5 mph, for a 200 Kv SK3 motor, 2.55x ish gearing ratio, and 90mm wheels is 380 A
```

---
## \#28 Posted by: Hummie Posted at: 2018-08-06T16:06:16.931Z Reads: 200

```
the esc is going to limit the current likely.  the vesc does maybe 100 battery amps max.  but of course the motor amps max is what would be more relevant and it's about the same max  
the two motors will ultimately have more max torque potential (unless the one is as big as the two) because they have more iron and will therefore be able to produce a greater magnetic field and torque without magnetic saturation.
```

---
## \#29 Posted by: professor_shartsis Posted at: 2018-08-06T16:14:23.929Z Reads: 207

```
[quote="Jmding, post:27, topic:63997"]
I dont understand where the battery amps calculation is coming from.
[/quote]

Here are some of the equations used in the spreadsheet... the example values are from a separate thread. The motor and battery currents are limited below what the motor is physically capable of by software settings in the ESC, which vary depending on user preference and software limits imposed by the various ESC manufacturers.


[quote="professor_shartsis, post:1082, topic:25251"]
here’s all the formulas used (and verified)…

let’s take 50v @ 20mph from the graph (30a battery limit &amp; 60a motor limit, 0.07ohm winding)

20mph @ 83mm diameter = **2057.30454rpm**

2057.30454rpm / 85kv = **24.20358v back emf**

50v * %55.91814 duty = **27.95907v effective voltage**

((27.95907v effective voltage) - 24.20358v back emf) / 0.07ohm = **53.64984a motor current**

27.95907v effective voltage * 53.64984a motor current = **1500w electrical watts**

1500w electrical watts / 50v battery = **30a battery current**

(53.64984a motor current)^2 * 0.07ohm = **201.48142w ohmic heating &amp; copper loss**

(2057.30454rpm * 2 * pi) / 60 = **215.440427 rad/sec angular velocity**

60 / (2 * pi * 85kv) = **0.11234 newton meter torque per motor amp**

0.11234 newton meter torque per motor amp * 53.64984a motor current = **6.02702 newton meter torque**

6.02702 newton meter torque * 215.440427 rad/sec angular velocity = **1298.46376w mechanical watts**

1298.46376w mechanical watts / 1500w electrical watts = **%86.564 electrical to mechanical conversion efficiency**

1298.46376w mechanical watts + 201.48142w ohmic heating &amp; copper loss = **1500w electrical watts**
[/quote]
```

---
## \#30 Posted by: Michael319 Posted at: 2018-08-06T16:16:56.034Z Reads: 183

```
But idlers can prevent that...
```

---
## \#31 Posted by: b264 Posted at: 2018-08-06T18:32:21.882Z Reads: 181

```
Everyone here is talking about electrical losses and math when the real reason I like dual drive is because you have TWO WHEELs in traction with the ground and no torquesteer/skidding when you smash the brakes.  The electrical efficiency is irrelevant to me.

Also when you have a tail, if the front wheels are off the ground, you basically can't use the accelerator/brake until you put the front wheels back down -- UNLESS you have dual drive
```

---
## \#32 Posted by: Battosaii Posted at: 2018-08-06T18:57:20.392Z Reads: 175

```
Redundancy is important on a dual set up if you loose a belt then one slowing you down is better than none.
```

---
## \#33 Posted by: Michaelinvegas Posted at: 2018-08-07T01:16:27.954Z Reads: 165

```
[quote="Maxid, post:10, topic:63997"]
@jacobbloy should have gotten a PhD then.
[/quote]

I guess only the OGs can appreciate this burn hahahha
```

---
## \#34 Posted by: Mikenopolis Posted at: 2018-08-07T01:32:51.814Z Reads: 161

```
Do you think a PhD that would help Jacob balance his audio levels? His tutorials were a nightmare when I started building (with a sleeping infant in the next room)
```

---
## \#35 Posted by: Jmding Posted at: 2018-08-07T01:38:23.109Z Reads: 160

```
Prof, sorry I dont follow. Specifically, where is this 56% duty cycle coming from?  Do you have an article explaining the fundamentals that I could read over?  

[quote="professor_shartsis, post:29, topic:63997"]
%55.91814 duty
[/quote]

I thought that duty * battery_voltage * kv = motor rpm, but I must be wrong there
```

---
## \#36 Posted by: professor_shartsis Posted at: 2018-08-07T04:33:39.837Z Reads: 161

```
[quote="Jmding, post:35, topic:63997"]
Prof, sorry I dont follow. Specifically, where is this 56% duty cycle coming from?
[/quote]

Sure, In this example, we already know the Pack Voltage ( A ), Back EMF Voltage ( D ), Winding Resistance ( E ) & Electrical Watts ( G ).

A = 50 = Pack Voltage
B = X.XXX = %Duty Cycle
C = X.XXX = Effective Voltage
D = 24.20358 = Back EMF Voltage
E = 0.07 = Winding Resistance Ohms
F = X.XXX = Motor Current Amps
G = 1500 = Electrical Watts (30a battery amps @ 50V)

We seek to determine the Duty Cycle % ( B ), Effective Voltage ( C ), and Motor Current Amps ( F ).

We need to combine & rearrange these equations to solve for the missing variables ( B ), ( C ) & ( F ):

A * B = C
(C - D) / E = F
C * F = G

------------------------

Step 1: Combine the equations... we already know the values of all variables except Duty Cycle ( B )

(A * B) * (((A * B) - D) / E) = G

------------------------

Step 2: Rearrange the equation to solve for B:

B = (sqrt(D^2+(4 * G * E)) + D) / (2 * A)

https://image.ibb.co/id8N0e/B.jpg

------------------------

Step 3: Now that we know B, solve for C:

A * B = C

------------------------

Step 4: Now that we know C, solve for F:

(C - D) / E = F

------------------------

Final Values:

A = 50 = Pack Voltage
B = 0.5591813 = %55.91813 = %Duty Cycle
C = 27.95909 = Effective Voltage
D = 24.20358 = Back EMF Voltage
E = 0.07 = Winding Resistance Ohms
F = 53.64978 = Motor Current Amps
G = 1500 = Electrical Watts (30a battery amps @ 50V)
```

---
## \#37 Posted by: Jmding Posted at: 2018-08-07T05:16:08.727Z Reads: 141

```
Interesting. What is confusing me is, what happens to the 30a that the battery is supplying, that doesn't go through the motor. I'm going to have to think about this for a while, but thank you for pointing me in the right direction.
```

---
## \#38 Posted by: professor_shartsis Posted at: 2018-08-07T05:21:54.664Z Reads: 145

```
[quote="Jmding, post:37, topic:63997"]
what happens to the 30a that the battery is supplying
[/quote]


the battery is actually discharging a series of avg 53.64978a pulses (55.91813% of the time) at a frequency on the order of 20,000-30,000 cycles per second which averages to 30a.

53.64978a * 0.5591813 = 30a
```

---
## \#39 Posted by: Jmding Posted at: 2018-08-07T05:25:26.937Z Reads: 143

```
Gotcha, and for some reason "effective current" is not duty cycle * peak current, the way "effective voltage" is? That's not intuitive to me, but I guess that is the only way the math works
```

---
## \#40 Posted by: dareno Posted at: 2018-08-07T05:27:38.825Z Reads: 146

```
[quote="b264, post:31, topic:63997"]
Everyone here is talking about electrical losses and math when the real reason I like dual drive is because you have TWO WHEELs in traction with the ground and no torquesteer/skidding when you smash the brakes. The electrical efficiency is irrelevant to me.
[/quote]

Thankyou for some real world sense!  calculate all you like but when you ride the bloody thing you will know!!!
```

---
## \#41 Posted by: Jmding Posted at: 2018-08-07T05:31:57.141Z Reads: 138

```
Yeah, it's time for me to build and ride one to see what you guys mean, torque steer and traction could be deal killers
```

---
## \#42 Posted by: b264 Posted at: 2018-08-07T05:36:29.136Z Reads: 135

```
To be clear, *I love me a 6374 single-drive too*.

But I was saying that electrical efficiency or battery range is not why I like dual so much better.  **It's because now you have two wheels biting the ground instead of one wheel.**  Also redundancy -- if you have a failure with two independent drivetrains you probably still have braking ability and can probably still get home without pushing or crashing.  *(It's of-note here that most dual builds are not two independent drivetrains)*

single 5065 < single 6355 < single 6374 < dual 5065 < dual 6355 < dual 6374

So yea, I'd rather have dual 5065 than single 6374 even if it's less power
```

---
## \#43 Posted by: Jmding Posted at: 2018-08-07T05:40:37.384Z Reads: 134

```
Yeah the two points of traction thing is undeniably valid. Wondering if the ugly but light weight solution though would be to use a wider driven wheel (flywheels seem to be very narrow by modern standards) with a larger contact patch... Redundancy is a good point too, but I feel that if you know how to foot break (which every e skate rider probably ought to learn), and otherwise design for reliability, it might not be so crazy to trade the redundancy for weight.
```

---
## \#44 Posted by: b264 Posted at: 2018-08-07T05:47:17.581Z Reads: 137

```
It also has a lot to do with what your priorities are and *if you want a toy or a tool*.

Some folks might want to optimize for **range** while others want to optimize for **weight** while others want to optimize for **reliability** and yet others might want to optimize for **performance** and yet others might want to optimize for **compact size** and still yet others might want to optimize for **cost**.  Those folks might pick single 6374, single 5065, dual 6355, dual 6374, dual 5065, and single 6355, respectively.  They all have their merits.  I'm in the third group: reliability.
```

---
## \#45 Posted by: dareno Posted at: 2018-08-07T07:43:54.639Z Reads: 134

```
[quote="Jmding, post:43, topic:63997"]
but I feel that if you know how to foot break
[/quote]

well that is a good point right there 
Skills that are necessary on analog boards are still necessary on esk8.  More so I would imagine with the speeds some of these builds achieve.  Hand slides, hard carve slides are all very good ways of saving your ass but for those of us that are getting a bit long in the tooth for extreme manoeuvres the foot brake is awesome.
```

---
## \#46 Posted by: dareno Posted at: 2018-08-07T08:07:43.502Z Reads: 143

```
[quote="b264, post:42, topic:63997"]
*(It’s of-note here that most dual builds are not two independent drivetrains)*
[/quote]

This is the second time a term of yours has me questioning and for that I thank you
first was "drinking the koolaid" (for that guy who did the ios app) and please put me out of my misery for that one.
and now this.  Please elaborate on the dual drive-train thing.
```

---
## \#47 Posted by: topcloud Posted at: 2018-08-07T13:24:47.838Z Reads: 138

```
https://youtu.be/jzRvT3fHtVA

here's the newest single-motor on the planet - with a gear drive.

Of course, the single gear drive completely fixes the belt slippage issue.

Check out the review.  End-product works exactly as predicted.
```

---
## \#48 Posted by: b264 Posted at: 2018-08-07T18:29:56.384Z Reads: 131

```
[quote="b264, post:42, topic:63997"]
two independent drivetrains
[/quote]

@dareno I'm referring to a system where the only connection between the left and right wheels is the battery.  There are 2 separate radio receivers paired to the same remote and no "split PPM" or "CANBUS" connection between them, so that one ESC can fail and not cause a failure in the other one.   I suppose you could even use 2 separate batteries, but I haven't yet seen that done in practice.
```

---
## \#49 Posted by: b264 Posted at: 2018-08-07T18:30:43.766Z Reads: 133

```
@topcloud Gear drive is not direct drive.  Direct drive is hub motors (radial direct drive) or Carvon-style (axial direct drive)

Some manufacturers might try to say otherwise for marketing purposes, but a quick internet search clears everything up.
```

---
## \#50 Posted by: Deckoz Posted at: 2018-08-07T20:26:25.367Z Reads: 131

```
Tl:Dr

Your topic title is wrong. Forget costs

Dual anything > single anything in anyway you put it except cost. And if you say otherwise, it's just a matter of how the board is setup.

Efficiency, power, braking. Dual can and will always win, it's just a matter of how it's configured.
```

---
## \#51 Posted by: Hummie Posted at: 2018-08-08T16:08:08.575Z Reads: 113

```
and you can use the traction control on the vesc with the two which is really nice.  amazing and never slips in the wetness or when you unweight a wheel around a sharp turn.

I bet the two is more efficient too even with the drivetrain loss.
```

---
## \#52 Posted by: longhairedboy Posted at: 2018-08-08T16:19:35.018Z Reads: 115

```
[quote="dareno, post:13, topic:63997, full:true"]
Its not rocket science really it isn’t. Driving both rear wheels is a lot better than driving one. Stop doing math and build it and ride it and see.
[/quote]

LOL! That was my gut reaction too. 

Theory and papers often go right out the window when actual street testing happens.
```

---
## \#53 Posted by: longhairedboy Posted at: 2018-08-08T16:21:43.582Z Reads: 116

```
[quote="topcloud, post:47, topic:63997, full:true"]
here’s the newest single-motor on the planet - with a gear drive.

Of course, the single gear drive completely fixes the belt slippage issue.

Check out the review. End-product works exactly as predicted.
[/quote]

wait till you see their new single drive... with a 5095. No, that's not a typo. We're going to be doing some AB customer upgrades soon, swapping out their old drives for the new ones.
```

---
## \#54 Posted by: longhairedboy Posted at: 2018-08-08T16:23:11.925Z Reads: 117

```
[quote="Hummie, post:51, topic:63997"]
I bet the two is more efficient too even with the drivetrain loss.
[/quote]

less heat, more load distribution... the long term benefits are better as well.
```

---
## \#55 Posted by: professor_shartsis Posted at: 2018-08-09T02:20:15.127Z Reads: 108

```
he specified the dual system motors had about 2.5 times as much electrical resistance as the single motor...

so the single had lower thrust, but it also had greater electrical to mechanical conversion efficiency during full throttle acceleration (green line, top left chart).

https://image.ibb.co/eWMnYz/2_30a_1_60a.gif
```

---
## \#56 Posted by: Virol Posted at: 2019-01-14T21:54:27.311Z Reads: 66

```
That's what happend in any experiment, first you go like "perfect, got great result, and numbers match" then when you take it to practice everythinkg goes Hiroshima XD
```

---
