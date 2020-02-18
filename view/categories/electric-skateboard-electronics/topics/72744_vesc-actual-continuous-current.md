# Vesc actual continuous current

### Replies: 19 Views: 511

## \#1 Posted by: Ouch Posted at: 2018-10-29T21:47:36.235Z Reads: 142

```
Hey guys, this is my first post but I have been reading for a while.

I have a 6374 single setup and I need more current from my vesc.
I get thermal shut downs, the motor and bat can both take more current but the vesc is the bottle neck.
I currently run 63/63 motor/bat amps and it's OK but will over heat the FETs.
Which vesc will take the most current? I have a HK which has need good but I think it's around 30a cont, I'm looking for 55
Cheers
```

---
## \#2 Posted by: professor_shartsis Posted at: 2018-10-29T21:49:15.768Z Reads: 143

```
get a second motor and use half the motor current setting you currently use on both, you'll get the same acceleration performance and half the total losses (1/4th as much heating rate per vesc), boosting efficiency.
```

---
## \#3 Posted by: Ouch Posted at: 2018-10-29T21:50:55.578Z Reads: 137

```
This would be good but I like the simplicity and weight of a single set up, there must be a be a vesc that actually does the current it advertised
```

---
## \#4 Posted by: Livid Posted at: 2018-10-29T22:03:48.198Z Reads: 117

```
What vesc are you using? how's it installed?
```

---
## \#5 Posted by: Grozniy Posted at: 2018-10-29T22:06:38.481Z Reads: 114

```
He's using hobby king vesc.
I would recommend: ollin 4.12 vesc/focbox/flipsky 6.6 w/heatsink
```

---
## \#6 Posted by: Livid Posted at: 2018-10-29T22:08:02.132Z Reads: 111

```
make sure it's getting some airflow, maybe get some vrm heatsinks and put them on the fets to keep them cool, no need to fork out for a new esc
```

---
## \#7 Posted by: Ouch Posted at: 2018-10-29T22:18:41.174Z Reads: 108

```
Yeah I thought about heat sinks but I'm not sure if they will do much on the tops on the FETs, I was thinking a new vesc would be the easiest considering I am after 30/40% more cont current, does anyone know the continuous output of the onlins or flipsky 6.6, are they as good as they state?
```

---
## \#8 Posted by: professor_shartsis Posted at: 2018-10-29T22:25:06.817Z Reads: 105

```
[quote="Trillium, post:34, topic:71697"]
it’ll be a 200-300A motor current limit, with a custom controller my buddy and I are working on.
[/quote]

maybe @Trillium can help here...

[quote="Trillium, post:43, topic:71697"]
I don’t have any plans to pursue a 660A motor controller, as its another $40 of controller to make.
[/quote]
```

---
## \#9 Posted by: Livid Posted at: 2018-10-29T22:28:08.959Z Reads: 93

```
They will definitely help sitting on the top, they'll work even better if you cut the heatshrink out over the fets so it gets a bit better cooling, and a few slots in your encloseure will help. any vesc will thermal cutout if you keep it in an enclosed space under high load
```

---
## \#10 Posted by: Battosaii Posted at: 2018-10-29T22:31:09.775Z Reads: 89

```
300a at 1s I think he said lol
```

---
## \#11 Posted by: Ouch Posted at: 2018-10-29T22:39:01.466Z Reads: 92

```
Cool, I will give a heat sink a go before trying another vesc, see if that makes the difference, I like the water proof, air tight enclosure I have so I will put the heat sink in the air flow but not the vesc
Cheers
```

---
## \#12 Posted by: Battosaii Posted at: 2018-10-29T23:09:41.283Z Reads: 76

```
Sometimes just a heatsink would be enough but putting it in airflow will help for sure.
```

---
## \#13 Posted by: Jmding Posted at: 2018-10-29T23:19:55.470Z Reads: 71

```
I'm also running single 6374.  I've configured at +75/-75 motor, +60/-60 battery, with FSESC6.6 and have had no problems yet.  I am running 12s and 3:1 gearing with 76mm wheels though, to try to keep actual current levels low.  If the heatsinks dont fix it, maybe it is worth going up in voltage and up in gearing.
```

---
## \#14 Posted by: Battosaii Posted at: 2018-10-30T00:08:21.477Z Reads: 65

```
Damn 76 is very small only esk8 I've seen with those size wheels is boosted v1 with 75mm in heat wheels
```

---
## \#15 Posted by: dareno Posted at: 2018-10-30T01:07:00.725Z Reads: 62

```
I run hk vesc at 40 each and have no issues.
```

---
## \#16 Posted by: lrdesigns Posted at: 2018-10-30T01:07:15.325Z Reads: 62

```
[quote="Ouch, post:3, topic:72744"]
there must be a be a vesc that actually does the current it advertised
[/quote]

Unfortunately nope. And there is no standard for "continuous"  Although 1 minute is probably enough for esk8. 

I would recommend focbox or fesc 6.6

What voltage is your battery? If you go to a higher voltage you can run lower battery amps and still get the same performance.

[quote="Jmding, post:13, topic:72744"]
If the heatsinks dont fix it, maybe it is worth going up in voltage and up in gearing.
[/quote]
This is also a good suggestion. :point_up_2: I higher gear ratio will lower amp draw.
```

---
## \#17 Posted by: Ouch Posted at: 2018-10-30T13:35:10.748Z Reads: 50

```
I'm running 12s but with 90% duty cycle to stop the jolt as it goes to full duty cycle, and I'm running 15/40 with 83mm, I have a 42 on its way to run with my 97mm.
```

---
## \#18 Posted by: lrdesigns Posted at: 2018-10-30T14:14:10.138Z Reads: 46

```
Ok your pretty maxed out then. 

I would go for focbox and the cooling case By @Kug3lis
Not sure he still makes singles? 
https://shop.3dservisas.eu/collections/cases/products/single-focbox-case-without-cooling-fins?variant=5988890443803 

Also you could try lowering the battery amps and increasing motor amps see if it thermal throttles less. Like 70 motor 40 batt
```

---
## \#19 Posted by: professor_shartsis Posted at: 2018-10-30T16:30:16.106Z Reads: 35

```
[quote="Ouch, post:17, topic:72744"]
I’m running 15/40 with 83mm, I have a 42 on its way to run with my 97mm.
[/quote]

@Ouch this wheel/gearing change will require even more motor current to have the same acceleration as before...

97mm / 83mm =  **1.16x diameter increase**
2.8 / 2.66 =  **1.05x ratio increase**
(1/1.05) * 1.16 =  **1.1x top speed increase**
1/1.1 =  **0.909x acceleration/thrust decrease**
1/0.909 =  **1.1x more motor current required to have the same thrust/acceleration as previously**

to keep the same ratio of motor current to thrust i believe you'll need roughly 46T on your wheel pulley with the 97mm wheel.
```

---
