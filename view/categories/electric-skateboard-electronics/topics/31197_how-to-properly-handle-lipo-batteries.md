# How to properly handle Lipo batteries

### Replies: 11 Views: 1026

## \#1 Posted by: Mikkiller Posted at: 2017-08-21T22:32:36.439Z Reads: 172

```
Hi, I just got my 2x [5s 5000mah lipo batteries](https://hobbyking.com/it_it/turnigy-5000mah-5s-30c-lipo-pack.html) from hobbyking. I have a few doubts on how to properly handle them without ruining them, or worse, making them blow up. I'll just write a list of questions I have to make the post more tidy. I know they are probably noob questions, but I couldn't find answers in other topics.

For the record, I'l be using the batteries in series with a FOCBOX and a 6364 190kv motor. 

**_1._** Hobbyking wrote on the box that the batteries are **30% charged** and that they **need to be charged to storage charge** ASAP. First of all, how much is storage charge? How much time do I actually need to charge the battery before they get fucked up? I won't be using them for at least 2 weeks (probably more) because I'm waiting for the other components to arrive.

**_2._** To charge and to use the batteries I need to **put an XT60 connector** on them. They came with bullet connectors and a **8awg wire**, which looks rather thick for an XT60 connector. Can I trim a few mm from it  and solder it on an XT60 connector, like they do in this video? Does this affect performance or is it dangerous in any way?

https://www.youtube.com/watch?v=8H1Ib6Gihy0&t=27s&index=3&list=PLZ9A1G_uWwES_NLeCy8QbcIBrS8Grtrha

**_3._** Once built, I probably won't be using my esk8 for 2-3 months at least (I'm moving to a place where laws on esk8s are really strict). Is it best to keep the batteries connected to the VESC or to take them out of the esk8?

**_4._** How exactly do I charge the batteries? On my lipo charger (I-MAX B6) I can choose different programs and different Amps for charging (1.0 to 5.0). What should I choose?

Thanks a lot in advance for your answers, this forum has helped me a lot :slight_smile:
```

---
## \#2 Posted by: nw-esk8 Posted at: 2017-08-21T22:49:24.801Z Reads: 159

```
(DISCLAIMER:  I'm kind of a noob w/ lipos... I have some experience coming from RC cars/quads, but I'm much more familiar with the best practices for lithium ion cells.)

1) Guessing a bit here, since I'm not as familiar w/ lipos, but for lithium ion you want to store them around nominal voltage (3.6v/3.7v) where they are most stable.

2) That's more than fine. Even if you're charging at 10a (max for those packs... 2C * 5AH) at 18.5v (5s), you're only looking at 185 watts.  There is guidance online about watts vs. wire gauge for a given distance, but you're nowhere near the recommended limits, especially for charging.

3) You don't necessarily have to take them out, but they should be disconnected from the VESCs (either unplugged or via switch, etc) or anything else that could have a slow drain on them.

4) 1C = 5 amps should be a good starting point.  They are rated up to 10A (2C) charging, but if you charge at 5, it should be easier on the batteries (at least it is w/ li ion cells) and maximize the life of the batteries.
```

---
## \#3 Posted by: Rinzler Posted at: 2017-08-21T22:53:49.966Z Reads: 152

```
1.I kept my batteries for 3 weeks until my components arrived, the voltage they where shipped at was something like  3.73V per cel which is not too far from the recommended 2.8V for storage.They will be fine.If you can charge them,charge them.

2.Shortening the wire increases performance, lenghtening decrease it.Also when soldering dont let the phase wires touch, if they do youre in for a fireworks show.The connectors are fine, rated for 60A.

3.Discharge or charge the battery to 3.8v per cell, every cell needs to be balanced.Take them out and store in a cool dry place.Bonus points if you put them in fireproof bags and fire resistant enclosures. 

4.Charge on a lipo charger with balance leads plugged in.The charging amp rating should be 1C, to calculate it take the Ah of your finished battery and multiply it by 1.But for longevity charge at 0.5C
```

---
## \#4 Posted by: Hummie Posted at: 2017-08-21T23:16:55.995Z Reads: 136

```
trying to get too fat a wire on those xt60 will be easy short potential.  all those xt plugs with the slide-up cover are kinda risky because you have to have the two wires so close together.   xt90s maybe at least you should try.  I use xt90s and doubt youi'll get the 10awg on the 60s.   even with the 90s and 12awg I just fit and that's without adding shrink wrap as in this video.  the wires really have to fall into the spot theyre supposed to go with those or getting that cover to come down over everything doesn't happen.
```

---
## \#5 Posted by: Mikkiller Posted at: 2017-08-22T06:48:24.376Z Reads: 116

```
Thank you everyone for your answers. 
There is something I still haven't completely understood. Do we measure the charge of the battery in volts? I've always seen it measured in mAh (laptops, smartphones etc.).

I see that my charger has a storage function, so I guess it will charge/discharge the batteries to 3.8v. 

Also, for how long can I store a battery at storage charge if it is not connected to the vesc?

Last question about BMS: if I use a cheap BMS for charging only, will it protect my batteries in any way? From my understanding, only more expensive BMSes can discharge at a rate sufficient to power an esk8
```

---
## \#6 Posted by: nw-esk8 Posted at: 2017-08-22T09:33:05.362Z Reads: 99

```
Yeah, you measure the charge/level of the battery using volts.  mAh or Ah refers to how much current the battery can supply.

*3.8 (or w/e)... per cell... so, w/ a 5s (5 cells in a **s**eries), that'd be ~19v.(or 21v fully charged)

As far as how long you can store... it depends... better batteries will last a long time (years), but some may only last months.

RE: BMS: No, not really, AFAIK... other than not overcharging, etc.  Those batteries are rated at 150A discharge (30c x 5ah), but I think that's probably overrated by a decent margin...and if you're going w/ a single focbox/motor, then you couldn't use all of that anyway (focbox = 60a continuous max).  A 10s 60A BMS is going to be $38 or less... probably just a few $$ over a smaller one that is going to be discharge bypassed.
```

---
## \#7 Posted by: ShutterShock Posted at: 2017-08-22T14:07:43.555Z Reads: 85

```
I managed to fit two 10 AWG wires onto my charging connector for my board when I set up my bms, it is a little bit tight, but it can be done.  However, both are covered in heatshrink and my joints are very clean on the inside.  I tinned the wires and then cut the tips into a chisel shape to better fit into the rear of the connector.  

10AWG works perfectly for my XT-90's, I used the BenTechGo stuff from Amazon, and it's super nice.
```

---
## \#8 Posted by: rich Posted at: 2017-08-22T18:25:01.025Z Reads: 72

```
[quote="Mikkiller, post:1, topic:31197"]
To charge and to use the batteries I need to put an XT60 connector
[/quote]

You could just solder a short adapter wire. Once I soldered 10AWG to XT60, it was a pain. Do you use an antispark switch? Because if not you should use XT 90 antispark and a fuse. Why it must be XT60?

With your balance charger you have to charge the batteries seperately, that sucks! On my first build I had the same,charged the 2 lipos one after one. Often the first Lipo was full and i wanted to ride but had to wait for the second. And balance charger are often lame.

I have 2 builds now running with 10s (one finished). For my finished one i use 2 lipos in series with bypassed bms for charging only. The bms was 10€ and the 3A li-ion charger 18€ from china, waterproof charging port was 5€ for 10 pieces. This combination works well (I use vedder antispark switch with fuse). The funny thing is that bms and charger were cheaper than the cheapest HK balance charger. I love it. Just plug the charger and that's it. The charging time is ridicolously short copmpared to my balance charger.

On my second build I'll use 10s4p Li-ion and BMS (60A cont./120A max. for 40€) for discharging/charging. The advantage of this kind of BMS is that you have much more safety features compared to fuse only.
```

---
## \#9 Posted by: Mikkiller Posted at: 2017-08-22T22:42:34.985Z Reads: 59

```
I want to use an XT60 because the FOCBOX uses XT60s and I have already bought the series connector and all. Also, my balance charger came with an XT60 cable for charging. 

I know that using a BMS for charging is better and faster, I will look into it in the future ( I just started to understand the most basic stuff :joy:)

Anyway, thank you so much to everyone for being so kind and helpful. Your help has been precious to me
```

---
## \#10 Posted by: rich Posted at: 2017-08-23T05:08:56.301Z Reads: 54

```
[quote="Mikkiller, post:9, topic:31197"]
I want to use an XT60 because the FOCBOX uses XT60s
[/quote]

If you don't use an (antispark) switch or XT90 antispark between battery and FOCBOX you'll get a loud and shiny spark everytime you plug it. It will work but could damage the FOCBOX in long term and also the XT60.


[quote="Mikkiller, post:9, topic:31197"]
I know that using a BMS for charging is better and faster, I will look into it in the future ( I just started to understand the most basic stuff :joy:)
[/quote]

You are right, don't rush with the BMS, it also took some time for me to fully understand and it can be dangerous if wrong connected. Also earlier I thought it's a good idea to buy another balance charger for charging the second lipo at the same time. Fortunately I've never tried that because it would short the battery (or destroy one charger in best case) if the two lipos are connected in series and not disconnected.

No matter the charging, riding is always the same fun :wink:
```

---
## \#11 Posted by: Mikkiller Posted at: 2017-08-23T06:17:37.273Z Reads: 51

```
Yeah, I forgot to mention that I am buying an antispark switch (with xt60s)
```

---
