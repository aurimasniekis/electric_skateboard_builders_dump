# Horrible range on the SPACE CELL with sk3 6374 192 Kv motor&hellip;anyone having the same issue?

### Replies: 23 Views: 3075

## \#1 Posted by: theviith Posted at: 2016-05-15T03:37:46.971Z Reads: 307

```
Does anyone have a sk3 6374 192 Kv motor hooked up to VESC and SPACE CELL? If so, what is your VESC settings specific for that motor? Also what is the approx range you're getting? I just tested my second build with those components and my range was pretty bad. I only totaled about 5 miles before I stopped at 40% battery life, which is about 1.8 miles per 20% battery!!! Did I do something wrong? could it be my gearing? Thanks in advance

My current setup:
VESC with 10S space cell
single [SK3 6374 192kv](http://www.hobbyking.com/hobbyking/store/__18129__Turnigy_Aerodrive_SK3_6374_192kv_Brushless_Outrunner_Motor.html) on 14T 50T
5 in.(127mm) pneumatic wheels
GT2B r/c system

My VESC settings:
Motor max: 80
Motor min (regen): -60
Batt max: 30
Batt min (regen): -12
Absolute max: 130
```

---
## \#2 Posted by: Namasaki Posted at: 2016-05-15T04:05:10.763Z Reads: 297

```
I'm gonna guess that its because of the very low gearing and the really big pneumatic tires. 
I bet if you where running a street setup like 16/36 gears and 83-90mm wheels, your mileage would be better.
What you have there is an off road hill climbing machine. Thats gotta cost some mileage.
```

---
## \#3 Posted by: seanpain4 Posted at: 2016-05-15T04:41:50.009Z Reads: 286

```
Do you have a watt meter so you can measure total Wh pulled from the battery during usage? That will allow you to see of you are getting everything out of your space cell
```

---
## \#4 Posted by: Namasaki Posted at: 2016-05-15T05:18:54.277Z Reads: 286

```
http://www.all-battery.com/TenergyWattMeterandPowerAnalyzer.aspx?utm_source=GoogleShopping&utm_medium=GDF&gdftrk=gdfV26767_a_7c354_a_7c922_a_7c01446&gclid=CLK80uef28wCFUdrfgodZ_4BVw
```

---
## \#5 Posted by: EnertionSupport Posted at: 2016-05-15T12:08:03.405Z Reads: 261

```
pneumatics while drain your battery way faster than normal skate wheels. 

With urethane, you can easily coast, and you are restricted to pavement- all terrain wheels open up some more challenging environments, and take more power to start them up and keep them going. 

it is simply that they (on average) have to pull more watts than street wheels!

Back when we sold the 5inch pneumatic wheels, I did a single motor range test with both the pneumatics and 83mm Enertion wheels on the same route (all street, some light hills), and had 70%+ left on the street setup when the pneumatics had under 40% at the same point.
```

---
## \#6 Posted by: chaka Posted at: 2016-05-15T12:28:24.183Z Reads: 249

```
If your belt is too tight it can cause excessive watt usage. Be sure you have a little slack in that belt. Rotate the wheel and check the belt through the whole rotation to be sure the belt does not get tight at any point. Don't make the belt so loose that you end up skipping teeth constantly either.
```

---
## \#7 Posted by: theviith Posted at: 2016-05-16T00:55:20.312Z Reads: 226

```
thanks for the clarification. Maybe I'll try swapping out the wheels with normal wheels and see if there is a difference. 
Hm so then what type of batteries would support the high drain and can give a decent amount of range for pneumatic wheels?
```

---
## \#8 Posted by: zool774 Posted at: 2016-05-18T22:13:50.165Z Reads: 197

```
I guess a 12S and slick tires might help...?!!?
Also LIPo batteries have more kick, that may help 2.
```

---
## \#9 Posted by: longhairedboy Posted at: 2016-05-18T22:51:06.790Z Reads: 192

```
if you're packin pneumies on there then you have plenty of room for a giant box filled with cells. i say stack on the watt hours.
```

---
## \#10 Posted by: Namasaki Posted at: 2016-05-18T23:36:55.661Z Reads: 186

```
How about this, 2 space cells stacked and connected  in parallel!!!!
```

---
## \#11 Posted by: theviith Posted at: 2016-05-20T18:26:35.456Z Reads: 176

```
thanks guys for the support. I think I might try the Lipo option as I find Lipo's to be more efficient for high power consumption setup
```

---
## \#12 Posted by: theviith Posted at: 2016-05-20T18:27:34.194Z Reads: 171

```
2 space cells?! that's ~$800 right there! :scream:
```

---
## \#13 Posted by: theviith Posted at: 2016-05-20T18:30:01.068Z Reads: 168

```
also, I'm not sure if I want to deal with Enertion anymore due to the terrible wait and increasingly poor customer service. Last time I purchased a space cell, I waited for 3+ months...
```

---
## \#14 Posted by: Namasaki Posted at: 2016-05-22T20:54:24.986Z Reads: 161

```
i'm using Lipos. They are a good option if your wanting maximum power. And if you mount them in a easy access enclosure, you can bring extras in a backpack to go on long treks. I have a maximum 30 mile range with 3 packs.
Although, I doubt my legs would hold up for that distance.
I'm running 12s with dual motors and the power is amazing. You really have to brace yourself when you get on throttle.
```

---
## \#15 Posted by: zool774 Posted at: 2016-05-23T00:19:33.425Z Reads: 159

```
No way, 3 months?? 
How long ago was that? Just ordered mine 3 weeks ago..
```

---
## \#16 Posted by: theviith Posted at: 2016-05-23T23:02:56.276Z Reads: 145

```
yup, 3 full months.. this was back in mid Jan. when I made the order. Didn't receive it until April.
```

---
## \#17 Posted by: theviith Posted at: 2016-05-23T23:05:24.847Z Reads: 142

```
yeah, I am going with Lipo as well for the pneumatics. I'll most likely run it in 10S because I read somewhere that it's not good for the VESC to be in 12S as it creates heating issues with the FETs and such. Plus, 10S on a sk3 192kv and 5in pneumatic wheels is fast enough haha
```

---
## \#18 Posted by: zool774 Posted at: 2016-05-23T23:44:54.614Z Reads: 144

```
Holy sshh... 
So by the time I'd get mine, it'd be  the end of the summer....
```

---
## \#19 Posted by: theviith Posted at: 2016-05-23T23:55:55.084Z Reads: 143

```
yea, sorry buddy. That is why I decided to make my own pack instead. But just need to figure out how to connect everything without blowing my apartment up lol
```

---
## \#20 Posted by: Namasaki Posted at: 2016-05-23T23:56:43.636Z Reads: 142

```
I'll have to agree that running 12s is pushing everything to its limits.
10s is surely better for longevity. 
I almost went with 10s but found 6s lipos cheaper and more readily available than 5s lipos. 
So I went with 12s. 
12s is ok with belt drive because with gear reduction
You draw less amps. 
If your running any form of hub motors, then better to go 10s in my opinion.
```

---
## \#21 Posted by: Troyi00 Posted at: 2016-07-24T19:56:09.373Z Reads: 116

```
The bigger the radius of the wheels, the greater the moment inertia. The greater the moment inertia, the harder it is to move, but once it starts moving, the harder it is to stop. Like rolling and stopping a boulder vs a marble. Takes a lot more more force or torque.
```

---
## \#22 Posted by: barajabali Posted at: 2016-07-24T20:12:34.266Z Reads: 117

```
Didn't see this thread back in my but keep your tires inflated pretty hard to reduce rolling resistance
```

---
## \#23 Posted by: lilracerboi Posted at: 2016-09-28T16:44:18.738Z Reads: 69

```
This thread is pretty old, but I came across a similar issue, but on street wheels.  
Here's my thread about it: http://www.electric-skateboard.builders/t/space-cell-pro4-maximum-charge-stuck-at-94/10269/4

Don't know what could've happened. I rarely take the battery/case off.
```

---
