# 14S 120A Drone ESC for 63$. what could go wrong?

### Replies: 7 Views: 763

## \#1 Posted by: Drom Posted at: 2019-07-01T20:27:19.859Z Reads: 136

```
As usual, I'm trying to find the cheapest, powerful and reliable ESC :joy:

The reason I don’t like VESC is very expensive for a **+5000W** single drive and easy to break due to novice mistakes and lack of protection, so I can't accept the price of VESC6 until I understand why other controllers suck.

I found [**DJI ESC on Taobao**](https://item.taobao.com/item.htm?spm=a230r.1.14.1.6a584ef8ReSDwm&id=547801675241) for only **$63** and specs are really impressive. As I understood the release was in 2017, but I didn't find any reviews or something. It definitely confuses me, but still..

https://www.dji.com/takyon-z14120

[![s2-bg-4ad6932832d8039051c0d7551ae0a523|690x204](upload://5ViU9m4yhGHfmnjq9uIvFNArfFq.jpeg)](https://www.dji.com/takyon-z14120)
**PDF files**: https://www.dji.com/downloads/products/takyon-z14120

[details="Some specs"]

- Max Voltage: 61V
- Max continuous current: 120A
- Max peak current (< 3 sec): 160A
- ERPM limit: 280'000

Protection:
- overheating (power limit if >120*C, cut off if >140*C)
- overvoltage
- undervoltage
- short circuit
- stall
- phase-loss

**IP66** Rated

Settings:
- timing (don't know what it is)
- active braking
- throttle range
- Data export

[/details]

__________
Another two cheap and powerful ESCs :
- [Hobbywing Flyfun HV OPTO V5](https://item.taobao.com/item.htm?spm=a230r.1.14.40.5ba96e42N9OF3l&id=558630989705) **14S 130A** - **$117**
- [T-motor ALPHA (**FOC**)](https://item.taobao.com/item.htm?spm=a230r.1.14.39.6bc66b66i5NluS&id=594155584316) **14S 80A** - **$117**

_________________
So my question is why no one try these drone ESCs for esk8/ebike builds? At least for budget ?
```

---
## \#2 Posted by: niuva Posted at: 2019-07-01T20:34:37.773Z Reads: 132

```
IIRC Drone escs lack the ability to brake.
```

---
## \#3 Posted by: Drom Posted at: 2019-07-01T20:35:18.802Z Reads: 131

```
The specifications say that there is..

And active braking settings (through PC)
```

---
## \#4 Posted by: maxchilton Posted at: 2019-07-01T20:55:50.567Z Reads: 125

```
[quote="Drom, post:3, topic:97669"]
And active braking settings (through PC)
[/quote]

those brakes aren't strong enough to for esk8 purposes.  They're use only to slow down the propellers so the drone is more agile.  

But you can definitely give that ESC a try and report back your findings.
```

---
## \#5 Posted by: Drom Posted at: 2019-07-01T22:17:16.588Z Reads: 114

```
Probably you are right. But if this ESC works at +5000W continuously for only $63, then we pay a lot of money for smoother throttle and stronger brake :thinking:
```

---
## \#6 Posted by: AlanZhou Posted at: 2019-07-01T22:42:21.777Z Reads: 107

```
well, a flipsky vesc 4.12 is only 50$, also 120a seems a bit overrated.

it also has no bec and it seems it does not work on PPM directly which problaly means you need to get a flight controller along with it from DJI.

![download|690x212](upload://9EixtHCIODhHE8D6cM6qFAklB1h.png)
```

---
## \#7 Posted by: Sn4pz Posted at: 2019-07-02T03:35:46.908Z Reads: 81

```
We both know it's not the addition of smoother throttle and usable breaks that makes the vesc more expensive to manufacture and distribute, it's the modularity and openness of the unit that drives the price up.

 I'm sure that if @AlanZhou is correct, and the ESC requires the remote control, then either that controller is going to expensive as hell, or they're going to find another way to get money out of you 

I've always jokingly thought about a build where in my right hand I hold my remote, and in my left I hold a manual break, similar to ones for mountain boards.... just for both rear wheels 🤷

Seems silly to me as I believe the electronics should be able to do both . But if you're going to use an ESC that only accelerates, it's not a bad idea 👍
```

---
