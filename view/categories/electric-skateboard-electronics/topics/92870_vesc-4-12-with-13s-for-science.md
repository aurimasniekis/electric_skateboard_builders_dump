# Vesc 4.12 with 13s for science

### Replies: 53 Views: 804

## \#1 Posted by: AgressivStreetLamp Posted at: 2019-05-05T17:23:47.129Z Reads: 200

```
Alright, I've been reading quite a bit about this but I haven't found anyone who's run this setup and reported back. I'm building (rebuilding) my old setup and due to some lapses in initial judgement I have been going on a 13s design. That is to say 149KV sk3, 13s3p q30 battery, vesc 4.12 from torque and a Vedder Antispark Switch. 

I have gotten the very clear sense that 13s is risky due to voltage spikes nuking the drv chip on the vesc. At this point I want to stick with the 13s for science and to see if we can't push some boundaries.
What I am hoping to collect here are the improvements that can be made, whilst keeping the 13s, to ensure the best possible reliability. My approach to this is to minimize the chance of voltage spikes at all. And to understand how they occur.

I have read that a TVS Diode across a the battery inputs will help. Can anyone detail this some more? Specs on the diode? I'm guessing one with 60v brake down voltage but what about quiescent current and power rating? This sounds similar to ESD protection setups I've heard about.  
Along the same.lines I've heard of adding more caps across the battery terminal on the vesc? 
Another topic is braking. It sounds like braking is when the voltage spikes occur. Is there a way to perhaps set up the firmware such that I retain some braking but reduce back EMF spikes? 

A definite possibility for me is to move to the vesc 6 or any other esc (esk8 specific preferably). From my understanding that vesc 6 is also only recommended at 12s. But still rated for 60v in theory. Is this a much safer option? Does this or any other esc have the hardware that protects from spikes?
```

---
## \#2 Posted by: bluegreen Posted at: 2019-05-05T19:17:19.092Z Reads: 180

```
From what I understand even 12s is pushing it on 4 hardware if you are running in FOC anywhere near 50amps.

You might be able to do what you describe running in BLDC, but I doubt it. This is almost certainly a path to melted VESCs.
```

---
## \#3 Posted by: AgressivStreetLamp Posted at: 2019-05-05T19:57:29.566Z Reads: 169

```
Well I'll keep you posted. I'll be sure to run bldc mode then. Any tips on the diode?
```

---
## \#4 Posted by: bluegreen Posted at: 2019-05-05T20:50:04.803Z Reads: 158

```
Not really, this is just a bad idea. It it's known for not being able to handle it's rated capacity and you are planning to go over this. Nobody else is commenting because they don't want to touch this with an insulated 9 foot pole.
```

---
## \#5 Posted by: AgressivStreetLamp Posted at: 2019-05-05T21:09:33.844Z Reads: 148

```
Fair enough. Thanks for the input. Nothing's built yet. I'm still working on the campus cruiser for a friend. Sounds like I'll just cut my losses on the charger and BMS and go for 12s.
```

---
## \#6 Posted by: will_manners Posted at: 2019-05-06T04:33:10.022Z Reads: 135

```
Torqueboard Vesc + 13S = 💣💥

Please prove us wrong!
```

---
## \#7 Posted by: b264 Posted at: 2019-05-06T04:34:12.034Z Reads: 133

```
You'd be better off donating this VESC to a college student in need than intentionally destroying it :stuck_out_tongue:
```

---
## \#8 Posted by: dareno Posted at: 2019-05-06T04:42:41.065Z Reads: 129

```
I seriously wouldn't run 13s through that particular vesc.  They don't stand up to 12s and this I know by experience.  One of mine went in a week of normal riding.
```

---
## \#9 Posted by: Dirt_Bag Posted at: 2019-05-06T04:43:39.487Z Reads: 130

```
4.xx or 6.xx hardware?
```

---
## \#10 Posted by: dareno Posted at: 2019-05-06T04:54:37.401Z Reads: 125

```
TB 4,12  The HK work fine with 12s though.
```

---
## \#11 Posted by: AgressivStreetLamp Posted at: 2019-05-06T05:11:31.582Z Reads: 125

```
Well then to the second half of my inquiry, how do I maximize 12s runtime? Heatsink? Antispark? TVs diode?
```

---
## \#12 Posted by: AgressivStreetLamp Posted at: 2019-05-06T05:11:54.369Z Reads: 126

```
I am a college student in need :(
```

---
## \#13 Posted by: Dirt_Bag Posted at: 2019-05-06T05:17:00.419Z Reads: 125

```
Well then run your 4.xx vesc on 10s.
```

---
## \#14 Posted by: sk8l8r Posted at: 2019-05-06T05:28:55.739Z Reads: 127

```
[quote="AgressivStreetLamp, post:12, topic:92870"]
am a college student in need
[/quote]

I would not be doing any possible 'destructive' testing with any parts if I had no $$
```

---
## \#15 Posted by: Eboosted Posted at: 2019-05-06T05:38:41.183Z Reads: 121

```
[quote="bluegreen, post:2, topic:92870, full:true"]
From what I understand even 12s is pushing it on 4 hardware if you are running in FOC anywhere near 50amps.

You might be able to do what you describe running in BLDC, but I doubt it. This is almost certainly a path to melted VESCs.
[/quote]

My Darth Maul has been runing almost 3 years wuth 12s4p, no issues related with FOC as 12s.

My Trampa 12s4p has been runing for over 1.5 years on v4.12 and FOC, not a single issue

My Sidekick 12s5p has been runing for 8 months pushing the shot out of the system, VESCs are 100% perfect from day one

My Century 40" 12s4p made of Samsung 30Ts is runing 100A of battery discharge and it's a fucking rocket runing Unity and it's the best eboard I have riden in my life, again zero issues.

This is has been my experience, would I recommend 12s and FOC, yes but only with Focbox or Unities as I never tried anything else besides them
```

---
## \#16 Posted by: bluegreen Posted at: 2019-05-06T05:44:58.038Z Reads: 120

```
[quote="Eboosted, post:15, topic:92870"]
Focbox or Unities
[/quote]

Isn't that the key here? You are right it makes sense to not just say VESC, because actually arent both those mfg known for making upgrades to the design that help them handle the higher voltages?
```

---
## \#17 Posted by: Andy87 Posted at: 2019-05-06T06:05:12.588Z Reads: 115

```
@AgressivStreetLamp Voltage spikes are what could most likely kill your vesc. I think @Winfly run 13s and has some data logs where he hit like 58v during breaking.
```

---
## \#18 Posted by: bluegreen Posted at: 2019-05-06T06:06:19.815Z Reads: 115

```
You know what, heck with my naysaying. If science = risking your time, money, and personal safety for very little to no reason, then heck! go for it!
```

---
## \#19 Posted by: dareno Posted at: 2019-05-06T06:08:10.732Z Reads: 118

```
[quote="Eboosted, post:15, topic:92870"]
This is has been my experience, would I recommend 12s and FOC, yes but only with Focbox or Unities as I never tried anything else besides them
[/quote]

That is the most important point.  Focboxes.  They can handle the voltage no drama.

[quote="Eboosted, post:15, topic:92870"]
My Century 40" 12s4p made of Samsung 30Ts is runing 100A of battery discharge and it’s a fucking rocket runing Unity and it’s the best eboard I have riden in my life, again zero issues.
[/quote]
This is something I would love to try.  Must rip the soles off your shoes at those amps.  Mines bad enough at 80
```

---
## \#20 Posted by: Winfly Posted at: 2019-05-06T06:12:41.305Z Reads: 111

```
still running 13s on my hummie build. used to have 6.6s now Focboxes. at full charge and I live on a hill. It can spike up to 58V so I raised the default over voltage fault to 59V. never have a problem since.
```

---
## \#21 Posted by: b264 Posted at: 2019-05-06T06:22:01.888Z Reads: 107

```
It's incredibly hard to believe that you built 4 DIY boards and had zero issues with any of them.
```

---
## \#22 Posted by: bluegreen Posted at: 2019-05-06T06:24:28.016Z Reads: 103

```
@Eboosted knock on some wood! knock on all your decks! quick!
```

---
## \#23 Posted by: dareno Posted at: 2019-05-06T07:00:26.097Z Reads: 100

```
Yeah I can't say I've had that much luck.  Focboxes are reliable though.  Very much so.  Alan rides like a nutcase too.  I have bought 8 of those things and only killed 3.  Of those 3 two were my fault and the other one just randomly died on me. Middle mosfet and drv.    So 1 out of 8 is not bad for esc's.  Killed far more than that with rc.  They are a bit tetchy.
```

---
## \#24 Posted by: dareno Posted at: 2019-05-06T07:01:40.033Z Reads: 105

```
[quote="bluegreen, post:22, topic:92870"]
knock on all your decks! quick!
[/quote]

Not the trampa though because thats not wood mate!  find a table!
```

---
## \#25 Posted by: dareno Posted at: 2019-05-06T07:09:23.489Z Reads: 103

```
https://youtu.be/JwDwEHQCk5g?t=16

This is how you kill an esc like a boss.
```

---
## \#26 Posted by: bluegreen Posted at: 2019-05-06T07:18:23.613Z Reads: 101

```
So a failure like this is similar to what happened to me, mine was just about 5% of that. Heat causes a component to catch fire, which is what is seen at first but then a secondary more violent reaction occurs and that is the arc that is being formed when the short circuit results from whatever component dying.

The runaway arc is a superheated gas that consumes everything remotely flammable around it until there is no longer enough material to sustain the arc. (or you pull the loop key) I mean it's not accurate to say this but with plasma is so hot the air itself is burning.
```

---
## \#27 Posted by: Eboosted Posted at: 2019-05-06T13:34:50.166Z Reads: 89

```


[quote="b264, post:21, topic:92870, full:true"]
It’s incredibly hard to believe that you built 4 DIY boards and had zero issues with any of them.
[/quote]

I didn't say that. 

I had a lot of issues but none related to Focbox/Unity failing because of runing 12s in FOC at high current.

I must add to my previous statement, I did try other 4.12 vesc and they have failed at 12s and FOC within hours
```

---
## \#28 Posted by: AgressivStreetLamp Posted at: 2019-05-06T14:50:21.828Z Reads: 82

```
Voltage spikes coming from battery or motor? What causes those spikes?
```

---
## \#29 Posted by: Andy87 Posted at: 2019-05-06T14:53:12.921Z Reads: 83

```
It can come from too long and too thin battery wires as inductive voltage spike (this spikes are flattened by the capacitors on the input) or from the motor side, but honestly this I didn’t fully understood how the spikes build up there.
```

---
## \#30 Posted by: AgressivStreetLamp Posted at: 2019-05-06T14:59:07.629Z Reads: 86

```
So to converge some thoughts here. 
Sounds like 12s is safe on focbox and unity vesc 4.12 hardware. And risky on most/all other 4.12 hardware. What about flipsky hardware?

13s is doable but risky on high quality vesc 4.12 hardware but not recommendable. Impossible on cheaper hardware.

So what that tells me is there is some difference between.the two hardware designs or component list that makes this possible. Anybody know what it is?

For the record, at this point I've resolved to using the TB 4.12 on a request build with 8s and moving to a flipsky dual on the build.in question.
```

---
## \#31 Posted by: sk8l8r Posted at: 2019-05-06T15:07:00.738Z Reads: 80

```
the flipsky 4.12 I belive @longhairedboy tested on 12s (without problems) 

[quote="AgressivStreetLamp, post:30, topic:92870"]
13s is doable but risky on high quality vesc 4.12 hardware but not recommendable.
[/quote]

where did you get that from? I've NEVER seen a build on 13s that does not use a FOCBOX
```

---
## \#32 Posted by: Andy87 Posted at: 2019-05-06T15:08:23.106Z Reads: 79

```
@Winfly @flipsky 6.6 earlier, no?
```

---
## \#33 Posted by: AlanZhou Posted at: 2019-05-06T15:26:39.636Z Reads: 79

```
But a focbox is also a 4.12...

Many people have also used 13s on Focboxs without much issue

I will be running 13s on the unity (13s10p) and see how the unity will do
```

---
## \#34 Posted by: AlanZhou Posted at: 2019-05-06T15:29:21.536Z Reads: 76

```
Chaka @chaka 4.12 can handle 12s

They claim other names because they are not allowed to call their vesc 4.12 (technically) because it is trademarked, even torqueboards refers to their vesc as torque esc

[quote="bluegreen, post:16, topic:92870"]
mfg known for making upgrades to the design that help them handle the higher voltages?
[/quote]

No they upgrade their vesc to be more reliable and handle higher amperage. (Ex, using direct fets and a heatsink) both 4.12 hardware, and unity and also focbox's use hardware rated up to 60v (drv is the limiter)
```

---
## \#35 Posted by: Andy87 Posted at: 2019-05-06T15:37:45.006Z Reads: 70

```
[quote="AlanZhou, post:33, topic:92870"]
Many people
[/quote]

I think I can count them on two hands. As min from the people in here. Maybe there is a 13s focbox fb group I don’t know about 😜 but besides I wouldn’t call it many.
```

---
## \#36 Posted by: AlanZhou Posted at: 2019-05-06T15:40:26.038Z Reads: 71

```
[quote="Andy87, post:35, topic:92870"]
13s focbox fb group I don’t know about
[/quote]

Hmm I get to join soon 🤣
```

---
## \#37 Posted by: AgressivStreetLamp Posted at: 2019-05-06T15:55:01.570Z Reads: 72

```
High quality vesc 4.12 hardware includes focbox and unity ? Or are you saying focbox 6.6 hardware?
```

---
## \#38 Posted by: AgressivStreetLamp Posted at: 2019-05-06T15:56:27.113Z Reads: 72

```
Also, can anyone weigh in on the flipsky 4.2 hardware and flipsky FSESC 6 hardware? How reliable are they for 12s and for 13s?
```

---
## \#39 Posted by: AlanZhou Posted at: 2019-05-06T16:00:46.463Z Reads: 75

```
Flipsky 4.2, don't try em at 13s, but 6.6 should do fine at 13s
```

---
## \#40 Posted by: sk8l8r Posted at: 2019-05-06T16:00:49.285Z Reads: 76

```
Sorry I was wrong, should have said 'all  4.12 builds I've seen use focboxes'

that includes my evo, I'm all up for doing stuff for science and as far as 4.12 or 4.20 I thought I was going to pushing them with the 12s lipo testing I have planned for them
```

---
## \#41 Posted by: AlanZhou Posted at: 2019-05-06T16:00:58.229Z Reads: 74

```
[quote="AgressivStreetLamp, post:37, topic:92870, full:true"]
High quality vesc 4.12 hardware includes focbox and unity ? Or are you saying focbox 6.6 hardware?
[/quote]

There is no 6.6 focbox
```

---
## \#42 Posted by: sk8l8r Posted at: 2019-05-06T16:02:10.482Z Reads: 70

```
[quote="AgressivStreetLamp, post:38, topic:92870"]
flipsky FSESC 6 hardware
[/quote]

I would be willing to try one of those for science on 13 if I had one
```

---
## \#43 Posted by: AgressivStreetLamp Posted at: 2019-05-06T16:08:33.538Z Reads: 69

```
[quote="sk8l8r, post:42, topic:92870"]
would be willing to try one of those for science on 13 if I had one
[/quote]

[quote="AlanZhou, post:41, topic:92870"]
There is no 6.6 focbox
[/quote]

Got it thanks.
```

---
## \#44 Posted by: AgressivStreetLamp Posted at: 2019-05-06T16:22:25.504Z Reads: 68

```
So how does this summarize it? 

List of max voltage usable for various VESC hardware:

Most 4.12 hardware including Torque Vesc 4.12: less than 12s to be reliable
Focbox : 12 or 13s (experimental) 
Flipsky 4: 12s
Flipsky 6: 13s (experimental)

What about other vesc hardware I'm missing here?
```

---
## \#45 Posted by: longhairedboy Posted at: 2019-05-06T16:30:20.063Z Reads: 66

```
[quote="sk8l8r, post:31, topic:92870"]
the flipsky 4.12 I belive @longhairedboy tested on 12s (without problems)
[/quote]

that thing is garbage for anyone over 100 pounds. The dual 100 is also garbage. The flipsky vesc 6 variant is decent but its self contained with its own switch and enclosure so its not ideal for dual builds, or any builds that i would do, seems solid for off road apps maybe.
```

---
## \#46 Posted by: AgressivStreetLamp Posted at: 2019-05-06T17:22:57.086Z Reads: 61

```
When you say "garbage" care to elaborate?

Would it be accurate to state:
 The flipsky 4 is not suited for 12s  applications. 

And the flipsky 6 is solid  from an electronics hardware perspective but has unfavorable configuration of accessories.
```

---
## \#47 Posted by: Hummie Posted at: 2019-05-06T18:07:35.861Z Reads: 58

```
There’s lots of bogus components in some escs.  So they’re 4.12 but with capacitors which aren’t capable of their stated capacitance and stuff like that.  Even a model from a single manufacturer could be different in different batches.


If u have gearing why bother risking it doing 13s and u could just change gear.   It shows even more likely to be inefficient at higher voltage ironically unless you’re alwats hanging at the higher speed   The esc won’t be at full duty cycle as often and ilthe increased pwm is a loss.  If u look at the grin motor simulator u can see
```

---
## \#48 Posted by: brenternet Posted at: 2019-05-06T18:15:15.593Z Reads: 58

```
Just run 8s and carry a large beer. Lifeishortyolo :call_me_hand:
```

---
## \#49 Posted by: longhairedboy Posted at: 2019-05-06T20:13:38.356Z Reads: 57

```
What i mean is we ran them at 12S and within a week they were dead. By dead i mean they weren't functioning anymore and  there was smoke and blown components involved. This happened three times in a row, we were part of the beta test group for flipsky. They sent us units, we blew them up and reported back. We did the same for brother hobby, that company with the motors that throw magnets. We did it for skate machines, we broke every board they sent us. Probably the only thing we haven't broken that was sent to us for feedback was Boa Wheels, which reminds me: i still have to break some TorqueBoards wheels.  

If you're stuck using a dual420 or dual420 100 then run it at 10S or less and keep the total battery amps below 40. And make sure you run motor detection without the belts on, they need to be unloaded because they're quirky. And it probably wouldn't hurt to say a few Hail Skatans while you're doing that.
```

---
## \#50 Posted by: brenternet Posted at: 2019-05-06T20:15:10.867Z Reads: 55

```
Have you tested the plus versions Damon? If not I would urge it or your advice here is based on an old BOM that was gash.
```

---
## \#51 Posted by: Sn4pz Posted at: 2019-05-06T20:15:41.835Z Reads: 52

```
Damon's reply should just be the first reply to this thread. 

Take his advice OP, he certainly knows what he's talking about when it comes to breaking things... 😂
```

---
## \#52 Posted by: longhairedboy Posted at: 2019-05-06T20:19:42.901Z Reads: 51

```
We ran the plus last. It popped some caps but it had some nice features, i think it had the "remote on " feature for one thing.
```

---
## \#53 Posted by: AgressivStreetLamp Posted at: 2019-05-06T20:24:09.285Z Reads: 49

```
Awesome thanks for the advice guys.
Glad we could nail this info down in one spot. This has kept me from melting a vesc needlessly. Hopefully it will do the same for future builds.

   Sounds like the 4.12 will be moving to the 8s build and a focbox or flipsky 6 will be on order soon for the 12s build.
```

---
