# 2x 3S lipo problem

### Replies: 49 Views: 492

## \#1 Posted by: SanderG Posted at: 2018-07-31T19:29:16.623Z Reads: 85

```
Hi,
I have a problem with my battery's i use two turnigy 3S 5000mah (40-50C) in series, but for some reason they start to puff up a bit, the batterys do not have many cycles on them. im still using them how they are now and still work, i do take care of them, balance charge them at 1C. 

some of my parts:
Motor: Turnigy Aerodrive SK3 - 5055, 70A, 5-8S lipo, 430kv, 1750W
ESC: X-car beast 120A (burst 760A), 2-6S lipo

Here are some pictures, you cannot see it that well, buts its a slight bulge and can be pressed in a bit.
![IMG_6053|375x500](upload://3pfbKq3hPY7GBTfUDXoALBdhCvk.JPG)![IMG_1962|375x500](upload://ta68YgvxmbDQcKlNrqE9vGV3zv8.JPG)![IMG_4201|375x500](upload://5hD16OzXOw4acWvuwgtRoPNUxSt.JPG)![IMG_4682|375x500](upload://ikQmudoxBKnGd6Qq4S9kdRGXtPL.JPG)![IMG_5348|375x500](upload://3IDlkeNlee2YXMBQ9aUfygHaUPA.JPG)![IMG_2738|375x500](upload://bUI1m7KFZ5BQJMgjK5A03sEQbNz.JPG)
```

---
## \#2 Posted by: E1Allen Posted at: 2018-07-31T21:20:25.973Z Reads: 69

```
Not ideal, at least one of the cells in each pack is degraded.  Sometimes it just happens.  You're probably going to need to replace them soon.  Also if you're going to use them have a fire plan in case they go nuts while charging or being discharged.
```

---
## \#3 Posted by: AutoItKing Posted at: 2018-08-01T04:02:32.027Z Reads: 62

```
Please stop using that battery! Once they start puffing up the degradation accelerates. You're liable to burst into flames at any point.
What's happening is that the electrolyte is basically evaporating and eventually the two electrodes can touch causing a short and a lot of heat. Toss it and eat your losses, seriously, don't take battery safety lightly. These cells have a huge amount of energy stored in them and you don't want to let it out uncontrolled.
If the batteries are new-ish you may be able to get some sort of warranty on them. Not sure what Turnigy's terms are though...

Edit: also I should note, take the C rating with a grain of salt, they tend to lie a bit. Which is why I have two 190A rated batteries in parallel.
```

---
## \#4 Posted by: deucesdown Posted at: 2018-08-01T04:43:36.474Z Reads: 60

```
What's your low voltage cutoff? Lipos are almost empty at 3.7v/cell.
```

---
## \#5 Posted by: AutoItKing Posted at: 2018-08-01T05:10:57.542Z Reads: 60

```
That is somewhat false. See image from http://learningrc.com/lipo-battery/. You can find others by searching "LiPo discharge curve" on your favorite search engine.
![image|690x421](upload://u3L5Bh2amN5DTMqrCzygfJQ29VH.png)
Under heavy loads the voltage drops to below 3.7V fairly quickly. Very light loads (less than 1C) will keep a higher voltage for longer and the battery may float back up when load is removed, but the float voltage is not a good indication of charge remaining.

You can safely cutoff around 3 volts (experienced users only!), not much lower though. That being said, over discharging your cells can cause damage, as can over charging. Check cell voltages after charging with an independent measurement device (multimeter). 0.01 volts over isn't going to hurt, but 0.1 might.

Edit: Here's a plot of low load discharge (not super realistic for our purposes either):
![image|579x445](upload://5SnKM461ethe5ZtxtwdjQUMm79w.png)
```

---
## \#6 Posted by: deucesdown Posted at: 2018-08-01T05:40:52.527Z Reads: 53

```
that chart is 25c or more on a 1.7ah cell. 25c on a 5ah cell is 125a. I don't think this is representative. 

I do agree that voltage under load varies a lot. But if you want long healthy life from hobby packs, you want to stay far from the knee of the discharge curve, and also not leave the packs at full charge for more than a few hours. Well at least that's what I've read on teh internets.
```

---
## \#7 Posted by: telnoi Posted at: 2018-08-01T08:35:49.626Z Reads: 48

```
[quote="AutoItKing, post:5, topic:63430"]
You can safely cutoff around 3 volts
[/quote]

I found that below 3.6 under load, a Lipo will heat up relatively quickly and you will shorten the lifespan significantly. Most will begin to puff.

That is based on destroying 12 packs a year for the past 4 years (Graphene packs - race drones). 

ESK8 example. A couple of days ago, I had to make it back after a 35 km trip. The last two km I had to drop my cell voltage down to 3.5V. Puffed my lipos (granted, they were a year old but no issues before that).
```

---
## \#8 Posted by: PatRocks Posted at: 2018-08-01T10:43:55.171Z Reads: 45

```
[quote="AutoItKing, post:5, topic:63430"]
That is somewhat false.
[/quote]

Bro. I would advise that whatever @deucesdown says should be regarded as an informed statement (especially when he's helping me harrass @psychotiller lol). everything else that you mentioned in your reply is accurate, except the "discharging to 3v safely" part. It is safe to do this if you are testing the endurance/longevity of a battery (like, for science), but that's only "safe" under controlled conditions, and with precision instruments. The original post-er has obviously puffed these packs under non-extreme conditions, and these are not batteries which are test-dummies, they're for transportation (where loads change like the salmon of capistrano). As your other comments indicate, I'm respectfully assuming that you know what you're talking about in regards to these chemistries, but I would also tend to advise a very generous safety-margin when publishing statements that may cause problems for other readers. My point here being, that in testing-scenarios you're right. But eSk8 is real-world-scenario, and for someone who wants to keep their battery healthy, happy and slim, high amp discharging below a VERY conservative threshold (50%) isn't good practice. 

...aaand for a 40-50c lipo, a 25c load is probably way unsafe. Also, what @telnoi said. 
Please understand @AutoItKing , that I mean no rudeness or disrespect, but whith so many fires recently, CAUTION FIRST!! Heard?

Edit: having read some of your posts, it's obvious that you know what you're talking about. let me restate that my only concern with your above post is that kiddies may burn their stuff without the level of understanding that comes with in-depth research. Btw, just curious, what IS the nature of your extensive electrical experience @AutoItKing? your profile is vague but interesting
```

---
## \#9 Posted by: PatRocks Posted at: 2018-08-01T10:58:57.727Z Reads: 39

```
And another thing: @SanderG , What the hell are you doing with such a small, and such a high-kV motor on an esk8 anyway?? without a ridiculously-low gear ratio you're gonna puff ANY lipo at that low of voltage to do x-amount of watts (6s, right? tldr). go higher voltage, <190kV and a more gentile esc, and you'll have less battery puffage :wink:  

ps: output watts can be equated to the ability to do work over time (like horsepower for example). this is a generalization tho, and I've been drinking. while your esc can handle a shitload of amps, those batteries aren't suited for it!!

Edit: no disrespect to YOU either, my b
```

---
## \#10 Posted by: deucesdown Posted at: 2018-08-01T12:28:59.978Z Reads: 40

```
Hey @PatRocks thanks but I mean it when I say I just read it on the internet. I've read a lot though with a focus on safety and longevity. I'll instantly and always defer to those with experience.

[quote="telnoi, post:7, topic:63430"]
That is based on destroying 12 packs a year for the past 4 years (Graphene packs - race drones).
[/quote]

Like this guy :)

But, I'm stupid, 6s so those high amps are in the range of possible.
```

---
## \#11 Posted by: SanderG Posted at: 2018-08-01T13:17:00.305Z Reads: 34

```
i charge them in a lipo safe bag..
```

---
## \#12 Posted by: SanderG Posted at: 2018-08-01T13:18:28.047Z Reads: 34

```
how many cells do u use? 2X 6S in parallel?
```

---
## \#13 Posted by: SanderG Posted at: 2018-08-01T13:18:59.183Z Reads: 34

```
my ESC cuts off at 3.7
```

---
## \#14 Posted by: SanderG Posted at: 2018-08-01T13:20:37.908Z Reads: 34

```
my battery's are always charged to 4.2
```

---
## \#15 Posted by: SanderG Posted at: 2018-08-01T13:22:52.090Z Reads: 32

```
The motor is 70A, my batteries can handle up to 250A no?
```

---
## \#16 Posted by: SanderG Posted at: 2018-08-01T13:24:16.078Z Reads: 33

```
what is the best thing to do here? these are my second pair of batteries that puffed...
```

---
## \#17 Posted by: SanderG Posted at: 2018-08-01T13:27:07.018Z Reads: 32

```
will something like this work better?
(https://www.ebay.com/itm/90mm-dual-6364-hub-motors-drive-kit-for-electric-skateboard-longboard-part/302546262750)
```

---
## \#18 Posted by: TarzanHBK Posted at: 2018-08-01T13:34:24.010Z Reads: 30

```
[quote="SanderG, post:13, topic:63430, full:true"]
my ESC cuts off at 3.7
[/quote]

there might be your problem.
The highest Cutoff the X-Car is able to do is 3,4V general voltage. That means if you stress these lipos a bit, they decharge unevenly between the cells. So one cell could be at 3,0V when the ESC cuts off.
3,4V is already too low. So don´t rely on the X-Car cutoff!
```

---
## \#19 Posted by: SanderG Posted at: 2018-08-01T13:36:44.259Z Reads: 29

```
it cuts off when im giving full power when i have ridden for around 10km, so i think they go to that rate under heavy load, when i messure under no load they are 3.7V
```

---
## \#20 Posted by: TarzanHBK Posted at: 2018-08-01T13:38:49.158Z Reads: 27

```
They sag down under load and the ESC cuts off, after that the battery goes up again.
Get a voltmeter to monitor your cells to know whats going on.
If they sag too much down, they drift from each other and go bad over time.
```

---
## \#21 Posted by: SanderG Posted at: 2018-08-01T13:40:04.837Z Reads: 23

```
il put a meter on it while riding and see whats going on, if it sags much, whats the best thing to do? whats bad in my setup? maybe get dual hub motors (90mm dual 6364 hub motors 550W each), and a better ESC?
```

---
## \#22 Posted by: TarzanHBK Posted at: 2018-08-01T13:41:57.528Z Reads: 23

```
get better batteries that don´t sag as much and don´t discharge them too low. The ESC is cool, just get a lower kv motor
```

---
## \#23 Posted by: SanderG Posted at: 2018-08-01T13:42:51.075Z Reads: 26

```
What kind of motor and batteries do u recomend?
```

---
## \#24 Posted by: TarzanHBK Posted at: 2018-08-01T13:46:06.910Z Reads: 27

```
If you want to go the lipo route again. Get some higher C batteries like Graphenes.
A good and cheap motor is something like a hobbyking motor SK3 or Sk8 6364 or 6374 with about 245 - 260kv for 6s.
```

---
## \#25 Posted by: SanderG Posted at: 2018-08-01T13:48:49.429Z Reads: 28

```
what kind of speeds can u get with those? and its okay to use 2x 3S in series right?
```

---
## \#26 Posted by: E1Allen Posted at: 2018-08-01T13:58:12.186Z Reads: 28

```
http://calc.esk8.today

This calc is good for speed.  Also there is nothing wrong with wiring in series.
```

---
## \#27 Posted by: SanderG Posted at: 2018-08-01T14:02:12.378Z Reads: 28

```
il try that thanks, also is this a good setup, looking to make a new one:
(https://www.ebay.com/itm/For-Hub-Motor-Dual-motors-longboard-skateboard-control-modula-ESC-Substitute/332377676534?hash=item4d6340daf6%3Ag%3AleIAAOSw3ZtaKl7T&_sacat=0&_nkw=dual+hub+motor+esc&_from=R40&rt=nc&_trksid=m570.l1313)

(https://www.ebay.com/itm/90mm-dual-6364-hub-motors-drive-kit-for-electric-skateboard-longboard-part/302546262750?epid=23007163377&hash=item4671299ade%3Ag%3A5AYAAOSw3gJZJKe5&_sacat=0&_nkw=90mm+dual+6364+hub%60&_from=R40&rt=nc&_trksid=m570.l1313#shpCntId)
```

---
## \#28 Posted by: Andy87 Posted at: 2018-08-01T14:13:42.234Z Reads: 27

```
I would investigate in a set of vesc or focboxes 
With them you also can log your voltage and look how is your voltage sag. With it you can adjust your battery cut off if it’s not ideal.
10-12s with a 150-200kv Motor(s) 6374 or something around this should give you a good performance.
Higher voltage should lower the current from your batteries.
If that still not enough than you need to find higher c rated lipos
```

---
## \#29 Posted by: SanderG Posted at: 2018-08-01T14:15:18.231Z Reads: 29

```
[quote="TarzanHBK, post:24, topic:63430"]
this is what i have now, but i maybe want to go dual hub motors, the vesc is only single motor right?
[/quote]

![13|690x407](upload://3BuhxetaG6Gsiy1c0eKrtycuifN.png)
```

---
## \#30 Posted by: E1Allen Posted at: 2018-08-01T14:18:43.616Z Reads: 29

```
Currently vesc is single motor
```

---
## \#31 Posted by: SanderG Posted at: 2018-08-01T14:20:24.227Z Reads: 29

```
i do not need the open source, i do not need to program it, for me a simple esc is good, i just wanna make a simple board with dual hub motors, maybe 18650? but i do not have a spot welder..
```

---
## \#32 Posted by: Andy87 Posted at: 2018-08-01T14:22:02.072Z Reads: 29

```
There are no welding modules here in the forum.
They seem to be good and easy to use
```

---
## \#33 Posted by: Andy87 Posted at: 2018-08-01T14:24:44.693Z Reads: 27

```
![image|230x500](upload://gcs3KmY2Y7TBmOIoJduDPmGP1Vt.jpg)
```

---
## \#34 Posted by: SanderG Posted at: 2018-08-01T14:25:40.973Z Reads: 27

```
cool! need to check them out, are 18650 a better solution, expencive but safer right?
```

---
## \#35 Posted by: Andy87 Posted at: 2018-08-01T14:28:50.431Z Reads: 26

```
Just was close to burn down my house with 18650s...so wouldn’t say safer😅
Just look that you get original.
There a lot of fakes out there.
Use high drain batteries like Samsung q30, Sony vtc5, vtc5a or vtc6 
And look that you fuse your pack
Better would be also to use a bms
```

---
## \#36 Posted by: Andy87 Posted at: 2018-08-01T14:31:08.006Z Reads: 28

```
They all store a lot of energy. 
Work safe and be prepared.
Doesn’t matter if lipo or LiIon.
Believe me some 50-100bugs for safety can safe you thousands of dollars
```

---
## \#37 Posted by: SanderG Posted at: 2018-08-01T14:31:34.121Z Reads: 29

```
yes also a BMS, and maybe the original sony US18650VTC5 2600mAh - 30A, 6 in series and 2 in parallel?
```

---
## \#38 Posted by: Andy87 Posted at: 2018-08-01T14:33:47.841Z Reads: 29

```
They also sag. Wouldn’t go under 3p
```

---
## \#39 Posted by: SanderG Posted at: 2018-08-01T14:34:22.259Z Reads: 29

```
oh okay so 6S3P to start out?
```

---
## \#40 Posted by: Andy87 Posted at: 2018-08-01T14:40:30.145Z Reads: 29

```
Vtc5 are rated to 30a I think
But that’s not 100% true.
There are some tests which show that they should be rated only about 15-20a I think. 
Look it up here in the forum. There some articles about it. The same with the vtc6.
30q rated 15a but you can safe get them to 20.
And they more cheep.
If you have the place make a 6-8s 4p Samsung 30q. That’s what I would make as min. Should be good for dual hub.
```

---
## \#41 Posted by: SanderG Posted at: 2018-08-01T14:42:40.038Z Reads: 28

```
okay cool! il look into that, the batteries are around 3,5€, so for a 6S4P thats around 85€, what is a good BMS, i have no experience with that :stuck_out_tongue:
```

---
## \#42 Posted by: Andy87 Posted at: 2018-08-01T14:45:22.761Z Reads: 27

```
You in the states? If no nkon.nl is a good source for batteries. 2,90€ for a q30 and they legit 
About bms I can’t say so much
Look bestech here in the forum 
Maybe there is a group buy at the moment 
If no you can find them on Alibaba.com
```

---
## \#43 Posted by: SanderG Posted at: 2018-08-01T14:46:34.064Z Reads: 29

```
im from belgium, and yes i have got 18650 from nkon before (vape) what should be the rates for a BMS, you maybe wanna chat private, thats a bit easier ;)
```

---
## \#44 Posted by: deucesdown Posted at: 2018-08-01T15:21:50.163Z Reads: 28

```
If you stay 6s, I think HK Graphene 65c will be good for you. Or if you stay with the blue packs, put them in parallel, 6s2p. You'll need to be more consious if you go 2p though. Some rules of thumb to make them last:

- charge to 4.1/cell. This will increase cycle life by like 50-100%.
- try to figure out how much energy you spend per mile. charge to 4.1/cell, ride for a set distance, like 3 miles, then charge, and take note of how much watt-hours your charger puts back in. Divide by the distance, and you'll see watt-hours per mile.
- don't discharge more than say 60%, based on above. This will give lots of safety margin and your packs will be less stressed. The bottom 30% of a pack is usually not so great anyway, lots of sag, etc.
- try to store the cells around 50% charge

I think, hobby lipos are expected to do about 50 cycles. 150 cycles if you treat them real nice. If you treat them like I said above, I would not be surprised to get 300 or more cycles.

The HK Graphenes seem to do a lot better, like 1000 fairly abusive cycles. So they cost more but are way cheaper in the long run (unless you get unlucky or make a mistake).
```

---
## \#45 Posted by: SanderG Posted at: 2018-08-01T15:27:44.101Z Reads: 28

```
the graphenes are like 65$ for a 3S 5000mah 75C, thats kinda expencive :p is 18650 not a better solution? also for charging and using?
```

---
## \#46 Posted by: deucesdown Posted at: 2018-08-01T16:10:12.694Z Reads: 28

```
You won't match the high current capabilities of lipo with 18650 without going really big on p groups. And assembly is a lot more involved and fraught with danger. But generally they're a lot more tolerant of abuse and have longer cycle life (HK Graphene kind of changes the cycle life picture). Also some people have had bad luck with Graphene packs. It may vary batch-to-batch...

Above 8s it gets hard to charge with hobby chargers, but with 6s you can do interesting creative one-plug charging tricks using hobby chargers.

The 75c are new and more $$. The ideal thing is to catch a sale on 5000mah+ 65c+ packs.

18650 and lipos are both good though. Just different pros and cons.
```

---
## \#47 Posted by: AutoItKing Posted at: 2018-08-01T18:39:24.528Z Reads: 24

```
[quote="deucesdown, post:6, topic:63430"]
Well at least that’s what I’ve read on teh internets.
[/quote]
Can't always trust what you read on teh interweebs!

[quote="telnoi, post:7, topic:63430"]
That is based on destroying 12 packs a year for the past 4 years (Graphene packs - race drones).
[/quote]

12? Damn dude, you got me there! I've only destroyed two... maybe I got lucky?

[quote="PatRocks, post:8, topic:63430"]
having read some of your posts, it’s obvious that you know what you’re talking about. let me restate that my only concern with your above post is that kiddies may burn their stuff without the level of understanding that comes with in-depth research. Btw, just curious, what IS the nature of your extensive electrical experience @AutoItKing? your profile is vague but interesting
[/quote]

I take no disrespect, no worries! I agree, caution first for sure, we've seen way too many fires recently. I think part of the problem is also cheap cells from unknown Chinese sources.
Although I would never advocate harassing @psychotiller, he seems like a stand up guy! :joy:
Since you asked: MSEE and currently PhD student. Several start ups and contract work doing embedded systems, electromagnetics, etc.

Back on topic: being conservative is always a good idea, I tend to design in at least a 3:1 safety margin. Not much I can add here, you guys covered it pretty well. I would say, if you KNOW what you're doing you can push these limits but for newbies or even those not 100% confident in their battery knowledge, stay conservative. I cutoff at 3V, but I "know" what I'm doing... :neutral_face:
```

---
## \#48 Posted by: telnoi Posted at: 2018-08-01T18:44:06.060Z Reads: 22

```
[quote="AutoItKing, post:47, topic:63430"]
12? Damn dude, you got me there! I’ve only destroyed two… maybe I got lucky?
[/quote]

I flew almost daily :slight_smile: so the abuse of high amp draws at low voltage & loads of charge cycles  made it rather easy to kill them. 

''Luckily'', esk8 replaced that hobby almost entirely. Now I only kill 4 lipos per year :sweat_smile:
```

---
## \#49 Posted by: AutoItKing Posted at: 2018-08-01T18:49:24.014Z Reads: 22

```
Yeah that'll do it! Haven't had a battery blow up on me yet, knock on wood!
```

---
