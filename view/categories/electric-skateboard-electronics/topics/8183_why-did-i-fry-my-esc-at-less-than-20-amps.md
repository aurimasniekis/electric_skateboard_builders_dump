# Why did I fry my ESC at less than 20 amps?

### Replies: 36 Views: 1691

## \#1 Posted by: stuxtruth Posted at: 2016-08-23T18:19:54.185Z Reads: 173

```
My setup

2X Sk3 6355
2X FVT Esc
6s4p batt 
40A inline fuse (didn't blow)

I was riding for about 5 minutes. Was braking down a hill and lost my brakes.  I flipped the board over and one of my esc was smoking. The other was fine. The light was flickering but the fan was still on. Wouldn't power the motor. Why do you think this happened?
```

---
## \#2 Posted by: Skitzor Posted at: 2016-08-23T18:56:39.276Z Reads: 163

```
Too much regen current from braking together with an almost full battery ?
```

---
## \#3 Posted by: stuxtruth Posted at: 2016-08-23T19:00:18.122Z Reads: 160

```
Possible. Battery was full.
```

---
## \#4 Posted by: Skitzor Posted at: 2016-08-23T19:01:38.262Z Reads: 162

```
And were you braking gradually or full ?
```

---
## \#5 Posted by: stuxtruth Posted at: 2016-08-23T19:03:25.419Z Reads: 155

```
Gradual to full
```

---
## \#6 Posted by: Michaelinvegas Posted at: 2016-08-23T19:22:09.860Z Reads: 148

```
I hardly use the breaks for the first five minutes ... And never hard break during that time .... Think that may be the issue
```

---
## \#7 Posted by: sl33py Posted at: 2016-08-23T19:35:26.168Z Reads: 141

```
that was my thought as well.  I wasn't sure that the FVT did regen braking?  If it were VESC i'd definitely think it was regen voltage with nowhere to go...
```

---
## \#8 Posted by: Michaelinvegas Posted at: 2016-08-23T19:39:51.924Z Reads: 141

```
Best practice is to use up a little juice before breaking...
I'm sure a voltage spike occurred
```

---
## \#9 Posted by: stuxtruth Posted at: 2016-08-23T19:43:03.620Z Reads: 129

```
Well at least I got my answer! Thanks
```

---
## \#10 Posted by: Skitzor Posted at: 2016-08-23T19:44:00.185Z Reads: 124

```
At least they're cheaper than a vesc :wink:
```

---
## \#11 Posted by: sl33py Posted at: 2016-08-23T19:51:16.508Z Reads: 117

```
Does the one that didn't fry still work?
```

---
## \#12 Posted by: stuxtruth Posted at: 2016-08-23T20:03:16.713Z Reads: 112

```
Yes. Weird though I had an inline 40 amp fuse
```

---
## \#13 Posted by: JLabs Posted at: 2016-08-23T20:22:20.999Z Reads: 108

```
In my testing / expirence the FVT 120a does not have regen braking. My guess is that something shorted. Did you take the cover off and look around?
```

---
## \#14 Posted by: stuxtruth Posted at: 2016-08-23T20:49:17.416Z Reads: 101

```
<img src="/uploads/db1493/original/2X/f/f476cf95c7954672a43c9f4c33005ec183c28546.jpeg" width="375" height="500">
```

---
## \#15 Posted by: JLabs Posted at: 2016-08-23T20:51:29.566Z Reads: 97

```
Thats odd, I am almost 100% sure the FVT does not have regen breaking. Not sure what would have caused it to fry.
```

---
## \#16 Posted by: Namasaki Posted at: 2016-08-23T20:55:27.733Z Reads: 97

```
Could it be that they are just not designed for heavy braking with heavy loads going down steep hills?
I mean really, it's a model car esc.
```

---
## \#17 Posted by: JLabs Posted at: 2016-08-23T20:57:10.745Z Reads: 97

```
Possibly, I have done 20% grade hills while heavy breaking. The only time when there was a problem was when my battery was low and didnt have any power to power the breaks.
```

---
## \#18 Posted by: Namasaki Posted at: 2016-08-23T20:59:35.104Z Reads: 97

```
Ok, he must have gotten a short then.
```

---
## \#19 Posted by: stuxtruth Posted at: 2016-08-23T21:12:24.651Z Reads: 99

```
Didn't see anywhere where it could have shorter except the fact that the outer body of the sk3 rubbed down the insulation on the motor wire. But this is the esc opposite of the one that blew.
```

---
## \#20 Posted by: stuxtruth Posted at: 2016-08-23T21:13:07.365Z Reads: 98

```
<img src="/uploads/db1493/original/2X/b/b28c521e04cc0900e1691c57836cddaa628060d7.jpeg" width="375" height="500">
```

---
## \#21 Posted by: JLabs Posted at: 2016-08-23T21:21:40.866Z Reads: 96

```
Since the motor is metal it may have touched the wire and cause a short that way.
```

---
## \#22 Posted by: NNGG Posted at: 2016-08-23T22:27:25.695Z Reads: 86

```
So if my lipos are at 4 volts a cell, can I safely brake?
```

---
## \#23 Posted by: JLabs Posted at: 2016-08-23T22:31:29.627Z Reads: 89

```
You can brake at full charge, I have had no problems at high voltage. The problem is when you get down near the cutoff voltage of 3 - 3.2v/s
```

---
## \#24 Posted by: Weberp7593 Posted at: 2016-08-23T22:38:06.343Z Reads: 86

```
Sry Guys i am new here, and i am not a nativ English speaker -.- I can not start a new posting.
I read the FAQ but I don't know why, or how to do.

Is it maybe blocked because I am new?

Best wishes from Germany
```

---
## \#25 Posted by: barajabali Posted at: 2016-08-23T22:39:52.574Z Reads: 87

```
Yes just be active on our forum for a little while and it will unlock

Welcome!
```

---
## \#26 Posted by: evoheyax Posted at: 2016-08-23T22:42:26.796Z Reads: 92

```
[quote="JLabs, post:23, topic:8183"]
You can brake at full charge
[/quote]

This is true. And how I know the FVT does NOT have regen braking. Cause I never had issues and if it had regen braking, you would over charge you battery an you would know. The VESC, you must be careful with at a full charge. The reason theres an issue is say you run 10s, you should have your absolute min set to 28 volts and max set to 42 volts. If your at full charge (4.2 volts per cell), you will trigger the over voltage protection. Alternatively, you can set it to 43 volts (which is what I do), but you do need to be careful, cause you could over charge your battery doing that. Starting at 40 volts (or 4 volts per cell) solves that issue also. If I know I'm starting on a hill (as I do when I leave my university), I just under charge a slight bit to 41 volts. It's the same logic behind whatever voltage battery you use, I just like to use 10s as an example because the numbers are really easy to see and understand due to the overall being a factor of 10 of what your cells are at.

@stuxtruth My question is what where your acceleration and the one next to that? I remember blowing out a few of these because I had those two settings set too high. And the burn mark on mine was exactly what I see on yours...
```

---
## \#27 Posted by: stuxtruth Posted at: 2016-08-23T22:46:39.089Z Reads: 84

```
My acceleration was set on high and timing set on very high
```

---
## \#28 Posted by: DeathCookies Posted at: 2016-08-24T06:43:56.079Z Reads: 72

```
[quote="stuxtruth, post:27, topic:8183"]
timing set on very high
[/quote]

That results in a hotter motor and maybe in a hotter ESC which then has broken. But dunno...
```

---
## \#29 Posted by: thisrealhuman Posted at: 2016-08-24T08:41:26.575Z Reads: 71

```
My first esc burned while breaking downhil. I bought another just like it and set my timing all the way down and the pwn freq to 8. Solved my heat issues. That was a turnigy esc.
```

---
## \#30 Posted by: ra.rend Posted at: 2016-08-24T20:13:41.728Z Reads: 53

```
I have the 10s3p space cell and max set to 43v. Am I overcharging the battery if I charge to 100% or is the bms stopping that?
```

---
## \#31 Posted by: evoheyax Posted at: 2016-08-24T20:15:37.041Z Reads: 55

```
bms should stop that. The charger will also stop it. I'm charging without a bms right now and if the cells were balanced before, I can actually charge and it'll stop on its own But both will stop it.
```

---
## \#32 Posted by: JdogAwesome Posted at: 2016-08-24T21:50:53.576Z Reads: 53

```
It's weird that the VESC won't let current flow if your batterys are fully charged, I would think if your just braking down a hill for lets say like 10-20 seconds  even on full break with even like 5-10A (hypothetically) flowing to the Lipo, that will barely charge a full, for example, 5AH 10S battery so you shouldn't have to worry about any over charging. Anyways even if you do have to worry about it overcharging there should be something built into the VESC like some high wattage resistors to let some excess current flow for just a matter of seconds in case your LiPo is full and your braking. And I know high wattage resistors are large but even some smaller ones can dissipate a relatively high amount of current for a short amount of time. Anyways that's just my 2 cents about the situation.
```

---
## \#33 Posted by: stuxtruth Posted at: 2016-08-26T22:19:05.078Z Reads: 42

```
Just got my new FVT esc in I figured I would give it one more go. Any last suggestions before I maybe fry this one? (Other than VESC)
```

---
## \#34 Posted by: stuxtruth Posted at: 2016-08-27T17:28:50.890Z Reads: 39

```
So I got the board working again. I noticed that my voltage meter was flickering on and off. I checked the main battery xt60 and it was very loose! So I pinched it a little with some pliers so that it was a tight fit and wrapped in electrical tape and everything is good so far. I think that's how I fried my esc before.
```

---
## \#35 Posted by: barajabali Posted at: 2016-08-28T00:24:19.850Z Reads: 33

```
So you're not leaving the hobby anymore ?
```

---
## \#36 Posted by: stuxtruth Posted at: 2016-08-28T03:01:35.560Z Reads: 27

```
Never wanted to leave. Just had my other issues figured out.
```

---
