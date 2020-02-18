# Bldc/ foc / hyrid

### Replies: 11 Views: 1258

## \#1 Posted by: pshaw Posted at: 2017-07-31T00:00:01.178Z Reads: 222

```
I just want to make sure I have a thorough understanding of these modes. 

BLDC - tried and proven. No sensors needed. Might have to kick start as it will cog from standstill 

FOC - quiet. Less too speed compared to bldc. Smooth start no need to kickstart. Might not work on 12S???

Hybrid - best of both worlds. Should work fine on 12S. 

Am I correct here?
```

---
## \#2 Posted by: evoheyax Posted at: 2017-07-31T00:09:16.245Z Reads: 218

```
FOC doesn't mean no kick start, maybe a bit of a less kick. For me, it's less noise and just a better riding feel to me.

Hybrid requires hall effect sensors in your motor. It runs BLDC, not FOC. At a certain erpm, which you can set, it will turn off the sensors. The reason is a pure sensor mode is inefficient at higher speeds. Sensor are only there for low speed torque. So hybrid mode fixes this.

FOC though, if ran in sensored mode, will do the same thing as hybrid, but in FOC, instead of BLDC.
```

---
## \#3 Posted by: pshaw Posted at: 2017-07-31T01:01:19.950Z Reads: 209

```
[quote="evoheyax, post:2, topic:29168, full:true"]
FOC doesn't mean no kick start, maybe a bit of a less kick. For me, it's less noise and just a better riding feel to me.

Hybrid requires hall effect sensors in your motor. It runs BLDC, not FOC. At a certain erpm, which you can set, it will turn off the sensors. The reason is a pure sensor mode is inefficient at higher speeds. Sensor are only there for low speed torque. So hybrid mode fixes this.

FOC though, if ran in sensored mode, will do the same thing as hybrid, but in FOC, instead of BLDC.
[/quote]

Really? So hybrid never runs FOC? I thought the low end was FOC them it kicked to BLDC at the top end? 

So if FOC can't start from a complete stop without studdering how is boosted doing it?
```

---
## \#4 Posted by: Stef Posted at: 2017-07-31T01:09:39.711Z Reads: 198

```
FOC still cogs at startup if you dont use sensors. Boosted uses sensors if im not mistaken.
```

---
## \#5 Posted by: pshaw Posted at: 2017-07-31T01:10:50.202Z Reads: 198

```
[quote="Stef, post:4, topic:29168, full:true"]
FOC still cogs at startup if you dont use sensors. Boosted uses sensors if im not mistaken.
[/quote]

I thought you have to run sensors on FOC. 

I'm planning on using sensors.
```

---
## \#6 Posted by: Stef Posted at: 2017-07-31T01:13:49.317Z Reads: 193

```
No you can run BLDC and FOC sensored or unsensored.

I highly recommend sensors, it is a little extra work but gives you a much better performing board. I ran unsensored for some days and the cogging is a pain in ass. Added bonus of my sensored motors is that they include a temp sensor so I never have to worry about overheating.
```

---
## \#7 Posted by: PartyPoison Posted at: 2017-08-01T04:11:09.463Z Reads: 170

```
I got a dual 200kv sensored motor, 10s4p,
It runs in bldc, but when i try the hybrid, only one motor works, what i did was, 
motor1 detect motor, write the given numbers, write config, disconnect, test with controller, then its ok,
Motor 2 same,... But when I connect both the vesc, motor1 didnt run only 2., i did it all over again this time motor 2 was first to detect, then motor 1, after connecting both, motor 2 didnt run... Anyone experience this? (the first motor i detect wont run in dual system) sorry for long post..
```

---
## \#8 Posted by: pshaw Posted at: 2017-08-03T02:36:51.527Z Reads: 148

```
Man the more is read about these modes the more I'm confused. It seems everyone is saying conflicting things.... 

I'm trying to run the newest @Ackmaniac firmware so I can do watt mode/ sensored/ FOC. 

12S wouldn't be a good idea?
```

---
## \#9 Posted by: Jinra Posted at: 2017-08-03T04:08:41.035Z Reads: 141

```
I'll say what I know for sure

* BLDC and FOC can both be sensored or unsensored and the first two have nothing to do with the latter
* Hybird or Sensored modes **NEED** sensors
* BLDC has an audible hum while accelerating and braking
* BLDC switching frequency is much lower than FOC (which is why FOC is more likely to blow your VESC
* Your likely-hood of blowing your VESC on FOC increases with higher eRPM. This is why hubs are great for 12s FOC as their kv is typically lower than belt setups

Any other questions?
```

---
## \#10 Posted by: pshaw Posted at: 2017-08-03T05:07:07.484Z Reads: 138

```
[quote="Jinra, post:9, topic:29168, full:true"]
I'll say what I know for sure

* BLDC and FOC can both be sensored or unsensored and the first two have nothing to do with the latter
* Hybird or Sensored modes **NEED** sensors
* BLDC has an audible hum while accelerating and braking
* BLDC switching frequency is much lower than FOC (which is why FOC is more likely to blow your VESC
* Your likely-hood of blowing your VESC on FOC increases with higher eRPM. This is why hubs are great for 12s FOC as their kv is typically lower than belt setups

Any other questions?
[/quote]

This helps alot thanks man! I feel like hybrid is the way to go to be safe. I was just hoping I could get the benefit of the more quiet FOC ... oh well :confused:

I'd hate to pop an esc or two..... 

When using sensors and hybrid will it stutter from a dead stop or will it be nice and smooth like the boosted board I'm used to?
```

---
## \#11 Posted by: Jinra Posted at: 2017-08-03T05:08:57.644Z Reads: 133

```
It's smooth, though can occasionally hiccup, but will start up from dead stop no problem in most cases.
```

---
