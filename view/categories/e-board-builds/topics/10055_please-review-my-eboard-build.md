# Please review my eboard build

### Replies: 9 Views: 1109

## \#1 Posted by: Keln18 Posted at: 2016-09-24T00:40:43.035Z Reads: 143

```
Hello, Im currently in the R&D phase of my first electronic longboard and have just finalised the parts i want to use. However, Id like to run them by you experienced fellows before I go ahead and purchase them as it is a lot of money and i want to get it right. So the parts i am hoping to get are:

Motor: Enertion Rspec 2.0 6355 190kv 2400W motor
ESC: VESC from enertion
Battery: 2 5200mAh 4s Lipos to create an 8s setup
Gears: 14-16 tooth htd5 pulley, 32-36 tooth htd5 pulley and a neoprene belt
Controller: GT2B controller as it seems to be the safest and most reliable

I have experience with electronics from building a quadcopter and can ride a longboard decently(already own one that id like to convert, wheels are 70mm), so I would like some speed (at least 20mph) with good torque too (I weigh around 140lb/65kg)
I'm hoping my above setup can provide this, if you notice anything that wont work together please let me know, or if you have any suggestions. Thank you for your help!
```

---
## \#2 Posted by: lox897 Posted at: 2016-09-24T01:45:05.345Z Reads: 127

```
Looks good! Maybe go 10S with a 190kv motor though because it will go faster.
```

---
## \#3 Posted by: saul Posted at: 2016-09-24T03:31:41.450Z Reads: 123

```
8s should still get about 20...
are those 5200mah packs the multistar 10c? you might want a higher c pack. I have them on 12s but with 8s don't think they will give enough power.

also I would grab one of these motors before the price goes up. similar to rspec, 190kv, sensored. $40 cheaper!
http://www.electric-skateboard.builders/t/6354-6374-stealth-motor-group-buy-part-2-rotating-light-rocket/8828/
```

---
## \#4 Posted by: evoheyax Posted at: 2016-09-24T03:46:00.968Z Reads: 108

```
Seems good. If you want a smaller remote than the gt2b, I would recommend the one from torqueboards. That remote is the one I'm using now, it's solid, really good throttle range, and no calibration or settings need to be changed on the vesc.

10s or 12s would be better if your going with a single drive. my first build was basically this with a 6s instead of 8s, and my top speed in the real world was about 18 mph if I was on a slight downhill, 15 mph on flat, and 1o mph or less if climbing. I am also almost 200 pounds, so your top speeds will likely be a bit higher. But the higher the voltage, the less amps you draw from your battery, which also means your vesc will stay cooler and you'll get a higher top speed. Liion batteries also last 4x+ as long as lipos, are much safer, and from my experience, a bit more durable. They may be a bit more expensive up front, but they are cheaper in the long run. 5.2 Ah is also on the lower side. at 8s, that's 174 Wh. Idk the range your looking for, but I don't like to go less than 400 Wh personally, and I'm running a 504 Wh 12s4p right now, which I think is a really nice size battery.
```

---
## \#5 Posted by: Namasaki Posted at: 2016-09-24T03:48:18.422Z Reads: 95

```
I would also recommend going 10s with 190kv motor. Its a sweet combination.
2 5s Lipos in series 5000mah would give you about 10mi range
The higher the C rating, the better. Less voltage sag, more range
http://www.hobbyking.com/hobbyking/store/__9175__Turnigy_5000mAh_5S_25C_Lipo_Pack.html
http://www.hobbyking.com/hobbyking/store/__9517__Turnigy_5000mAh_5S_30C_Lipo_Pack.html
```

---
## \#6 Posted by: Keln18 Posted at: 2016-09-26T19:32:11.251Z Reads: 61

```
Thanks for the reply guys, all info taken on board. However, I am trying to keep cost to a minimum and I already have a 4s battery from my quadcopter (only used a few times) so if i went with 8s id only have to buy one more 4s lipo, as opposed to going 10s and having to buy two 5s. Is there any way of getting over 20mph on flat with decent torque for hills using 8s with a 190kv motor? Iv used 3 different online calculators and im getting anywhere between 16 and 29 mph top speed when i input my desired parts (190kv, 8s, 70mm wheels and 16-32 gearing). Theres obviously a big difference there so im still slightly hesitant to go ahead and buy the parts ..

Also if i go 8s i will have 10400 mAh in my lipos fully charged as they are two 5200 mAh
```

---
## \#7 Posted by: Catchmeifucan Posted at: 2016-09-28T18:10:13.191Z Reads: 48

```
Hi Evoheyax,
Does that mean you have chosen the Battery;
Lithium ion mnc  (Lithium Magnesium Nickel )?
Would you say that you are getting a massive 50km range?
```

---
## \#8 Posted by: sl33py Posted at: 2016-09-28T18:21:29.947Z Reads: 45

```
You are missing the point a bit here regarding batteries.

your existing quadcopter 4s battery (Multistar? 4s 5200mAh 10c) will have problems providing the amps needed for an esk8.  As @Namasaki said you want a higher C battery.  Your 10c 5.2Ah multistar (or similar) will only provide a constant amps of (10c * 5.2Ah) = 52a - and that's what they *claim* for that pack.  **Not what you will get, and _not what your motor will need to move you down the road_.**

You will either have poor performance (unable to provide amps needed), or damage the batteries, or likely both.

I would keep them for your quadcopter, and get some correctly sized lipos dedicated to esk8.  My *minimum* recommended is 100a capability (so 5000mAh/5Ah packs w/ 20c rating at the least).  The more capable they are the less the voltage will sag under load... better range, bettery pack life, better all around. 

You have nearly a duplicate thread - so look at the other one on gearing and wheel size.  Your 70mm wheels likely will not work with a regular wheel gear (most setup for Flywheels or Kegels).  Drilling and bolting will work, but 70mm is small and you won't have much if any ground clearance depending on #t of the pulley.

GL!
```

---
## \#9 Posted by: Carvin_Ginger Posted at: 2016-09-28T18:27:30.070Z Reads: 43

```
Get the warranty on the VESC! Or get a Ollin board co. VESC.  Ollin includes free repairs for a year and repairs at cost from then on.

Well worth the investment/headache.
```

---
