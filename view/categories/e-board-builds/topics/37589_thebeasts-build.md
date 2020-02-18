# Thebeast&rsquo;s build

### Replies: 49 Views: 1637

## \#1 Posted by: thebeast Posted at: 2017-11-07T04:38:59.766Z Reads: 247

```
I have not gone out and bought everything. I simply want to know if my set up is going to meet my needs.

That being said I am going to go with a 14/36 pulley set up, A 190 kv motor size 6355.  My wheels are fairly small at 73 mm diameter with spokes so I can mount it . I most likely need to make my randles trucks flat to mount my motor.I have a deck already.

As for batteries I don't know what I should go for. Everyone says just grab some lipo's and stick them on your board.  I am skeptical about the graphine batteries. I don't think there that reliable from a scientific standpoint.

What potentially I would want to do is do half parallel and half in series. This makes things a little more complicated, but I am thinging of doing 6 batteries in series that on one side are connected in parallel. I am aiming for 12 s 
How many batteries do I need for that?
The reason I want to pair parallel and series is I want a fast board, however I also would like a  decent range.
Does this build work and suggestions are welcome.
I want to be able to go 25 miles per hour with a range of 20 miles.
```

---
## \#2 Posted by: saul Posted at: 2017-11-07T04:45:13.761Z Reads: 229

```
i'll say before someone else does. use search! lol
also  http://calc.esk8.today/

also randles and 73mm wheels will suck.
@psychotiller has the only randal mount that doesnt.
you still want kegels or flywheels.

unless you have a serious workshop, then do whatever...
```

---
## \#3 Posted by: MysticalDork Posted at: 2017-11-07T04:50:38.594Z Reads: 214

```
@thebeast   I would stick to 10s with 190kv motors, with 12s you'll exceed the erpm limit on your vesc (assuming you're going to use a vesc, which you should.)

73mm wheels are pretty small, which will result in a rough ride and lower ground clearance.

With brushless motors, current is torque, not speed. That means that having larger batteries that can supply more power won't give you more top speed, it'll jsut improve your acceleration and ability to climb hills.

Voltage is speed, so for a given motor kv and battery voltage, the only way to change your speed is by changing your gearing (pulleys) or your wheel size.

Assuming you go with a 10s battery, 10000mah should give you around 20 miles of range, and if you use 90mm flywheels or similar with that 14/36 gearing, you'll still get about 25mph. Since 5s 10000mah packs are huge, I'd recommend going with two 5000mah packs in parallel instead. So you'd have 10s2p, for a total of four 5s 5000mah packs.
```

---
## \#4 Posted by: Jinra Posted at: 2017-11-07T06:20:53.618Z Reads: 170

```
You won't hit the eRPM limit with 12s and 90kv due in inefficiencies. Pretty much every LHB board runs this setup, and I was personally using 10s @ 230kv on mine.
```

---
## \#5 Posted by: MysticalDork Posted at: 2017-11-07T06:36:02.928Z Reads: 162

```
It makes me cringe just hearing that! I guess I just like to play it extra safe.
```

---
## \#6 Posted by: thebeast Posted at: 2017-11-07T15:13:19.631Z Reads: 147

```
[quote="FredrikHems, post:2, topic:37066, full:true"]
At 100% efficiency The erpm will be 63500, but you will likely never hit this, unless you go full throttle downhill
[/quote]
I am aware of the Erpm calculation, but like this other guy said only when it is 100% efficient and going down hill will I hit the Erpm limit.
```

---
## \#7 Posted by: GrecoMan Posted at: 2017-11-07T15:14:01.989Z Reads: 135

```
I currently run 245kv on 10s :wink:

not a single problem (knock on wood) as long as you limit erpm and uncheck "limit erpm with negative torque"
```

---
## \#8 Posted by: thebeast Posted at: 2017-11-07T15:15:36.008Z Reads: 120

```
How fast can you go?
```

---
## \#9 Posted by: GrecoMan Posted at: 2017-11-07T15:16:13.151Z Reads: 121

```
hit 32mph yesterday... scary as FUCK
```

---
## \#10 Posted by: thebeast Posted at: 2017-11-07T15:23:34.428Z Reads: 123

```
[quote="thebeast, post:1, topic:37589"]
6355
[/quote]
That is the size of the motor. Series is more for torque vs. parallel is more for longevity. Parallel is what tesla's use. Tesla's have around 1 million battery cells which is why they are able to draw so much power.
```

---
## \#11 Posted by: thebeast Posted at: 2017-11-07T15:29:35.813Z Reads: 121

```
Ya I think electric long boards are more for short commutes instead of being transportation. Especially since long boards are not recognized as being the same as a bike. A bike is more accepted on roads. While it would be sick to be able to ride your electric long board next to a motor cycle, however I don't think too many people have the leg strength to hang on going 30 Mph.
```

---
## \#12 Posted by: MysticalDork Posted at: 2017-11-07T15:41:51.952Z Reads: 114

```
No, that's wrong. You can have a very high voltage setup, but if it doesn't deliver enough amps, you will have no torque. 

The more voltage you have, the more power you can draw, **IF** you have a battery that will support the current required.

Why do you think there are 8s setups on here hitting 25+mph? They have good gearing and plenty of **current**!

A top of the line Tesla has about 970 ft-lbs of torque at the wheels, because the battery can supply about 1300 amps at full blast.
```

---
## \#13 Posted by: Idle Posted at: 2017-11-07T15:41:52.588Z Reads: 106

```
[quote="thebeast, post:10, topic:37589"]
Parallel is what tesla's use. Tesla's have around 1 million battery cells which is why they are able to draw so much power
[/quote]

I think the extended range model S tesla has even more than that?
🤷🏼‍♀️
```

---
## \#14 Posted by: MysticalDork Posted at: 2017-11-07T15:43:57.291Z Reads: 102

```
8256 cells in a 100kwh Tesla battery pack.
```

---
## \#15 Posted by: Idle Posted at: 2017-11-07T16:11:31.075Z Reads: 95

```
Yes but wired in parallel so it's like 30,000 V
```

---
## \#16 Posted by: MysticalDork Posted at: 2017-11-07T16:26:19.969Z Reads: 91

```
The pack is 96s86p, so 96*3.6=345v.
```

---
## \#17 Posted by: Idle Posted at: 2017-11-07T16:37:14.064Z Reads: 91

```
Ok ok
I'll stop now
```

---
## \#18 Posted by: thebeast Posted at: 2017-11-07T16:46:53.417Z Reads: 87

```
I need at least 10s.  Yes this is true that 8s can go that fast however the capacity is lower. You can go that fast, but the range is affected.
```

---
## \#19 Posted by: scepterr Posted at: 2017-11-07T16:58:05.854Z Reads: 88

```
Voltage and capacity are not tied together
```

---
## \#20 Posted by: thebeast Posted at: 2017-11-07T17:02:30.210Z Reads: 93

```
Your telling me that having 10 s of power is less capacity than 8s? Also I didn't think that voltage and capacity are tied together.
```

---
## \#21 Posted by: Michael319 Posted at: 2017-11-07T17:12:40.979Z Reads: 79

```
Don't use series as a capacity Indication. Use Watt hours, do the calculations and use Whr pretty much explicitly when speaking about capacity.

You can make a 6s2p and a 12s1p. Both have same amount of capacity , but according to your logic, the 12s has more capacity? Wrong.
```

---
## \#22 Posted by: thebeast Posted at: 2017-11-07T17:19:10.479Z Reads: 73

```
I have no idea what you are talking about. I never said series was a capacity indication.
```

---
## \#23 Posted by: Michael319 Posted at: 2017-11-07T17:19:39.005Z Reads: 73

```
I never said you said. But you use it. Just reread your posts.
```

---
## \#24 Posted by: scepterr Posted at: 2017-11-07T17:20:12.255Z Reads: 72

```
[quote="thebeast, post:18, topic:37589, full:true"]
I need at least 10s.  Yes this is true that 8s can go that fast however the capacity is lower. You can go that fast, but the range is affected.
[/quote]

You're talking voltage and capacity here
```

---
## \#25 Posted by: thebeast Posted at: 2017-11-07T17:22:55.247Z Reads: 70

```
Tell me how 20 cells has less capacity than 8 cells? You aren't really explaining much?
```

---
## \#26 Posted by: scepterr Posted at: 2017-11-07T17:23:35.240Z Reads: 70

```
You can have a 10s or 8s of the same capacity, science 🤣
You can have more capacity on the 8S to equal the watthour of the 10S
```

---
## \#27 Posted by: Michael319 Posted at: 2017-11-07T17:25:05.702Z Reads: 72

```
No one has ever said that. I didn't realize I had to a it out for you. Do some reading. 

12s1p has 12 cells, 12 in series and 1 in parelell. 12*1=12

6s2p has 12 cells, 6 in series 2 in parelell. 6*2=12.

Sane amount of cells, same amount of capacity.

Although I hate the word capacity.
```

---
## \#28 Posted by: Maxid Posted at: 2017-11-07T17:25:34.680Z Reads: 68

```
1 cell could have more capacity than 28 cells. Capacity is not a measure for energy - Wh is.
```

---
## \#29 Posted by: Maxid Posted at: 2017-11-07T17:26:49.027Z Reads: 68

```
Noooo - you made the same mistake. That 6S Pack has double the capacity but half the voltage
```

---
## \#30 Posted by: thebeast Posted at: 2017-11-07T17:27:49.663Z Reads: 66

```
I do know this. I literally said the same thing for 10s.
```

---
## \#31 Posted by: Michael319 Posted at: 2017-11-07T17:32:18.094Z Reads: 67

```
I think it's the way we are using the word capacity. This stemmed from a discussion on range, which is the important factor here.
```

---
## \#32 Posted by: thebeast Posted at: 2017-11-07T17:33:42.842Z Reads: 65

```
A 8s system on a full charge can go faster than a 10s. However, the range, aka how far you can go on your board, is lower on 8s.
```

---
## \#33 Posted by: Michael319 Posted at: 2017-11-07T17:34:05.573Z Reads: 65

```
Same amount of cells, same amount of Whr (given they're the same cells)=same amount of range.
```

---
## \#34 Posted by: Michael319 Posted at: 2017-11-07T17:35:55.315Z Reads: 63

```
Sorry you are still wrong. A 10s system will actually get a faster top speed than an 8s. Look at the calculator.
```

---
## \#35 Posted by: b264 Posted at: 2017-11-07T17:38:37.860Z Reads: 67

```
[quote="thebeast, post:32, topic:37589, full:true"]
A 8s system on a full charge can go faster than a 10s. However, the range, aka how far you can go on your board, is lower on 8s.
[/quote]

Please provide evidence for this, because it's not true.
```

---
## \#36 Posted by: Michael319 Posted at: 2017-11-07T17:39:35.753Z Reads: 60

```
If we're talking about range, then it's the same.
```

---
## \#37 Posted by: thebeast Posted at: 2017-11-07T17:43:51.580Z Reads: 63

```
well I was just responding to @mysticalDork
```

---
## \#38 Posted by: Michael319 Posted at: 2017-11-07T17:46:32.385Z Reads: 61

```
Well, now you know!
```

---
## \#39 Posted by: thebeast Posted at: 2017-11-07T17:48:12.663Z Reads: 65

```
[quote="MysticalDork, post:12, topic:37589"]
The more voltage you have, the more power you can draw, IF you have a battery that will support the current required.

Why do you think there are 8s setups on here hitting 25+mph? They have good gearing and plenty of current!

A top of the line Tesla has about 970 ft-lbs of torque at the wheels, because the battery can supply about 1300 amps at full blast.
[/quote]
THAT IS WHERE I GOT MY INFO FROM
```

---
## \#40 Posted by: Michael319 Posted at: 2017-11-07T17:49:13.661Z Reads: 56

```
And his info is correct, I think you might have misunderstood
```

---
## \#41 Posted by: thebeast Posted at: 2017-11-07T17:52:09.598Z Reads: 48

```
[quote="thebeast, post:39, topic:37589"]
Why do you think there are 8s setups on here hitting 25+mph? They have good gearing and plenty of current!
[/quote]

So the way that the batteries are configured doesn't matter?
```

---
## \#42 Posted by: b264 Posted at: 2017-11-07T18:10:06.984Z Reads: 51

```
[quote="thebeast, post:41, topic:37589"]
So the way that the batteries are configured doesn't matter?
[/quote]

Dig into a little about Ohm's law and electrical power and see how current (amps), voltage (volts), power (watts), energy (watt*hours) and charge (amp*hours) are all related.  Then check back
```

---
## \#43 Posted by: MysticalDork Posted at: 2017-11-07T18:25:05.996Z Reads: 55

```
The way the battery is configured does matter, but it's not the **ONLY** thing that matters. You have to look at the whole system. You could build a 12s2p pack, or you could build a 10s4p pack, or this or that. 

Range is measured in miles. Efficiency is watt-hours per mile.  So assuming X efficiency, Y watt hours gets you Z miles. You can build a pack any way you want. As long as the system can handle it, **if the pack has the same watt-hours**, it doesn't matter if it's 4s, 6s, 10s or 20s, the range will be the same. 

To get the same watt-hours, the total number of cells will be the same. So a 6s setup with the same watt-hours as a 12s setup will have twice the number in parallel.
```

---
## \#44 Posted by: thebeast Posted at: 2017-11-07T19:13:16.069Z Reads: 56

```
I do know this however every one besides you doesn't think so. I think before you talked about making a 8s2p pack could go the same speed as a 12s 1p.
```

---
## \#45 Posted by: MysticalDork Posted at: 2017-11-07T20:05:36.102Z Reads: 54

```
It can, IF you get the gearing, wheel size and motor kv correct.  If you're going to use 18650 batteries, both 8s2p and 12s1p are pretty weak though. Assuming 20 amps per cell, that would get you 40 amps at 8s or 20 amps at 1s. 12s2p or 10s3p would be better, especially if you want 20 miles of range.
```

---
## \#46 Posted by: briman05 Posted at: 2017-11-07T21:41:03.115Z Reads: 55

```
Someone on here sells Randal trucks mounts I can’t remember but I know someone does
```

---
## \#47 Posted by: thebeast Posted at: 2017-11-08T01:25:00.934Z Reads: 53

```
Ohh this isn't a problem I can flatten it. I have the tools needed.
```

---
## \#48 Posted by: briman05 Posted at: 2017-11-08T02:18:04.242Z Reads: 52

```
@psychotiller has them for the Randal trucks.
```

---
## \#49 Posted by: thebeast Posted at: 2017-11-09T03:54:58.055Z Reads: 35

```
I am going to make my own out of metal. I have a grinder saw that cuts through medal. https://www.youtube.com/watch?v=UF1weFm6wS4 the same tool this dude uses at 1:30 in the video.
```

---
