# Adding a Speed Limit

### Replies: 32 Views: 1070

## \#1 Posted by: CookyMellow Posted at: 2019-02-19T00:05:59.094Z Reads: 230

```
Hi everyone, im planning on building an electric longboard with HUB motors for a school project. The school requires the board to have a speed limit of 15km/h and I have no idea how I am going to add a speed limit on this. But I also want to be able to take this off in the future so I dont want it to be permanent.
```

---
## \#2 Posted by: Skunk Posted at: 2019-02-19T00:07:24.055Z Reads: 226

```
If using vesc you can just limit the Throttle
```

---
## \#3 Posted by: CookyMellow Posted at: 2019-02-19T00:08:26.375Z Reads: 219

```
is this only for certain ESC's or can I do it for all?
```

---
## \#4 Posted by: AlanZhou Posted at: 2019-02-19T00:10:14.145Z Reads: 217

```
VESC ( Vedder Electric Speed Controller) Only vesc and maybe a Arc 200
```

---
## \#5 Posted by: Skunk Posted at: 2019-02-19T00:20:31.206Z Reads: 216

```
If you're going to use an ESC rather than a quality vesc you could go lipos and configure in 6s and then reconfigure later for 10s or 12s
```

---
## \#6 Posted by: mishrasubhransu Posted at: 2019-02-19T00:27:28.823Z Reads: 209

```
VESC has inbuilt ways of limiting the max speed in an elegant way. Either change the erpm limit or use profiles
![Screenshot_20190218-192531|281x500](upload://oB87ngXPctrDVjFR6MDDqx2n3Ys.png) 
![Screenshot_20190218-192711|281x500](upload://4LUn0N7ti5DxCXx51eetXhg4WOi.png)
```

---
## \#7 Posted by: Jacobee Posted at: 2019-02-19T01:33:35.210Z Reads: 180

```
Be careful with erpm limits on the VESC before I had one of my boards set to go 15mph max and was riding around with my friend. He was accelerating (and leaning forward to compensate) and he hit the speed limit and it cut power to prevent him going faster causing him to go off the board. (He ended up being fine with just a couple scratches to show) for me personally this is the reason I will never limit the speed with erpm again
```

---
## \#8 Posted by: Pedrodemio Posted at: 2019-02-19T01:42:50.467Z Reads: 171

```
For me the ERPM cut is pretty smooth, just be sure to disable the use of brake to limit the speed, that's what makes things go bad
```

---
## \#9 Posted by: Jacobee Posted at: 2019-02-19T02:42:23.185Z Reads: 167

```
I'm pretty sure that setting was off but I can't say for sure. Anyway to me it's still not preferable because I would rather use lower kv and gearing to reduce the speed to your target speed so that you get the max torque and speed out of your board. (Although in @CookyMellow 's case since the target speed is very low erpm limit makes sense)
```

---
## \#10 Posted by: lrdesigns Posted at: 2019-02-19T02:56:52.589Z Reads: 159

```
It's a good idea to test a max eprm limit setting on the bench first. If it works well it should come to a smooth limit at the top end. If the brake to limit speed feature is enabled it will oscillate at max speed. Bap Bap Bap kind of thing. Though I think this brake feature was removed from newer version of vesc tool. So should not cause an issue for anyone now.

![image|690x315](upload://kwDO8aH3HedEpBAR1y1zet5bEhz.png)
```

---
## \#11 Posted by: b264 Posted at: 2019-02-19T02:58:51.264Z Reads: 139

```
Hub motors suck.  Do yourself a favor and use belts.  Later you can remove the speed limit in software after the project is over.
```

---
## \#13 Posted by: DerelictRobot Posted at: 2019-02-19T03:00:37.192Z Reads: 134

```
[quote="b264, post:11, topic:84611"]
Hub motors suck. Do yourself a favor and use belts.
[/quote]

School project. 

I disagree entirely for this reason. Hub motors are dead simple to get up and running, building a belt drive needlessly overcomplicates this when it's clearly not aimed at performance
```

---
## \#14 Posted by: b264 Posted at: 2019-02-19T03:01:42.433Z Reads: 124

```
Hub motors will make this a pile of trash later --- whereas if it's built properly, it can be turned into something awesome.

Also this, you could remove one side and run single motor.

https://www.electric-skateboard.builders/t/130-for-complete-caliber-v2-drive-kit/84105

But keep the other parts for later.
```

---
## \#15 Posted by: DerelictRobot Posted at: 2019-02-19T03:03:18.864Z Reads: 120

```
[quote="b264, post:14, topic:84611"]
Hub motors will make this a pile of trash later
[/quote]

Actually no, building with budget parts will do that regardless.

What you're suggesting vastly increases the technical difficulty of this project to someone starting out.

Not everyone is feeding a family of 9 via ESK8, *Brian*.
```

---
## \#16 Posted by: Jacobee Posted at: 2019-02-19T03:03:45.883Z Reads: 113

```
Hmm I don't know but it was older. this incident happened about a year ago and the VESC was setup with the bldc tool so it's possible that it was me accidentally checking the limit erpm with negative torque box.
```

---
## \#17 Posted by: maxchilton Posted at: 2019-02-19T03:48:18.779Z Reads: 111

```
build the board as fast as you want with whatever components you want then use a cheap rc controller/transmitter that has adjustable throttle end points.  Set end points to achieve your limited speed.
```

---
## \#18 Posted by: b264 Posted at: 2019-02-19T03:58:53.747Z Reads: 110

```
That would only add a power limit and not a speed limit.
```

---
## \#19 Posted by: maxchilton Posted at: 2019-02-19T04:25:26.292Z Reads: 110

```
without knowing the components used, the objective of the build, op's skill level or budget or anything else... limiting the throttle on the transmitter is the simplest/fool proof way to limit speed.
```

---
## \#20 Posted by: b264 Posted at: 2019-02-19T04:26:08.531Z Reads: 110

```
The simplest way to limit speed is to remove the wheels.  There are better ways though.  Limiting the throttle will only limit the power and not the speed.
```

---
## \#21 Posted by: CookyMellow Posted at: 2019-02-19T05:00:21.100Z Reads: 97

```
The main reason I want HUB motors was because I like being able to push it around aswell, rather than just purely using the motor. @b264
```

---
## \#22 Posted by: b264 Posted at: 2019-02-19T05:02:48.382Z Reads: 90

```
This is mostly a marketing myth spread by hub motor manufacturers.  You can use hub motors if you want.  They are crappy though.  Direct drive would be much better but there aren't any manufacturers selling single-motor direct drive and even if there were, they would be really expensive.
```

---
## \#23 Posted by: Jacobee Posted at: 2019-02-19T05:03:43.201Z Reads: 88

```
I think improved push ability is more or less a marketing gimmick / hype. If you run belts with the correct tension they are pushable too.
```

---
## \#24 Posted by: Jacobee Posted at: 2019-02-19T05:05:02.067Z Reads: 88

```
Lmao beat me too it. I've also heard gear drives (with proper backlash) have very little rolling resistance.
```

---
## \#25 Posted by: DerelictRobot Posted at: 2019-02-19T08:01:02.459Z Reads: 82

```
Both are definitely true. My gear drives feels like they have less resistance than my belt drive boards, but both are a matter of tuning. 

You will have less rolling resistance with hubs but it's negligible in most cases.

The cheap hub motors out there are to be considered a consumable, but there's no arguing how much easier they are to get rolling vs building out a belt drive for a first time builder.
```

---
## \#26 Posted by: DerelictRobot Posted at: 2019-02-19T08:03:04.280Z Reads: 85

```
[quote="b264, post:20, topic:84611"]
Limiting the throttle will only limit the power and not the speed.
[/quote]

Totally correct. Current driven control systems control power, not speed. Important to understand the difference here if you're trying to limit speed. There's still duty cycle being controlled in proportion to your throttle, but any time you're limiting speed this will be impacted rather than current.
```

---
## \#27 Posted by: Slak Posted at: 2019-02-19T10:45:13.827Z Reads: 78

```
Is there a problem if you push a belt/VESC setup as the controller will receive energy from the motor (enough to get a blue led lit on my FOXbox, for instance) then stop (not enough energy from the motor) then receive energy again (because I pushed again with my foot) then stop, then start, etc ? I don't dare push because of that...I'm wrong ?
```

---
## \#28 Posted by: Jacobee Posted at: 2019-02-19T17:24:44.801Z Reads: 69

```
Yeah it's totally fine to kick push your board regardless of belt/hub/gears or rc car esc or vesc it can definitely handle that.
```

---
## \#29 Posted by: mmaner Posted at: 2019-02-19T17:37:09.725Z Reads: 66

```
https://www.electric-skateboard.builders/t/vesc-is-pushing-the-board-good-or-bad/10912/3?u=mmaner

https://www.electric-skateboard.builders/t/vesc-is-pushing-the-board-good-or-bad/10912/7?u=mmaner
```

---
## \#30 Posted by: Slak Posted at: 2019-02-19T21:33:55.144Z Reads: 52

```
Thank you
10 char
```

---
## \#31 Posted by: Slak Posted at: 2019-02-19T21:34:36.038Z Reads: 51

```
Ok, thanks !
```

---
## \#32 Posted by: b264 Posted at: 2019-02-19T21:37:05.415Z Reads: 52

```
[quote="Slak, post:27, topic:84611, full:true"]
Is there a problem if you push a belt/VESC setup as the controller will receive energy from the motor (enough to get a blue led lit on my FOXbox, for instance) then stop (not enough energy from the motor) then receive energy again (because I pushed again with my foot) then stop, then start, etc ? I don’t dare push because of that…I’m wrong ?
[/quote]

Just don't exceed the maximum speed your board can go while under power.  That could start to blow stuff.  Otherwise you should be okay

Generally, it's much better to power the board on if you want to push it
```

---
## \#33 Posted by: Meeep Posted at: 2019-04-13T17:30:06.885Z Reads: 37

```
So my new theoretical top speed when I briefly hooked up the unity was 34 mph. After my car crash, I think i'll stick to the 22-24mph range and enjoy the increased torque for a bit before increasing the top speed to 30mph. 

I don't know much about the different control methods (current, duty cycle, watt mode). Is limiting erpm the preferred speed limiting method?
```

---
