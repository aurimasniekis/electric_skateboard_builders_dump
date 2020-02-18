# Best vesc for 260kv motors at 10s?

### Replies: 21 Views: 461

## \#1 Posted by: Dariks Posted at: 2018-08-03T03:02:17.030Z Reads: 120

```
I'm trying to make a quick single drive setup--weight reduction is the goal of this so I want to use 10s to keep the motor efficient as it's peak efficiency is at 10s. Also does the vesc still have a high rpm max?
```

---
## \#2 Posted by: uigiroux Posted at: 2018-08-03T03:20:35.825Z Reads: 115

```
I believe the VESC's V4.12 have the 60k ERPM limit.  I think the FOCBOX can go higher, though not sure if it's as high as the VESC 6, which is 100k ERPM.
```

---
## \#3 Posted by: Dariks Posted at: 2018-08-03T03:22:17.624Z Reads: 111

```
Is that in bldc?
```

---
## \#4 Posted by: Sn4pz Posted at: 2018-08-03T03:37:02.844Z Reads: 105

```
yes it is
char
```

---
## \#5 Posted by: Dariks Posted at: 2018-08-03T03:37:51.965Z Reads: 98

```
I have a vescX whats the rpm limit on that?
```

---
## \#6 Posted by: AutoItKing Posted at: 2018-08-03T03:45:54.116Z Reads: 92

```
That's a FOCBOX from before they renamed it, so 60k.
```

---
## \#7 Posted by: Dariks Posted at: 2018-08-03T03:46:35.714Z Reads: 92

```
F i feel like I'm gonna go over that at 10s.
```

---
## \#8 Posted by: AutoItKing Posted at: 2018-08-03T03:50:30.970Z Reads: 90

```
You will probably hit around 67k which may just be okay on a FOCBOX.
3.7V * 10S * 260kV * 7 pole pairs = 67,340 ERPM.
```

---
## \#9 Posted by: Dariks Posted at: 2018-08-03T03:53:11.399Z Reads: 92

```
Umm you have to use a fully charged battery in that equation. so I will hit 76440 ERPM
```

---
## \#10 Posted by: TowerCrisis Posted at: 2018-08-03T03:53:32.475Z Reads: 93

```
You'll be doing 68796 erpm at 90% efficiency, 64974 at 85%, which I believe a lot of people assume.

Honestly you can probably just set your limit at 60k and chop off a little bit of your top speed.

My last build was 280kv at 10S. Even with that I only reached 60k when I was REALLY pushing it (checked logs) and testing my speed capability. Over 20mph is uncomfortable for me.

EDIT: also that was on a stock vesc 4.12, I'm sure you'll be fine on a focbox as they are a little more robust.
```

---
## \#11 Posted by: AutoItKing Posted at: 2018-08-03T03:56:24.165Z Reads: 90

```
[quote="Dariks, post:9, topic:63674, full:true"]
Umm you have to use a fully charged battery in that equation. so I will hit 76440 ERPM
[/quote]

Your loaded voltage will not be 4.2V. The only time your voltage will be 4.2V per cell is fresh off the charger with no load. Practically you will never see even close to that.
```

---
## \#12 Posted by: Dariks Posted at: 2018-08-03T04:00:09.263Z Reads: 79

```
True but its always better to account for that. I think I'm just gonna run it and set the rpm limit at 60k. I'v fallen on this same setup before so I'm a bit apprehensive. Although I was using a cheap maytech vesc at that time.
```

---
## \#13 Posted by: dareno Posted at: 2018-08-03T04:22:47.299Z Reads: 72

```
You are not going to get anywhere near the max erpm while riding unless you are going down a steep hill 10 miles long with the wind behind you.  Just don't spin it on a bench and you will be fine.
```

---
## \#14 Posted by: Dariks Posted at: 2018-08-03T04:29:18.663Z Reads: 70

```
I have hit max rpm before with these but I was using a 8p pack back then so there was no sag at all. But now that I'm using a 2p pack I should have tons of sag so I'm probably never hitting max rpm. Its reassuring to hear from other people using this type of setup.
```

---
## \#15 Posted by: dareno Posted at: 2018-08-03T05:49:59.678Z Reads: 71

```
what was your top speed when you hit 60k?
```

---
## \#16 Posted by: Dariks Posted at: 2018-08-03T06:07:36.472Z Reads: 68

```
@dareno 37mph on a flat strait. For about 10 seconds then the vesc burned that's when I hit 60k
```

---
## \#17 Posted by: TowerCrisis Posted at: 2018-08-03T12:28:39.910Z Reads: 58

```
23mph was what I peaked at. This was on a track around a football field and I could barely make the turns at that speed.

In the area I'll be using this the roads are narrow and there are lots of frequent intersections, so there's really nowhere else I'd be comfortable going that speed.

Current build with 270kv on 8s instead of 10s is projected to have a similar top end, with better acceleration due to a much larger stator and different gearing.
```

---
## \#18 Posted by: Dariks Posted at: 2018-08-04T00:12:37.856Z Reads: 42

```
Oh don't test speed on a track that's a really bad idea find a straightaway and just let em rip. @TowerCrisis Oh your going to have less torque at 8s not more but if your using gearing its probably gonna be the same.
```

---
## \#19 Posted by: Dariks Posted at: 2018-08-04T00:14:12.748Z Reads: 42

```
@TowerCrisis Biggest recommendation for traffic go with sensor's on your motor it helps so much.
```

---
## \#20 Posted by: TowerCrisis Posted at: 2018-08-04T09:47:42.281Z Reads: 38

```
Got higher wattage motors, rated only up to 8S, so I will be pulling significantly more amps. But as I've seen so far, they're very high efficiency motors, and the board could have a fairly "eco" friendly group of settings.
```

---
## \#21 Posted by: TowerCrisis Posted at: 2018-08-04T10:46:33.630Z Reads: 33

```
Also in regards to stop and go city scenarios, I believe in higher KV. With most motors we use having 14 pole pairs, the chance of cogging is decreased with higher gear ratios. So with two boards geared to the same top speed, same wattage motors, and same voltage, but with different KV, the higher KV board will cog less on low end torque from a standstill. Just my two cents if sensored isn't appealing or possible for some others out there. But also don't exceed 60k :stuck_out_tongue:
```

---
