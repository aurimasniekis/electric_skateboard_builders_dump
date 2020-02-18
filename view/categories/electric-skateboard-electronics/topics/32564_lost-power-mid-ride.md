# Lost power mid-ride

### Replies: 15 Views: 610

## \#1 Posted by: topherbarnett Posted at: 2017-09-07T23:00:19.423Z Reads: 123

```
Well, I was crossing a street at very slow speed when I lost power to the motor. It worked fine this morning and this afternoon for my 15-minute work commute. This time I had only been going for a couple minutes.

:walk of shame home:

Setup:
6374 190kv motor, MEB OESC, 10S1P 5000mAh

Symptoms:
VESC powers up and shows blue and green light. No blinking.
VESC green light gets brighter when giving input to remote.
VESC is getting power and connects to BLDC Tool. No Faults in Realtime Data tab.
Motor rolls freely, no electrical resistance.
PPM input show correctly in PPM tab.
Trying to run motor detection fails.
Voltage meter reads 39v.
In Realtime Data tab, "Drawn Cap" increases as I pull the remote.

Here are my VESC configs:
<img src="/uploads/db1493/original/3X/2/5/25372e8c07aae7aaa43eef163d398d72f4d5361e.png" width="690" height="455">
<br>
<img src="/uploads/db1493/original/3X/8/7/87a10d9704389a12a0f493de68ec7925c00fd3a9.png" width="690" height="455">
<br>
<img src="/uploads/db1493/original/3X/3/a/3aef6f297999779a998a42bd86887ef58e644be4.png" width="690" height="456">
<br>
<img src="/uploads/db1493/original/3X/b/8/b80a2d70caebaf6e82b2596bbc299d09c5f0c237.png" width="689" height="455">

Can anyone tell where I went wrong? I'm really hoping I didn't destroy the VESC or motor.
```

---
## \#2 Posted by: mmaner Posted at: 2017-09-07T23:26:40.598Z Reads: 94

```
Check and see if you have broken or shorted leads to the motor.
```

---
## \#3 Posted by: topherbarnett Posted at: 2017-09-07T23:36:09.720Z Reads: 89

```
Tested with the multimeter and have no shorts from the battery lead to the motor housing

Also tested rolling resistance while shorting motor wires together while unpowered, and with each pair, the resistance increased. Even more so with all three wires shorted.
```

---
## \#4 Posted by: topherbarnett Posted at: 2017-09-07T23:48:44.285Z Reads: 86

```
I think I may have fried the VESC. Upon removal, it has that distinct smell to it. Everything that I can plainly see looks fine though, so I'm guessing it's one of the components inside that I can't get to.
```

---
## \#5 Posted by: mmaner Posted at: 2017-09-07T23:51:58.606Z Reads: 81

```
If you connect to the BLDC tool what does it say in the terminal?
```

---
## \#6 Posted by: topherbarnett Posted at: 2017-09-08T00:03:25.930Z Reads: 77

```
Terminal didn't say anything, but I didn't type anything in.

Think I found it:
<img src="/uploads/db1493/original/3X/5/8/58d13ec9399f786a172c13ef080eb83dad2406b0.jpg" width="452" height="500">

Is that the infamous DRV chip?
```

---
## \#7 Posted by: cwazy1 Posted at: 2017-09-08T00:05:23.338Z Reads: 74

```
yup, and how ironic its got the QC passes sticker on it.
```

---
## \#8 Posted by: oriol360 Posted at: 2017-09-08T00:46:35.244Z Reads: 67

```
Please send me an email
```

---
## \#9 Posted by: trancejunkiexxl Posted at: 2017-09-08T01:29:02.718Z Reads: 64

```
you should talk to @JohnnyMeduse =)
```

---
## \#10 Posted by: ARetardedPillow Posted at: 2017-09-08T03:12:18.241Z Reads: 55

```
same thing happened to me.... I bought a new vesc from @chaka and now Im waiting for it to arrive to me, im probably going to talk to @JohnnyMeduse to get my vesc repaired soon, I just dont understand? I was going really slow too and all of a sudden boom vesc died
```

---
## \#11 Posted by: StormTrooperBert Posted at: 2017-09-08T04:13:17.850Z Reads: 56

```
How many rides did this VESC have on it? Just curious.
```

---
## \#12 Posted by: ARetardedPillow Posted at: 2017-09-08T04:24:52.606Z Reads: 54

```
I would say around 5-10 rides, under 20 miles and still in testing and it just died on me
```

---
## \#13 Posted by: topherbarnett Posted at: 2017-09-08T09:23:46.683Z Reads: 37

```
[quote="oriol360, post:8, topic:32564, full:true"]
Please send me an email
[/quote]
Message sent.

[quote="trancejunkiexxl, post:9, topic:32564, full:true"]
you should talk to @JohnnyMeduse =)
[/quote]
Will do, thanks for the recommendation.

[quote="ARetardedPillow, post:10, topic:32564"]
same thing happened to me....
[/quote]
What brand of VESC did it happen to?

[quote="StormTrooperBert, post:11, topic:32564, full:true"]
How many rides did this VESC have on it? Just curious.
[/quote]
Mine has has 4 rides, all pretty short. I haven't gone through a whole battery yet.
```

---
## \#14 Posted by: ARetardedPillow Posted at: 2017-09-08T16:28:39.110Z Reads: 21

```
It was a vesc by diy for 98 dollars but I bought one from @chaka so hopefully this one is a lot better
```

---
## \#15 Posted by: StormTrooperBert Posted at: 2017-09-08T17:29:41.558Z Reads: 19

```
My first VESC from DIY took a shit on me before I even put one ride on it. I bought another because they had the best price and I've out roughly ten miles on it. It's been working great. I'm learning these vescs are VERY sensitive. I've heard of them throwing drv codes from simply riding on bumpy sidewalks. Do yourself a favor and figure how to properly isolate/pad where you're mounting the VESC in the enclosure.
```

---
