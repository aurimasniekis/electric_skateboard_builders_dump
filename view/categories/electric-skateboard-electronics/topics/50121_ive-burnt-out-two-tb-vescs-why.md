# I&rsquo;ve burnt out two TB VESCs&hellip; why?

### Replies: 47 Views: 1302

## \#1 Posted by: TheFluffiest Posted at: 2018-03-25T22:16:16.658Z Reads: 243

```
Hello there!

Long story made short: I have been trying to build a board with dual sk3 5055 280kv motors. It worked for awhile, but the phase wires on one of them shorted. Dead DRV. So I ordered a better motor (KEDA 6364 190kv) because it's cheaper than a new VESC. Yesterday, the second vesc died for no apparent reason. I tested it without load before the ride to make sure everything was working, got on, and it wouldn't go. . Went home, plugged in the board, and it threw a DRV8302 error. Joy. I had the phase wires taped over this time, so it wasn't a short. There was no visible damage to either of the chips. So I am wondering what caused the second one to burn out.

My current setup is: 
KEDA 6364 190kv motor (ran in BLDC mode)
TB VESC
Two 4s 5000mAh 20c LiPo batteries wired in series
TB nano remote and reciever
Anti-Spark loop key
HK lipo voltage meter
 
Not sure if any of this matters, but the other specs are:
TB 218mm trucks
TB 63mm mount
90mm flywheel clones
Arbor Axis 40 deck

I don't have the money to upgrade to an Ollin vesc, so my next thing will be a FOCBOX unless I can figure out why the TB vescs keep dying. I would like to stick to vescs, because they are super nice for this purpose. 

Pictures:
[Wiring](https://photos.app.goo.gl/gL95QCBDlHkPmkSw1)
Looking at BLDC Tool, it seems whatever happened reset the vesc settings too. I verified my settings by comparing with multiple other threads and videos, so I highly doubt that is the problem.

Input from @torqueboards would also be greatly appreciated.

I don't have the equipment or knowledge to fix the DRV8302 chip, so I was planning on selling the vescs to contribute to the FOCBOX fund, unless I can get the TB VESCs replaced somehow. I read somewhere else that $30 was a fair price. Thoughts on that?

Thanks in advanced!
```

---
## \#2 Posted by: b264 Posted at: 2018-03-25T22:21:07.748Z Reads: 225

```
[quote="TheFluffiest, post:1, topic:50121"]
upgrade to an Ollin vesc
[/quote]

Ollin stopped selling HW4.12
```

---
## \#3 Posted by: GrecoMan Posted at: 2018-03-25T22:23:21.562Z Reads: 219

```
1. those pants you’re wearing in that wiring picture are awesome

2. can we get screenshots of BLDC settings?
```

---
## \#4 Posted by: TheFluffiest Posted at: 2018-03-25T22:30:54.910Z Reads: 216

```
1.) Thank you sir. I take great pride in them :joy:

2.) The BLDC settings were reset somehow, so nothing useful would come out of that. When I went to take screenshots the settings were the same as the default settings, which definitely wasn't the case. I compared them to other threads and videos to make sure they would work beforehand. I know they were fairly conservative values though.
```

---
## \#5 Posted by: TheFluffiest Posted at: 2018-03-25T22:31:40.303Z Reads: 203

```
So it will probably be even more expensive to get a vesc from him?
```

---
## \#6 Posted by: b264 Posted at: 2018-03-25T22:31:45.518Z Reads: 194

```
Are you sure you were clicking "Read" on every screen, then "Write" before you went to a different screen?  Just changing the numbers does not change the numbers.
```

---
## \#7 Posted by: b264 Posted at: 2018-03-25T22:32:03.868Z Reads: 194

```
[quote="TheFluffiest, post:5, topic:50121, full:true"]
So it will probably be even more expensive to get a vesc from him?
[/quote]

You can't get them.  They are unobtainium.
```

---
## \#8 Posted by: TheFluffiest Posted at: 2018-03-25T22:33:11.046Z Reads: 193

```
Yes I was. I double checked all the setting before I closed the program to ride too, just to make sure
```

---
## \#9 Posted by: TheFluffiest Posted at: 2018-03-25T22:33:41.570Z Reads: 186

```
Ah. What about the VESC6 hardware? or does he have his own motor controller now?
```

---
## \#10 Posted by: TheFluffiest Posted at: 2018-03-25T22:34:22.542Z Reads: 186

```
@b264 @GrecoMan

It should be noted that this VESC was used less that 7 miles before it burned out
```

---
## \#11 Posted by: b264 Posted at: 2018-03-25T22:34:28.644Z Reads: 183

```
The only thing you can get from Ollin are the [things they have listed for sale](http://www.ollinboardcompany.com/products), which is nearly limited to belts and wheels.

He has them as far as I'm aware, but won't sell them.  He announced in late December he was going to be selling completes only, but those are not currently for sale, so I don't know what is going on at Ollin.
```

---
## \#12 Posted by: GrecoMan Posted at: 2018-03-25T22:41:32.308Z Reads: 174

```
he’s doing some cool stuff behind the scenes
```

---
## \#13 Posted by: TheFluffiest Posted at: 2018-03-25T22:44:39.837Z Reads: 176

```
@GrecoMan @b264

It looks like he has his own [esc based on HW4.12](http://www.ollinboardcompany.com/product/ollin-esc-v1-1). Although it is sold out. 

Any ideas as to why this is happening to my VESCs?
```

---
## \#14 Posted by: GrecoMan Posted at: 2018-03-25T22:46:40.857Z Reads: 169

```
did you hit wrote config after setting it up?
```

---
## \#15 Posted by: b264 Posted at: 2018-03-25T22:46:56.596Z Reads: 168

```
[quote="TheFluffiest, post:13, topic:50121"]
It looks like he has his own esc based on HW4.12. Although it is sold out.
[/quote]

You can’t get them. They are unobtainium.  He announced in December they won't be for sale.  So onto your TB hardware...
```

---
## \#16 Posted by: torqueboards Posted at: 2018-03-25T23:40:31.269Z Reads: 160

```
Mention the step by step process on how you started/used it/programmed it.

As far as your motor wires.. what soldering iron are you using?

BTW Those voltage meters you want to eventually disconnect from your battery pack when it's not in use otherwise they'll lower voltage on 1 or 2 cells and ruin your battery pack.
```

---
## \#17 Posted by: TheFluffiest Posted at: 2018-03-26T01:40:24.344Z Reads: 148

```
@torqueboards 

Starting with the first setup (dual drive)
-ordered, did tons of research to make sure I do everything right (knowing how fragile vescs tend to be)
-wired everything up
-verified the wiring with multiple videos and threads
-turned on the board using an antispark loop key
-connected to windows 10 pc with BLDC tool
-put in conservative values for a dual drive
-board worked perfectly until phase wires shorted and blew one vesc

Second setup (single drive)
-same process, up until after the conservative values part
-taped phase wires to make sure they didn't short
-Board worked perfectly again with new motor, until it stopped for no apparent reason

I never accelerated hard, and never went faster than 26 mph (crashed pretty hard at that speed and never had the guts to try it again). I rode dual drive for roughly 5 miles, and rode single for less that 2 miles.

Like i said in other replies, the exact values were lost due to the vesc resetting to default. I can't give a screenshot for that reason, but I can tell you for certain that the values were conservative because of the fragility of the vescs. 

[Soldering iron](https://www.amazon.com/Sywon-Soldering-Adjustable-Temperature-Desoldering/dp/B01E1ISGH0)

I disconnect the voltage meter after each ride.
```

---
## \#18 Posted by: TheFluffiest Posted at: 2018-03-26T01:41:11.636Z Reads: 141

```
Yes I did. I double checked all values before I exited out of BLDC tool, just to make sure
```

---
## \#19 Posted by: TheFluffiest Posted at: 2018-03-26T01:42:12.672Z Reads: 137

```
Got it. Any ideas as to why this is happening?
```

---
## \#20 Posted by: b264 Posted at: 2018-03-26T01:55:39.838Z Reads: 136

```
[quote="TheFluffiest, post:18, topic:50121"]
I double checked all values before I exited out of BLDC tool, just to make sure
[/quote]

If you don't click "read" on EVERY SCREEN then it's not double-checking anything
```

---
## \#21 Posted by: TheFluffiest Posted at: 2018-03-26T02:21:41.447Z Reads: 121

```
I did do that. That's why I'm so confused
```

---
## \#22 Posted by: Pedrodemio Posted at: 2018-03-26T02:28:37.735Z Reads: 119

```
Lots of people had VESC from toqueboards, they say they are improving quality control

Mine didn’t even manage to spin the motor during detection before getting DRV error, and having to ship it back to get a replacement makes matter worse since for  some countries international shipping cost almost half a VESC

Hope they improve because competition is good
```

---
## \#23 Posted by: Squidprorow Posted at: 2018-03-26T03:46:33.530Z Reads: 116

```
I just got a TB esc and it had a DRV error after like 1 hour of riding. I sent it back and for $50 they are going to send me a replacement. Kinda dissapointed but w/e. Next time i'll probably get a regular esc or a FOCBOX | 
VESC6
```

---
## \#24 Posted by: Jc06505n Posted at: 2018-03-26T03:57:02.187Z Reads: 117

```
I think the lesson here is: stay away from TB VESC’s. Any research into them should eventually lead to that conclusion.
```

---
## \#25 Posted by: ARetardedPillow Posted at: 2018-03-26T04:05:42.983Z Reads: 114

```
Hey, DRV error doesn't just go away when you get a new motor, that stuff is damage to the VESC not the motor
```

---
## \#26 Posted by: ARetardedPillow Posted at: 2018-03-26T04:06:38.233Z Reads: 112

```
[quote="TheFluffiest, post:1, topic:50121"]
So I ordered a better motor (KEDA 6364 190kv) because it’s cheaper than a new VESC.
[/quote]
Yea.... DRV error doesn't go away when you buy a new motor
```

---
## \#27 Posted by: trancejunkiexxl Posted at: 2018-03-26T04:09:23.789Z Reads: 109

```
I'm running a tb vesc, it's been solid so far 🤔
```

---
## \#28 Posted by: TheFluffiest Posted at: 2018-03-26T04:46:49.773Z Reads: 106

```
It was a dual setup, one vesc died, got a stronger motor to use with the working vesc, it died too.
```

---
## \#29 Posted by: TheFluffiest Posted at: 2018-03-26T04:47:07.244Z Reads: 108

```
how long is "so far"?
```

---
## \#30 Posted by: trancejunkiexxl Posted at: 2018-03-26T04:48:09.846Z Reads: 107

```
Couple months, then again I've ruined like 5 vesc so far =3
```

---
## \#31 Posted by: TheFluffiest Posted at: 2018-03-26T04:49:30.651Z Reads: 106

```
@Jc06505n @Pedrodemio @Squidprorow

If im not able to get a replacement from them, I will probably get a focbox. If @torqueboards can help me out though, hopefully i won't need to
```

---
## \#32 Posted by: TheFluffiest Posted at: 2018-03-26T04:49:49.222Z Reads: 105

```
How did the other ones die?
```

---
## \#33 Posted by: trancejunkiexxl Posted at: 2018-03-26T04:55:04.610Z Reads: 107

```
One was belt tension too tight, another was Drv,  recent one was soldering improperly. 👿 i break everything though
```

---
## \#34 Posted by: TheFluffiest Posted at: 2018-03-26T05:30:07.748Z Reads: 108

```
How does belt tension kill a vesc?
```

---
## \#35 Posted by: lrdesigns Posted at: 2018-03-26T06:09:35.365Z Reads: 106

```
I don't know what caused your DVR errors, but your battery to esc wires look excessively long. Which can introduce voltage spikes that are hard on the esc. Could be bad for long term usage but shouldn't give an instant death. 

This pinch point where all the wires go through a small metal hole would make me paranoid of shorts, could the enclosure compromised the insulation of some of the wires here?

![image|686x499](upload://xZ5Z6ZSzJ40WHVA3EyorEkt8Vh3.jpg)
```

---
## \#36 Posted by: TheFluffiest Posted at: 2018-03-26T06:22:52.040Z Reads: 102

```
Well shit. You are paranoid for good reason. Two of the three wires are completely torn up. That is the exact reason for the DRV error. Good information about the wiring, thanks!

In the future, once I get a new ESC, I will cut a larger hole and 3d print a thing around it to make sure the wires can't rub together. That was a pretty huge oversight, thank you for your wisdom!
```

---
## \#37 Posted by: Tuomalar Posted at: 2018-03-26T07:45:18.983Z Reads: 100

```
Once AGAIN "poor quality vescs" was actually user based faults like in 99% of times. There is always some good reason why vesc's broke, people just assume that it is manufacturers fault without proper diagnostics.

But nice to know what was the reason at this time.

[quote="Jc06505n, post:24, topic:50121, full:true"]
I think the lesson here is: stay away from TB VESC’s. Any research into them should eventually lead to that conclusion.
[/quote]
```

---
## \#38 Posted by: Jc06505n Posted at: 2018-03-26T09:44:20.334Z Reads: 96

```
[quote="Tuomalar, post:37, topic:50121"]
Once AGAIN “poor quality vescs” was actually user based faults like in 99% of times. There is always some good reason why vesc’s broke, people just assume that it is manufacturers fault without proper diagnostics.
[/quote]

That doesn’t mean that TB VESC don’t have their issues , but it’s nice to know it was user error rather than MANU error. I would still advocate them for people to stay away from them, at least until they pull down any FOC related setup material for their ESC.
```

---
## \#39 Posted by: Bjork3n Posted at: 2018-03-26T09:58:18.774Z Reads: 95

```
Tb vesc are one of the worst vesc I used. 
Failed within a week. 
Cheap components I guess. 

My maytech vesc been more reliable with exact same settings.
```

---
## \#40 Posted by: pat.speed Posted at: 2018-03-26T10:07:32.325Z Reads: 93

```
Well I’ve got 2 vescs coming my way thanks to @Funktapus. Let’s hope these last longer than some of the others I’ve seen. I will be adding extra caps to try and help with voltage spikes too though
```

---
## \#41 Posted by: TheFluffiest Posted at: 2018-03-26T17:20:26.536Z Reads: 83

```
Make sure the phase wires don't short :joy:
```

---
## \#42 Posted by: pat.speed Posted at: 2018-03-26T20:57:23.560Z Reads: 74

```
I will. lol
```

---
## \#43 Posted by: torqueboards Posted at: 2018-03-27T02:29:05.588Z Reads: 66

```
@TheFluffiest - I'd double check the solder on the connectors also I've gotten some cold solder wires back some fell directly off as soon as you touched them.
```

---
## \#44 Posted by: b264 Posted at: 2018-03-27T02:35:39.247Z Reads: 64

```
To expand on this, any time you solder something together, wait for it to cool briefly then try to yank the wire back off, kind-of hard and firm but not crazy hard.  If you can't pull it apart, it's *more likely* it's a good solder joint.
```

---
## \#45 Posted by: TheFluffiest Posted at: 2018-03-27T02:47:46.585Z Reads: 66

```
I figured out the problem, the insulation on the motor wires stripped and shorted. I will keep that in mind though
```

---
## \#46 Posted by: Apolo Posted at: 2018-03-27T03:31:12.465Z Reads: 66

```
Can I have your pants
I'll trade a vesc6 or two
```

---
## \#47 Posted by: TheFluffiest Posted at: 2018-03-27T06:38:39.883Z Reads: 60

```
Haha I wish. I freaking love these pants!
```

---
