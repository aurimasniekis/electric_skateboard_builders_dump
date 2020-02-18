# Help with new build electronics

### Replies: 27 Views: 824

## \#1 Posted by: ArsenalMain Posted at: 2018-02-03T06:05:49.000Z Reads: 124

```
Hello, I am a new builder and I have been researching and gathering information on what components I should get. After much investigation, I have determined, for the most part, what parts to get. These include:
Motor Kit:
Single drive motor kit with 83 mm wheels
products/single-motor-mechanical-kit

Motor:
Sk3 6374 192kv Brushless Outrunner- 80A
https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-192kv-brushless-outrunner-motor.html?___store=en_us

Battery:
2x 5s1p 8000mAh 30c Batteries (https://hobbyking.com/en_us/zippy-flightmax-8000mah-5s1p-30c-xt90.html?___store=en_us) in series.
I already know that I need to buy a series adapter

VESC:
products/torque-esc-vesc-bldc-electronic-speed-controller

Board:
I'm using the board that I currently use to get around. 

In spite of my many hours of searching, I have a few questions that I would love answered:
----I know that I need to get a BMS. The problem is that I don't really know why you need one. I know you need it to balance charge your higher felled batteries but I don't know what specs to look for. 
----After getting the BMS, I need the charger. In one thread, someone mentioned a bulk charger but I am unsure of what that is exactly. 
---- For the VESC, i know that the current max is around 50A, but I know that people use motors rated beyond that current. I am aware that there are two different curcuits at play and that the battery can be pulled at 50% voltage but still produce enough current for the motor. Regardless of this, will my motor be bottlenecked? 
----Does a loop key basically count as a on/off switch so you don't have to continually plug and unplug the batteries? 
----Did I miss anything major or any other connectors that I may need? 

Sorry for the long post, I just wanted it to be thorough so I can get some clear answers. 

Thank you
```

---
## \#2 Posted by: ARetardedPillow Posted at: 2018-02-03T06:45:13.511Z Reads: 100

```
Be sure to learn to solder and buy some xt90 connectors, bullets and an xt90 anti-spark, you're going to need it

Also, a balance charger, or else you won't be able to even charge your batteries, unless you're going to use a bms which is going to be just a tad more complicated and also requires soldering.

A loopkey completes the circuit, you don't unplug and plug in your batteries, and make sure its an anti-spark loopkey

(I really do not recommend getting a bms at this point, use a balance charger first and understand the basics of the electronics then move onto a bms)
```

---
## \#3 Posted by: louwii Posted at: 2018-02-03T07:58:08.349Z Reads: 88

```
I would say a BMS requires some skills and understanding to be wired properly. If you're still not sure about all this, a balance charger is an easy option. That's what I'm using right now.
```

---
## \#4 Posted by: ArsenalMain Posted at: 2018-02-03T16:41:37.212Z Reads: 65

```
Do you think going the bms route would be more advantageous for future projects and builds or would you just recommend sticking to the balance charger?
```

---
## \#5 Posted by: Achmed20 Posted at: 2018-02-03T16:46:14.074Z Reads: 66

```
it will since you jsut have to plug in a power supply to your board and not remove the batterys every time you want to recharge
```

---
## \#6 Posted by: ArsenalMain Posted at: 2018-02-03T16:55:02.590Z Reads: 57

```
My biggest question a out bms's is how to determine which currencts to pick for the continuous discharge. Also, someone mentiomed that if I get a bms, I need to get something called a bulk charger. I don't really know what that is.
```

---
## \#7 Posted by: Sebike Posted at: 2018-02-03T17:07:43.816Z Reads: 54

```
Depending on 2 things mainly.. Are you going to use bms for both charge and discharge and how many amps will you draw from the whole pack ; ie what cells and how many in parallel? 

If only for charging, a lower rated bms will be fine as long as you pay attention to it being matched up regarding number of batteries in series and type of cells. 

If using for discharge as well it depends on your battery and how many amps you will draw. For example a 10s4p battery would usually require a bms rated at 60 or 80 amps. 

I use 10s4p with 30q cells with a 60a bms for discharge.

The charger is usually a laptop style charger. Match according to batteries in series and type of cells and choose how fast you want to charge ; output charging amps.
```

---
## \#8 Posted by: Holyman92 Posted at: 2018-02-03T17:20:01.545Z Reads: 55

```
You do know that diy skate sells 6374 motors right?![518bed8205949e153446537f696eeac29c24887d_1_374x500|374x500](upload://7Sw9rz3EtBPmL7QAqAkX0Z8RMwN.jpg)
```

---
## \#9 Posted by: Holyman92 Posted at: 2018-02-03T17:21:36.798Z Reads: 52

```
If you get their 218mm truck upgrade option, later on down the road u can upgrade to dual rear motors
```

---
## \#10 Posted by: ArsenalMain Posted at: 2018-02-03T17:34:29.331Z Reads: 50

```
@Holyman92 That is a good recommendation, to go for the 218 trucks to future proof it. Also, the reason I will go through hobby king for my motor is that it is ~$40 less expensive.  @Sebike the batteries that I am planning on getting are 2 5s1p batteries. Does this mean  it would be a 10s2p battery? Also, if I go for a bms for both charge and discharge, won't it be significantly more expensive then a low rated bms for charging only?
```

---
## \#11 Posted by: Holyman92 Posted at: 2018-02-03T17:35:50.050Z Reads: 47

```
Sk3, don't have hall sensors and 30$ for a sensors motor really isn't that bad
```

---
## \#12 Posted by: ArsenalMain Posted at: 2018-02-03T17:36:46.418Z Reads: 47

```
Because I know that's you got the VESC from diy, any chance you know the answer to my VESC question regarding motor bottlenecking with the low max current in the vesc?
```

---
## \#13 Posted by: Holyman92 Posted at: 2018-02-03T17:37:41.512Z Reads: 48

```
I don't, I haven't set my board up yet... I have to get the trucks, mounts and drive kits still
```

---
## \#14 Posted by: ArsenalMain Posted at: 2018-02-03T17:37:49.086Z Reads: 45

```
I've heard mention of that. What exactly is a sensored motor? And in another thread, someone mentioned that the vesc is able to make up for a sensor less motor
```

---
## \#15 Posted by: Holyman92 Posted at: 2018-02-03T17:38:49.963Z Reads: 44

```
The vesc can but sensors help the vesc understand the orientation of the motors stator, helps to keep the motors in sync
```

---
## \#16 Posted by: ArsenalMain Posted at: 2018-02-03T17:42:20.868Z Reads: 40

```
So if I end up going to a dual mount at some point, it will be alot more beneficial to sensored motors? My only hang up I'd that the hobby king motor has about 1000 more power capability than the diy motor. @Holyman92
```

---
## \#17 Posted by: Sebike Posted at: 2018-02-03T17:46:09.940Z Reads: 42

```
If wired in series 2x 5s1p will double cells in series ; 10s1p. If wired in parallel this will double cells in parallel ; 5s2p.

A higher amp rated bms will cost more than a lower rated bms if going with same quality range bms. 

The charger you need could be cheap though. Without bms your cells won't be balance charged unless you solve balance charging some other way. 

Plenty to read on these topics in other threads...
```

---
## \#18 Posted by: ArsenalMain Posted at: 2018-02-03T17:48:34.158Z Reads: 41

```
Ya definitely. The question  that I keep trying to figure out though, that I can't find on other threads, is whether or not the motor will be bottlenecked with the max 50A on the vesc, considering the motor is rated at 80A max.
```

---
## \#19 Posted by: Sebike Posted at: 2018-02-03T17:52:40.117Z Reads: 38

```
Vesc rating is regarding drawn amps from battery. That's more related to your battery output and not as much with the motor. Motor amps are what the vesc feeds it with, which can be limited in the vesc software.
```

---
## \#20 Posted by: Holyman92 Posted at: 2018-02-03T17:53:33.083Z Reads: 36

```
@Sebike he could always do what I'm doing, get a BM12 cell logger (or any other cell logger) and a balance charger, u will have total control and monitoring of your cells at all times with the added feature of the cell logger alerting you if your cell gets too low or too far outta balance... with a BMS u have to trust that it's working and hope it doesn't break.... If it does break u won't know (usually) until u have caused permanent damage to ur cells
```

---
## \#21 Posted by: Achmed20 Posted at: 2018-02-03T18:06:33.986Z Reads: 34

```
[quote="ArsenalMain, post:6, topic:45427"]
My biggest question a out bms’s is how to determine which currencts to pick for the continuous discharge.
[/quote]
if you are going with lipos, then jsut use the cheap BMS for charging and skip it all together when drawing power (its simple wiring solution).
if you go with Li-ion', then you probably should go the expensive route. unless you pack can spit out more then 80A and if you use only one motor.
```

---
## \#22 Posted by: ArsenalMain Posted at: 2018-02-03T18:30:48.643Z Reads: 32

```
The batteries are 8000mAh and rated at 30c so it could handle the 80A, the I might be moving up to a dual motor at some point however. I think the route you suggested is the best one though, just using it for charging and then have a loop key for its connection to the vesc. @Holyman92 brought up a good point. Would it be more worth it to go for the sensored motor at $40 more or the unsensored motor (which could output 1000w more)?
```

---
## \#23 Posted by: ArsenalMain Posted at: 2018-02-03T18:32:06.826Z Reads: 28

```
And thank you all for your help. I know that some of these questions have been answered in other threads, I just couldn't find them all. I appreciate the time you took to answer.
```

---
## \#24 Posted by: Holyman92 Posted at: 2018-02-03T18:39:40.424Z Reads: 30

```
since both motors can only handle 80a max, and have different wattages, u can do the math which tells us the only difference is the ammount of voltage u can pass through them... going based on the max amps and the max wattage for the DIY motor u can pass 39.37v through it (based on their ratings) and the SK3 can handle 50.4v. 

so i guess it depends on what u plan to do power wise, and rather or not you want to kick off before starting ur motors or just take off from a stand still... my understanding of non sensored motors is twitchy startups, however this is all just from me reading about in the forums
```

---
## \#25 Posted by: ArsenalMain Posted at: 2018-02-03T19:28:14.875Z Reads: 28

```
This is completely different area than we were discussing, but i just read through the whole loop key thread that you were a part of a couple months ago. Many of the contributors to that thread used different sized connectors for the connection. @sl33py used 6mm bullet connectors, while others used as small as 2mm bullet connectors. Does it matter which size I go with?
```

---
## \#26 Posted by: Sebike Posted at: 2018-02-03T20:07:24.429Z Reads: 27

```
Not sure I'm following... Loop key usually involves an anti-spark connector, and most people use a XT90S plug for this. The connector itself is 4.5 mm I believe. Did this answer your question at all?

Edit:
Oh ok. >Checked the thread. My suggestion is not to overcomplicate things by diying the anti-spark plug itself using a resistor and bullets aso, just go the easy way using the XT90S and you're fine. 

If using bullets on battery side, I'd say you're definately good using 4-6mm.
```

---
## \#27 Posted by: ArsenalMain Posted at: 2018-02-03T20:50:28.837Z Reads: 25

```
@Sebike thanks for the help, I got pretty much everything cleared up by now, and I can get everything else from other threads
```

---
