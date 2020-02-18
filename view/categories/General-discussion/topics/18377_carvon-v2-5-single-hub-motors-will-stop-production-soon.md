# CarvOn v2.5 single hub motors will stop production soon

### Replies: 27 Views: 1923

## \#1 Posted by: scrapheap Posted at: 2017-02-28T17:58:31.000Z Reads: 250

```
Just an FYI for everyone interested in Jerry's CarvOn v2.5 single hub motors, he mentioned to me in an email that production will stop on them in 1-2 weeks. So basically beginning to middle of March, it's going to be all v3 motors for him.

Thought I'd put this topic up for people who haven't heard yet.
```

---
## \#2 Posted by: makevoid Posted at: 2017-02-28T23:31:22.836Z Reads: 219

```
does this mean that also the v.2.5 dual will stop production some time soon also or just the single?

edit: I can't find them on the site anymore so probably they're out already ( I guess if I take a dual v3 I will have to limit their max rpm to not sh*t myself for the speed [high kv] lol )
```

---
## \#3 Posted by: Namasaki Posted at: 2017-03-01T01:15:01.268Z Reads: 205

```
anyone know what the KV is on the V3?
```

---
## \#4 Posted by: makevoid Posted at: 2017-03-01T01:31:32.135Z Reads: 194

```
100kv according to the site

edit: @Namasaki check [the description](http://www.carvonskates.com/store/p43/CARVON_V3_Dual_Direct_Drive_Sensored_Motors._Pre-Order%2C_shipping_starts_May..html)


edit2: pretty crazy, calculator gives me [~40mph theoretical max at 10s](http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":10,"motor-kv":100,"system-efficiency":80,"motor-pulley-teeth":1,"wheel-pulley-teeth":1,"wheel-size":90}|) lol
```

---
## \#5 Posted by: Namasaki Posted at: 2017-03-01T01:45:00.100Z Reads: 187

```
I don't pay much mind to speed calculators. Seems they are never accurate.
My dual Carvon 2.0 hubs where 145kv and with 12s and TB 120a esc's I only got up to 33mph on 90mm wheels.
that was on a short straight away though. Still, I don't think I could have gotten 40mph unless I was 140 lbs.
Or, maybe if I had set them up with dual Vesc's. I truly believe that the Vesc is more efficient than other esc's.
```

---
## \#6 Posted by: Michaelinvegas Posted at: 2017-03-01T02:44:03.297Z Reads: 175

```
I've tried @ekitesurfer dual 2.5 at 10s .... the thing is a beast .... 30mph+ is non issue and the touque is amazing
```

---
## \#7 Posted by: Namasaki Posted at: 2017-03-01T02:49:15.501Z Reads: 173

```
I think the trick is pairing them up with Vesc's. I never tried that and its probably a good thing cuz I may have wound up in the hospital!!
I seldom go over 20mph anymore. I'm just getting too old for that crazy stuff.
```

---
## \#8 Posted by: evoheyax Posted at: 2017-03-01T04:22:59.174Z Reads: 164

```
[quote="Namasaki, post:5, topic:18377"]
My dual Carvon 2.0 hubs where 145kv and with 12s and TB 120a esc's I only got up to 33mph on 90mm wheels.
[/quote]


With my v2s at 12s with vescs in foc, I got up to 38 mph before letting off, but at 30-40 mph, it has hella torque. I think 50 mph is totally possible, and is what I'm aiming for when Jerry sends me back my 4wd v2's :P
```

---
## \#9 Posted by: Namasaki Posted at: 2017-03-01T06:17:35.674Z Reads: 143

```
That is very impressive.  And it's all  fine for the young and restless, born to be wild and life in the fast lane.
As for me, I'm happy just going 20 mph. 
The one time I did go over 30 it was too scary :fearful:
```

---
## \#10 Posted by: Snow4us Posted at: 2017-03-10T17:40:06.487Z Reads: 121

```
Hey Namasaki,

I doubt this is the thread for my question, but your posts have been a big help as I begin to think about building my own setup.  I'm converting an old drop through low profile board and am thinking of separating out my old Multirotor Lipos for low profile and using CarvOns v3 hub motors.  1st question, do you think if I run my two 6600 4s in serial to make a 13,200 8s with a discharge of 35c and burst of 70c it would be enough to get me around 18+ miles of range and 20+mph?  completely new to this hobby and trying to figure out what's needed to achieve my goals of not spending much money and making a board that I can use to efficiently commute to my job at a summer mountain biking resort (about 7 miles of gradual uphill and 1/2 mile of steeper 7%+ at the end of the commute.
```

---
## \#11 Posted by: Namasaki Posted at: 2017-03-10T18:54:24.377Z Reads: 116

```
I would highly recommend adding a 3rd battery and making it 12s which will give you more torque, more speed and more range. The V3's are 100kv motors without any gear reduction so higher voltage is a definite plus.
My V2 where 145kv and I ran them at 12s. The formula for mileage with them was watt hours divided by 22 = range in miles.
in your case using 2 8s in series would double the voltage but not the capacity. 
Series doubles voltage
Parallel doubles capacity
C rating does not change whether series or parallel
4.2v x 8s = 33.6v
33.6v x 6.6ah = 221.76 watt hours
221.76wh / 22 = 10.08 miles
Add another battery in series to make 12s
4.2v x 12s =50.4v
50.4v x 6.6ah = 332.64watt hours
332.64wh / 22 = 15.12 miles.
These are theoretical numbers, actual mileage may vary.
If you are needing more mileage, you might want to consider getting the Zippy flightmax 8000/30c packs
to get 18+ miles, you're gonna need 400-440 what hours.
```

---
## \#12 Posted by: Snow4us Posted at: 2017-06-18T17:18:22.814Z Reads: 97

```
Thanks for the reply mate!  Just got my ABEC11 90mm wheels in and expecting Carvon to start ship[ping the new v3 motors any day now.  I think I'm going to take your advice and order another 6600 4s and see if that gets me the range I need. (I can always order larger capacity down the road if need be)   I did have a few more questions that I have come across while researching battery setups.

-When using lipos for multirotors my low voltage cutoff is set around 3.5v for the lowest cell.  As I understand it, going lower than ~3.3v that can ruin your battery.  I assume the same principle applies to an Eboard.  Question is, are the calculations you have provided about range based on the theoretical maximum of the battery, or do they assume a safe low voltage stop level?

-The other question I have is around charging.  Can you provide any insight as to how to charge a 12s battery?  I have a nice:  http://www.progressiverc.com/icharger-406duo.html  charger for my smaller drone lipos, but it seems that the 12s chargers are incredibly expensive.  Are there any resources you can point me to or insight you can provide about the most efficient way to charge this 12s 6.6ah setup?  Would it be best to leave the batteries separate and charge them as 3 different 4s packs?

Thanks again for your detailed response to my initial question!
```

---
## \#13 Posted by: Namasaki Posted at: 2017-06-18T20:31:54.559Z Reads: 94

```
The theoretical numbers are not including stopping at a safe low voltage.
I think that 3.4v is a good safe stopping point for most Lipos.
I have had Lipos (Venom brand) that stated right on the pack that their min voltage was 3.0v
They are ridiculously expensive and I have only seen them sold by Amazon.com
As for charging, there are 2 options that I have tried. 
**1st option:** My 12s setup was with 2 6s Lipos in series. I used 5.5 bullet connectors that made it easy to connect them in series or parallel and to disconnect them for charging on my dual bank hobby charger. I used a quick access enclosure to be able to remove the batteries for charing.
<img src="/uploads/db1493/original/3X/2/c/2ce4949d57a22748fd114616c076a8bdc24d8090.JPG" width="375" height="500">
<img src="/uploads/db1493/original/3X/a/a/aa00d76d264e2c95f657ca1d895ba13e669484ad.jpeg" width="375" height="500">
<img src="/uploads/db1493/original/3X/b/c/bc022cb17de76b77561c1209eb73a67b3b40429e.jpeg" width="372" height="500">

**Option 2:**
My 10s setup with 5 2s Lipos with an onboard bms and sealed enclosure for simple charging.
<img src="/uploads/db1493/original/3X/6/1/61504ccd3c14fd443c02ac734cc070037d4f7d21.png" width="280" height="500">
<img src="/uploads/db1493/original/3X/f/d/fdfa4d8c2b524b308707e39d830b0341ebb901f6.jpeg" width="666" height="500">
```

---
## \#14 Posted by: Snow4us Posted at: 2017-06-18T23:31:57.680Z Reads: 83

```
You are a legend!  thanks for the info and great pictures.  Checking out your 5 turnigy pack build now.  You got me thinking the BMS may be the way to go for simplicity's sake.  Although already having the 2 4s 6600 mah packs is a great cost savings.  Thanks for the help and info!  I will post pics when I end up building and will likely be back here with more questions!
```

---
## \#15 Posted by: Namasaki Posted at: 2017-06-19T02:02:35.979Z Reads: 80

```
those bms's are also available for 12s so you could use your existing batteries and add a 3rd one.

http://bestechpower.com/444v12spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html
```

---
## \#16 Posted by: Snow4us Posted at: 2017-08-03T22:25:32.162Z Reads: 60

```
Still waiting on my V3's :sob:

I just pulled the trigger on a 3rd battery.  Looking at the BMS you linked, I had a few questions.  Under features of the BMS, website states, "1.Protection Circuit Board for 44.4V 12S 15A Li-ion and Li-polymer battery pack"   my setup will be 50.4V, will this be an issue?  Also, the specs state over discharge protection voltage 2.3-3v, will it be possible to set the low voltage to 3.4v?
```

---
## \#17 Posted by: BigBoyToys Posted at: 2017-08-03T22:31:40.175Z Reads: 61

```
Per Jerry last week he said the V3's are closer 110KV.
```

---
## \#18 Posted by: Namasaki Posted at: 2017-08-03T23:27:36.306Z Reads: 63

```
44.4 is the nominal voltage. the charging voltage is 50.4
The over discharger voltage can be set at the factory between 2.3v and 3.0v if you want it higher, you can ask them but I don't know if they can accommodate or not.
<img src="/uploads/db1493/original/3X/4/0/403d2ac196bb8afd839d68de607d9a76d8199d34.png" width="417" height="499">
```

---
## \#19 Posted by: Snow4us Posted at: 2017-08-23T00:11:14.811Z Reads: 57

```
Thanks for the info.  I have ordered a BMS with the following settings:

Overcharge Detection Voltage: 4.28
Overcharge Release Voltage: 4.08
Over discharge Detection Voltage: 3.0
Over discharge Release Voltage: 3.0
Over Current detection current: 200A

If you would be willing to critique my build, I'm going with the following:

-3x 4S 6600mAh
-BMS (details above)
-ABEC11 90mm Flywheels
-Double V3 Carvon Hub motors w/ liquid truck
-1x Surf Rodz RKP front truck
-2x 50A Maytech VESC
-Thumb remote/ receiver from Psychotiller
-Enclosure also from Psycho
-[voltmeter](https://www.amazon.com/gp/product/B00IG1AYEW/ref=oh_aui_detailpage_o02_s00?ie=UTF8&psc=1)
-[48V 10A power Supply](https://www.amazon.com/gp/product/B01MV4249T/ref=oh_aui_detailpage_o02_s00?ie=UTF8&psc=1)
-[waterproof charging plug](https://www.amazon.com/gp/product/B01F4DTIQY/ref=oh_aui_detailpage_o02_s00?ie=UTF8&psc=1)

What do you think?  Anything I'm missing or should I be good to go?
```

---
## \#20 Posted by: Namasaki Posted at: 2017-08-23T02:53:33.228Z Reads: 53

```
The power supply you listed will not work.
It's the wrong voltage (you need 50.4v charge) and it does not have CC/CV mode
If you want to use a power supply you need something like this with adjustable voltage and current and auto switching between CC and CV modes. Or just use a brick charger.
https://www.amazon.com/gp/product/B00G0HAY3U/ref=oh_aui_detailpage_o03_s00?ie=UTF8&psc=1
```

---
## \#21 Posted by: Snow4us Posted at: 2017-08-23T03:22:27.170Z Reads: 49

```
Thanks.  I was going off of this [guide](http://www.instructables.com/id/Fast-Electric-Skateboard-LiPo-Charging-System-BMS-/).  In the 'Choosing a Power Supply' section it implies that 48V PSU will work for 12S.

Anyhow, appreciate the catch.  Not as stoked on the increased spend for a PSU.  The KORAD has a max of 5A, which would give me a charging time of just over an hour correct?

Any other blunders you notice in the part selection?
```

---
## \#22 Posted by: willpark16 Posted at: 2017-08-23T03:27:53.217Z Reads: 47

```
Faster charge time but you decrease your cells life
```

---
## \#23 Posted by: Snow4us Posted at: 2017-08-23T03:35:23.573Z Reads: 45

```
At 5A I wouldn't even be charging at 1c.  Most hobby lipos are rated to at least 1c charging and many can take much more.  I occasionally charge my multirotor lipo's at 2-3c and have 100's of cycles with little damage to the batteries.  Some of the packs I own are rated to 5c charge rate.  I like my house in its unburnt state so I would not push to 5c.
```

---
## \#24 Posted by: Namasaki Posted at: 2017-08-23T03:59:30.784Z Reads: 42

```
My batteries are also rated for 5C charge but I charge them at 1C. Fast enough for my recreational riding.
The power supply in the article you posted shows specs with CC/CV output but I didn't see that in the power supply you listed.
```

---
## \#25 Posted by: Snow4us Posted at: 2017-08-23T05:13:26.403Z Reads: 39

```
Going to get a brick charger for the time being.  As always, thanks Namasaki.  Do you suggest I put the other BMS for sale or keep as a backup?
```

---
## \#26 Posted by: Namasaki Posted at: 2017-08-23T05:18:26.118Z Reads: 40

```
I have not had one fail yet but it's never a bad idea to keep a backup. If you can afford to keep it then that is what I would recommend.
```

---
## \#27 Posted by: Snow4us Posted at: 2017-08-23T05:23:15.987Z Reads: 38

```
Copy, I will keep for the time being.  I'm sure I will be back in a few weeks when everything comes in and the build process begins. If not, pictures of the finished build to follow!
```

---
