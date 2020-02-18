# Trampa motors low kv

### Replies: 32 Views: 3030

## \#1 Posted by: f1rstb81 Posted at: 2016-12-05T06:03:57.943Z Reads: 388

```
Has anybody tried the low kv super expensive motors from trampa and if so any input on performance and top speeds your getting trampa says if you like the sk3 you will love the trampa motors the only problem I'm seeing for me is the low kv it's good for torque but not so good for speed I believe. I'm putting together parts for a emtb build and trying to put together the right setup for me. I will be using it in the grass and dirt but on concrete the most no tricks or jumps just riding for fun and some commuting.
```

---
## \#2 Posted by: saul Posted at: 2016-12-05T06:13:33.395Z Reads: 387

```
on 8" pneumatics you still get plenty of speed. Lower kv should actually give better efficiency at cruising speed.

most mtb builds use 149kv but this is the lowest kv for stock sk3's. only aps has lower kv.
```

---
## \#3 Posted by: trampa Posted at: 2016-12-05T21:16:06.663Z Reads: 350

```
Hi, we really tested out the motors to be perfect for MTB usage. 
The actual no load KV is slightly higher. 118KV@1Nm is roughly 125KV at zero load. 136KV@1Nm is roughly 145 at zero load. Both motors have fantastic torque and use only the finest components. Gearing down is an issue on MTB builds, so riding 12S requires low KV motors. Gearing to 40km/h is about right for MTBs, twin motors are a must have IMOH.

Frank
```

---
## \#4 Posted by: saul Posted at: 2016-12-05T22:40:03.536Z Reads: 332

```
@trampa I keep forgetting you're on here now. 

There's not much info on these motors. are they 6374 size?
anything more custom mods aside from kv? Delta or Wye?
```

---
## \#5 Posted by: laurnts Posted at: 2016-12-06T00:10:53.984Z Reads: 319

```
I have these motors, so well build and powerful. But I havent tested it out to the max, didn't have to as I don't ride hard. One thing I didn't like, the white color. All the rest of trampa is on black, only the motor is white. Maybe that would be a feedback for @trampa in the future.
```

---
## \#6 Posted by: f1rstb81 Posted at: 2016-12-06T03:53:49.918Z Reads: 309

```
Do you ride twin motors or single and what type of speed you producing with your setup.
```

---
## \#7 Posted by: laurnts Posted at: 2016-12-06T09:55:38.244Z Reads: 298

```
Twin motor. 24v 118kv 14 tooth, top speed 25kmh, very slow.
Currently I am going to upgrade to 36v to reach 30-35kmh, not aiming going faster atm.
```

---
## \#8 Posted by: f1rstb81 Posted at: 2016-12-06T10:17:31.839Z Reads: 290

```
Yeah that's what I'm afraid of I'm wanting about 30-35mph on 12s I'm looking at the trampa 136kv motors just not sure if I would get the speed I'm looking for
```

---
## \#9 Posted by: trampa Posted at: 2016-12-06T12:03:51.743Z Reads: 276

```
This should give some answers:

http://www.trampaboards.com/gearing.php
15/66 gearing, twin engine, 12S, 136 KV = 29mph = More than fast enough for an MTB.

Frank
```

---
## \#10 Posted by: f1rstb81 Posted at: 2016-12-07T09:36:25.017Z Reads: 257

```
That may be fast enough for you but you can't tell people what is fast enough for them because that's not enough for me I need a about 10 more mph to be on the safe side not gonna ride full speed all the time I just want it there for when it's needed
```

---
## \#11 Posted by: trampa Posted at: 2016-12-07T22:43:28.123Z Reads: 250

```
Well, speed whobble gets an issue at 30+ mph and gearing to that speed makes you run outside the peak performance of the electrical system most of the time. It's a matter of the perfect balance. However, if you want to go faster, you simply drop in a bigger motor pulley. Its that easy! That's the beauty of a transmission. A bigger motor sided pulley is better anyway. 

Frank
```

---
## \#12 Posted by: trampa Posted at: 2016-12-07T22:49:58.627Z Reads: 240

```
If you like them black, its easy to stick some foil on. I used car foil. 5minute job... We like the white, since white was always our Ultimate range. There are to many black motors out there. Glad you like the Quality. These motors are made without compromise an you can feel that. 

Frank
```

---
## \#13 Posted by: trampa Posted at: 2016-12-20T18:54:05.384Z Reads: 227

```
Our motors are 6364, ultra high temp copper, best magnets you can buy today, Japanese precision bearings, hardened axle shaft, hall and temp. sensor, CNCed housing with extra long front cap and dust filter disc, dual keyway shaft, delta connected and hand wound for 100% copper fill. Full spec in every detail....

Frank
```

---
## \#14 Posted by: Randyc1 Posted at: 2016-12-20T19:11:21.307Z Reads: 223

```
Can motors be purchased alone ?
```

---
## \#15 Posted by: trampa Posted at: 2016-12-20T19:44:09.507Z Reads: 228

```
http://www.trampaboards.com/136-kv-2400w-dc-brushless-motor-6364-61-p-12967.html

Frank
```

---
## \#16 Posted by: ripcurldog Posted at: 2018-05-12T18:15:21.670Z Reads: 175

```
Does anyone have settings for the 136kv TRampa motor (for the VESC6 settings)?  The motor setup asks for motor amps and battery amps.  I'm using the Trampa 136kv motor with 4 * 6s batteries (12s2p).  I can't find these settings anywhere on Trampas web site.  There are no videos, nothing.
```

---
## \#17 Posted by: rich Posted at: 2018-05-12T18:31:47.953Z Reads: 172

```
For motor amps you can set 45-50A. The batt max and regen depends on your battery. You can find further info here: https://www.vesc-project.com/node/178
```

---
## \#18 Posted by: E1Allen Posted at: 2018-05-12T18:44:16.745Z Reads: 169

```
What Rich said.  It's a 2400w motor.  Divide by voltage and you get Max amps.  45-50 is good for both batt Max and motor Max according to the specs.
```

---
## \#19 Posted by: ripcurldog Posted at: 2018-05-12T20:53:47.344Z Reads: 175

```
thanks.  Does the sensor option need to have HALL sensor added, or do I leave it as sensor-less.  I have a cable from the motor attached to the sense port.  

I set motor max and batter max to 50A - thanks for that.

What would you suggest for the voltage cutoff start and end specs?  I am using 4 * Zippy 6S 6200mah 40C .  12S2P essentially.
```

---
## \#20 Posted by: E1Allen Posted at: 2018-05-12T21:00:15.106Z Reads: 173

```
3.4v per cell is conservative for lipo. Maybe cutoff at 3.2 but I recommend not below 3.0v per cell.
```

---
## \#21 Posted by: trampa Posted at: 2018-05-12T21:24:15.965Z Reads: 166

```
In vesc-tool you can set the cutoff by cells used. Select 12 cells and press the black apply button.

Sensor should be used. Select Hall sensors. Sensor detection is done after measuring the motor parameters. 

There is a step by step guide on the vesc-project website. Click on Documentation.

45-50A is fine for the motor btw. Brakes at -30A (both, motor regen and battery regen)
```

---
## \#22 Posted by: ripcurldog Posted at: 2018-05-13T03:00:23.436Z Reads: 157

```
Thanks.  I just read that to get AMps of your battery, for the 6200mah, 40C 6s battery, you multiply 6.2A * 40C and you get your max amp output (248A).  So can't I set my battery current max to much higher than 40 to 50?  I rode my board today for the first time.  It studders at low speed (just upon take off).  If I increase the motor current max to say, and the battery current max to 80, will that be safe?  I am using FOC.  I didn't have the HALL (Sensor) option selected because I read your comment after my ride.  Would that fix the sag/studder?
```

---
## \#23 Posted by: Achmed20 Posted at: 2018-05-13T08:11:34.389Z Reads: 143

```
stuttering  when starting is normal if you do not have a sensor, if you have them, enable them.

the sensors figure out where the magnets currently are. and if the ESC doesnt know where they are, it will just fire up the wrong magnets and create the stuttering in the process..
```

---
## \#24 Posted by: rich Posted at: 2018-05-13T19:18:37.076Z Reads: 144

```
[quote="ripcurldog, post:22, topic:14198"]
So can’t I set my battery current max to much higher than 40 to 50?
[/quote]


It wouldn't make sense, the batt max. is never set higher than motor amps. Don't go higher than 50A with this motor.

[quote="ripcurldog, post:22, topic:14198"]
I am using FOC.  I didn’t have the HALL (Sensor) option selected because I read your comment after my ride.  Would that fix the sag/studder?
[/quote]

With sensored FOC this motor is supersmooth at startup but not with sensored/hybrid BLDC so stay with FOC and use the sensors, no more studdering :grin:


[quote="ripcurldog, post:19, topic:14198"]
What would you suggest for the voltage cutoff start and end specs?
[/quote]

Personally I set 42V (3.5V per cell) as cutoff start and 40V (3.2V per cell)  as end.
```

---
## \#25 Posted by: CheapSk8s Posted at: 2018-10-29T17:58:34.799Z Reads: 112

```
Hi guys,

Just thought I'd reactive an old thread as I have a similar kind of question if thats okay.  Me and some mates are getting Trampa pro drive emountain boards but unsure what the best motor option would be in the build.  We're new to this and would appreciate any input.  I'm heavy set at 15 stone and cant decide between the 118kv with 15 tooth cog or the 154kv with the 13 cog.

It'll be used for mixed terrain, plenty of flats and plenty of hills so a mixed bag.  We will be using 2 x 6s 22000mAh HRBs.

Cant seem to decide which way would be best - if anyone has 2 cents worth they would like to throw in, it would be much appreciated!

Thanks chaps, just don't want to make any expensive mistakes if there are mistakes to be made here :slight_smile:
```

---
## \#26 Posted by: Santino Posted at: 2018-11-01T15:48:04.457Z Reads: 110

```
Hi, I have Trampa 154kv twin, 14 teeth all rounder and 15 teeth...My weight 75 kilos (not really heavy). But I use 4 6s HRBs, so my set up is 12s (really torque beast)...My thoughts, the lower the kv the highest torque, so if you are planning on ridding the way described, I would think about the battery, since 12s with a high C rating on a twin set up, with 14 teeth on motor pulley, will be more suitable for your needs. Also If I were you, will write to Trampa, because they are going to be releasing a 6380 motor soon, just to check with them....Hope this helps..
```

---
## \#27 Posted by: Sooty Posted at: 2018-11-18T20:42:10.790Z Reads: 106

```
What performance benefits will 6380 give?
```

---
## \#28 Posted by: trampa Posted at: 2018-11-18T20:53:02.887Z Reads: 103

```
[quote="rich, post:24, topic:14198"]
It wouldn’t make sense, the batt max. is never set higher than motor amps. Don’t go higher than 50A with this motor.
[/quote]

Actually you can set the battery max same as motor max. You could also set it way higher, since motor max will define the max battery current in that case. It will never be exceeded even if you would drop in 100A for battery max.
```

---
## \#29 Posted by: Tamim Posted at: 2019-12-30T02:07:16.136Z Reads: 41

```
Hi, I came upon 2 TRAMPA 118kV motors and I'd like to use them for an autonomous mini car that I am building. However, there are no data sheets available for the motors online and I am not sure if they would fit my requirement of providing 11Nm at 105 RPM. Can anyone help me with this please ?
```

---
## \#30 Posted by: Hummie Posted at: 2019-12-30T06:02:43.740Z Reads: 37

```
[quote="trampa, post:13, topic:14198"]
Our motors are 6364, ultra high temp copper, best magnets you can buy today, Japanese precision bearings, hardened axle shaft, hall and temp. sensor, CNCed housing with extra long front cap and dust filter disc, dual keyway shaft, delta connected and hand wound for 100% copper fill. Full spec in every detail…
[/quote]
What does that mean? Not a real spec in it. 
I’ve never seen 100% copper fill in my life and pretty much impossible.  Amazing how empty advertising can be.
```

---
## \#31 Posted by: trampa Posted at: 2020-01-04T09:43:47.353Z Reads: 32

```
11Nm is too much. 4Nm is possible on the 118. With gearing you can up the Nm at the wheel.
```

---
## \#32 Posted by: Hummie Posted at: 2020-01-04T16:34:14.603Z Reads: 30

```
Kv doesn’t determine max torque. A motor the same size can produce the same torque regardless of its kv.
```

---
