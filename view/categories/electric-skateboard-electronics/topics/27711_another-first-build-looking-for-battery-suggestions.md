# Another first build, looking for battery suggestions

### Replies: 8 Views: 711

## \#1 Posted by: Octavio Posted at: 2017-07-15T18:08:33.103Z Reads: 80

```
Hello,

I am building an e mountainboard as my first build. mainly due to the debris and cracks on my home town streets. I live at elevation 7,500 feet (2280 M) and have quite a few hills to climb. I weigh 230 lbs (104 kg) with protective equipment on. 

I need some help choosing a battery. The more I read on this subject, the more confused I get. 

What I have:

-MBS comp 95 mountainboard with Matrix2 trucks, 8 inch pneumatic tires. (aprox 570mm)
-(2)Torque boards 6355 190KV EPOWER Motor 
-(2) FOCBOX vesc
-70t wheel pulley
-15t motor pulley
-20mm belt drive

What I want in a battery, distance over speed, in fact 10-15 mph (16-25 kmh) seems like plenty of speed right now.  But I'd like to get my fat arse up these hills and get a distance of at least 8 miles (13km)

I'm looking to just copy Tonys's mountainboard and buy (2) ZIPPY Flightmax 5000mAh 5S1P 20C but he looks a lot lighter than me and he is on flats.

Should I pony up the money to buy higher capacity batteries like 8000 mAh?

Thanks in advance
```

---
## \#2 Posted by: aigenic Posted at: 2017-07-15T19:25:51.124Z Reads: 72

```
Yeah you should...why? because your motors take 60A each...together 120A...5Ah 20C battery would give you discharge rating of 100A which is too low...also with all terrain wheels you will get lower range than with PU wheels...

I would recommend you to use 8Ah 20C at least, if you can afford to go for higer discharge rating (25C, 30C...) go for it...your batteries wont sag that much :) 

Also on 10S you would get about [48 kmph](http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":10,"motor-kv":190,"system-efficiency":85,"motor-pulley-teeth":15,"wheel-pulley-teeth":70,"wheel-size":200}|), if I set up the diameter of the wheels correctly :D
```

---
## \#3 Posted by: Okami Posted at: 2017-07-15T19:31:46.165Z Reads: 71

```
For distance u might need more.juice than tony i think.

 I dunno for hills but going at 800w constant (versus 500w i usually consume.on flats)

U might.need 400 wh (more or less) for 30mins riding.

This depending at what speed u go might bring you either 10km or 15km.

General rule of.thumb for mountainboard energy consumtion is 15 - 20wh/km (except for some builds like @SimosMCmuffin who got something like 11-12wh/km I think )

So.. for flats only 13 km (8miles) might take = 13km x 15 - 20 = **195 wh - 260 wh**

----
Tonys battery = 4.9ah (margin) x 37v = **181,3 wh**

So i would say u might need 8000mah at least more or less

---

Ok didnt get to finish but I wanted to point out that if you would find out average watthour rating you might consume, then you could tell would your battery would be enough for range you desire.

Taking, 25wh / km, you might need 325wh of energy, more or less.

the 8ah pack (7.6ah - with small margin), at 37v = 281.2 Wh

--

So it looks like 10 ah pack would be more suited:

~9ah (with some reserve), x 37v = **333Wh**

This means, that in theory, you could ride at 333W of power for an hour, though im not sure you would get such average number.. but who knows :) 

My estimate is that you could see something more like 600W average at least (dual motors, too), so taking 666W (hah good number of choice, right), 30minutes or ride should be possible but speed is hard to tell at which you would go at such power level and also versus the hills/downhills you take.

Regen might also give some energy back but I dont have a good estimate for that.

Non the less, it looks like if you want some room for your battery, it would be best to go with 10s 10Ah or maybe even 12ah.

----
This comes from personal opinion and some numbers I crunched it. It might be possible to go the distance with 8ah pack but I wouldnt bet on that much, as it would produce close to 285 wh, if you calculate some reserve into it.

 And 285wh at 20wh/km, comes at around 14km (so only 1km reserve), so it is hard for me to speculate would you come below 20wh/km mark or not with the extra terrain conditions you mentioned.. though then again i havent done much data on hills, and this might be all false.

Though I hope i gave you some impression to go with and @aigenic also explained why it would be better to go with a pack with more power for example.
```

---
## \#4 Posted by: kieraneboard Posted at: 2017-07-15T21:41:39.665Z Reads: 54

```
I don't understand why you guys need so big current.
A 12A 36V motor is at power 432 Watt,  and 860 Watts when we have dual motor.

Allow me do a easy calculation of the power you need when up hill.

Say rider is 100kg  （1000N）
Say The slope is 15% Its already very very steep, if you disagree, carry a slope meter someday. 
Rider Horizen speed 21 KMH （6m/s） 
The vertical speed is 15%*6=0.9m/s
1 N-M/S is equal to 1 watt 
So the motors Power is 1000N*0.9M/S=900W
That means, the power of each mother is need to be 450W around.

And if you need 10KMH up hill at 15% slope is already enough.  means 225 Watt each motor is good.
Less power comsuption means bigger range, smaller current means more potection to ESC and motor and everything.
```

---
## \#5 Posted by: Octavio Posted at: 2017-07-15T22:25:26.677Z Reads: 53

```
So.  Having a hard time finding batteries that fit that description. 

I can find:

https://hobbyking.com/en_us/zippy-flightmax-8000mah-6s1p-30c.html

or 

https://hobbyking.com/en_us/multistar-high-capacity-4s-10000mah-multi-rotor-lipo-pack.html

Most 10Ah batteries I see out there are 10C, I am a noob and want to be conservative, not wanting to blow my VESC or Motors.
```

---
## \#6 Posted by: aigenic Posted at: 2017-07-15T22:34:44.914Z Reads: 47

```
Do you want to run 10s or 12s...I think you said 10s, but the batteries you sent are suitable only for 12s...
[5s 8Ah 30C](https://hobbyking.com/en_us/zippy-flightmax-8000mah-5s1p-30c.html)
YOu can always buy two with lower capacity and connect them in paralel...
```

---
## \#7 Posted by: Octavio Posted at: 2017-07-15T22:39:15.075Z Reads: 46

```
So linking 2 of these in series would be ok for my needs?

https://hobbyking.com/en_us/zippy-flightmax-8000mah-5s1p-30c.html
```

---
## \#8 Posted by: aigenic Posted at: 2017-07-15T22:43:27.818Z Reads: 44

```
More than ok :) you would be ok even with 20c :)
```

---
