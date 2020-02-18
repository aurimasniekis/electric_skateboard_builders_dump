# Boys, check my battery choice before i hit &ldquo;Checkout&rdquo;

### Replies: 20 Views: 619

## \#1 Posted by: Proxy Posted at: 2017-12-07T07:51:50.100Z Reads: 181

```
**The battery last part to complete my build. I plan on putting 2 8000mAh 5S1P 30C in series to give me a total of 37v. Still not feeling confident about my choice so i need some of help deciding if i should hit the "Checkout" Button.. I need some confirmation from more experienced builders...What do you guy think?**

**VESC**: collections/esc-speed-controller/products/torque-esc-vesc-bldc-electronic-speed-controller

**MOTOR**: collections/electric-skateboard-motors/products/electric-skateboard-motor-6355-190kv

**BATTERY**: https://hobbyking.com/en_us/zippy-flightmax-8000mah-5s1p-30c.html
```

---
## \#2 Posted by: saul Posted at: 2017-12-07T08:14:03.291Z Reads: 171

```
30C is much more than you need.
thats 240A continuous. wayyy overkill..

oh and on't forget the connectors and wires and heatshirk and all that extra stuff...
```

---
## \#3 Posted by: ShutterShock Posted at: 2017-12-07T08:16:29.346Z Reads: 158

```
I disagree that it is overkill, I think it is a nice safe number.  Often, they are not actually running at their full rating.  I say it is a good choice.
```

---
## \#4 Posted by: Proxy Posted at: 2017-12-07T08:25:49.764Z Reads: 146

```
Weird. I Choose 25c before and most people were telling me to at least go 30c
```

---
## \#5 Posted by: ShutterShock Posted at: 2017-12-07T08:26:39.604Z Reads: 139

```
Yeah I have 25C on mine too and I see "get 30C" all over lol

I haven't had any problems
```

---
## \#6 Posted by: scepterr Posted at: 2017-12-07T08:27:27.179Z Reads: 130

```
Yes and no, kinda, not really lol
Personally I hate C ratings and think they should die
At 8Ah, it's 240, but at 2Ah it's 60A, so through the whole capacity of the battery "30C" is pretty reasonable.
```

---
## \#7 Posted by: Proxy Posted at: 2017-12-07T08:28:07.664Z Reads: 122

```
Do you think Maybe my 8000 mah might make the amps to high?
```

---
## \#8 Posted by: scepterr Posted at: 2017-12-07T08:29:51.309Z Reads: 121

```
It's fine, all it means is you could for whatever insane reason pull 240 at full charge, but what it really means is you could do 50-60A through the whole usable  capacity of the battery
```

---
## \#9 Posted by: saul Posted at: 2017-12-07T08:34:13.951Z Reads: 119

```
[quote="scepterr, post:6, topic:40352"]
At 8Ah, it's 240, but at 2Ah it's 60A, so through the whole capacity of the battery "30C" is pretty reasonable.
[/quote]

I am <s>pretty</s> **sure** this is not how a C rating works.

but yes you also see people on here saying that you shouldn't do anything less than 4wd or 500watt hours.

I've tested combinations of batteries with high and and low C ratings, 3Ah - 10Ah. 
high kv low kv. big wheels, small wheels, hills, flats, all of it.


You Do Not Need 30C for a single 10s 190kv.
----------
```

---
## \#10 Posted by: scepterr Posted at: 2017-12-07T08:36:32.232Z Reads: 108

```
C is a relative rating, it's Ah*C=dischargeA, as Ah decreases, C stays the same, dischargeA decreases
```

---
## \#11 Posted by: saul Posted at: 2017-12-07T08:40:37.650Z Reads: 108

```
[quote="scepterr, post:10, topic:40352, full:true"]
C is a relative rating, it's Ah*C=dischargeA, as Ah decreases, C stays the same, dischargeA decreases
[/quote]

I get what you're saying,
but C ratings are defined for Nominal Voltage. which means they hold for the full charge cycle.
you do get Less power as voltage drops, but you can still produce the same amount of Amps.

apply your math to an old 18650 ( you obviously have plenty of those laying around)
do it for science, I wouldn't mind being proved wrong. but I don't think I am...
```

---
## \#12 Posted by: scepterr Posted at: 2017-12-07T08:46:41.613Z Reads: 102

```
I use 3s 5ah 60c lipos for my Arduino spot welder and it needs at least 200-250amps, I can't draw that through the whole capacity of the battery, even at bursts I can use around 1-5ah before it's noticably warm and at 2-2.5ah it's pretty hot
```

---
## \#13 Posted by: pat.speed Posted at: 2017-12-07T08:49:33.811Z Reads: 92

```
I think @scepterr is right. I don't know for sure and haven't done any testing but it makes sense what he is saying. Correct me if I'm wrong but as you drain your battery it will have less and less amps in it. So let's say around 50% charge it will only have about 4amps left so 4*30= 120amps output
```

---
## \#14 Posted by: saul Posted at: 2017-12-07T08:54:59.446Z Reads: 92

```
ok but a spot welder is about as opposite as you can get from an esk8.

For a spot welder you need high impulse bursts on power.
for an esk8, its much more gradual thanks to the current limited of the esc...

also 12v vs 36v.

C = Capacity, and lets say k = Current charged state
It seems like you are making  C = k, but they are not at all the same.
C is constant. 
k changes as you use (charge/discharge) the cells. 


this is off topic.
----------

@Proxy the cells will work.
but you can get lower C rating because 8ah x 30c = 240A. 
you really only need 60A(even 30A works..slowly) for a great board with that kv. 
so even 8ah x 10c = 80A is plenty.
And I know this from experience, not theory.
```

---
## \#15 Posted by: PXSS Posted at: 2017-12-07T14:48:59.368Z Reads: 86

```
C rating is not relative...

The C-rating is purely based on time. A 1C discharge means you discharge your battery capacity at a constant current in exactly 1 hour. 

A 10C discharge means you discharge your battery capacity at a constant current in exactly 6 minutes. 

A 30C discharge means you discharge your battery capacity at a constant current in exactly 2 minutes. 

The reason your cells are heating up is because most of the numbers are over spec'd on hobby grade batteries. They can do 250A provided you have enough airflow to keep them cool.

Remember that these batteries were made for competitive RC flying, where the batteries are usually mounted where they get a ton of airflow. 

I have seen a guy fly a 4Ah battery from full to empty in under 1minute. That meant discharging at over 60C for the entire flight, drawing upwards of 300A during bursts. The guys that fly quadcopters competitively constantly see these values but they go tgrough batteries like there is no tomorrow
```

---
## \#16 Posted by: saul Posted at: 2017-12-07T16:36:46.859Z Reads: 74

```
[quote="PXSS, post:15, topic:40352"]
A 10C discharge means you discharge your battery capacity at a constant current in exactly 6 minutes. 

A 30C discharge means you discharge your battery capacity at a constant current in exactly 2 minutes.
[/quote]

I never thought of it in that way! it makes more sense with drones when you are right on the edge of the battery's capability!
```

---
## \#17 Posted by: Hummie Posted at: 2017-12-07T18:39:30.806Z Reads: 66

```
i think it's all temp related and if the cells arent hitting that temp (forget what temp exactly!) its all good.  temp kills cells.   the c ratings are bunk and a guideline at best for most lipo.  with lipo i like to have access to them to see and feel their temp and if they're puffing while charging especially
```

---
## \#18 Posted by: Namasaki Posted at: 2017-12-08T01:14:20.846Z Reads: 49

```
My battery is 10s, 5ah, 60/120C and I still get a little voltage sag but no overheating and no swelling after a year of use.
Before that I used 5ah 25C 12s battery and they saged more and got warm and started swelling after a few rides.
I say get the highest C rating you can find.
And multiplying the C rating with the capacity does not give a true discharge current.
In my opinion there's no such thing as overkill when it comes to the battery.
It's always better to have more battery than you need.
```

---
## \#19 Posted by: Proxy Posted at: 2017-12-08T01:33:01.009Z Reads: 45

```
Also i read that "The C Rating is simply a measure of how fast the battery can be discharged safely and without harming the battery". So it being a little bit higher should be good coverage?
```

---
## \#20 Posted by: squishy654 Posted at: 2017-12-08T17:18:57.188Z Reads: 33

```
C rating is the measured internal resistance of the battery itself, it matters a lot and can be be measured. Most documented C ratings are just that, only documented #'s.  You want more amps, put in more amps for your X c-rating to multiply and go further too...
```

---
