# Why is my range so low? 10s 4000mah lipo battery

### Replies: 31 Views: 902

## \#1 Posted by: Lucajo16 Posted at: 2018-11-01T23:09:34.656Z Reads: 250

```
Hi so I just finished my electric skateboard the other day and I've fallen in love with the thing. (( think metaphorically here not literally love)) But I have one slight problem.....it only lasts for about 3 to 4 miles before the cheap SEC turns itself off for safety purposes. My problem is I want to ride it to work and back without having to swap a new set of batteries out mid commute. Its not a high powered motor its a cheap hub motor from [ebay](https://www.ebay.com/itm/90mm-dual-6364-hub-motors-drive-kit-for-electric-skateboard-longboard-part-USA/223082324395?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2057872.m2749.l2649) I also got these 2 [lipo's](https://www.ebay.com/itm/TURNIGY-4000mAh-5S-18-5V-30C-40C-LIPO-BATTERY-XT60-CAR-TRUCK-TRUGGY-BOAT-PLANE/282727183075?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2057872.m2749.l2649) and here is my[ESC](https://www.ebay.com/itm/Dual-motors-longboard-skateboard-controller-with-remote-ESC-Substitute/302812941839?ssPageName=STRK%3AMEBIDX%3AIT&var=601709105317&_trksid=p2057872.m2749.l2649) But again I'm only getting 3 or 4 miles of range out of this set up. I'm woundering if I make my own 18650 pack and maybe a smaller motor like this [one](collections/electric-skateboard-motors/products/electric-skateboard-motor-6355-260kv) will dropping the voltage and making a bigger battery would it help at all? pleast help!
```

---
## \#2 Posted by: b264 Posted at: 2018-11-01T23:13:04.190Z Reads: 246

```
That sounds about right for 10S 4Ah.  If you put two more of those batteries in parallel, it will double the range (10S 8Ah)
```

---
## \#3 Posted by: RedEagle Posted at: 2018-11-01T23:14:59.172Z Reads: 243

```
First off, that esc is crap. second, your battery mah is the main reason you're getting so little range. buy 2 more and put them in parallel.
Oh i see @b264 beat me to it :sweat_smile:
```

---
## \#4 Posted by: b264 Posted at: 2018-11-01T23:16:57.915Z Reads: 239

```
Don't use 260kv motors though.  Use 190kv at the highest.  140kv to 190kv.
```

---
## \#5 Posted by: Lucajo16 Posted at: 2018-11-01T23:23:02.184Z Reads: 225

```
what would be wrong using that motor? also if I drop the voltage and make my own pack would I expect more range? I was thinking of starting another build and use the battery's I have for an Arduino spot welder. I live in an apartment with dated electrical so I don't want to buy one of those cheapo spot welders.
```

---
## \#6 Posted by: b264 Posted at: 2018-11-01T23:25:44.952Z Reads: 219

```
If/when you want to upgrade your ESC you won't be able to without buying a new motor.  Plus when the kv is over 190 they have little if any resale value on the used market.  Trust those who have trodden before you.  Don't go over 190kv :wink:

The same motor is available for the same price [wound at 190kv instead](collections/electric-skateboard-motors/products/electric-skateboard-motor-6355-190kv) and those are good motors.  I'd put acrylic conformal coating on the sensor assembly though otherwise it's not water resistant.
```

---
## \#7 Posted by: Lucajo16 Posted at: 2018-11-01T23:47:12.487Z Reads: 210

```
[quote="b264, post:6, topic:73087, full:true"]
If/when you want to upgrade your ESC you won't be able to without buying a new motor.  Plus when the kv is over 190 they have little if any resale value on the used market.  Trust those who have trodden before you.  Don't go over 190kv :wink:

The same motor is available for the same price [wound at 190kv instead](collections/electric-skateboard-motors/products/electric-skateboard-motor-6355-190kv) and those are good motors.  I'd put acrylic conformal coating on the sensor assembly though otherwise it's not water resistant.
[/quote]

ok sounds like ill be using that motor then. But to ask would lowering my voltage and building my own 18650 pack do anything for range?  I want to stay between the 20-30 MPH range and about 10-20 miles in range. so i was thinking maybe a 6s 4p pack would do just that.
```

---
## \#8 Posted by: b264 Posted at: 2018-11-01T23:51:17.774Z Reads: 196

```
Lowering your voltage won't increase your range.  Adding amp*hours of course is the ultimate range-extender. 
 Limiting motor current (in software) will increase your range too.  But the single biggest thing that will increase your range is learning how to pilot the esk8 in a way that is much more efficient.

I suggest limiting the motor current in software, seeing how it rides, then turning it back up and trying to ride the way you remember it felt most of the time.  Then occasionally you can hit the throttle hard if you want... but for the most part you just feather the throttle enough to keep you moving.  Also kicking to start can help a lot with extending range.

But with that ESC, you can't adjust anything at all.  But the rest is still do-able.
```

---
## \#9 Posted by: Lucajo16 Posted at: 2018-11-01T23:56:49.939Z Reads: 184

```
well thanks for the info. It helps out a lot! ^_^ i will look into upgrading my ESC here soon. I might go with a dual vesc set up. im already thinking of my next build as it is! Thanks! :smiley:
```

---
## \#10 Posted by: dareno Posted at: 2018-11-02T00:02:15.021Z Reads: 178

```
Of course you are my friend

[quote="Lucajo16, post:9, topic:73087"]
im already thinking of my next build as it is!
[/quote]
welcome to the hotel california.  Its an addiction make no mistake.
```

---
## \#11 Posted by: Santino Posted at: 2018-11-02T02:17:36.467Z Reads: 162

```
Buy the best ESC if it's possible (Vesc6, Focbox, etc..), 130kv - 170kv...No need for twin set up if you can not afford a great ESC, but with one VESC6 for example, you could go 12s 4P (2 x 6s 2P 22000mAh each)....Just try not to waste money....Read a lot, learn a lot, then spend a lot... Enjoy!!!
```

---
## \#12 Posted by: Deodand Posted at: 2018-11-02T02:52:16.323Z Reads: 153

```
For batteries its best to think in terms of watt hours, amp hours is only a fair comparison  for batteries of the same voltage. Take the amp hours of the pack and multiply it by the nominal voltage to get the watt hours. For reference a good 10s4p Li-Ion pack will have somewhere around 400-450 Watt hours capacity and that will get you somewhere in the 20 mile range if your lightweight and riding efficiently. Your pack is 37V * 4 Ah = 140 Watt hours, so about 1/3rd the size if the Ah rating on your lipos can be trusted. 

Unless you plan to make/weld multiple batteries I would strongly encourage you to simply buy one off the shelf. I've done some cost breakdowns on this and even if you don't mess anything up and make a perfect battery each time you have to make a few before you recoup costs on all the equipment (time, BMS, nickel strip, cells, shrink wrap, wiring etc.). You can even just slap two meepo batteries in parallel if your low on funds and want a cheap solution, the form factor isn't the best though and if you look around on the forum here you'll find some other competitive offerings. 

@b264 is steering you right on lower kv motors, additionally I wanted to add in some extra info that may be somewhat counter-intuitive. The bigger the motor used (more copper) the more efficient that motor will be **IF** you ride the board conservatively. Very different from how gas cars work here, **big beefy motors ridden gently will get the most efficiency**. 

Also since I'm me, let me shamelessly plug the new [focbox unity!](https://www.enertionboards.com/focbox-speed-controller/focbox-unity-dual-motor-foc-controller-esc/) It's a great dual setup and includes power switch/bluetooth and app and offers all the customization of vesc based designs.  It's nice because it is an easy swap out for your existing controller without any more wiring/parts. Perhaps a bit pricey, but its the brain of your board and the unity will be able to handle pretty much anything in your upgrade path. If you need something cheaper I'd stay away from the flipsky dual 4.20 esc, a lot of reported issues there. Better off going with some of the other cheap alternatives like hobbyking or something, just be aware they won't be able to push the same amps since they have no dedicated heatsink attached and use cheaper components.
```

---
## \#13 Posted by: b264 Posted at: 2018-11-02T06:04:39.127Z Reads: 126

```
Upgrading to a Unity or other similar ESC based on VESC technology should definitely be in your long-term plans.

6374 will be more efficient than the 6355 but they are also rather heavy and kind-of overkill.  In my honest opinion, dual 6355 are perfect for esk8.  6374 maybe for a performance build, but they also add a lot of weight for a minimal amount of gain relative to the cost/weight/space increase.
```

---
## \#14 Posted by: Andy87 Posted at: 2018-11-02T06:06:05.214Z Reads: 120

```
one thing i want to add here too, just that it´s said.
there some things besides your weight and riding style which influence your range.
if you use pneumantic wheels it will decrease your range about 20%. 
Also which drive train you use. I don´t have experience with direct drive or hubs yet, but i can say chain - belts - geardrive in this order your range will expand.
for example i got about 10km out of a 12s 5Ah pack with a belt drive train.
than i changed to chains and now my range is only about 8-8,5km
```

---
## \#15 Posted by: pat.speed Posted at: 2018-11-02T09:06:40.927Z Reads: 112

```
Not sure how this went so wrong. Your batteries are the main problem, not your motors and esc. 

With those batteries you could expect somewhere around 10km of range. I have a dual chain board with a 12s5000mah battery (222wh) and I can get anywhere between 20 and 12km of range depending on how I ride. I also have a single board with 10s5000mah battery, that board gets between 20 and 15km of range. 

Now you have a 10s4000mah battery (148wh) with the average wh usage of 10wh/km you would get something like 15km of range. That isn’t accurate unless you ride under 20km/h though. I like to use 12-14wh/km as my rule as it gives some more room for faster riding. According to that you should get about 10km of range. But if you ride at top speed constantly you will probably only get 7-8km. 

If you really want long range you need to listen to others and get a li-ion pack, something like 10s4p or even 5p. Otherwise just don’t ride so fast all the time, I know it’s hard at the start I used to gun it the whole ride, but now I prefer to cruise about 25km/h and enjoy carving and the scenery
```

---
## \#16 Posted by: b264 Posted at: 2018-11-02T09:13:10.673Z Reads: 103

```
[quote="pat.speed, post:15, topic:73087"]
If you really want long range you need to listen to others and get a li-ion pack, something like 10s4p or even 5p. Otherwise just don’t ride so fast all the time, I know it’s hard at the start I used to gun it the whole ride, but now I prefer to cruise about 25km/h and enjoy carving and the scenery
[/quote]

Long range is definitely possible without a li-ion pack.  LiFePO4 or LiPo can definitely get long range.

I think it's mainly riding style and mAh
```

---
## \#17 Posted by: Andy87 Posted at: 2018-11-02T09:14:11.387Z Reads: 100

```
[quote="pat.speed, post:15, topic:73087"]
I have a dual chain board with a 12s5000mah battery (222wh) and I can get anywhere between 20 and 12km
[/quote]

hey @pat.speed how you manage to get 20km out of that with chains? you have chains and pneumatics or urethan?
i once got like 17km out of my 12s 5Ah packs but with belt and the average speed was about 8-10km/h :sweat_smile:
maybe i make something wrong :thinking:
or maybe i shouldn´t go so hard offroad :rofl:
```

---
## \#18 Posted by: pat.speed Posted at: 2018-11-02T09:24:34.967Z Reads: 95

```
I ride thanes and only weight 60kg so that def helps, I came back from a ride the other day, we did about 17km and my cells were at 3.65v so I could easily squeeze out a few more kms.


@b264 yeah I agree lipos can also be used for longer range, I personally think it is just easy to use a 18650 pack when you need one that big. The tangle of wires from lipos in parallel would drive me crazy
```

---
## \#19 Posted by: Sebike Posted at: 2018-11-02T11:10:11.508Z Reads: 89

```
The stated Ah for a cell is determined by measuring at a low current draw and down to a lower voltage level than the cut off value we usually use on our boards, so to get a better estimate of range one should have that in mind when calculating Wh. 

A 10s4p of 30q cells will more likely have around 330 usuable Wh in our applications.
```

---
## \#20 Posted by: bartroosen12 Posted at: 2018-11-02T12:50:50.492Z Reads: 87

```
10S 4Ah so around 150Wh, those lipo's must give you at least 11km (7miles) range.
The esc an hubmotors pull around 20A max so if the lipo's are good that shouldn't be a problem.
The only thing I can imagine why you get such a low range is voltage sag, maybe these batteries are not as good as described.
```

---
## \#21 Posted by: Lucajo16 Posted at: 2018-11-02T13:04:56.508Z Reads: 79

```
I was thinking of the unity which If I remember is about 300 dollars. its not a major investment for me if it means I can run dual motors.  I live in  Cincinnati Ohio and a lot of my commute is up or down hills. there are flat spots but not a ton. I just need to figure out when I can start my next build. It wont be until later next month though for sure.
```

---
## \#22 Posted by: Bob6677 Posted at: 2018-11-02T13:10:42.485Z Reads: 79

```
Try Samsung 30Q battery. It's the best choose for building electric skateboard.
```

---
## \#23 Posted by: bartroosen12 Posted at: 2018-11-02T13:18:24.950Z Reads: 77

```
Yeah I have a 10S4P 30Q pack and a 10S3P VTC6 pack and they are awesome, but lipo's can also be great if you use them right. He must get a lot more range out of his 10S 4Ah battery
```

---
## \#24 Posted by: Lucajo16 Posted at: 2018-11-02T13:23:21.847Z Reads: 74

```
@Bob6677 I was thinking of building my own battery sense I have a LIPO pack. there are spot welders
out there that can run off of a LIPO pack. it costs about 125 dollars but I did plan on building more then one pack. I have a history of building weird stuff in my town and people tend to ask me about my builds. so to other's saying just buy a pack id rather build my own first and if I cant build it then I will buy one. 

@bartroosen12 i get about 4 miles of range out of my LIPOs I never intended this to be a final project. I planned to build a few more and maybe sell them to some capacity.. weather I build just packs or whole boards.
```

---
## \#25 Posted by: Lucajo16 Posted at: 2018-11-02T13:37:25.438Z Reads: 69

```
For those that might be thinking about that spot welder I was talking about here is a link to it. I thought it might help you guys out who want to build a pack but live in an apartment like me. [spot welder and soldering iron combo](https://www.ebay.com/itm/Arduino-S2-Spot-welder-Soldering-Iron-for-Hakko-T12-EMS-Shipping/202487588570)
```

---
## \#26 Posted by: venom121212 Posted at: 2018-11-02T15:09:45.780Z Reads: 61

```
Only other dude in the natti area I've seen on here!
```

---
## \#27 Posted by: Lucajo16 Posted at: 2018-11-02T15:25:01.038Z Reads: 61

```
@venom121212 so do you live in the norwood area? I think i see you every few days riding by some chemical plants do you?
```

---
## \#28 Posted by: venom121212 Posted at: 2018-11-02T15:37:09.415Z Reads: 61

```
@Lucajo16 Nah must be another cool guy. I'm up by Armco Park / Lebanon area outside the city
```

---
## \#29 Posted by: Lucajo16 Posted at: 2018-11-02T15:57:23.366Z Reads: 62

```
@venom121212 ya there is a guy who rides by my job back and fourth. But i dont think he builds em. His seemed pretty much like a finished product or something. I still need to put grip tape on my board and consider doing some upgrades
```

---
## \#30 Posted by: venom121212 Posted at: 2018-11-04T22:38:38.074Z Reads: 52

```
Nice, I just left Ault park and wished I brought my board so bad. You ever ride there?
```

---
## \#31 Posted by: Lucajo16 Posted at: 2018-11-07T17:55:18.802Z Reads: 41

```
No @venom121212 i have dont even know where that is. My board is my main form of commuting when not on the local metro. I live really close to downtown so i dont have a car at this moment. Im shooting for my license the spring of this year. If youd like to ride there is a local park called winton woods...has a great trail by the lake thats kept in order. Id love to check out your board. Right now im getting ready for my next build as we speak. Im building my own spot welder and everything!
```

---
