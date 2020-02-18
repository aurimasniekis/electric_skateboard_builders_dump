# My first build final questions/suggestions

### Replies: 27 Views: 2284

## \#1 Posted by: Theshiatispimpin Posted at: 2017-02-09T03:44:47.702Z Reads: 145

```
Had some questions, I have the Majority of info I need, but as far as any connectors or other things I might need I'm not to sure.

Getting a Single motor mount kit (enertion or diy)

2x https://hobbyking.com/en_us/turnigy-5000mah-6s-40c-lipo-pack.html 

this motor https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-192kv-brushless-outrunner-motor.html

to run in series for 12 s https://hobbyking.com/en_us/xt90-battery-harness-10awg-for-2-packs-in-series.html 

Standard vesc idk from where yet, seems like most places are sold out?

Would this work? https://www.amazon.com/GERI-Battery-Capacity-Indicator-Lead-acid/dp/B011R35GLG/ref=sr_1_2?s=hi&ie=UTF8&qid=1469500867&sr=1-2&keywords=lipo+battery+capacity


My MAIN questions are:

Do I need different connectors to run my batteries in series? since it is not the 4.5 bullet connect (or 4) it is 5.5?

Do I need any other connectors?

Should i go with an anti spark loop key (and how?) or a power button?? 

I will find a 2.4 remote and receiver no worries, and a batter charger no worries (theres alot of info on these forums)

thanks for any help!
```

---
## \#2 Posted by: zmoney Posted at: 2017-02-09T04:11:55.237Z Reads: 133

```
[quote="Theshiatispimpin, post:1, topic:17424"]
Should i go with an anti spark loop key (and how?) or a power button??
[/quote]

They are in essence the same thing. If you want something fancier, then a electronic switch like Vedders Anti-Spark switch should do the trick. If you want something that works on the cheap, then a spark loop is for you. :slight_smile:
```

---
## \#3 Posted by: Hummie Posted at: 2017-02-09T04:18:25.546Z Reads: 122

```
or just an xt90s plug.  easiest for me by far.  you can buy it
```

---
## \#4 Posted by: Theshiatispimpin Posted at: 2017-02-09T04:32:50.482Z Reads: 119

```
Isnt an anti spark needed or highly recommended?
```

---
## \#5 Posted by: Theshiatispimpin Posted at: 2017-02-09T04:33:36.041Z Reads: 117

```
thanks for the reply! yea but do they sell them as a whole? or do i just need to get the xt90 connector and solder a copper piece loop on it?
```

---
## \#6 Posted by: Hummie Posted at: 2017-02-09T04:45:45.516Z Reads: 109

```
an xt90s has an antispark in it.  easier.
```

---
## \#7 Posted by: Namasaki Posted at: 2017-02-09T05:55:25.582Z Reads: 105

```
192kv is too high for 12s voltage on a Vesc. It will exceed the Erpm limit of the Vesc and burn out the DRV chip.
What you'll need is 170kv or below for 12s.
This would work:
https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-168kv-brushless-outrunner-motor.html
```

---
## \#8 Posted by: Namasaki Posted at: 2017-02-09T06:04:15.041Z Reads: 101

```
[quote="Theshiatispimpin, post:1, topic:17424"]
Getting a Single motor mount kit (enertion or diy
[/quote]

I have both and their both excellent quality.
```

---
## \#9 Posted by: eitan Posted at: 2017-02-09T17:17:13.959Z Reads: 93

```
@Theshiatispimpin The capacity indicator you selected won't work for the batteries you selected.

Because you are running 2*6S, your voltage will be 2*22.2V = 44.4V. 
Meanwhile the capacity indicator only works up to 30V.
```

---
## \#10 Posted by: Hummie Posted at: 2017-02-09T18:17:55.363Z Reads: 84

```
or you could limit the erpm and do 12s still.
```

---
## \#11 Posted by: Theshiatispimpin Posted at: 2017-02-09T19:18:23.257Z Reads: 81

```
thanks man
```

---
## \#12 Posted by: Theshiatispimpin Posted at: 2017-02-09T19:19:47.715Z Reads: 78

```
Hmm how do so many people use 12s 190? maybve ill just go with a 10s and a 200+ motor setup.. Can you explain the loop key to me? thanks!
```

---
## \#13 Posted by: Namasaki Posted at: 2017-02-09T22:09:05.116Z Reads: 74

```
I highly recommend 10s for a street board because it will provide plenty of power and will be less stressful on electronics therefore more dependable. 
The loop key uses a set of anti- spark XT90 connectors and is an inexpensive alternative to having a high voltage high current electronic on/off switch. It also serves as a key to keep your little brother or kids or grand kids from taking your board out without permission.
```

---
## \#14 Posted by: mmaner Posted at: 2017-02-09T22:32:55.859Z Reads: 107

```
[quote="Namasaki, post:13, topic:17424"]
It also serves as a key to keep your little brother or kids or grand kids from taking your board out without permission.
[/quote]

Or your wife, my steals my board all the damned time.  I don't think shes ever gone more than 5mph, but she sure does like to toodle around :).
```

---
## \#15 Posted by: rich Posted at: 2017-02-09T23:33:09.458Z Reads: 109

```
Hi @Theshiatispimpin, just wanna share some info about my first build which could help you for some decisions and saving money because in the end i had to change almost everything!
 
Main parts:
APS 6355 190kV Brushless outrunner motor sensorless 2400W
APS Motor mount
HTD5M 9mm Belt 265mm, Gearing 15T/32T
Vesc 4.12
Turnigy Graphene Lipos 10Ah. I used one 4s and a 6s in series to reach 10s. discharge 150A, charge 50A
Paris 180mm trucks
Orangatang Kegel wheels 80mm
HK GT2E remote

Battery range about 42 kilometers
Top speed about 45 kmh

First of all i never had problems with the vesc in bldc mode, it's a great thing.
The motor is really powerful and nice. But the problem with sensorless motors is not to be able to start from zero. It stutters like hell no matter which vesc settings. After a little push everything is fine and working great. Now i have sensored motors and the vesc knows exactly the rpm of the motors so no problem anymore. I would say 190kV is the max. with 15T/32T or 36T gearing, maybe better 170kV unless you won't ride over 40kmh, and you have more torque.

9mm HTD5M Belt sucks!!!!!! In daily use they burst every 14days or less (max. 120km and i'm 74kg) and can't transfer the power to the wheels. Maybe also the pulleys had too sharp edges. That's why i switched to 15mm belts and pulleys, a must! My new wheel pulley is 36T instead of 32T to get a bit more torque for hills.

The motor mount wasn't working well although i filed off the truck. I love paris trucks that's why i wanted to use them.but they are round, the only way is to epoxy glue or weld it. With none round trucks that's not a problem but motor mounts often have a fixed position so you can't change the angle, that's an disadvantage.
The motor mount material should be a bit wider on the place where the motor is mounted or should contain some protection, otherwise it looks like this after 3 months riding (on the right side a new one):

<img src="/uploads/db1493/original/3X/3/9/39d737c25febdf06d5b676a2eb338dcf2f8872cd.jpg" width="690" height="388">

According the power switch / loopkey etc. I stopped thinking about a loop key because i read many bad stories and fails about it and wasn't motivated to try that. First i used an anti-spark XT90 connection with soldered fuse on + (top of the picture). It worked well but after a few weeks i had enough from plugging and unplugging and i was ready to spent extra money for a vedder anti-spark switch with fuse (bottom of the pic). This thing is great and in my opinion the only option if you use your board daily, i love it. After switching on it takes some seconds to get the full voltage.

<img src="/uploads/db1493/original/3X/e/0/e0dbb10b43abac978137f0739f311f3658e4c050.jpg" width="690" height="388">

On the right side is a battery capacity indicator (in percentage). Switchable between 6s, 8s,10s, 12s. The only thing, it's made for Li-ion. The lipo is empty at about 40% on the display but i can live with that. It was about 15 euros, my second indicator i ordered in china for 5 euros :grin:

About the GT2E remote from hobbyking. It's great in the beginning but after a while it seems too big. Everytime when i entered eg a shop i had to put the remote in my backpack. Also after 6 weeks the receiver was broke.
It's nice to have a remote that fits in your trouser pocket but such remotes are quite expensive but i had to order a steez remote, here the comparison between steez, GT2E and GT2 in the back:

<img src="/uploads/db1493/original/3X/7/6/766d706ee95e57aa506384ee55936a79a3ceeb74.jpg" width="690" height="388">

I didn't test it so far but it's nice when it's invisible in your hands and not like a gun.

About the battery: I bought this big block (4s+6s= 10s 10Ah) because i wanted to use it on a e-mountainboard as well (save money) and switch it to the drop-through longboard deck with battery top mounted above the back truck. Stupid idea :joy: it didn't work well and i got speed wobbles at higher speed, too. Beside that it was ugly. Then i mounted the electronics underneath the deck but my ground clearance was ridiculous less. Now i'm switching to 18650 Li-ion cells.

BATTERIES IN SERIES
The worst on my build was the charging process. You have to charge the batteries one by one with a balance charger. My hobbyking 6A charger had max 2A on 6s and 3A on 4s. One full cycle charging for both batteries was over 10 hours!
And when you fall asleep while the first lipo is charging then you can't ride it in the morning because the second one is empty! Also just a short charge is impossible when you are not able to charge all cells at the same time! That's the most disadvantage in my eyes. Also this fiddly balance wires are not funny. And if you try to charge both batteries at the same time with 2 chargers when they wired in series then you short-out the battery and in worst case - Kaboom!!!

For my e-mountainboard build i found a cheap and wonderful solution for this problem with 2 batteries in series and charging all together: a BMS with charger, so sweet
Here you see the batteries in series (with yellow tape marked is the connection between both). Minus wire is Battery 1 and plus wire Batterie 2. That's important for wiring to the bms. If you need further instructions how to wire it, let me know.

<img src="/uploads/db1493/original/3X/5/1/519c6a5a12a6fa4f99f58df8049794f7948130d2.jpg" width="690" height="388">

The small blue thing on top is a cheap BMS 40A which i use for charging only, it's about 10 Euros. For Lipo alright, for Li-ion you would need a bigger BMS with discharge through it, too. For the lipos i just bypassed it. I put balance wire extensions there to be able to charge them via balance charger, too if necessary. The 10s balance wire for the BMS is soldered together with two balance connectors (in my case 4s and 6s)

<img src="/uploads/db1493/original/3X/e/5/e565aad40ea10f349002b3fb94fdc1e3b0c9f313.jpg" width="690" height="388">

Finally the charger with charging connector for the enclosure.


<img src="/uploads/db1493/original/3X/8/b/8b0a6fac6d05315c215ca82c9a3ff3bfb92ac5d3.jpg" width="690" height="388">

TOTAL COST OF BMS AND 3A CHARGER from china: 28 Euros :joy: That's the same amount as a cheap balance charger and i prefer this method.

I would have saved money if i bought the proper stuff. It's always the same, you want to save money but in the end it is more expensive because you have to buy things twice or even more.
Hope i could help you with some thoughts or maybe you are totally confused now :fearful:
```

---
## \#16 Posted by: Namasaki Posted at: 2017-02-10T02:09:28.071Z Reads: 95

```
[quote="rich, post:15, topic:17424"]
9mm HTD5M Belt sucks!!!!!! In daily use they burst every 14days or less (max. 120km and i'm 74kg) and can't transfer the power to the wheels. Maybe also the pulleys had too sharp edges.
[/quote]

Hey Rich, sorry to have to disagree with you but I've been running dual 9mm belts for about a year now and have not yet broke a single belt. Not even after getting rocks stuck in them. Not sure why they're only lasting 14 days for you unless as you mentioned, something was wrong with your pulleys. Or maybe you where running them too tight. 
I run mine rather loose so that they skip if I hit the brakes hard. But I have no problem with them while accelerating and charging up hills.
```

---
## \#17 Posted by: Namasaki Posted at: 2017-02-10T02:11:12.853Z Reads: 89

```
[quote="mmaner, post:14, topic:17424"]
Or your wife, my steals my board all the damned time.  I don't think shes ever gone more than 5mph, but she sure does like to toodle around :).
[/quote]

Sounds like it's time to build your wife a board of her own!
:slight_smile:
```

---
## \#18 Posted by: mmaner Posted at: 2017-02-10T02:16:49.839Z Reads: 85

```
I did, she likes my dual motor arbor more than her single. Even though she can go just as fast as she is willing to go in hers 😀
```

---
## \#19 Posted by: rich Posted at: 2017-02-10T02:28:48.970Z Reads: 89

```
interesting to hear, so maybe the sharp APS aluminium pulleys were the bigger problem. The belt broke no matter if tight or loose , tried all settings. But it was a single drive not dual. When the belt was loose and skipped, with every skip the belt gots weaker and weaker up to the point where i couldn't ride up a hill because of skipping only. It must be the pulleys
```

---
## \#20 Posted by: Mikenopolis Posted at: 2017-02-10T20:23:15.584Z Reads: 82

```
lol, same here, I have multiple boards, the DIY is my favorite....so is hers.
```

---
## \#21 Posted by: rich Posted at: 2017-02-10T20:37:44.039Z Reads: 78

```
[quote="Namasaki, post:16, topic:17424"]
something was wrong with your pulleys.
[/quote]

Jesus Christ! I've never seen my old pulley so close, it's even worse than "only" sharp edges. Additional to that sharpness the edges are not straight at all! On the left side a new pulley like it should be! Both are from alien power systems, the awful one i bought last summer and the price wasn't cheap. If only I had known before. So big up 9mm belts and a shout out to proper pulleys!

<img src="/uploads/db1493/original/3X/8/9/897cfae19943343965d6b7c519dc33c2f40f73dd.jpg" width="690" height="388">
```

---
## \#22 Posted by: Namasaki Posted at: 2017-02-10T21:04:30.495Z Reads: 67

```
Wow! That thing looks terrible. 
No wonder it was eating belts.
```

---
## \#23 Posted by: rich Posted at: 2017-02-10T21:12:15.484Z Reads: 70

```
@Namasaki this picture is for you because I think you don't know how broken belts look like :joy: 
Zoom in and laugh, also watch the profile! Unbelievable!

<img src="/uploads/db1493/original/3X/a/5/a58ddcfa209c18747ed3892ed0c0839cb9b49dfa.jpg" width="690" height="388">

Also interesting to see, the belt in front is nice quality (it last 3 weeks) and was the only belt without squeaking, The brand is GATES and i ordered it from an local power train engineering company. STRONGBELT is also good brand.
The original belt last 1 week and squeaked! And the others I ordered at 2 different esk8 shops last 2 weeks each and looked like the belt in the picture in the back. You can see the difference in quality.
```

---
## \#24 Posted by: faithfulpuppy Posted at: 2017-02-10T21:17:43.319Z Reads: 69

```
wait, for real? i've already ordered my batteries and VESC and BMS, and i'm waiting on the motor to restock
```

---
## \#25 Posted by: Namasaki Posted at: 2017-02-10T23:15:50.761Z Reads: 69

```
[quote="faithfulpuppy, post:24, topic:17424, full:true"]
wait, for real? i've already ordered my batteries and VESC and BMS, and i'm waiting on the motor to restock
[/quote]
http://www.electric-skateboard.builders/t/choosing-the-right-motor-kv-for-the-vesc/3125
```

---
## \#26 Posted by: willpark16 Posted at: 2017-02-14T05:53:40.628Z Reads: 58

```
<img src="/uploads/db1493/original/3X/9/e/9edf4641e58d87958442674d8aeba4c917fa450e.jpg" width="374" height="500"> this bms?
```

---
## \#27 Posted by: rich Posted at: 2017-02-14T12:41:53.815Z Reads: 55

```
Yes, looks like mine. Mine has about 40A Peak. So charging only. Or you spend 40$ for a bms with discharging as well. I bought one with 60A  cont. and 120A peak. You need charge/discharge same port for regen. braking. I have it seperately so i need a new one.
```

---
