# Help Needed: Flat Battery

### Replies: 34 Views: 1342

## \#1 Posted by: TunaTee Posted at: 2017-09-22T23:16:35.190Z Reads: 177

```
Hello, guys.
I built my board about 4 days ago and never had a chance to test its limit.
Well, today I went to the central park and rode till my battery runs out of juice. I set the cutoff limit to 3.2 V.
I got some pretty happy result. Seried three 3s1p 5000mah and it went 13.2 miles with a top speed of 24.2(I think it can go faster but I am not able handle speed above 24.)
Got back home, trying to charge, the battery told me that I have a low voltage pack. I lowered the charging current to 1/10 of the C so 0.5A according to some tutorials. However, the charger is only able to detect 2S instead of 3S. What is the problem? Is the battery still good for use?
Addition to that, another battery pack is fine. How come the motor did not draw current from each of them equally? 

Thanks for your help.
```

---
## \#2 Posted by: gogomrrobot Posted at: 2017-09-22T23:18:47.263Z Reads: 166

```
Put charger on NiCD mode and charge for 40seconds to a minute until the voltage is high enough. Then go to Lipo mode and charge normally
```

---
## \#3 Posted by: pat.speed Posted at: 2017-09-22T23:19:20.662Z Reads: 160

```
Check he cells with a multimeter and report back
```

---
## \#4 Posted by: TunaTee Posted at: 2017-09-22T23:28:50.914Z Reads: 148

```
Unfortunately, my charger is LiPro Balance Charger, it can only charge in lipo mode, no other modes :(
```

---
## \#5 Posted by: TunaTee Posted at: 2017-09-22T23:29:10.016Z Reads: 145

```
Another unfortunate that I do not have a multimeter:(
```

---
## \#6 Posted by: pat.speed Posted at: 2017-09-22T23:41:04.734Z Reads: 140

```
Ahhh well in this hobby it is a very important tool and I highly recommend one. They are a few bucks from a hardware store or maybe automotive shop
```

---
## \#7 Posted by: TunaTee Posted at: 2017-09-22T23:44:38.615Z Reads: 141

```
alright, I will pick them up tmr in my local hardware store. Thanks.
```

---
## \#8 Posted by: pat.speed Posted at: 2017-09-22T23:45:20.873Z Reads: 134

```
No worries
```

---
## \#9 Posted by: Acido Posted at: 2017-09-23T07:23:18.518Z Reads: 119

```
Get a bms they arent expensive
```

---
## \#10 Posted by: darkkevind Posted at: 2017-09-23T08:12:15.303Z Reads: 117

```
I've had this, in fact I still do, I need to fix it but basically one of your balance leads have come off of its connection inside your lipo pack, maybe desoldered or just plain broken... This is why it can only detect two cells.

You need to take your pack apart, use a multimeter to detect which wire has disconnected and solder it back on...
```

---
## \#11 Posted by: TunaTee Posted at: 2017-09-23T22:16:04.352Z Reads: 90

```
That is my plan. But do you think I should just throw these batteries to trash?
```

---
## \#12 Posted by: TunaTee Posted at: 2017-09-23T22:16:26.732Z Reads: 85

```
Wow, solder a lipo pack sounds like a fire hazard.
```

---
## \#13 Posted by: darkkevind Posted at: 2017-09-23T22:18:51.367Z Reads: 80

```
Lol, how do you think the balance wires were connected in the first place?
```

---
## \#14 Posted by: TunaTee Posted at: 2017-09-23T22:19:44.896Z Reads: 76

```
I will leave these things to the pro lol. Do you think I should throw them or sell them at a very low price?
```

---
## \#15 Posted by: darkkevind Posted at: 2017-09-23T22:26:00.290Z Reads: 77

```
Don't throw them, someone could salvage them. Sell them with full disclosure if you don't want to solder it yourself, as long as they're not all puffed up...

Where are you based? What's the spec of the batteries?
```

---
## \#16 Posted by: TunaTee Posted at: 2017-09-23T22:30:33.811Z Reads: 78

```
I got three 3s1p 5000mah. $32 each. I am planning to sell three for $40 and get three new ones.
```

---
## \#17 Posted by: darkkevind Posted at: 2017-09-23T22:33:46.547Z Reads: 78

```
Ahhh if you EU based I'd have had them off you :confused:
```

---
## \#18 Posted by: TunaTee Posted at: 2017-09-23T23:25:09.385Z Reads: 78

```
I got my batteries fixed.

So basically I charged it at 1A(for safety issues), although the charger only detected 2 cells, I still went ahead and charged at 3 cells. After the voltage climbed up to about 3.2 V per cell, the charger is able to detect it as a 3 cell battery pack. So if anyone have this same issue, please charge at a much lower rate and always charge your battery pack in a Lipo safe bag.
```

---
## \#19 Posted by: TunaTee Posted at: 2017-09-24T01:13:16.402Z Reads: 76

```
one of my battery can only charge up to 12.5V and the other 12.47. Am I able to connect them to serie or will this cause a fire?
```

---
## \#20 Posted by: darkkevind Posted at: 2017-09-24T07:00:07.422Z Reads: 72

```
It sounds like you have a bad cell if the voltage dropped below a detectable level. You may get lucky and it may be ok from now, but it sounds like you'd be better off towing that dodgey cell.

Putting them in series now though will be fine, it doesn't matter about the voltage difference.
```

---
## \#21 Posted by: TunaTee Posted at: 2017-09-25T03:57:35.363Z Reads: 53

```
Thanks. It is strange how I re-charged them and they were able to climb up to 12.6  V.
```

---
## \#22 Posted by: Silverline Posted at: 2017-09-25T06:00:35.744Z Reads: 46

```
You run those lipo's way to low. On racing drones we land when the cell voltage is about 3,7 volt.
Watch out for fire bombs....i would put those lipo's in salty water, and buy new Ones.
```

---
## \#23 Posted by: Hummie Posted at: 2017-09-25T06:40:16.903Z Reads: 46

```
putting lipo in salty water I thought was a way to discharge them so they could then go in the trash but the terminals quickly get coated with an oxide and they often will still be holding a big charge.  you really have to cut the battery leads and expose a lot of material in my experience.
```

---
## \#24 Posted by: Silverline Posted at: 2017-09-25T06:51:08.562Z Reads: 44

```
Yes exactly. They should be in the trash...
```

---
## \#25 Posted by: TunaTee Posted at: 2017-09-25T14:04:23.884Z Reads: 44

```
They are working fine now :)
```

---
## \#26 Posted by: Wilsonliang777 Posted at: 2017-09-28T01:56:39.522Z Reads: 34

```
I am confused.  I don't know too much about lipo batteries.  I used to run my lipo cells down to 3.2v and the battery manual also suggested that lipo cells should not go below 3.2v.       But recently I noticed a lot of ppl suggests lipo cells should not go be low 3.6v.   I noticed that if I charge my lipo when the cells reach 3.6v the battery is only half of its stated capacity.  My lipo battery is stated 7000mah i get about 3500mah of usable capacity if I charge my battery cells at 3.6v.
```

---
## \#27 Posted by: TunaTee Posted at: 2017-09-28T02:38:29.055Z Reads: 34

```
I am no expert here, but I think what he means is that you should not run your battery below that level, doesnt mean you cannot charge them over that level. 4.2V is the max.
```

---
## \#28 Posted by: Wilsonliang777 Posted at: 2017-09-28T03:13:20.204Z Reads: 33

```
I charge it to the max. Like 4.1 to 4.2v.  But I still get only like half the stated capacity if I charge the cells reach around 3.6v.
```

---
## \#29 Posted by: TunaTee Posted at: 2017-09-28T03:54:57.718Z Reads: 31

```
Well, if you want to take good care of your battery and dont let it stress alot, this is the way to go. Or you can connect more in parallel so you get more mAh.

Again I am no expert in this, you should ask someone else with more experience :D
```

---
## \#30 Posted by: SORRENTINO Posted at: 2017-09-28T04:12:56.689Z Reads: 28

```
You only use a certain percentage of your batteries total capacity. Same goes for lithium ion. Now if you could discharge your battery from 4.2v per cell to 0.0v per cell then you would have used all 7000mah. I think you are just over thinking this. 3.5v a cell is the lowest I would go with lipos to be safe and to have them last longer.
```

---
## \#31 Posted by: telnoi Posted at: 2017-09-28T05:10:24.862Z Reads: 27

```
I don't run Lipos below 3.6 under load. During my 3 years of high performance multimotor flying I have noticed that lipos that are drained to 3.2 under load will get comparatively hot and will die much sooner. 

I am talking about a life cycle that is cut in half, especially with low c Lipos. I typically only get 60c to get the most out of them/these go down to say 3.4 a bit easier.

C rating is often inflated though. MyLipo offers Parcour Lipos with a true c rating. The Turnigy Graphene are ok, but the c rating is more like 45 for the 60 version. Still, a good and relatively cheap lipo.
```

---
## \#32 Posted by: Cobber Posted at: 2017-09-28T05:33:23.599Z Reads: 26

```
The rc guys talk about this a bit. The old recommendation used to start at 3.5v, now with the new generation lipos it is from 3.7v.
```

---
## \#33 Posted by: telnoi Posted at: 2017-09-28T05:46:33.405Z Reads: 27

```
They have way more power but also can take a bit more abuse. The voltage sag is not linear anymore and indeed drops like a stone.

I have to land within 5 seconds to stay within the safe voltage range after hitting 3.6v per cell. Resting voltage ends up being 15.3v on 4s.
```

---
## \#34 Posted by: Cobber Posted at: 2017-09-28T05:51:36.329Z Reads: 27

```
oops sorry @telnoi, I thought I was posting but I edited my post.  :confounded:
on my way back to work, figured I didn't have time to to convince anyone if...
```

---
