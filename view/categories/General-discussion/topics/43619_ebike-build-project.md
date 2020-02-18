# Ebike build project

### Replies: 37 Views: 2309

## \#1 Posted by: vagosofron Posted at: 2018-01-13T14:25:56.497Z Reads: 257

```
Hello from Greece. My name is Vaggelis and i've been reading this forum for a while and i can say that you guys are very helpfull.
I'm building an ebike ( like Tom Stantons project) and so far i have the bike ( single speed) and the motor ( keda 63-64 190kv).
I need an esc and i see most people here like the focbox from enertion. The problem is, that it is a little over my price range and while i was looking for a cheaper alternative ( if there is one), i saw one on hobbyking
[esc](https://hobbyking.com/en_us/turnigy-sk8-esc-for-electric-skateboard-conversion.html?___store=en_us) at 89$. Some of you might say that it's not a big price difference, but does it worth it? Because i also have to make my battery pack ( li-ion) and get a balance charger ( or ad a bms and use a regular charger) and i can't go cheap on those.
Any help would be appreciative, cheers.
```

---
## \#2 Posted by: FredrikHems Posted at: 2018-01-13T15:11:35.387Z Reads: 242

```
If you're building an e-bike, you will draw more current. That esc isnt know to be good quality, Because it is a 4.10 hw version. If you want something reaible Get a brand new focbox from @Titoxd10001 It cost $125 plus shipping, and is  definitely worth it
```

---
## \#3 Posted by: vagosofron Posted at: 2018-01-13T15:23:57.031Z Reads: 236

```
Is he from US? I can only get it from EU, because of custom taxes.
```

---
## \#4 Posted by: vishal_tejwani Posted at: 2018-01-13T16:21:12.927Z Reads: 218

```
He made it and may be can help
@wafflejock
```

---
## \#5 Posted by: vagosofron Posted at: 2018-01-13T17:31:45.750Z Reads: 210

```
He made an ebike you mean?
```

---
## \#6 Posted by: aigenic Posted at: 2018-01-13T17:51:34.139Z Reads: 198

```
Maybe try asking [here](https://endless-sphere.com/forums/), there are much more ebike builders who might help you with your project :) Also much more topics more related to your build ;)
```

---
## \#7 Posted by: vagosofron Posted at: 2018-01-13T20:48:44.726Z Reads: 186

```
I already did, but then I found this forum and it looks like you know your staff.
```

---
## \#8 Posted by: wafflejock Posted at: 2018-01-14T20:33:13.215Z Reads: 185

```
Endless loop really is the place for ebike stuff.  I've experimented with moving my esk8 parts including one of the older 4.10 hardware VESCs over to a bike (using Stanton's parts for the motor mount and wheel pulley), but so far mixed success.  I haven't run into issues with burning out the VESC yet (on a bike), but I have followed Tom's stuff for a while here and he did mention he blew at least a few VESCs and did eventually start using FOCBox (maybe it was vesc6 I forgot but pretty sure he got upgraded for free).

https://www.youtube.com/watch?v=PPyHvkypKjo

I printed and molded the parts for the wheel pulley but unfortunately the tooth spacing doesn't seem to be 100% correct.  Same issue is present on the original 3d print as on the molds but I didn't have a belt to check when I did the 3d print and assumed it would be good, so if you're doing the 1/4 pieces would verify your belt fits snugly before proceeding to make the whole thing.

Aside from tooth spacing I ran into a couple of other issues (possible exacerbated by the imperfect tooth spacing).  One of the other issues was if the pulley on the wheel isn't 100% concentric with the wheel itself then there is some play as it rotates the belt gets tighter and looser (obvious in hindsight but didn't really consider this as a major problem).  To get around that one I'm using an idler on a spring load to keep some tension on the belt but allow it to move to compensate for the lack of perfectly concentric wheel/pulley.  Last problem I ran into is needing to adjust the motor mount so that it would be able to be mounted on the particular bike I was putting it on (craigslist garbage mongoose bike for $45 to experiment with).  Actually the last bit about the bike brings up another point, make sure the bike has a big enough wheel diameter so the motor doesn't end up in the way of the wheel itself, I tried on a foldable cruiser someone gave me to try out but with smaller wheels the motor position ended up right next to the wheel (you want regular mountainbike or street bike size wheels, also street bike wheels are ideal, I think in terms of the bike a hard tail 1-by is ideal, see seth's bike hacks on youtube for some good beginner tips on picking bikes in general etc.)

https://www.youtube.com/watch?v=o98-0m8a9fg

^ there's a video testing my setup upside down, I was able to do a little bit of testing riding around before Chicago entirely froze over, but have been working on making my own skateboard wheel pulley design as an intermediary step to redoing the bike one (ideally so I can print it all in one go) but need to do the math etc. on gearing to see how that will work out.. basically how much torque will I be sacrificing if I make it small enough to print on a 200x200mm bed.

[Custom Pulleys](https://photos.app.goo.gl/HUOVVVXtyQYjQy9T2)

I'd say if you're just trying to get something working then going with a hub motor setup is a ton easier (avoid all the alignment issues and potential for belt slipping off in different directions and trying to avoid having spokes run into any of the motor mount parts, long story short alignment is more difficult than you think).
```

---
## \#9 Posted by: vagosofron Posted at: 2018-01-14T20:44:19.432Z Reads: 155

```
Thanks for the tips! I know where i'm getting into though. I know the problems and the difficulties and i think i will solve them ( with a lot of help). My base is an old single bike ( restored) and right now i'm trying to fit a freewheel on the left side and then bolt the pulley on the freewheel, so when i lay of the "gas", the wheel will keep spinning without draging the motor. But, until i solve that issue, i have to find a good esc.
```

---
## \#10 Posted by: wafflejock Posted at: 2018-01-14T20:51:30.181Z Reads: 158

```
Yeah so long as you limit things properly to avoid going over 60,000erpm (8571 motor RPM on a 14 pole or 7 pole pair motor which is typical) you should be fine.  So you take that 8571motor rpm/190kv = 45.1V.

A 10S battery is 42V fully charged a 12 S adds another 8.4V fully charged so 50.4V (10S would be safe 12S would be too much)

Above that 60,000erpm there is a high probability that the DRV chip on the older VESC will blow, it happens pretty consistently so best to avoid that if you go older hardware.  Also FOC mode is known to cause issues on the older hardware so I wouldn't risk it, just run BLDC, if you can get a sensored motor I've been told it helps a lot (makes sense the motor controller can actually tell the position of the motor without relying on back electromotive force to infer the position).

If you keep the stuff above in mind I don't think you're likely to blow the VESC even using the old one but newer ones have improvements to mitigate some of these problems (FOCBox gets past issues with FOC mode and VESC6 gets passed the erpm issues as well)
```

---
## \#11 Posted by: wafflejock Posted at: 2018-01-14T20:55:24.416Z Reads: 142

```
Also regarding costs on components I think you are better off buying balance chargers than getting a cheap BMS that just ends up causing you problems.  You can also use LiPos instead of 18650 based to bring your cost down a lot.  Getting a cheap 18650 cell is IMO more dangerous than getting a cheap LiPo pack, you need cells that can deal with the amperage being pulled through them without overheating and damaging themselves.  If you need to go cheap just go LiPo and balance charger, if you have an extra few to five hundred to put into the project then 18650 and BMS.
```

---
## \#12 Posted by: vagosofron Posted at: 2018-01-14T20:59:35.548Z Reads: 134

```
I haven't thought about batteries yet, but i understand what you mean. I already have the motor ( keda 63-64 190kv). If i go lipo, i'll have to use two 5s in series, but i'll have to charge them in parallel with a balance charger, is that correct? The good thing is, that i have a couple of people here to help me with the electric parts ( batteries, connections etc.).
```

---
## \#13 Posted by: wafflejock Posted at: 2018-01-14T21:05:26.989Z Reads: 140

```
Yup you would hook them in series for getting 10S and you could charge them in parallel.  I find that I'm actually limited by the charger I have so I wouldn't benefit from parallel charging so I just do them back to back.  Since I have an 80W charger if you do 80W/ (5S*4.2V) = 3.8A in reality I can only charge at 3.6A (charger gets toasty) which is still under 1C charge rate for 5Ah 5S batteries.  So if I were to parallel charge them it wouldn't go any faster I just wouldn't have to swap batteries between charging, but I don't really mind, I designed my battery tray so I can slide them out to make that not such a PITA (at first just had balance leads hanging out of the box, also works but not as safe/convenient).

[swappable batteries](https://photos.app.goo.gl/KzDYcYYeHPuD4u5e2)


Battery box link below if you'd like to tweak these, onshape is free for public models and cross platform so I use it:
https://cad.onshape.com/documents/15cd342c90ae1b0b6fd666bf/w/40780c7d8d67fd69a32fbf6e/e/aa247b01c3dd60bc5ba24701

VESC and receiver and metr/bluetooth/telemetry module box below
https://cad.onshape.com/documents/d8179a83484264c79e6adb1a/w/af2067b944ad3aa57f532370/e/35b4562d3dcad3a56c9b531f

---

Also to note charging at less than 1C is better really, slower is generally better on the battery health but in terms of waiting for it to fill the 5000mAh it's not ideal unless you are testing your patience :)

https://www.youtube.com/watch?v=mRlsaD5tf_8
```

---
## \#14 Posted by: vagosofron Posted at: 2018-01-14T21:09:45.428Z Reads: 126

```
Ok, so my thoughts are correct ( i'm a noob). I don't mind charging batteries back to back. This is for an ebike and my route is only 4.5klm, slightly uphill, so on the way back the mototr will be off. Thank you!
```

---
## \#15 Posted by: wafflejock Posted at: 2018-01-14T21:12:19.487Z Reads: 125

```
No problem use the magnifying lense/search in the top of the page to find stuff on different battery setup options when you get to it, there are tons of threads covering different options/setups.

---

Also on esk8 roughly 10Wh = 1km so 4.5km should be no problem with a relatively small battery.
```

---
## \#16 Posted by: vagosofron Posted at: 2018-01-14T21:14:06.128Z Reads: 112

```
Thanks @wafflejock, right now my concern is the esc. I want one to use plag and play if it is possible. I don't mind configuration, but since i'm noob to this, i don't want to brick it.
```

---
## \#17 Posted by: wafflejock Posted at: 2018-01-14T21:22:29.697Z Reads: 115

```
Gotcha yeah was just getting into batteries since that is one way to brick it :) too much voltage combined with too high kv motor ends up with too high erpm which blows the chip that deals with getting the motor to turn at that speed.

Reason people all go with the VESC is it's pretty reliable for "high voltage" applications whereas there are not a lot of other RC consumer ESCs that can handle the voltage (they are made for at most big RC cars like 1:8 scale).   Also the ability to configure it means you can make it work for different applications and can do things like reduce the max motor amperage which in turn reduces the torque/acceleration, and you can limit the low voltage cut off with the VESC itself so it reduces power to the motor as the batteries are getting low and once they are too low it cuts off power entirely to avoid damaging the batteries (called low voltage cut off, some other ESCs offer this, often configuring them involves doing voodoo with a controller or using a proprietary windows only app).

If you go lower voltage like 6S then can use X-Car Beast, or FVT 120A with active cooling on them (fan on heatsink) but I'm not sure they have higher voltage versions.  I tried a few other ESCs but you want one that has variable braking (and ideally regenerative to get that power back).

---

I also blew a couple other ESCs, believe one was made for boats and the other was made for planes, believe the plane one had "brakes" but it was just instant braking to stop a propeller not something you really want on a skateboard or bike.
```

---
## \#18 Posted by: vagosofron Posted at: 2018-01-14T21:29:12.220Z Reads: 103

```
I'm still trying to figure out which one is compatible with my motor, max current 90A. Sure, when you can configure it to your needs, it's great, but also pricy. So instead on spending money on cheaper, but not reliable escs, it's better to invest on a vesc. Any way, when this project evolves, i will definetely need your help. 
Cheers, Vagos.
```

---
## \#19 Posted by: wafflejock Posted at: 2018-01-14T21:39:08.655Z Reads: 109

```
Sure once you have a better idea of what components you're thinking of putting together can just put together a "build post' showing what the plan is before you buy things then can avoid returning or spending twice on parts if I or someone else sees something that isn't going to work.

In general I'd say most people don't hit the max limits of their hardware anyhow but if you want to figure out what you need to do to allow you to use the motor to it's full potential you would take the motor wattage and divide by your battery voltage to get the amperage that would need to get to the motor to max it out, that said I have a 2200W motor and I push about 20A @ 40V or 800W to it at most when accelerating hard (but I'm lightweight and don't ride crazy and live in Chicago).

---

Running higher voltage means less amperage to get the same watts to the motor, this is the reason we want to run higher voltage when possible too just to clarify.
```

---
## \#20 Posted by: vagosofron Posted at: 2018-01-14T21:42:53.254Z Reads: 110

```
Ok, i just realized something.....i have a lot of reading to do. Thank you, again.
I think this is my "build post".
```

---
## \#21 Posted by: wafflejock Posted at: 2018-01-14T21:43:45.144Z Reads: 101

```
Yeah can just edit this to include more details as you find them ideally link to components so we don't have to guess on what is what.

If you search for "build thread" on the forum here you'll find some examples where people list out all the components in one post (motor, battery, esc, BMS if applicable, charger, safety gear, control... everything so you can see if something is missing or some components won't work well together)
```

---
## \#22 Posted by: lrdesigns Posted at: 2018-01-15T03:02:20.076Z Reads: 99

```
Try to keep the power wires from the battery to the esc as short as possible, this will help reduce strain on the esc that could make it blow in a bike application. and / or add additional capacitors to the esc.
```

---
## \#23 Posted by: vagosofron Posted at: 2018-01-15T12:42:59.821Z Reads: 98

```
Thanks for the tip mate.
```

---
## \#24 Posted by: SpeedyGonzales Posted at: 2018-01-15T16:45:42.208Z Reads: 91

```
I think that at this point I built the most advanced Ebike with VESC and RC motor.
You can find everything about that build here: https://endless-sphere.com/forums/viewtopic.php?f=3&t=90432
The most difficult part of using RC motor with bicycle is reduction of RPM of your motor to RPM of pedals or rear wheel. I recommend you to sell the motor you have and go with hub motor. If you have hills to deal with get a 2 speed hub motor. This will be your best setup for a commuter Ebike. 
Right now I'm building something like that for my son. Let me know if you need more info.
Good luck.
```

---
## \#25 Posted by: vagosofron Posted at: 2018-01-15T19:06:22.736Z Reads: 89

```
Wow! Just wow! Tottaly Pro job. I could go that way, but it will cost me a lot more, because if i order a kit like that from outside EU, i will pay almost half the price on custom taxes. I don't know if i can find a used one though.
```

---
## \#26 Posted by: SpeedyGonzales Posted at: 2018-01-15T22:28:10.851Z Reads: 82

```
I'm sorry to tell you this but this not a kit. I just made it for myself. I spent on it about $2000 and I made most of aluminum parts by myself.
You can get 2 speed hub motor with controller and some other stuff from China.
http://www.xiongdamotor.com.cn/product/1580262905-220560510/New_Invention_Ebike_Motor_Double_speed_Motor_for_Front_Wheel.html
It will cost you $250 including shipping.

You will also need to buy a battery with charger for $350 including shipping. Also from China.
https://unitpackpower.en.alibaba.com/product/60469545598-800342742/13S4P_akku_rechargeable_e_bike_battery_48v_li_ion_battery_48v_11_6ah_NCR18650_PF_cell_.html
So, for about $600 you will be able to convert your bike to Ebike and it will work. 
I just don't know how much your government will ask you to pay for having all that. 
In the US nothing.
```

---
## \#27 Posted by: vagosofron Posted at: 2018-01-16T19:31:24.392Z Reads: 75

```
[quote="SpeedyGonzales, post:26, topic:43619"]
In the US nothing
[/quote]
In Greece...everything!
```

---
## \#28 Posted by: vagosofron Posted at: 2018-01-26T14:11:02.811Z Reads: 65

```
I finally got a dlux esc 60A, for now. I also found some cheap ( for me at least), hrb lipo batteries that are rated to 50c discharge. Is 50c to much or I can use them?
```

---
## \#29 Posted by: FredrikHems Posted at: 2018-01-26T15:17:56.433Z Reads: 61

```
[quote="vagosofron, post:28, topic:43619"]
to much
[/quote]


What is this??
```

---
## \#30 Posted by: vagosofron Posted at: 2018-01-26T18:28:21.296Z Reads: 58

```
Sorry, I meant too much...
```

---
## \#31 Posted by: FredrikHems Posted at: 2018-01-26T19:18:42.361Z Reads: 55

```
Haha, I didn't mean to correct your grammar. Trust me, I have a lot of grammar mistakes myself. What I meant was; Its never too much batteries!! The 50c will help you a lot with voltage sag (If the batteries have a capacity of 5Ah or so).
```

---
## \#32 Posted by: vagosofron Posted at: 2018-01-26T20:18:09.958Z Reads: 52

```
So, more is better, is that right?
```

---
## \#33 Posted by: FredrikHems Posted at: 2018-01-26T20:22:15.548Z Reads: 53

```
YESS!!!
10 Char
```

---
## \#34 Posted by: vagosofron Posted at: 2018-01-26T20:24:32.459Z Reads: 52

```
What is "10 Char"?
```

---
## \#35 Posted by: FredrikHems Posted at: 2018-01-26T20:36:04.490Z Reads: 53

```
The forum won't let you write a post if it has less than 10 characters..
```

---
## \#36 Posted by: vagosofron Posted at: 2018-01-26T20:39:22.627Z Reads: 53

```
@FredrikHems  Omg i am a huge noob! I think this sendence is more than 10 char...
Anyway, when i'll get all the parts needed, i wil post pics of the progress, thanks for the tips!
Question about gear ratio, how do i determine what gear ratio i need? I want to ride a 4klm distance with 1.5% elevation grade, without pedaling.
And also, what is better option, belt or chain drive?
```

---
## \#37 Posted by: vagosofron Posted at: 2018-01-30T21:52:37.111Z Reads: 47

```
A small update, I will build a hub motor ebike finally, so I will sell the motor and the esc I bought. I can't post the ad though.
```

---
