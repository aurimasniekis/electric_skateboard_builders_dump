# APS 80100 on trampa mountain board

### Replies: 32 Views: 532

## \#1 Posted by: Doneone Posted at: 2019-09-15T14:52:22.984Z Reads: 149

```
Hi. I am looking to somehow mount 2 aps 80100 to my trampa mountain board. What choices do I have regarding drive? I was looking at etoxx, but it can only take 8085. Then fatboy heavy duty drive needs adjustment of the motor shaft. Aps offer to adjust the shaft. But here I read that they are doing a shitty job with that. Any advice?
```

---
## \#2 Posted by: Skunk Posted at: 2019-09-15T16:11:16.801Z Reads: 142

```
I hear the trucks are super wide on the new Lacroix. @Sender @mmaner @DerelictRobot @BallsAndWeiners might know more
```

---
## \#3 Posted by: Skunk Posted at: 2019-09-15T16:11:52.410Z Reads: 139

```
Or @Arch lol
```

---
## \#4 Posted by: 3DServisas Posted at: 2019-09-15T16:17:05.005Z Reads: 139

```
You send me the motor axles and I will make them 10 mm diameter and keyway .
```

---
## \#5 Posted by: Doneone Posted at: 2019-09-15T16:27:56.314Z Reads: 135

```
Ok. What else do need? Adjusted trucks/hangers?
```

---
## \#6 Posted by: 3DServisas Posted at: 2019-09-15T16:43:33.061Z Reads: 130

```
I wrote to you in pm.
```

---
## \#7 Posted by: DavidC Posted at: 2019-09-15T17:51:37.552Z Reads: 127

```
[quote="Doneone, post:1, topic:101814"]
I was looking at etoxx, but it can only take 8085.
[/quote]


E-TOXX chain drive fits APS 80100 motors : 

![IMG_7219_HL|666x500](upload://beFh2kO2Gi9dIawbJsHVfw8bWST.jpeg)  

![IMG_7212|375x500](upload://jf8yZlrRos6PQ9efZ1CLsVFO4zF.jpeg)
```

---
## \#8 Posted by: Doneone Posted at: 2019-09-15T17:54:26.578Z Reads: 124

```
Wow massive motors! Don't know if I want chains though
```

---
## \#9 Posted by: Doneone Posted at: 2019-09-15T17:56:06.494Z Reads: 120

```
Where are you riding? Is it hot where you ride? I have heat issues with the Trampa 6374 160kv.
```

---
## \#10 Posted by: JensSjogren Posted at: 2019-09-15T20:10:34.716Z Reads: 110

```
![20190829_204646|374x500](upload://1zbK6zmDhBVTFJMgfWVAbk7PeHZ.jpeg) 


You can get the etoxx truck extensions in order to move the motor mounts further out from the centre to fit the APS 80100 with the etoxx 80mm gear drives, this is what i did and it works great. 

I also got the chain drives but i can't fit the motors there without modifications. The space between the motor mounts on the chain drive is 235mm and the motors build 120mm each with the 80mm adapter (the APS 80100 is in reality 107mm long). 

![20190826_194240|666x500](upload://mE8ttJ9IUTerw6Xs8PoQKO1bYeU.jpeg)
```

---
## \#11 Posted by: JensSjogren Posted at: 2019-09-15T20:19:51.145Z Reads: 104

```
In my experience both the 8085 and 80100 motors gets warmer than 63xx, even during relaxed riding, i guess they are not very effeciant. Also this setup for me gives an avarage consumption of 25wh/km (30wh+/km when pushing it) compared to 18 wh/km with my 6384 motors on the same board. 

Having my VESC's on the topbox means i have longer phase cables and that may have an impact on the losses i get with theese motors.
```

---
## \#12 Posted by: Doneone Posted at: 2019-09-15T20:59:48.492Z Reads: 104

```
Shit, I need to tackle the heat issue somehow. It's really frustrating.
```

---
## \#13 Posted by: DavidC Posted at: 2019-09-15T21:06:33.867Z Reads: 106

```
[quote="Doneone, post:9, topic:101814, full:true"]
Where are you riding? Is it hot where you ride? I have heat issues with the Trampa 6374 160kv.
[/quote]


I'm in the south of France. It's hot here at the time. No heat problem when riding in the evening (not in te afternoon). It gets less hot than Turnigy ESK8 6374 192KV. Gear ratio 1/3. Massive torque on dirt. Just turn without quitting drifting. A lot of fun.

@JensSjogren : APS 80100 fit E-TOXX chain drive. Look at my photos. Just cut axle, center side, cause yours may be a bit too long (dremel will be your friend). You have to unmount one the vertical panel, then put the motor on the panel, then put the panel with motor on the hanger, next to other motor already mounted).

![Untitled|217x79](upload://hYzleYGjWIWrPypWVpf7q9cu6KF.jpeg) Ok it's a bit tight :smile:
```

---
## \#14 Posted by: Doneone Posted at: 2019-09-15T21:16:43.367Z Reads: 95

```
The aps 80100 get less hot than the turnigy? 6374?
```

---
## \#15 Posted by: DavidC Posted at: 2019-09-15T21:17:42.879Z Reads: 93

```
That's what I've seen with mine.
```

---
## \#16 Posted by: Ben.Nexus Posted at: 2019-09-15T21:18:10.987Z Reads: 91

```
If you want cool motors, go really low kv and gear for speed, like trampa 118kv won't really ever get hot. Obviously it limits the speed but if you're offroading you probably won't blast at 30mph.
```

---
## \#17 Posted by: Doneone Posted at: 2019-09-15T21:19:17.088Z Reads: 89

```
I want torque and speed 😂
```

---
## \#18 Posted by: Doneone Posted at: 2019-09-15T21:19:58.620Z Reads: 90

```
And cool motors 🤗
```

---
## \#19 Posted by: DavidC Posted at: 2019-09-15T22:23:35.720Z Reads: 84

```
IMO if you prefer torque and speed (= fun) to cold no matter a bit more heat then go for 6374 190KV at the condition you use Lipo (less amps with Li-ions). If you want low KV without spitting at the face of fun then go for 80 mm motors (except APS 8072 that have bad reputation).
```

---
## \#20 Posted by: JensSjogren Posted at: 2019-09-16T04:07:48.872Z Reads: 78

```
Honestly i don't see a big point in using 80mm motors, i just had to try it out in order to convince myself but the reality is that most of our systems are to weak to utilize the potential of the 80100 motors. Even my board that's rocking dual Vesc 6's and a 12s9p 30Q pack 

The difference in speed and torque compared to my 6384 130KV motors is just a slight upgrade

80100, 180kv, gearing 1:5, 8" tyres = top speed of 55 kph and slightly better torque than 6384 

6384, 130kv, gearing 1:4, 8" tyres = top speed of 50 kph 

The cost for this small upgrade will be a heavier board and a whopping 50% (ish) increase in energy consumption. I used to get 60 km+ and now i'm at 40 km per charge, still good range so doesnt bother me that much but if you use a smaller battery you'll definitly notoce it. 

This next statement concerns all the APS motors. Battle harden them and do it good before you use them, otherwise you're gonna have a bad time
```

---
## \#21 Posted by: Doneone Posted at: 2019-09-16T05:37:48.031Z Reads: 67

```
Great info!
What do you mean by "battle harden the aps motors"?
```

---
## \#22 Posted by: JensSjogren Posted at: 2019-09-16T06:09:22.308Z Reads: 69

```
Basicly you need to open the motors up and fill  the gaps between the magnets in the rotor and between the windings on the stator with epoxy since the build quality of APS motors is kinda shitty. Just search for battle harden motors either here on the forum or on youtube
```

---
## \#23 Posted by: Doneone Posted at: 2019-09-16T06:16:59.072Z Reads: 68

```
Are there better 80mm motors than aps?
```

---
## \#24 Posted by: Fosterqc Posted at: 2019-09-16T06:17:53.321Z Reads: 69

```
Torqueboards 6384 ~~yah~~ 

Im dumb

they are technically 80mm in some regard lol and better.

this would be insane:
https://flipsky.net/products/brushless-dc-motor-80100-130kv-7000w-for-electric-bike-electric-skateboard-go-cart
```

---
## \#25 Posted by: JensSjogren Posted at: 2019-09-16T08:07:54.678Z Reads: 66

```
Well you got the maytech 8085 motors but they are like 350€ a piece or something. The APS motors works well once they are battle hardened properly but be ready to put a couple of hours into each motor before they are ready for duty
```

---
## \#26 Posted by: JensSjogren Posted at: 2019-09-16T08:08:46.975Z Reads: 67

```
Those flipskys looks identical to the APS, probabky from the same factory
```

---
## \#27 Posted by: Doneone Posted at: 2019-09-16T08:11:51.359Z Reads: 70

```
Where would I source the maytech motors in Europe?
```

---
## \#28 Posted by: JensSjogren Posted at: 2019-09-16T08:44:16.798Z Reads: 68

```
I think electricboardsolutions got them. 

Considered the 6880 motors? 

https://www.bioboards.se/produkt/bioboards-6880-motor-3600w-180kv/
```

---
## \#29 Posted by: Ben.Nexus Posted at: 2019-09-16T12:07:53.694Z Reads: 61

```
That isnt even their biggest boye, https://flipsky.net/collections/efoil-products/products/water-cooling-motor-9097-150kv-for-efoil-electric-bike-electric-skateboard 9097 lmao, its even water cooled. Up to 22S, 360 Amps. That is technically a peak of 33200W
```

---
## \#30 Posted by: Doneone Posted at: 2019-09-16T14:55:24.505Z Reads: 55

```
Well. Theoretically yes. But it starts with 14s. I don't think you will get the expected outcome with 12s
```

---
## \#31 Posted by: skslingo21 Posted at: 2019-09-16T17:25:51.664Z Reads: 52

```
I am 165lb, using  dual 6384S APS's direct drive 1:4 ratio on a TRAMPA deck.
 It tops at 33mph and has enough torque to flip my larger friends on their backs. I would only reccomend larger motors for those over 240lbs or so...
set at 55amps, the board has enough to climb hills from a stop with my weight on it. 
The 6384 is far more powerful (and power hungry) than my old TRAMPA 6364. 

I have no problem with the build quality of APS, however they are not built for the rigors of (offroad) eboarding. You must re-epoxy the can for a truly board ready motor, magnets will break away and the rings holding the magnets separate from one another will displace themselves...
edit: I also cut the wires out since they will break with vibration, I replaced them with super high strand flexible silicone stuff. I got sick of breaking a wire every six months or so..
Thermal sensors in my battery/motors/vesc6' will cut power in the event of overheating...
another note doneone,  you will need a MASSIVE power plant to keep up with those size motors. Just an FYI, dont try and save weight there ;)
```

---
## \#32 Posted by: Doneone Posted at: 2019-09-16T17:56:24.891Z Reads: 48

```
I need to try a big motor. I am just too curious and need a new system anyways. So why not upgrade. Powerplant I have ;)
```

---
