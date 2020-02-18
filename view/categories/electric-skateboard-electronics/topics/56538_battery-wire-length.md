# Battery wire length

### Replies: 18 Views: 809

## \#1 Posted by: Mathieu Posted at: 2018-05-23T22:32:59.421Z Reads: 158

```
Hey guys,

I am starting a new build with a board with some flex. I am 3D printing an enclosure and broke the first one due to it being to long in combination with the flex. Therefor I want to make 2 enclosures, one for the battery and one for the electronics. The 2 are placed on each side of the board, like boosted boards. So I will be running a battery cable from one side of the board to the other, about 50-60 cm I think. Can running long battery cables give problems with the VESC? I am running the VESC in bldc mode.
```

---
## \#2 Posted by: b264 Posted at: 2018-05-23T22:35:23.888Z Reads: 149

```
The VESC has capacitors to mitigate this, but you probably want to use 10AWG and not 12 gauge wire.  Use 10AWG super-stranded with silicone insulation as well if possible.
```

---
## \#3 Posted by: Mathias Posted at: 2018-05-23T23:47:48.389Z Reads: 134

```
[quote="b264, post:2, topic:56538"]
The VESC has capacitors to mitigate this
[/quote]
50-60 cm is maybe so long that it kills the capacitors or the VESC over time. I have a similar length of my battery wires, and I just had the 3rd TB VESC fail after each maybe 300-400 km in BLDC mode. I'm not 100% sure if that was the reason but now I switched to FOCBox and added extra caps. Let's see if that goes better.

@Mathieu, keep + and - as close together as possible (tape them together) to reduce their inductance. BLDC should be safer than FOC, but still, if you want to be on the safe side you could add a few extra capacitors directly in front of the stock ones. If you do so, make sure you buy caps with ultra low ESR, otherwise they don't help.
```

---
## \#4 Posted by: DevinG Posted at: 2018-05-24T00:47:39.635Z Reads: 114

```
So 14awg is too thick? im curious about this
```

---
## \#5 Posted by: wafflejock Posted at: 2018-05-24T00:53:50.336Z Reads: 111

```
Other way around wire gauge number goes up as wire gets thinner, 10 is thicker than 12 which is thicker than 14.

There are charts or calculators for DC voltage drop over a given length of wire but long story short thicker the wire lower the resistance over that length less voltage drop and heat build up from wires themselves.

https://www.rcgroups.com/forums/showthread.php?952523-too-long-battery-wires-will-kill-ESC-over-time-precautions-solutions-workarounds

Good generic write up there on issues and solutions.
```

---
## \#6 Posted by: Sn4pz Posted at: 2018-05-24T01:02:14.726Z Reads: 107

```
do you think that 40ish cm is too much? Youve got me worried now...haha
```

---
## \#7 Posted by: Mathias Posted at: 2018-05-24T01:29:56.484Z Reads: 102

```
I'm not sure what is "too much". If you keep the wires apart, don't add extra caps, and try FOC you'll probably fry your VESC4 right on the bench. BLDC will not, but that doesn't mean that the voltage spikes do not put extra stress on the caps and the VESC. This might destroy them over time. I have those long wires on my board too:
https://www.electric-skateboard.builders/t/first-build-vanguard-dual-tb-6355-190kv-tb-vesc-10s4p-lg-hg2-alien-mounts-paris-195mm-alien-remote/24295
And my TB VESC 4.12 have been dying quite frequently. But then again I've read many posts of those failing lately. 
Anyway, wires this long are definitely an issue. One should use thick wires and should keep them close together to keep the inductance as low as possible at this length. Extra caps are definitely worth thinking about, I would say. But again, I'm guessing here...
```

---
## \#8 Posted by: wafflejock Posted at: 2018-05-24T01:33:21.644Z Reads: 93

```
I had one tb vesc fry on me that I don't believe was my fault and another that was, on my third now but have been using it for over a year now and ride a couple time a week at least a few miles.  Curious what fried on yours was it the drv chip?  Also are you running a erpm close to 60k.  I have probably 15" or about 30cm between my batteries and vesc.
```

---
## \#9 Posted by: Sn4pz Posted at: 2018-05-24T01:37:46.854Z Reads: 91

```
both my tb vescs handled whatever i threw at them, even survived dual 130 hubs *kv FOC haha

bless their little souls :laughing:
```

---
## \#10 Posted by: Mathias Posted at: 2018-05-24T01:37:58.101Z Reads: 89

```
My max ERPM is around 45k. I got a couple of blown DRVs, and the last one started to show abs overcurrents. All in BLDC. Each ran for a few 100 km and than crapped out.
```

---
## \#11 Posted by: DevinG Posted at: 2018-05-24T01:48:03.324Z Reads: 87

```
So if i keep my wire length under 22cm should be good right
```

---
## \#12 Posted by: b264 Posted at: 2018-05-24T02:22:06.164Z Reads: 83

```
[quote="Mathias, post:3, topic:56538"]
if you want to be on the safe side you could add a few extra capacitors directly in front of the stock ones
[/quote]

This is better for your VESC but it will cook an antispark switch unless it's the new heavy-duty one @Kug3lis made.  Also it's worse for the loopkey as well but not as bad

Honestly you should be okay as long as you use 10AWG wire and a loopkey.  The rest is helpful, but not mandatory.
```

---
## \#13 Posted by: Sn4pz Posted at: 2018-05-24T02:23:47.723Z Reads: 79

```
if my VESC is wired for 45A for motor max and the antispark is rated for 50, will it ever present an issue? I dont want to fry my new stuff :C
```

---
## \#14 Posted by: b264 Posted at: 2018-05-24T02:35:39.498Z Reads: 72

```
The capacitors in the VESC will eventially fry the antispark because when it turns on, it's a sudden gush.  Also the motor max won't affect it, just the battery max and battery min.
```

---
## \#15 Posted by: Sn4pz Posted at: 2018-05-24T02:37:15.260Z Reads: 71

```
oh.... how long do they last? :(
```

---
## \#16 Posted by: devilzangelz Posted at: 2018-05-24T02:51:41.918Z Reads: 72

```
So I understand excessive battery length is bad, but what about [phase wires](https://www.amazon.com/Power-Extension-Chargers-Female-GT/dp/B01DFTNRXE/ref=sr_1_3?ie=UTF8&qid=1527130067&sr=8-3&keywords=4mm+bullet+extension&dpID=41yDofA6HeL&preST=_SX300_QL70_&dpSrc=srch)? Better? Worse? I will probably cut them down to size, but that begs the question: Any downsides to 2 foot long phase wires?(except for the space they take up)

In regard to the excessively long battery idea, what about boards like the WowMeepOwnGoBoard? They have an extension from the battery to the ESC that is probably closer to 2 feet long (unmeasured)... Does this have an impact?

Thanks!
```

---
## \#17 Posted by: Mathias Posted at: 2018-05-24T03:52:52.905Z Reads: 69

```
[quote="b264, post:14, topic:56538, full:true"]
The capacitors in the VESC will eventially fry the antispark because when it turns on, it’s a sudden gush.  Also the motor max won’t affect it, just the battery max and battery min.
[/quote]

How much capacity do you need to fry the antispark? That's the first time I hear of it. Did it happen to someone on this forum? I only added 3 mF of extremely low ESR capacitors. That will hardly increase the initial rush, but for sure helps with the voltage spikes.
```

---
## \#18 Posted by: Mathias Posted at: 2018-05-24T04:00:42.129Z Reads: 66

```
[quote="devilzangelz, post:16, topic:56538"]
So I understand excessive battery length is bad, but what about phase wires? Better? Worse?
[/quote]
Long phase wires shouldn't be a problem. Their inductance shouldn't matter compared to the inductance of most motors. So if your battery is far from the motors, put the ESCs rather close to the battery than close to the motors.
```

---
