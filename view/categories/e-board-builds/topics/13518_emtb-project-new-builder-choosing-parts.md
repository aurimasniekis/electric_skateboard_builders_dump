# eMTB project (New builder choosing parts)

### Replies: 20 Views: 2108

## \#1 Posted by: MBuilder Posted at: 2016-11-23T05:08:16.418Z Reads: 170

```
Electric-MountainBoard Project.

I wanted to share with you guys the build I think I'm going to do so you can give me your opinion or recommend me a different setup for this project.

Parts I found so far:

Motors:
 - 2x Turnigy 192KV -6374 SK3 Brushless Outrunner Motors
https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-192kv-brushless-outrunner-motor.html
Battery:
 - 2x ZIPPY Compact 4000mAh 10S 25C Lipo Pack
https://hobbyking.com/en_us/zippy-compact-4000mah-10s-25c-lipo-pack.html
* I think about putting them into parallel so I would double the mAh (Autonomy)
ESC:
 - 2x ESC (Open Source by Benjamin Vedder)
http://miamielectricboards.com/shop-1/vesc
* Taking advantatge of this post, let me ask how do you guys do the sync on a dualESC build.
Remote:
 - GT2B 2.4GHZ Trnasmitter
https://hobbyking.com/en_us/hobbykingr-tmhk-gt2b-3ch-2-4ghz-transmitter-and-receiver-w-rechargable-li-ion-battery-1.html 
Gearing:
 <img src="/uploads/db1493/original/3X/f/5/f58e63dfb8c5fcd60c3e26b5b529f62a7a8b5ab2.jpg" width="319" height="455">

Please let me know what do you think of this setup and what would you recommend me in order to build a torque eBoard with a good range autonomy.


Thank's a lot!
```

---
## \#2 Posted by: lox897 Posted at: 2016-11-23T05:52:30.207Z Reads: 148

```
What mounts are you going to use? Check out @trampa and @nowind for the other emtb parts
```

---
## \#3 Posted by: Nowind Posted at: 2016-11-23T06:22:00.973Z Reads: 146

```
Hey. 

Motors are very good.
Lipos are ok, (do you got a 10S Charger?)
VESC in actually version tend to go up in smoke on E-MTB.
GT2B is very good, maybe think about a mod to bring size down.

Gear Ratio is nice but depending on which gearstuff you choose not easy to archieve. 
10 tooth HDT5 pulleys i dont know...or you go not with a belt ?
1:5 or 1:6 is normally enough reduction, you could reduce Motor kv from Turnigy to hold your VMAX ..
```

---
## \#4 Posted by: trampa Posted at: 2016-11-23T08:56:26.390Z Reads: 140

```
Hi, the VESC had no issues in our tests, if it is a good one and you don't use crazy settings.
We ride them in FOC mode, timing set to 500µs, to prevent shutdown on wheelslip.
45A max, 12S. Small Pulley should not be smaller than 13 teeth! 15mm belt width is fine if you use a tension roller.
Wheel diameter is ususlly 195mm. If you want to go for 10S then better choose 12S.

Frank
```

---
## \#5 Posted by: tueboard Posted at: 2016-11-23T09:01:26.685Z Reads: 134

```
any VESC suggestion for an EMTB? I've two VESCs from enertion
```

---
## \#6 Posted by: Rob.Endless Posted at: 2016-11-23T11:37:14.510Z Reads: 132

```
@tueboard I spent months (and still doing so) reading up on eMTB Trampa builds, watching every youtube video I can find, reading every single Trampa build here on this forum, bothering people on this forum with eMTB questions through private messages, and so forth. I even came across other forums in different languages and just looked at the pictures haha.

Like stated above, perhaps if you don't use crazy settings, Vescs might work out. However, just ask Nowind himself as well as other members here on this forum about VESC reliability on EMTB Trampa builds.  From the top of my head, I know these guys will advise you to not go the Vesc route @nowind @kaly @barajabali @squad .  Also, If I remember correctly, one of these guys said Vesc on these type of build did not quite pack as mean of a punch.
```

---
## \#7 Posted by: Nowind Posted at: 2016-11-23T11:37:40.608Z Reads: 127

```
Ich cant recomend any VESC for MTB'S.  Maybe with Franks setting they will hold up. But 45A as Max Motorcurrent is really low IMO. This is less then the half of power which a Roxxy will put out. I dont wanna make the Vesc bad, really not but for me and many of my customers they dont work good.
```

---
## \#8 Posted by: trampa Posted at: 2016-11-23T12:02:20.828Z Reads: 128

```
https://www.youtube.com/watch?v=1iwN5LGGM80
Mabe we got to wait until VESC 6 is out.

Frank
```

---
## \#9 Posted by: MBuilder Posted at: 2016-11-23T14:48:54.099Z Reads: 122

```
I am not sure if 10s2p is the correct lipo equipment or should i go for 10s4p or 12s4p.
For gearing i was thinking about 15 pulley teeth to the motor and 60 or 65 to the wheel,  the wheel size is 20cm though (chain).
```

---
## \#10 Posted by: MBuilder Posted at: 2016-11-23T14:51:21.858Z Reads: 121

```
What vesc's do you reommend me to use?? 

This is the board I 'll be using. 
<img src="/uploads/db1493/original/3X/f/8/f88e9538fb4fa5a68bdd694ba6f5ecaeb1415966.jpg" width="480" height="300">
```

---
## \#12 Posted by: Nowind Posted at: 2016-11-23T17:22:14.188Z Reads: 114

```
Lipo size is a question of how far you wanna go... More miles means also more wheight.
I´m using some 12S2P to get max power and some 10S4P for Touring if i wanna go on a longer run.

[quote="MBuilder, post:10, topic:13518"]
What vesc's do you reommend me to use??
[/quote]

Many people using @torqueboards 12S ESC, seems a good choice.
I´m using Robbe Roxxy 9120 OPTO, for me its the best controller i used, still not perfect for sure, but i love it.
But it can burn also (-; Go to 1:39 for SLOMO 
https://www.youtube.com/watch?v=JwDwEHQCk5g
```

---
## \#13 Posted by: MarioGC Posted at: 2016-11-23T18:46:04.937Z Reads: 107

```
I want to go for long runs, so that's why I chose 10S LiPo, why did one of your ESC actually caught fire?
```

---
## \#14 Posted by: trampa Posted at: 2016-11-23T21:59:01.744Z Reads: 110

```
Sorry, the Board is not what you want as a platform. It features bad trucks, a cheep copy of our tire (plastics instead of high grade rubber), the worst bindings you can imagine and crap hubs.

Get yourself a better board, a used one if you don't have the $. This board will waste your money since you will buy twice.

Frank
```

---
## \#15 Posted by: Monte Posted at: 2016-11-24T11:11:59.510Z Reads: 106

```
Do i need a UBEC/SBEC for the Roxxy esc like Torqueboards?
```

---
## \#16 Posted by: saul Posted at: 2016-11-24T11:27:12.521Z Reads: 105

```
use a real mtb not a toy board lol
also I would use esk8 motors not sk3s....they will break after 200+ miles :sob:
```

---
## \#17 Posted by: DeathCookies Posted at: 2016-11-24T12:18:09.213Z Reads: 104

```
[quote="saul, post:16, topic:13518"]
also I would use esk8 motors not sk3s....they will break after 200+ miles :sob:
[/quote]

A SK3 motor is somehow a esk8 motor. Many people here would recommend you a motor from SK3!
```

---
## \#18 Posted by: TarzanHBK Posted at: 2016-11-24T13:52:53.040Z Reads: 105

```
don´t know where you get this from. SKs are really nice motors. Perhaps you got a broken one and bad experience?
```

---
## \#19 Posted by: saul Posted at: 2016-11-24T15:06:55.652Z Reads: 102

```
I've got this from **experience**. I had a 149kv 6374 sk3 running for a few months. then I got some strange wobble when hit throttle or hard break.

2 of the _**3 tiny m3 screws that hold the front plate/bearings together broke.**_ I figured i must have hit something to cause this. luckily I had the very same motor sitting brand new in the box so it was a quick fix!

At this point I should have changed the m3's for some stainless versions but really they are all the same...
_**less than a month later the 2nd motor failed the same way!**_

I switched to an old diy 5065 and now a jlab 6355 with no problems because they use proper circ clips and larger bearings. + keyway would help with high torque setups. but 2x grubs with flat spots work well enough....


I will add that at this point I was riding everyday(commute/fun) for 10-25+ miles on LA Streets/sidewalks. so a month of riding for is easily 400+ miles torture test.

edit: thinking of those miles I should probably get some new wheels soon :money_mouth:
```

---
## \#20 Posted by: Nowind Posted at: 2016-11-24T16:18:28.071Z Reads: 96

```
Yes its OPTO, so you need an UBEC/SBEC
```

---
## \#21 Posted by: MBuilder Posted at: 2017-01-02T01:54:34.901Z Reads: 80

```
I bought a different board, different tracks and wheels, I'll post my build soon
```

---
