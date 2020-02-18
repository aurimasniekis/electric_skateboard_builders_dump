# Motor discussion. Are 6374&rsquo;s worth it?

### Replies: 128 Views: 3293

## \#1 Posted by: ctincristy Posted at: 2018-09-10T04:49:16.343Z Reads: 534

```
I had a discussion with the guys from the Skatemetric youtube channel and I am starting to think that most dual 6374 builds are severely bottlenecked and just wasted money (don't get triggered yet)...

There are a few comparisons between dual 6355 vs dual 6374 (or 5065), but all of them are basically useless since they use either different battery configurations or different kv motors, even different gearing, so they are always biased (and stupid).

The battery is the bottleneck usually, so you might have to go lipo or multiple li-ion packs in parallel.

Larger motors, even though they use more battery for doing the same task, might be more efficient for long distance cruising because of the heat dissipation. Lower heat also means lower resistance which makes it more efficient. Hot motors have high resistance and eat more battery than cool ones.

I thought about it again: larger motors can be more powerful (listed W). Torque does not mean everything, a more powerful motor will move a bigger mass more easily. That is **IF ONLY** the battery can keep up with it. 

The question is what would be the difference between motor performance if they have the same specs all around, besides dimensions and power, while being constrained by the battery (which is the case for most boards).

A 12s4p samsung 30q battery can only supply 3.6V * 12 * 4 * 15A = 2592W at 43.2V.
6374 motors are rated for over 3000W, multiply that by two for a dual setup.
Result: you have a crazy bottleneck caused by the battery. I assume 90% of eboarders don't have more than 50 cell batteries.

Makes you question if it's worth getting a 6374 setup that will have the same actual power as a 5055 setup﻿.

Can someone shine some light on me and tell me what the actual benefit of a 6374 setup is in a build like the one above?
```

---
## \#2 Posted by: Skunk Posted at: 2018-09-10T04:56:48.312Z Reads: 511

```
Following this discussion.
I don't know but I want to
```

---
## \#3 Posted by: Andy87 Posted at: 2018-09-10T04:58:11.276Z Reads: 508

```
[quote="ctincristy, post:1, topic:67569"]
Torque does not mean everything
[/quote]

Torque IS everything if you on a mtb...😅

I stated this calculation before also.
The thing is, that a lot of guys here wanna go bigger and bigger but for the most they can’t even reach out the max performance of there Motor as they restricted by the battery or the vesc.

Besides this I would say a 63xx is still a good choice. You get better breaks and better heat dissipation.

Edit: I would step up your calculation...
The 30q can handle 20a so 80a total
And I wouldn‘t take the nominal voltage here as you look for the max values 
So now we here:
12 x 4,2 x 80 = 4032W
That would be 2000w for each motor in dual
```

---
## \#4 Posted by: b264 Posted at: 2018-09-10T05:20:45.080Z Reads: 498

```
Let's be straight for a moment -- a single 5065 is *enough* for an esk8.  It will move you and keep you moving.  Many commercial boards use it.  I've done it before across town, no problems at all.  But the performance is **very** underwhelming, to say the least.  Especially if you've ridden anything else, ever.

single 5065 - adequate, but crappy
single 6355 - it works
single 6374 - minimum imho for a "good" build.  perfectly fine
dual 5065 - now that's much, much better omg :heart: 
dual 6355 - I think I have rocket skates
dual 6374 - I think I have rocket skates, but they don't get quite as hot and they're heavier
dual 6384 - I think I have rocket skates, but they don't get quite as hot and they're even heavier

So my answer is "not really but maybe sometimes, depending"

For a normal polyurethane-wheeled street esk8, dual 6355 is ***plenty*** to give you that Nascar feeling and is lighter and fits on trucks better than dual 6374 or 6384.

.

**TL;DR**: use dual 6355. saves weight. fits better. fast as balls.
```

---
## \#5 Posted by: Mikenopolis Posted at: 2018-09-10T05:25:27.078Z Reads: 481

```
Good summary. 

I have dual 6355 on just 10s3p 25r and they are plenty for me. The dual 6374 is just becuase I wanted wider trucks for stability (becuase I still suck at higher speeds). The 74s just looks better on wide trucks
```

---
## \#6 Posted by: b264 Posted at: 2018-09-10T05:31:04.294Z Reads: 475

```
[quote="Mikenopolis, post:5, topic:67569"]
The 74s just looks better on wide trucks
[/quote]

The x74s do indeed look better on wide trucks.  But overall, narrow trucks look even better than that :stuck_out_tongue:

Though I do like the wide ones
```

---
## \#7 Posted by: deucesdown Posted at: 2018-09-10T05:47:38.386Z Reads: 464

```
Hey so has anyone pulled much more than 1000w with a 6355 or 6374 190kv on 10s? Urethane wheels, around 15/36 gearing?

I've got a 12s2p a123 pack, and got ahold of a vtc4 10s4p, both on dual 6355 190kv with 50a batt max per vesc. Can't seem to pull more than 70a from either setup. About 1kw per motor. Both these packs should be able to at least show me 120a.

I also tried dual 6374 on a r2 pack (30q 10s4p) with similar power numbers in vesc. This one's 107mm wheels with I think 16/36.

Theoretically I should be able to pull more than 70a from the packs. Am I hitting the 42v bottleneck? I thought the 6374 would pull more out of the pack.
```

---
## \#8 Posted by: dareno Posted at: 2018-09-10T05:49:56.033Z Reads: 455

```
[quote="b264, post:4, topic:67569"]
So my answer is “not really but maybe sometimes, depending”
[/quote]

you changing careers?  with the current state of us politics I'm thinking with that comment you should run.
:stuck_out_tongue_winking_eye:
```

---
## \#9 Posted by: Jmding Posted at: 2018-09-10T05:59:22.928Z Reads: 455

```
I watched that video too. Also notable, they mentioned that the thing is geared to 50 mph, so if you ran a single 6374 instead, and geared down to 25 mph max, you would actually have the same torque they achieve. In their case, traction is the main bottleneck, and they really should have picked larger contact patch wheels to manage that torque. Venom Cannibals would be awesome. 

Assuming you gear to the same top speed, the only thing that matters for torque is max continuous current. 5045 200 kv motors are typically 30A max. 6374 200 kv is 80A max. So a single 6374 is capable of 33 percent more torque than dual 5045.

How much current do you need? Well, you can calculate the torque you need to accelerate up a given hill at a given weight, and convert that back to current based on Kt. I ran the numbers for my use case, and found that for my 12s setup, my gear ratio, body weight and terrain, I need about 60A capability. Dual 5045 would work barely, solo 6354 would work, hub motors would not, dual 6354 is way overkill.

Another interesting point from those videos, they mention the boosted lacks top end torque, but do very well down low. I think that is direct evidence that their bottleneck is battery current. Their dual 5045 setup can draw 65A from the batteries easily at low speeds/duty cycles, but closet to top speed, the a123 lifepo 12s1p setup they run, likely at a max battery current of around 40A, cannot supply enough current to fully utilize the capability of the motors.

I think a very sensible setup overall is dual 5045, and 12s3p vtc5a. Max motor current of 65A or so, and max battery current of 75A or so. Very well matched, and should be PLENTY torquey to hill climb most riders while still reaching 25 mph
```

---
## \#10 Posted by: anorak234 Posted at: 2018-09-10T06:08:34.237Z Reads: 423

```
Here’s the thing though - you get to *say* that you have dual 6374s. That’s enough to make jaws drop on boosted riders faces, which will make me happy enough to be worth it aside from the awesome torque.
```

---
## \#11 Posted by: Jmding Posted at: 2018-09-10T06:23:10.206Z Reads: 409

```
Lol fair point, more than 5x the torque is a pretty impressive stat
```

---
## \#12 Posted by: Nate Posted at: 2018-09-10T07:26:15.383Z Reads: 402

```
Then what does dual 80xx motors make?
```

---
## \#13 Posted by: ElectricCoast Posted at: 2018-09-10T07:38:03.026Z Reads: 389

```
It makes ladies throw their panties at you!
```

---
## \#14 Posted by: ivanflo Posted at: 2018-09-10T07:48:05.691Z Reads: 391

```
I've just wrapped up on my first build [The eLFF](https://www.electric-skateboard.builders/t/ellf-long-low-flexy-loaded-dervish-or-tan-tien-caliber-10-inch-dual-drive-mounting-method-10s1p-dual-focbox/40006), with dual 6374 TB motors on a flexible loaded board at stock drop thru height. That torque kick is absolutely amazing. It's like any good turbo car, no one ever wants to turn the boost down.
```

---
## \#15 Posted by: taz Posted at: 2018-09-10T08:03:36.498Z Reads: 398

```
IMO dual 6355 coupled with a 12s5p are more than enough as far as power is concerned 
That said I am thinking about switching to dual 6374 in the future.
Why may you ask? 
I live in Greece and it can get hot during the summer, this combined with some serious hills I have to climb during my commute has led to overheating the motors above 80C and leaving me without brakes. I weigh 77kg +backpack (ca. 10kg).
Here is a typical ride, check the motor temperatures near the end.

https://metr.at/r/qnbg0

So if you do not have overheating problems I see no reason to go for anything bigger.
If you are a heavy guy, live in a hot climate and have serious hills where you ride then bigger motors may be required.
```

---
## \#16 Posted by: ARetardedPillow Posted at: 2018-09-10T08:04:01.102Z Reads: 386

```
I've ridden many setups of motors before, single 6374, dual 6374, single 6355, dual 6355, and dual 5055, and as from I experienced anything less than dual 6374 doesn't really satisfy me, heck even dual 6374 on 10s are pretty meh.

And more motors = more boosted guys dropping their jaw, and it also makes it easier to do the "Hey I'm just cruising, and I see a bunch of people on the sidewalk. Time to impress them by passing them slowly and then full throttle to go flying"
```

---
## \#17 Posted by: brenternet Posted at: 2018-09-10T08:30:09.563Z Reads: 385

```
All the math aside, just riding them you can tell the difference.
```

---
## \#18 Posted by: 12meterkuk Posted at: 2018-09-10T08:35:59.220Z Reads: 381

```
It does also depend on the motor, let’s say you have a motor with 28 stator teeth compared to 14, it’ll have more torque off the line. Bigger motors do actually help at high speeds. The raptor 2 is also limited to 40 battery amps total in the firmware but it kicks like a mule even at high speeds.
```

---
## \#19 Posted by: Spatt Posted at: 2018-09-10T08:44:54.711Z Reads: 381

```
Urethane just gripped board—-> dual 6355 it’s the perfect combo!
Pneumatics gripped board daily commute—-> dual 6355 
Mtb with bindings—> 6374 and tons of amps and torque
```

---
## \#20 Posted by: Jc06505n Posted at: 2018-09-10T08:45:01.404Z Reads: 386

```
Relevant Topic:


https://www.electric-skateboard.builders/t/whats-the-difference-in-performance-between-dual-a-6374-and-dual-6355/25902




Btw is it possible for the forum to have a bot that links relevant topics / questions ?
```

---
## \#22 Posted by: brenternet Posted at: 2018-09-10T09:07:52.776Z Reads: 362

```
That's our job as forum police. If you like we can all say "beep boop" after we dish out knowledge to the plebeians.
```

---
## \#23 Posted by: Blitz Posted at: 2018-09-10T09:30:40.693Z Reads: 354

```
Why does nobody mention 6364 motors?
Could that be the sweet spot for dual?
```

---
## \#24 Posted by: Cobber Posted at: 2018-09-10T10:18:33.734Z Reads: 358

```
I'm sure it is not all, but I have seen some pull down pictures of 6364 motors here on the forum and the stator length was the same as 6355 :(
```

---
## \#25 Posted by: 12meterkuk Posted at: 2018-09-10T16:31:42.716Z Reads: 363

```
It depends on the motor. I don’t know about elsewhere but in China there’s a letter in front of the motor size N and C. N motors have longer stators compared to C. So for example a N5055 has the same stator size as a C5065![image|620x465](upload://jtr8zSndGBkqSOHCPqJT3nEETZ6.jpeg)![image|620x465](upload://9otkzDNOpgXQ5pQGxJ06RsbxFVy.jpeg)
```

---
## \#26 Posted by: b264 Posted at: 2018-09-10T16:59:10.522Z Reads: 354

```
[quote="Jc06505n, post:20, topic:67569"]
Btw is it possible for the forum to have a bot that links relevant topics / questions ?
[/quote]

Yep, the forum is run by the open-source software called [discourse](https://github.com/discourse/discourse) and is written in Ruby.  Feel free to write a plugin ;-)  Then feel free to ask @onloop to use it :slight_smile:
```

---
## \#27 Posted by: moon Posted at: 2018-09-10T17:00:10.163Z Reads: 349

```
Second part is the hardest part out of the two
```

---
## \#28 Posted by: psychotiller Posted at: 2018-09-10T17:05:38.618Z Reads: 355

```
Not true. The stator on Maytechs 6365 is closer to the 74 length than the 55. And the kv produces more torque.
```

---
## \#29 Posted by: Deckoz Posted at: 2018-09-10T18:06:39.456Z Reads: 361

```
If I could fit 8074 or 8084s I would.

Forget about power in torque, and just think about copper and resistance.

Big motors, small heat. Bigger the motor the better. I love all that my Evo is, it is tuned perfect and will never overheat.... Except the motors, I need more Copper and Iron. 

So I guess, are 6374 worth it? Sure, but I need bigger. I'm 132lbs and can heat soak a motor really easily. Some could say my motor amps are to high, and I'd say, your acceleration is to low. Solution = bigger motors. 

If I'm this light, and see issues, I can't imagine(actually already know) what the 200lb guys are going through. I've pretty much made it to the point where the stuff in the enclosures are tuned perfect, cool batteries, extra aluminum mass for focboxes, no antispark to fail, waterproofed enclosure, and water proof charge connections. The electrical "system" on the decks are perfect, the drive system setup for the wheels, whether gears or belts etc, setup perfect, but the motors being the failure point. 

If anything needs innovation it is the motors. I want to see 0.15 or smaller laminations, n52sh curved magnets, lower guage solid core windings, and maybe some heat pipes.

Maybe a diffuser/shroud in front of the center of the motors, So that turbulent air coming off of the board and under the deck hit the motor mount side of the motors(high pressure) and the middle behind the diffuser/shroud is low pressure so the motors actually pull air through them. Especially if a fan design like sk3 is used. 

/End random thoughts
```

---
## \#30 Posted by: Skunk Posted at: 2018-09-10T20:20:22.140Z Reads: 343

```
[quote="Deckoz, post:29, topic:67569"]
I can’t imagine(actually already know) what the 200lb guys are going through.
[/quote]

And this is why I picked 6374s for my first build, and I'm shooting for 6369s for my "light" commuter board.
```

---
## \#31 Posted by: b264 Posted at: 2018-09-10T20:28:38.869Z Reads: 341

```
How about a 210 lb guy with 40 lbs of groceries LoLz

even dual 5065 is perfectly adequate but dual 6355 or dual 6374 is obviously more fun
```

---
## \#32 Posted by: Skunk Posted at: 2018-09-10T20:41:28.732Z Reads: 341

```
[quote="b264, post:31, topic:67569"]
How about a 210 lb guy with 40 lbs of groceries and a 12 pound "dog"
[/quote]

Fixed :rofl:
```

---
## \#33 Posted by: b264 Posted at: 2018-09-10T20:44:25.289Z Reads: 331

```
LoL never groceries and dog at same time :rofl:
```

---
## \#34 Posted by: taz Posted at: 2018-09-10T20:47:20.400Z Reads: 329

```
I am a lot lighter than you and don't really push it while commuting (it's a different story if I ride for fun) yet overheat dual 6355 all the time. Take a look at the metr log I posted above.
Maybe where you live is a lot colder or has no hills.
```

---
## \#35 Posted by: danielz Posted at: 2018-09-10T21:37:15.934Z Reads: 331

```
For some builds yes, i pull over 60a per vesc regularly, (120a + total) at thats at 12s! I use 6:1 ratio and Im on pneumatics so I need all the power i can get for the initial launch. I got by on one motor for a few weeks, but it wasnt nearly as fun, all i care about is acceleration, for 95% on the ride im no where near that amperage.
```

---
## \#36 Posted by: b264 Posted at: 2018-09-10T21:57:18.306Z Reads: 326

```
I live downtown so it's mostly flat but a few hills around, some big.  Typically I'm not going that way, though
```

---
## \#37 Posted by: Jmding Posted at: 2018-09-10T22:58:11.077Z Reads: 327

```
I think you should consider swapping the dual 5065 to 6354.  6354s are actually lighter, capable of *slightly* more current than 5065s, and fit more easily narrower trucks (which should be lighter and less likely to bend)
```

---
## \#38 Posted by: Pedrodemio Posted at: 2018-09-11T01:10:40.659Z Reads: 323

```
I've run single 5065, single 6355 and dual 5055, the latter is obviously the most fun, I don't go fast, limited to 35km/h, but the little ones handle it all, they get hot but not uncomfortable, can hold them in my hand all day long

To this day haven't found a hill they could't climb with 40A each and 34:14 gearing and 80mm wheels, I think 20% was the steepest so far

Two(three) buts:

1: I'm severely limited on battery amps, 30A, so the motors stay most of the time far away from the 40A limit

2: If I geared them for greater top speed I can see them getting too hot on bug hills

3: they are lighter than a dual 6355, and since my goal was to go crazy on weight reduction they are perfect
```

---
## \#39 Posted by: xilw3r Posted at: 2018-09-11T13:20:40.585Z Reads: 314

```
You should keep in mind that what the motors are "rated for" is really just a load of bullshit. Try running a 6374 motor at 3kw and tell me how long it lasts before the magnets are overheated or the phases short out due to molten enamel. I think most 6374 are really rated for 2kw at peak. and thats optimistic. Look at lets say industrial motors that are rated for at least 1kw, the size is the thing you should take note of.

@Andy87 when calculating that peak power output you can not use 4.2V per cell, it will always drop to at least 3.9 (for example with 30q or vtc6 at 15A drain per cell, for 20 it goes even lower)

I find the single 6374 with 1:5 reduction still lacking in torque on 225mm wheels, which is kinda crazy since on wet pavement I am struggling to not do a burnout on low speed, but on good dry asphalt I would want more acceleration :). With a regular longboard its probably insane.
```

---
## \#40 Posted by: Pedrodemio Posted at: 2018-09-11T13:54:51.885Z Reads: 318

```
Just complementing, power doesn’t matter, what matter is current

There is a point you run into saturation in the core and any more current is turned to heat without increasing torque

@Deckoz have you trying lowering the motor current in small increments to see if there is any loss in performance and if the temperature drops? If you really are hitting these high currents for any significant amount of time I bet the motors are saturating, but since you ride at high speed and the battery current is way lower than the motors it could be just a high average current and the only way as you said is bigger motors
```

---
## \#41 Posted by: professor_shartsis Posted at: 2018-09-11T14:57:47.361Z Reads: 330

```
[quote="ctincristy, post:1, topic:67569"]
The question is what would be the **difference between motor performance if they have the same specs all around, besides dimensions and power**, while being constrained by the battery (which is the case for most boards).
[/quote]

here's some info from a different thread:

[quote="professor_shartsis, post:5, topic:64160"]
here’s what happens **when you double the resistance with the same KV** during full throttle acceleration…

**efficiency goes down** (green line, top left chart), **ohmic motor heating doubles** (90w -&gt; 180w), **battery amps increase** (black line, bottom right chart), **acceleration remains identical, top speed is nearly identical**.

(50v battery, 0.025ohm vs 0.050ohm, 100kv, 100mm tires, 1:1 gearing, 100% throttle, %95 max duty cycle, 60a motor current limit, 60a battery current limit per motor)
[/quote]

https://image.ibb.co/gAWwFp/0_025_vs_0_050.gif
```

---
## \#42 Posted by: Deckoz Posted at: 2018-09-11T15:23:26.059Z Reads: 310

```
[quote="Pedrodemio, post:40, topic:67569"]
high average current
[/quote]

This, sustaining 30mph+ is what does it. My amperage usage quadruples from 28-29mph @ 2.6-2.9 motor amps, into the 15-25+ motor amps and higher at 32-35mph. It's gotta do with some scientific wind breaking power around 30mph, same dilemma cyclist deal with breaking 30mph. 

That mixed with 100 degree days and 170F+ pavement 1.25" away makes all the issues. I can run in winter/spring/autumn on 65 degree days with 6374 just fine. I think it's a mix of internal and external saturation from ambient temps, more copper would just mean it's still saturated likely, just with a lower equalibrium temp. If the bigger motors we're just big enough to lower the temps by 15-20 degrees to hover around 145-155 it would keep the bell magnets far enough away from the 170F point where you start to see demagnetization.

Edit: as you can see 15-25A in the higher duty cycles is really only 700-1000 watts. Ie I can saturate a motor with only 700ish watts. This tells me I need more copper.
```

---
## \#43 Posted by: Pedrodemio Posted at: 2018-09-11T15:58:28.985Z Reads: 305

```
Yeah, makes sense

If the problem is saturation, that by your description and motor current it isn’t, you would need more iron, not copper, the saturation occurs when the magnetic flux  going through the laminations is higher than the material can handle

But for your case more copper and iron is the solution. cooper for lower losse per volume and iron for more thermal mass to smooth out the high power bursts, and also a bigger motor has more surface area to cool down

Some 3D printed fans maybe? Don’t know if you have space for that
```

---
## \#44 Posted by: strattos Posted at: 2018-09-11T19:01:57.499Z Reads: 301

```
The math makes sense for that appeared scaling. I'll send ya some links when I'm off work here.
```

---
## \#45 Posted by: aethyr Posted at: 2018-09-11T21:31:55.404Z Reads: 307

```
[quote="xilw3r, post:39, topic:67569"]
You should keep in mind that what the motors are “rated for” is really just a load of bullshit. Try running a 6374 motor at 3kw and tell me how long it lasts before the magnets are overheated or the phases short out due to molten enamel. I think most 6374 are really rated for 2kw at peak. and thats optimistic. Look at lets say industrial motors that are rated for at least 1kw, the size is the thing you should take note of.
[/quote]

100% THIS! Your average 6374 is nowhere near a 3kw motor. All these outrunners were originally designed to run on RC planes, with massive amounts of air pushed into them. And even then, they were never meant to be 3kw sustained. And high heat will permanently destroy the neodymium magnets in these cheap hobby motors far before wires melt.

It is true that an inadequate pack defeats high power motors. Hell, you can have enough parallel cells, but if you build it with single strip nickel, you also fail. But that doesn't mean the motors are overkill - it means you haven't built your pack right.
```

---
## \#46 Posted by: psychotiller Posted at: 2018-09-11T21:43:14.044Z Reads: 292

```
Most people here only think they need 12/13s and the biggest motors they can find because someone else said they did in another thread. HYPE.
```

---
## \#47 Posted by: Skunk Posted at: 2018-09-11T21:46:40.609Z Reads: 293

```
:wink::grin:
```

---
## \#48 Posted by: Skunk Posted at: 2018-09-11T21:49:45.964Z Reads: 298

```
[quote="psychotiller, post:46, topic:67569, full:true"]
Most people here only think they need 12/13s and the biggest motors they can find because someone else said they did in another thread. HYPE.
[/quote]

I basically did this with my first autox Datsun too.
Everyone said I should go performance n/a on the stock motor. Okay.  Week later I'm pulling a twin turbo w/5speed out of a wrecked Sylvia. Lol

*note. I made @psychotiller build me a 12s for my first esk8 build with 6374x2 :roll_eyes:  so I'm that guy lol
```

---
## \#49 Posted by: aethyr Posted at: 2018-09-11T21:49:53.865Z Reads: 300

```
[quote="Pedrodemio, post:40, topic:67569"]
Just complementing, power doesn’t matter, what matter is current
[/quote]

Power does matter, because through power, voltage and current are able to convert to one another. I can take a 10kw motor (and by changing the KV) run it 10000V at 1 amp, or 1 V at 10000 amps. The higher wattage motor will always win because it can always run at a higher current given the same kv.

Or in the case of battery pack build, with 100 18650s I could build a 1s100p pack or a 100s1p pack - same wattage, but very different voltage/amp characteristics.
```

---
## \#50 Posted by: Namasaki Posted at: 2018-09-11T22:01:24.787Z Reads: 300

```
[quote="ctincristy, post:1, topic:67569"]
There are a few comparisons between dual 6355 vs dual 6374 (or 5065), but all of them are basically useless since they use either different battery configurations or different kv motors, even different gearing, so they are always biased (and stupid).
[/quote]


I currently have 2 builds that both have the same battery system, electronics, wheels and gearing.
Both are street boards with similar decks.
One is running dual Alien HEV 6374/200kv  and the other dual Alien HEV 6355/190kv
Both sets of motors tested at 170-175kv  so not much difference there.
I have ridden both for some time now and while the 6374s have more torque and are better for climbing hills a **low speeds**, they have noticeably more drag when coasting/free wheeling than the 6355s so when riding on flat ground, I have to stay on the throttle more with the 6374s and I get better range with the 6355s
The 6374's are also more noisy running BLDC unsensored.
Bottom line, I much prefer the 6355s for all around street riding.
```

---
## \#51 Posted by: Battosaii Posted at: 2018-09-11T22:06:37.944Z Reads: 287

```
I thought you gain mechanical advantage over a smaller motor even if the power is the same.

I went from dual 6355 to dual 6374 with the same battery 10s3p and VescX and I did feel a noticeable increase in torque. I do weigh almost double what the average rider weighs though.
```

---
## \#52 Posted by: ivanflo Posted at: 2018-09-11T22:20:59.456Z Reads: 289

```
[quote="Deckoz, post:29, topic:67569"]
If I could  fit 8074 or 8084s i would.
[/quote]
The way i mount my motors i can literally have dual motors of any size. While i am running dual 6374 at the moment, what larger options are out there? I suppose i should just google 8084 and see what comes up? I’m running 10s at the moment, so i guess find anything with 190kv?
```

---
## \#53 Posted by: Jmding Posted at: 2018-09-11T22:59:23.393Z Reads: 287

```
[quote="psychotiller, post:46, topic:67569, full:true"]
Most people here only think they need 12/13s and the biggest motors they can find because someone else said they did in another thread. HYPE.
[/quote]

I suspect this is the case. It shows up in other hobbies as well.  In 3d printing, there's a huge camp of people that think they need name-brand, hardened linear-rails at $100 a foot on all axes, when in reality some cheapo $3 plastic roller wheels are more than good enough for the application.

A 100 kg rider riding up a 20% grade hill, on a 12s board geared to 40 kmh will theoretically draw roughly 50A.  6374's are typically "rated" at 70-80A.  5045's @200 Kv are "rated" to roughly 30A.

Some of us are heavier, climbing steeper hills, or riding at speeds where aerodynamic drag is even more taxing than hill-climbing, but most of us are probably fine running dual 5045's (or a single 6374, which should be more torquey than dual 5045's).
```

---
## \#54 Posted by: Battosaii Posted at: 2018-09-11T23:29:37.267Z Reads: 277

```
You should see me on my R2, the rear motors and Trucks get so hot you can't touch them but on the other hand I can ride my dual 6374 board and my motors barely get warm unless im riding consistently over 30mph, I'm adding more copper and iron to my set up but instead of bigger motors I'm going with more motors. Quad 6374 should feel pretty great. I'm going on a trip next week but when I get back my project will see some real progress
```

---
## \#55 Posted by: b264 Posted at: 2018-09-11T23:46:18.480Z Reads: 279

```
[quote="ivanflo, post:52, topic:67569"]
The way i mount my motors i can literally have dual motors of any size.
[/quote]

How about [12090](https://alienpowersystem.com/shop/brushless-motors/12090s-sensored-outrunner-brushless-motor-130kv-18000w/)
```

---
## \#56 Posted by: moon Posted at: 2018-09-11T23:55:24.579Z Reads: 285

```
That's heavy. 2.8kg :scream:

@Battosaii I suppose you mount diagonally?
```

---
## \#57 Posted by: Battosaii Posted at: 2018-09-12T00:16:49.524Z Reads: 289

```
Yeah it's heavy I did a test mount with just trucks motors and mounts and wheels no enclosure, battery or esc and it felt really heavy but it's okay I plan to ride it not carry it lol.

Not diagonally it's on TB 218 trucks using TB prototype reverse mounts, It's 4wd.
![received_615226992204923|666x500](upload://pFM9Vm5l4f65GALzhsQtDsvMXkN.jpeg)
```

---
## \#58 Posted by: Skunk Posted at: 2018-09-12T00:24:34.387Z Reads: 284

```
Damn....  that look fun
```

---
## \#59 Posted by: Jmding Posted at: 2018-09-12T01:52:42.585Z Reads: 284

```
Anyone know if R2 is using higher temperature epoxy and wire insulation enamel?  There's only so much heat you can pipe through an 8mm steel axle, I imagine they have to be employing some other strategies to manage the heat in addition?
```

---
## \#60 Posted by: Pedrodemio Posted at: 2018-09-12T02:08:15.889Z Reads: 278

```
Sorry, was not clear enough, was talking about what heats up a motor, the power going through doesn’t matter, the main losses are proportional to current, mainly copper loss in the windings loss and iron loss in the stator, the latter also function of ERPM
```

---
## \#61 Posted by: Thatdudedominic Posted at: 2018-10-07T04:44:05.615Z Reads: 251

```
Well I weight 309 pounds and I have dual 6374 on a 12s2p and I’m doing just fine 29mph
```

---
## \#62 Posted by: billappleton Posted at: 2018-10-07T10:13:28.362Z Reads: 246

```
Can someone explain what the motor numbers mean? Where does evolve fall on the spectrum? Boosted?
```

---
## \#63 Posted by: bigben Posted at: 2018-10-07T10:29:50.388Z Reads: 247

```
@billappleton 6374 63mm diameter can. 74mm long can. 
Evolve use 5065 so 50mm diameter motor can and 65mm long. 
I’m not sure about boosted.
```

---
## \#64 Posted by: Winfly Posted at: 2018-10-07T10:31:10.703Z Reads: 245

```
I think boosted either has dual 5045 or 5055. Also, they use gt2 3m belts so no one knows they gearing.
```

---
## \#65 Posted by: Goonman Posted at: 2018-10-07T10:54:15.537Z Reads: 240

```
It sounds like small motors are more efficient at low loads and bigger motors are better for hauling heavy loads and hills. Does anyone know if there is a difference in brands. They all look the same on the outside I'm guessing more than a few share the same manufacturer.
Is there any way to tell?
```

---
## \#66 Posted by: Skunk Posted at: 2018-10-07T12:10:03.504Z Reads: 234

```
@Goonman  I hear alot of people saying maytech is top notch right now.

*edit  i totally misunderstood the question...... just finished a 16 hour shift. Lol my bad
```

---
## \#67 Posted by: Goonman Posted at: 2018-10-07T12:15:37.006Z Reads: 231

```
Thanks they seem to be a reliable manufacturer.
```

---
## \#68 Posted by: Wraith Posted at: 2018-10-07T12:32:12.864Z Reads: 234

```
I’ve got 6374 maytechs. They’ve got warranty and have pretty responsive support. I think other premium vendors like @psychotiller use them for a reason and that reason is good for me too
```

---
## \#69 Posted by: billappleton Posted at: 2018-10-07T14:48:15.017Z Reads: 227

```
Are the mounting holes usually in the same place? Or do people create custom mounting plates?
```

---
## \#70 Posted by: professor_shartsis Posted at: 2018-10-07T14:57:39.470Z Reads: 227

```
in general, the larger motor of the same kv will produce fewer watts of ohmic heating for the same amount of torque... this is a result of generally lower electrical resistance w/ larger motors.
```

---
## \#71 Posted by: Jmding Posted at: 2018-10-07T15:07:57.845Z Reads: 228

```
Large motors = less resistance = less heat = you can put more current through them.
```

---
## \#72 Posted by: professor_shartsis Posted at: 2018-10-07T15:22:37.465Z Reads: 229

```
...consequently the larger motors also get longer range at the same avg speed because they waste less energy from the battery generating heat.
```

---
## \#73 Posted by: bigben Posted at: 2018-10-07T18:57:12.788Z Reads: 231

```
![image|375x500](upload://CziyMe8nvYMaDyxMiWa9clVvSw.jpeg) 
And they look so pretty.
```

---
## \#74 Posted by: meesie Posted at: 2018-10-10T11:54:55.162Z Reads: 226

```
so, to answer the question in the title, is it or is it not worth to go dual 6374?

(of course this all depends on your weight and if your area contains a lot of hills or not, but let's take a medium hilly area and the average weight of an adult man)
```

---
## \#75 Posted by: Skunk Posted at: 2018-10-10T11:57:35.929Z Reads: 222

```
Look at them @Sender.... so pretty
```

---
## \#76 Posted by: Pedrodemio Posted at: 2018-10-10T12:13:05.213Z Reads: 223

```
I would really like to see someone test with a pair and 6374 and a pair of 6355 using the same settings (apart from detection) of a similar motor on the same route to see what real life results look like

In my head 6374 would a little less efficient due to more magnetic material producing higher cogging torque, don’t know if is enough to make a difference 

Also all this assuming that we are within the limits of 6355 and not saturating/overheating 

If after finishing my gear drive the need arises to change for 6355 I will be able to teste 5055 vs 6355 both 190kv and both using the same current settings
```

---
## \#77 Posted by: Ixf Posted at: 2018-10-10T12:33:05.410Z Reads: 225

```
I have 3 boards running a mix of 6374 and 6355 1 evo build, 2 trampa builds (kaly + diy) all 12s.
Kaly is running 6374 and diy is running 6355 evo is running 6374.

Its not apples to apples comparison of course, different makers of motor, internals blah blah blah.  This isn't scientific one bit

But from a daily use with same setting couple of things that are noticeable
*Hill climb.. shouldn't be a surprise here
*Brakes.. this is actually a big one for me, they feel significantly different.  Alot more confidence with the bigger cans

What I don't notice
*Acceleration (honestly at 12s I rarely need to push the remote to the max)
```

---
## \#78 Posted by: Skunk Posted at: 2018-10-10T12:36:21.924Z Reads: 221

```
Mmm all that 12s.......
Someday. 
No 10s?
```

---
## \#79 Posted by: Battosaii Posted at: 2018-10-10T12:54:12.361Z Reads: 218

```
How about quad 6374 for that 50mph+ belt drive.
```

---
## \#80 Posted by: Ixf Posted at: 2018-10-10T12:57:32.934Z Reads: 217

```
I did run 10s for awhile on a carver.. it wasn't quite enough for me.. so all 12s foc pneumatic goodness now for me
```

---
## \#81 Posted by: Skunk Posted at: 2018-10-10T13:02:27.517Z Reads: 215

```
First build (about to start assembling)  12s5 6374 170kv x2 focboxes.... im pumped
```

---
## \#82 Posted by: Battosaii Posted at: 2018-10-10T13:06:28.201Z Reads: 210

```
You will love it. Lots of torque and speed out of those 6374 on 12s.
```

---
## \#83 Posted by: Skunk Posted at: 2018-10-10T13:32:51.329Z Reads: 211

```
Might try pushing for a awd build out of it if some things pan out.
```

---
## \#84 Posted by: professor_shartsis Posted at: 2018-10-10T14:08:21.602Z Reads: 219

```
[quote="Pedrodemio, post:76, topic:67569"]
In my head 6374 would a little less efficient due to more magnetic material producing higher cogging torque, don’t know if is enough to make a difference
[/quote]

if the electrical resistance is halved on the bigger motor (same kv) then the heat production in the copper would be halved for the same torque... and less heat produced means less electrical watt hours consumed for the same torque over the same time period & greater efficiency. as far as eddy current loss i believe this is estimated based the motor current at no load rpm...

which makes me think of something else... i think there are actually 2 different no load rpms... theres the max rpm the motor will do on its own.... and then there’s the rpm that’s a little bit faster that you’d have to spin the motor up to with outside energy (accounting for the bearing and eddy current loss) in order to make the back emf voltage produced by the motor equal to the battery pack voltage... at this slightly higher no load speed you shouldn’t be able to measure any motor current even at 100% duty cycle. i believe this second higher no load rpm is the one that’s used to calculate the torque per amp in newton meters via kt = 60 / (2 * pi * kv)
```

---
## \#85 Posted by: Blitz Posted at: 2018-10-10T14:45:22.525Z Reads: 215

```
[quote="moon, post:56, topic:67569"]
That’s heavy. 2.8kg :scream:
[/quote]

my deck weighs 4kg.
```

---
## \#86 Posted by: Battosaii Posted at: 2018-10-10T15:21:26.555Z Reads: 209

```
Lol my whole board isngona be 18-20kg when done... Super heavy but with 60miles range I shouldn't have to carry it much.
```

---
## \#87 Posted by: Ixf Posted at: 2018-10-10T16:52:03.673Z Reads: 210

```
BTW.. I don't understand the desire for AWD... I know I want one... but I don't know why I want one :smiley:
```

---
## \#88 Posted by: mixedcreation Posted at: 2018-10-10T17:18:00.689Z Reads: 211

```
This was @Eboosted 6374 vs 6355. Granted 10s vs 12s as well. But the difference is night and day. He has a post on here about it.

https://youtu.be/boBT9NsGcUc
```

---
## \#89 Posted by: taz Posted at: 2018-10-10T17:35:57.503Z Reads: 208

```
I am sorry but the difference you are seeing is 10S vs 12S, not 6355 vs 6374.
```

---
## \#90 Posted by: ksfacinelli Posted at: 2018-10-10T17:41:23.552Z Reads: 206

```
I like the 6374's as they are more torque if you get 190kv or less and setup the correct gearing ratio.  I love pneumatics and run 200mm x 50mm and even some 280mm x 250mm x 4 MBS T2 with a 16x72 gear ratio it is dialed in for my style of riding and conditions.
```

---
## \#91 Posted by: mixedcreation Posted at: 2018-10-10T17:53:54.015Z Reads: 205

```
Thus the reason I said it. Granted with my weight I noticed a difference with 12s 6355 vs 6374 on hilly terrain.  But I'm built like a running back.  Most ppl I doubt will ever noticed the slight acceleration difference
```

---
## \#92 Posted by: Jmding Posted at: 2018-10-10T18:21:46.064Z Reads: 210

```
TLDR:  6374's give you +25% torque at low to mid speeds.  6355's are already plenty torquey.  Not worth it.

Long:
This chart shows the maximum loading specs of 63XX motors (SunRay is the OEM for Turnigy SK3 motors).  It's hard to be 100% certain, but guessing based on motor weight and Kv/turns, I believe our 6374 is really a 5035 (the chart goes by stator dimensions instead of nominal can dimensions), and our 6355 is really a 5025.  For a 200 Kv motor, the 6374 is rated to 75A, and the 6355 is rated to 60A, before excessive heat from wire resistance and magnetic saturation risks motor meltdown.  Given that almost all of our ESCs are only rated to 60A, that means that upgrading to 6374's gets you up to 25% more torque (75A / 60A = 125%), until you reach 80% of top speed, at which point your ESC starts bottlenecking the current, and your torque drops off linearly to 6355 levels at 100% of top speed.  That extra 25% torque at low and mid speeds comes at the cost of around 350 grams (0.75 lb) per motor, and limited truck selection.  To me, for a dual motor setup, that is just not worth it, especially given that with dual 6355, that is already 120A continuous through the system, which for a 200 lb rider on 83mm wheels, is enough to climb 45% grade hills.  The one use case where I might imagine that you would actually want to go up to 6374's is if you cruise at very high speeds (>=30 mph), and therefore are constantly drawing a ton of current at high voltages to overcome air-resistance.  But even in this case, because the current is limited by the ESC at high speeds, 6374's are only capable of less that 25% more torque.  Seems like a pretty marginal improvement.  If you are going for a really bonkers build, sure go ahead and go up to 6374's, but make sure to spend the extra $300 of whatever it is to upgrade to dual Trampa VESC 6's, as those are the only ESCs (I know of at least) that can push the 75A continuous that it takes to really take advantage of the larger motors.

I dont expect any of the motor manufacturers make a product that is meaningfully higher quality than the others, to invalidate this logic.  With the sole exception of the Raptor 2's hub motors (where they seem to be getting very creative to deal with thermals), its hard to believe that anyone is doing anything particularly special given the extremely consistent pricing between product lines.


![image|690x400](upload://aJLA5p7GiZqWITM06pX6GB4bFcA.jpeg)
```

---
## \#93 Posted by: Hummie Posted at: 2018-10-10T18:24:04.066Z Reads: 202

```
Torque is determined by kv ( or its opposite kt).   A giant motor with a high kv n low kt will have less torque per amp than a tiny motor w low kv.  Only variable is efficiency and with a very small motor eff goes down n possible magnetic saturation w higher currents.
```

---
## \#94 Posted by: Pedrodemio Posted at: 2018-10-10T18:27:59.803Z Reads: 197

```
Do you know how stator length influence Kv? For example, get two stators one being double the length of the other, do I need different number of turns for the same Kv?
```

---
## \#95 Posted by: Jmding Posted at: 2018-10-10T18:33:19.424Z Reads: 197

```
Yup, check the table, it makes those kinds of relationships very easy to figure out. 5035 190kv = 18t, 5025 195kv = 24t.  With the shorter stator length, it takes a lot more turns to achieve the same Kv.

Another interesting effect is Kv vs current.  Higher Kv, higher current, until you get to the 5045 motor, where iron losses are becoming a more significant source of heat than wire resistance.  This means upgrading to a higher Kv motor actually get you MORE torque at the wheels than a lower Kv motor, assuming you adjust your gearing so that your top speed doesnt change.

Put this idea together with the Kv vs stator length concept, and that basically tells you why bigger motors are better.  Bigger motors = fewer turns required to achieve a relatively low kv = more current capability
```

---
## \#96 Posted by: Hummie Posted at: 2018-10-10T18:34:46.384Z Reads: 197

```
Double long will drop like half the kv. Similar to more turns
```

---
## \#97 Posted by: Pedrodemio Posted at: 2018-10-10T18:35:55.663Z Reads: 201

```
Damn, didn’t realize that

It makes sense since you have more copper
```

---
## \#98 Posted by: sharky Posted at: 2018-11-15T11:54:21.264Z Reads: 189

```
Dear Prof Shartsis may i ask you smthg.
when im upgrading my dual 6355 setup (190KV) to an Dual 6374 (200KV) setup am i correct tht ill get bit more speed, the motors wont get as hot as the 6355s and have more break power?
whats about the torque?
KR
```

---
## \#99 Posted by: professor_shartsis Posted at: 2018-11-15T14:02:23.566Z Reads: 186

```
since the kv’s are quite close, but the bigger stator allows more copper, the resistance should be significantly lower in the larger motor, likely resulting in less heat for similar torque. the bigger stator can ultimately produce more torque because it takes more current to magnetically saturate the iron, but before saturation is reached, the 190kv produces more torque per motor amp, but not necessarily more torque per battery amp, because if the resistance on the larger stator is lower, there are less copper losses.
```

---
## \#100 Posted by: sharky Posted at: 2018-11-15T14:18:01.115Z Reads: 179

```
thank you very much for the detailed infos
```

---
## \#101 Posted by: professor_shartsis Posted at: 2018-11-15T15:25:40.255Z Reads: 180

```
@sharky if we compare single motor smaller stator 190kv 0.05ohm vs larger stator 200kv 0.025ohm (assuming the larger, slightly higher kv stator has half the electrical resistance, and 40a motor current limit for both, and assuming neither stator saturates):

https://image.ibb.co/guMjPf/190kv-vs-200kv-1.gif

^torque & thrust are both slightly lower with the 200kv w/ larger stator, but the reduction in heating is more significant
```

---
## \#102 Posted by: kuphjr Posted at: 2018-11-15T15:32:19.780Z Reads: 169

```
In my understanding of physics, batteries and motors, you are correct. This is why I use 6355 on my dual builds and 6375 on my single builds. Dual 6374 is really just added weight that you cannot take advantage of and that’s about it.  That being said, both of the types of motors are either 190 or 170Kv.

You need a battery >120A for dual 6374 to make sense. That means at least 6-7p depending on the cells.
```

---
## \#103 Posted by: professor_shartsis Posted at: 2018-11-15T15:49:22.962Z Reads: 166

```
https://image.ibb.co/disSAL/190kv-vs-200kv-2.gif
^ @kuphjr @sharky  but (and this is a pretty big BUT), when we limit the power to 5a battery amps with no motor current limit (instead of 40a motor current limit), the results are reversed... the 200kv motor w/ larger stator and half the electrical resistance has more torque, thrust, max rpm AND lower heating than the smaller 190kv motor, because the same number of battery amps results in more motor current in the larger, higher kv motor due to the lower electrical resistance, ultimately resulting in higher torque.
```

---
## \#104 Posted by: harrypzee Posted at: 2018-11-15T15:50:10.641Z Reads: 167

```
Even though 6374s aren't able to use their full power due to the battery bottleneck, I still think they have an advantage over 6355s (I could be wrong - I don't have empirical evidence, I'm just hypothesizing ). I think the main advantage is the extra copper/metal that helps in dissipating heat and making it more efficient overall. When you're engineering something it's generally better to use components that are over rated rather than under rated for their purpose. The only downside (other than cost, which I'm disregarding since this is purely from an engineering standpoint) I can see is weight, but weight doesn't seem to matter nearly as much as the cooling advantages it gives. Each person's weight has much more variation than the weight the larger motors would add, so I don't think weight is a huge deal.
```

---
## \#105 Posted by: professor_shartsis Posted at: 2018-11-15T17:50:30.905Z Reads: 171

```
https://image.ibb.co/i6HQx0/190kv-vs-200kv-3.gif

^ @sharky @kuphjr finally if we compare the 190kv 0.05ohm vs 200kv 0.025 ohm w/ 60a motor limit and 30a battery limit (the battery limit is half the motor limit)--

the smaller 190kv motor with twice the electrical resistance has more torque off the starting line at low rpms (because power is limited by the motor current limit, and 190kv has more torque per motor amp than 200kv), but the larger 200kv motor with half the electrical resistance has more torque above the speed that the 30a battery limit is reached (around 20mph assuming 37v bat, 107mm tire, 2.125:1 ratio), because, due to the lower electrical resistance in the larger motor, the same # of battery amps results in more motor amps in the larger 200kv motor, resulting in greater torque in the larger stator with 200kv than the 190kv once the battery limit is reached.

the larger motor with half the electrical resistance has lower heating at all speeds.
```

---
## \#106 Posted by: sharky Posted at: 2018-11-15T19:06:59.769Z Reads: 158

```
Ok now i fully understand thank you verey much
When my 6374 setup is done ill test it in real life
```

---
## \#107 Posted by: sharky Posted at: 2018-11-15T19:08:52.155Z Reads: 160

```
Thx again for your time and the detailed infos
```

---
## \#108 Posted by: Jmding Posted at: 2018-11-15T19:09:02.374Z Reads: 162

```
Prof, why are you running both simulations using 60a motor limit? The point of bigger motors is that for the same Kv, they have lower winding resistance, and can therefore handle more current safely before overheating. If a 6355 190 Kv motor with 0.05 ohm resistance is good to 60A (60A^2 * 0.05ohm = 180W of heating), then a 6374 200 Kv with 0.025 ohm should be good to 85A (85A^2 * 0.025ohm = 180W of heating). Actually, a little more than that since the larger motor will also have larger surface area and therefore slightly better heat dissipation.

If you run the same electrical input through a 190 Kv, 0.05 ohm motor vs a 200 Kv, 0.025 ohm motor, the difference is going to be basically negligible, which your chart in the lower left demonstrates very effectively.
```

---
## \#109 Posted by: professor_shartsis Posted at: 2018-11-15T19:27:54.568Z Reads: 165

```
@Jmding some vescs have a coded 120a motor current limit in the firmware (because the current sensor becomes inaccurate above this value), so even if the bigger motor could handle more than 120a current, the ESC won't do it.

120a motor current would definitely saturate some stators but not others giving the larger motors an advantage here.

so the real bottleneck to low rpm acceleration is the controller... not the battery or motor (if the stator is large enough and the C rating of the battery as well). also even if the larger motor produces the same heat with double the motor current (because 1/2 resistance), the controller heats 2^2=4x more quickly, because the controller resistance remains unchanged.

so using the same motor current limit for both motors puts the bottleneck at either the controller heating rate or the current sensing ability for +120A motor currents.
```

---
## \#110 Posted by: Hummie Posted at: 2018-11-15T20:05:58.743Z Reads: 158

```
I can think of a reason to go with smaller motors, less magnetic cogging, so easier coasting.   could end up being more efficient if you coast a lot.
```

---
## \#111 Posted by: Battosaii Posted at: 2018-11-15T20:09:27.833Z Reads: 161

```
I felt a significant difference going from dual 6355 to dual 6374 especially during braking. 

I do run dual 6355 on my dual evolve build but I do use 6374 on my quad build, maybe it's cause I weigh significantly more than the average rider.
```

---
## \#112 Posted by: Jmding Posted at: 2018-11-15T20:20:39.432Z Reads: 160

```
Interesting... did you change your vesc settings at all? what motor did you start with, and what motor did you end with? did your top speed change?
```

---
## \#113 Posted by: Lunasi Posted at: 2018-11-15T20:33:29.388Z Reads: 161

```
If you watch about 10 and a half minutes in you'll see my 2 6374's on 12s4p with dual torque esc's leaving Robin from lazy rollers behind on a dual 6355, 12s5p with dual focboxes. They make a massive difference IMO.

https://youtu.be/b_uqtqzmRPQ
```

---
## \#114 Posted by: sharky Posted at: 2018-11-15T20:58:21.456Z Reads: 157

```
Great vid and race 👍👍
From my understang thts cause of the better torque / acceleration the bigger motors have at higher speeds like prof_shartsis explained am i right?
```

---
## \#115 Posted by: Battosaii Posted at: 2018-11-15T21:01:43.196Z Reads: 157

```
TB 6355 and then TB6374 same settings.
```

---
## \#116 Posted by: Lunasi Posted at: 2018-11-15T21:02:17.642Z Reads: 155

```
I believe you are correct 😊
```

---
## \#117 Posted by: sharky Posted at: 2018-11-15T21:06:18.064Z Reads: 158

```
Wht kv do your motors have?
```

---
## \#118 Posted by: Lunasi Posted at: 2018-11-15T21:24:16.674Z Reads: 158

```
190kv dual torque 74's
```

---
## \#119 Posted by: professor_shartsis Posted at: 2018-11-15T21:53:25.101Z Reads: 161

```
https://image.ibb.co/kMDr4f/190kv-vs-200kv-5.gif

^ @Jmding, suppose we explosion-proof everything (& use stators that don't saturate) and we just go 95% duty cycle the whole way...

it looks like the 200kv with half the resistance would have roughly double the peak mechanical power, double the thrust, double the torque, double the heating & double the power consumption compared to the 190kv.
```

---
## \#120 Posted by: malJohann Posted at: 2018-11-15T22:08:03.082Z Reads: 159

```
So for someone like me that has an 8S1P (2x 4S1P mounted in series) 6Ah 65c constant 130c burst battery, with ESCs putting out 160A each, dual 6374 192kV makes perfect sense.
```

---
## \#121 Posted by: Jmding Posted at: 2018-11-16T06:52:40.897Z Reads: 158

```
@Battosaii I dont understand how that's possible since torque = Kt * current. When you changed the motors, you didn't change Kt, and you didn't change current settings through the VESC, so where is the extra acceleration coming from?

Maybe the two motors are nominally the same Kv, but they are actually slightly different? My Sk3 6374 is listed as 192 Kv for example, but VESC Tool measures it closer to 170 Kv. That would be a 10% difference in torque relative to the nominal specs.
```

---
## \#122 Posted by: Battosaii Posted at: 2018-11-16T07:21:52.019Z Reads: 157

```
That could be possible. The biggest difference was actually brakes. They are so much more powerful I had to lower my settings. 

Funny thing is I can ride 20miles on my 6355 set up and the motors are still cool to the touch but on my 4wd set up they do get warm, not hot just slightly higher than skin temp warm.
```

---
## \#123 Posted by: 12meterkuk Posted at: 2018-11-16T10:00:10.163Z Reads: 153

```
Where’s the fun in that 😂
```

---
## \#124 Posted by: Hummie Posted at: 2018-11-17T13:49:15.901Z Reads: 146

```
True I’m on the throttle a lot instead of coasting but it could explain less efficiency w a bigger motor
```

---
## \#125 Posted by: Chrisjarram Posted at: 2019-02-05T08:47:51.854Z Reads: 116

```
Until something breaks when you're 10 miles from home ;)
```

---
## \#126 Posted by: dareno Posted at: 2019-02-05T08:58:07.677Z Reads: 115

```
I love that level of reading.  You sir go to the top of the class.
```

---
## \#127 Posted by: Chrisjarram Posted at: 2019-02-05T08:59:33.067Z Reads: 114

```
:P

10char.
```

---
## \#128 Posted by: Battosaii Posted at: 2019-02-05T11:02:32.519Z Reads: 106

```
I have 4 motors so I'd probably ride it out. If all else fails there's Lyft
```

---
## \#129 Posted by: Chrisjarram Posted at: 2019-02-05T11:20:05.491Z Reads: 103

```
Airlift? :)
```

---
