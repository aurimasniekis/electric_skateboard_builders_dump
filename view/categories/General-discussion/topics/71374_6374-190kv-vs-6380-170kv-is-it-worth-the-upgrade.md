# 6374 190kv vs 6380 170kv; is it worth the upgrade?

### Replies: 33 Views: 1392

## \#1 Posted by: Jasonkimberson Posted at: 2018-10-16T05:19:48.034Z Reads: 313

```
6374 190kv vs 6380 170kv; is it worth the upgrade?  I have both but not sure if it’s worth the effort to switch them out?


![image|375x500](upload://on8nixDKHwRcEZRrAj0xopkxAvj.jpeg)
```

---
## \#2 Posted by: Skunk Posted at: 2018-10-16T05:27:13.598Z Reads: 308

```
Lose a bit of top speed for a bit more torque.
The Chrome is sexy
```

---
## \#3 Posted by: Andy87 Posted at: 2018-10-16T05:32:54.690Z Reads: 307

```
Is it so big deal to swap motors in your build?
If no than just install them and have a look.
You already have both laying around...
You can always switch back...
```

---
## \#4 Posted by: Jmding Posted at: 2018-10-16T05:47:32.795Z Reads: 298

```
No, they are not worth it.  They are both rated to 12s and 80A.  Power = voltage * current, so they are both rated to the same power.  Changing the motors lowers the Kv, which increases torque at the expense of speed, but you can achieve the exact same effect by changing you gearing or wheel size.

Now, if they had taken advantage of the extra stator length to reduce the number of turns from 14 to 12, they could have made a 190 Kv, 90A, 6380 motor.  Then it would have been capable of 12.5% more power than the 6374.  That might have been interesting.  But alas...
```

---
## \#5 Posted by: Skunk Posted at: 2018-10-16T05:52:50.675Z Reads: 292

```
Thers probably a quality difference between the too as well. Good to keep in mind.
```

---
## \#6 Posted by: lrdesigns Posted at: 2018-10-16T06:26:48.547Z Reads: 281

```
[quote="Skunk, post:2, topic:71374"]
Lose a bit of top speed for a bit more torque.
[/quote]

Or go up motor pulley size for same top speed and torque and more reliability! This is why I like low kv motors. 

@Jasonkimberson what size is your motor pulley now? 

On the other hand more torque = better brakes which is for sure safer. More acceleration is more fun unless your a top speed :syringe:  junkie.
```

---
## \#7 Posted by: Jasonkimberson Posted at: 2018-10-16T06:36:22.177Z Reads: 267

```
15t/36t is my current gear rationrunninb 107s
```

---
## \#8 Posted by: Skunk Posted at: 2018-10-16T06:37:12.077Z Reads: 258

```
How often to you ride at top speed/full throttle? 
Climb hills much?
```

---
## \#9 Posted by: Jasonkimberson Posted at: 2018-10-16T06:45:08.405Z Reads: 255

```
The board is working really good right now, kind of don’t want to mess with it unless it’s worth it.  The chorme is pretty sexy though.  To get these motors to work, I would have to make cable extensions and move the motor mounts 5mm out.
```

---
## \#10 Posted by: thiswasandy Posted at: 2018-10-16T06:56:56.028Z Reads: 251

```
Save the other motors for your next build.
```

---
## \#11 Posted by: Skunk Posted at: 2018-10-16T07:02:53.710Z Reads: 247

```
Awd.... you know you want too
```

---
## \#12 Posted by: Sender Posted at: 2018-10-16T13:14:12.344Z Reads: 233

```
If your board is humming right now, I would leave it as is.  If it has to go on the bench for something else, try the motors.  Like @thiswasandy said, save these beauties for the next build!
```

---
## \#13 Posted by: mmaner Posted at: 2018-10-16T13:28:29.336Z Reads: 234

```
[quote="Sender, post:12, topic:71374"]
If your board is humming right now, I would leave it as is
[/quote]

This :arrow_up:
```

---
## \#14 Posted by: stewie Posted at: 2019-02-20T07:11:11.955Z Reads: 185

```
Are the TorqueBoards Motors Waterproof?
```

---
## \#15 Posted by: Jasonkimberson Posted at: 2019-02-21T06:14:50.410Z Reads: 170

```
I doubt it since they are not sealed
```

---
## \#16 Posted by: Lucifer100 Posted at: 2019-05-06T14:06:39.403Z Reads: 139

```
I don't know if anyone has noticed this but the 6380 has lower rated Max. Torque than the 6374.

A better "Torqueboards" motor produces less Torque..!?

![20190506_193558|500x500](upload://xf6QtikStE7cbYxgwLYSOdm4P8m.jpeg)
```

---
## \#17 Posted by: professor_shartsis Posted at: 2019-05-06T14:40:55.812Z Reads: 130

```
5nm implies ~100a motor current while 8nm implies ~160a motor current...
```

---
## \#18 Posted by: Andy87 Posted at: 2019-05-06T14:46:59.322Z Reads: 127

```
🤔 how that get along with the rated max motor amps in the specs 🤔
```

---
## \#19 Posted by: professor_shartsis Posted at: 2019-05-06T14:48:35.469Z Reads: 127

```
if it is actually based on anything it could be the amount of current that magnetically saturates the stator... the point at which torque no longer increases linearly with motor current... the max amps could be the amount of current that won’t overheat the motor... or it could be marketing.
```

---
## \#20 Posted by: Lucifer100 Posted at: 2019-05-06T15:51:06.548Z Reads: 121

```
@professor_shartsis Thank you for your explanation but for complete satisfaction I would like to have a look at a side-by-side comparison of these two if there's any..
```

---
## \#21 Posted by: professor_shartsis Posted at: 2019-05-06T15:52:37.226Z Reads: 116

```
@Lucifer100 you can get the torque in newton meters per motor amp (assuming the motor hasn't reached saturation current--this depends on stator size/geometry/material) from:

60 / (2 * pi * KV) = newton meters motor torque per motor amp = KT

^then multiply this times the actual motor current to get the total torque in newton meters.

60 / (2 * pi * **170kv**) = 0.05617233285nm/a

**5nm** / 0.05617233285nm/a = **89.01a** <--

60 / (2 * pi * **190kv**) = 0.05025945571nm/a

**8nm** /  0.05025945571nm/a = **159.17a** <--
```

---
## \#22 Posted by: professor_shartsis Posted at: 2019-05-06T16:12:05.653Z Reads: 114

```
@Lucifer100 so actually the 170kv motor that claims 5nm implies 89.01a and lists max 80a, which is reasonably close.

the other motor specs doesn't say the KV but if it is 190kv then it implies 159.17a while claiming max 85a
```

---
## \#23 Posted by: RedBaron Posted at: 2019-05-06T17:17:33.689Z Reads: 103

```
I'll buy those motors if you don't find a use for them.
```

---
## \#24 Posted by: Lucifer100 Posted at: 2019-05-06T20:00:24.754Z Reads: 100

```
@professor_shartsis So theoretically, 6374 is better with lower Power rating if the specs are true ?
```

---
## \#25 Posted by: professor_shartsis Posted at: 2019-05-06T20:26:53.401Z Reads: 96

```
“better” would depend on the KM or size constant which in turn depends on both the KV and resistance, and it would also depend on the saturation current which depends on the motor materials, geometry, size and and construction. other factor such as durability could come into play as well.

motors of the same construction with the same copper content but a different number of turns and different wire cross section have different KV and KT but the same KM

motors of the same KM are quite similar but the higher KV’s at the same KM gives higher theoretical performance and requires higher gear reduction ratios to obtain that theoretical performance increase.
```

---
## \#27 Posted by: kuphjr Posted at: 2019-05-06T20:44:55.050Z Reads: 84

```
I didn’t mean to delete this. What I said in the post was that I thought the same thing as you did until I took an advanced motors class at my university. The truth is you get significantly more torque with a larger stator.
```

---
## \#28 Posted by: kuphjr Posted at: 2019-05-06T20:47:08.226Z Reads: 82

```
Things would change under constant operation, but since electric skateboards are pretty much exclusively burst power machines, torque is really what matters, not its power rating.
```

---
## \#29 Posted by: professor_shartsis Posted at: 2019-05-06T22:10:03.384Z Reads: 74

```
[quote="kuphjr, post:27, topic:71374"]
The truth is you get significantly more torque with a larger stator.
[/quote]

In theory, yes, when the current is limited by the battery current limit at mid to high speeds, a lower resistance same kv motor will receive more motor current for the same battery current (because of the lower resistance), resulting in more torque during mid to high speed range acceleration with the “bigger” same kv motor. however, at very low speeds when the current is limited by the motor current limit, both motors will receive the same motor current, and thus generate the same torque unless the smaller motor has exceeded its saturation limit.
```

---
## \#30 Posted by: kuphjr Posted at: 2019-05-06T22:44:20.083Z Reads: 72

```
Much more well stated than I could have myself, thank you. In the end you just have to decide if you really care about having the torque at speed or if it only matters to accelerate from a slow/stop quickly.
```

---
## \#31 Posted by: kuphjr Posted at: 2019-05-06T22:46:07.328Z Reads: 75

```
I ride fast and push my boards really hard, so IMO the bigger the better. I wanna go 40MPH & get there in a hurry.

 Realistically though I find the speed controller to be the limiting factor as I almost always get it warm enough that I can feel it limiting itself a few miles into my ride. Next I will be using a CNC machine to cut a hole in the bottom of my enclosure and cut an aluminum heat sync plate that were perfectly fit in that hole so that I can easily waterproof around it.
```

---
## \#32 Posted by: kuphjr Posted at: 2019-05-06T22:51:43.179Z Reads: 71

```
Is there any data or charts comparing actual dyno tests of a 6355 vs 6374? I thought I remembered seeing a graph like that on this forum before but I cannot remember. A graph would really demonstrate very clearly the differences between the two for those who might not understand how about a BLDC operates.

Also, I highly doubt that the load of an electric skateboard causes a 6355 to reach its saturation point, but I wonder if an eMTB might while doing super steep climbs. Data on this would be nice too.
```

---
## \#33 Posted by: professor_shartsis Posted at: 2019-05-07T16:25:55.187Z Reads: 57

```
[quote="kuphjr, post:32, topic:71374"]
Is there any data or charts comparing actual dyno tests of a 6355 vs 6374? I thought I remembered seeing a graph like that on this forum before but I cannot remember. A graph would really demonstrate very clearly the differences between the two for those who might not understand how about a BLDC operates.
[/quote]


sure, here's a theoretical comparison of 2 different 190kv motors-- one is .01ohm, the other is 0.05ohm (46v battery, 2 motors, 0.01ohm vs 0.05ohm, 190kv, 80mm tire, 2.875:1 gear, 80a motor current limit and 30a battery current limit per motor):

https://i.ibb.co/6yc24Ln/10mohm-vs-50mohm.gif

^the lower resistance motor has significantly lower ohmic heating (bottom middle chart) while delivering better performance-- more thrust for the same battery current limit at mid to high speeds (yellow line, bottom left chart) and greater efficiency (green line, top left chart). at low speeds both motors generate the same peak torque (yellow line, top right chart) because the motor current on both is limited by the same motor current limit at this speed range. at higher speeds, the current is limited by the battery current limit, and the lower resistance motor sees more motor current for the same battery current, and thus develops more thrust and acceleration.
```

---
## \#34 Posted by: kuphjr Posted at: 2019-05-07T17:30:34.922Z Reads: 56

```
Thanks for posting this! I’m gonna save it for next time I see questions about motor size on the forum.
```

---
