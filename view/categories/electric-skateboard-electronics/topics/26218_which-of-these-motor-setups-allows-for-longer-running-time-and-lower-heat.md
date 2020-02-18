# Which of these motor setups allows for longer running time and lower heat?

### Replies: 21 Views: 1428

## \#1 Posted by: thetechtrader Posted at: 2017-06-26T21:18:28.267Z Reads: 156

```
Im debating these two setups but want the setup that runs longer with less stress on overall system:

In general, do lower KV motors like 170kv use up more battery power/life/run time vs 500kv?

Say I want a set RPM speed with lots of torque would I use:

1. A low KV motor like 170kv (maybe even 90kv for this project) with 12S, and reduction gearbox

OR

2. 500kv with 10S and reduction gearbox?
```

---
## \#2 Posted by: wafflejock Posted at: 2017-06-26T21:36:06.716Z Reads: 143

```
Doing the math:

170kv * 12 * 3.7 = 7548 rpm
500kv * 10 * 3.7 = 18500 rpm

500 is really a very high number from what I've seen most people stick in the 100-300 range somewhere.  Since 18500 rpm is more than twice 7548rpm I'm gonna guess the 500kv*10S is going to be more friction and more loss/stress in general (mechanically inefficient).  Sure you can do a greater reduction on the higher kv motor but it's still spinning at that speed and so it's internal bearings and the shaft are dealing with that extra speed regardless of what you do outside of that.  At 12V you're also going to get more Watts with less amperage and the amperage^2*ohms gives you the power loss in wires and the like so the higher voltage is generally more electrically efficient.

**edit missed the voltage multiplier but the math stays the same**
```

---
## \#3 Posted by: Alanhunt123 Posted at: 2017-06-26T21:41:12.137Z Reads: 137

```
Usually lower kv motors have more torque than an equivalent motor with higher kv. Lower kv is usually preferred for eSk8, since you want your low end torque to be good for starting from low speed, and for uphill riding.

Then there's also the concern of what kind of speed controller you're using. If you are using the VESC, you want to keep the ERPM (kv*7*voltage) under 60,000 to avoid frying the DRV chip. On 10S, (assume 42V full charge), you need a motor that is 204kv or lower. A 500kv motor like you suggest would fry a VESC. However, you didn't state your preferred ESC, so this may not be a concern to you.

Hope this helps!
```

---
## \#4 Posted by: thetechtrader Posted at: 2017-06-26T21:42:51.314Z Reads: 117

```
Thank you, well I'm building a custom hydrofoil board propulsion system and using VESC to control things. So dont picture a skateboard :)

I do need high RPM from 4400 - 10,000 RPM for this specific setup.
```

---
## \#5 Posted by: sl33py Posted at: 2017-06-26T21:49:09.148Z Reads: 109

```
recommend checking out the endless sphere forums for watercraft.

and why don't you water cool if on water?  heat would be relatively a non-issue w/ some basic water cooling.
```

---
## \#6 Posted by: thetechtrader Posted at: 2017-06-26T22:11:00.209Z Reads: 108

```
Ah.. ya, I was planning on using VESC, guess im building both setups now as I have half the parts for both and they wont work together, thanks guys, this forum rocks.. super fast answers, guess its why this site pops up on google for everything related to vesc and questions in the arena..
```

---
## \#7 Posted by: thetechtrader Posted at: 2017-06-26T22:14:47.131Z Reads: 104

```
Does anyone know where or if I can get 170kv Inrunner motor as that is only what will fit in this setup and must have wires out the back of motor, and not the side.
```

---
## \#8 Posted by: Alanhunt123 Posted at: 2017-06-27T02:45:59.048Z Reads: 91

```
Someone correct me if I'm wrong, but I believe the ratio between ERPM and RPM is completely dependent on the number of poles on the motor.

The outrunners we typically use on eSk8s have 14 poles, so to get ERPM from RPM, you need to multiply by 7 (number of poles÷2, or 14÷2 in this case). However, I think a lot of inrunners are 4 pole, so you might be able to get away with up to ~700kv if you have a 4 pole motor. If it's a 2 pole, you can go all the way up to ~1400kv!
```

---
## \#9 Posted by: thetechtrader Posted at: 2017-06-27T02:56:25.978Z Reads: 84

```
Wow, ya that makes a big difference, thank you for reading through and spotting that. My inrunner is 6 pole (500kv x 3 x 37v 10S = 55,500 erpm and may work...
```

---
## \#10 Posted by: Alanhunt123 Posted at: 2017-06-27T03:00:59.273Z Reads: 79

```
That sounds like it should work. Just go into your VESC settings and limit your ERPM in both directions to 60,000 (or lower, maybe 55,000 or 50,000 as a safety), and it should keep itself from over-revving. I've used motors that result in a higher ERPM before (245kv 7 pole on 10S, 72,000 potential ERPM), and just limited the RPM in the settings, and never had a failure. (My only failures have been due to electrical shorts on the motor wires!)
```

---
## \#11 Posted by: thetechtrader Posted at: 2017-06-27T03:05:05.188Z Reads: 74

```
Great to know thanks for looking out for me and helping... GREATLY appreciated!
```

---
## \#12 Posted by: thetechtrader Posted at: 2017-06-28T20:08:49.643Z Reads: 52

```
When you say shorts in the motor wires, did the melt down? 
What gauge wire should I be using for 12S running 50-125A as I need to run some longer wires about 6ft long to motor from battery.
```

---
## \#13 Posted by: Challlsss Posted at: 2017-06-28T20:53:02.030Z Reads: 46

```
You won't need more than 50A at 12S
10 or 12 Gauge will work
```

---
## \#14 Posted by: thetechtrader Posted at: 2017-06-29T15:07:56.366Z Reads: 37

```
Thanks,
Another question:
Say my motor has a max amp draw of 125A. If I limit the VESC to max 50A, and the motor is under load with wheel/propeller what issues will I have with motor trying to get up to speed, but does not have all the current it needs?

a. it will max out at 50A and keep running but not up to full speed if load it to high?

b. it will max at 50A until its up to speed then current drops off just to maintain speed?

c. motor breaks or some type of damage?
```

---
## \#15 Posted by: Challlsss Posted at: 2017-06-29T15:28:34.691Z Reads: 35

```
The VESC has a max motor and a max battery setting
The motor setting will be much higher than the battery setting. Just keep it below 125A and you'll be good
```

---
## \#16 Posted by: thetechtrader Posted at: 2017-06-29T15:57:32.879Z Reads: 34

```
I just dont want motor drawing more than 50a continious as VESC will burn out, that is my concern.
```

---
## \#17 Posted by: Hummie Posted at: 2017-06-29T16:02:07.958Z Reads: 35

```
If u want more than 50 (I just read 40 was enough to lift off the water) you can increase the battery and motor amps to much higher and if it's too much, and therefore gets too hot, it will just hit an over-temp shut-down and you'll be fine.   If u hook up some water cooling it'd be able to do way more. I think 160 is a possible hardware limit.
```

---
## \#18 Posted by: Challlsss Posted at: 2017-06-29T16:20:01.118Z Reads: 33

```
The vesc has **2** settings one for Battery max and one for motor max. I'm not sure why there are two but as long as you set the battery max correctly you shouldn't have an issue
```

---
## \#19 Posted by: wmj259 Posted at: 2017-06-29T16:42:06.209Z Reads: 32

```
Water cooling is a quite a mess. Especially if you go into any type of saltwater that can eat away at electronics. This would involve a water tight seal with a heat sink. 

It's similar to having a watercooled PC, if the hoses and seals are fine that it is a very good advantage, but if a seal breaks you basically lost your whole system, similar to the vesc, if something shorts in the vesc or battery, you will go flying off your hydrosail .
```

---
## \#20 Posted by: sl33py Posted at: 2017-06-29T17:46:22.029Z Reads: 35

```
I'm a long time watercooling PC geek.  I've killed a PC or two, but out of many, and years of use.

You can run a waterblock - or you can flush fit a heatsink w/ the exterior so it's exposed to the colder water.  Even mounted flush with a layer of CF/GF it'll cool better than in an enclosed space w/o airflow.  The other side FETs are the challenge then, and would need a waterblock most likely.  It's not hard to do it securely, and there are some PC watercooling "kits" now that are fully self contained - you could use a closed loop intended for a CPU/GPU on the top FETs i bet.  GIven enough space.  Or plumb flow through.  I'd look at some of the RC Boat solutions for cooling ESC's, which might be lighter and simpler.  And obviously proven and used for this type of use.

Tons of options.
```

---
## \#21 Posted by: thetechtrader Posted at: 2017-07-31T00:59:58.534Z Reads: 23

```
Thanks, yes just like any sport, if something fails you tend to crash. I prefer water sports like kiteboarding, surfing, and I'm now building my [DIY eFoil](http://www.diy-electric-hydrofoil.com/) propulsion system.

I posted some photos of motor setup on another post here: [DIY Electric Hydrofoil](http://www.electric-skateboard.builders/t/do-motor-wires-matter-which-ones-they-connect-to-vesc/28902/46)
```

---
