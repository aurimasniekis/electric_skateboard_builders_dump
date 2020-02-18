# Final recommendations for first build

### Replies: 26 Views: 1747

## \#1 Posted by: ArsenalMain Posted at: 2018-02-08T00:44:57.888Z Reads: 155

```
Hello,  while my account my not reflect it, I have been scouring this site for the past couple weeks, gradually learning about all the different components and parts. At this point, I think that I have figured out what I plan to order and wanted to check with the community to see if you guys had any final recommendations on my parts and if I should change/add anything. Here it goes: 
Turnigy Aerodrive SK3 - 6374-192KV Brushless Outrunner Motor
https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-192kv-brushless-outrunner-motor.html?___store=en_us
2x Zippy Flightmax 8000mAh 5s1p 30c with XT90 in series
https://hobbyking.com/en_us/zippy-flightmax-8000mah-5s1p-30c-xt90.html?___store=en_us
10s HCX-D223V1 BMS
http://www.electric-skateboard.builders/uploads/db1493/original/3X/d/0/d01297cebb990b052debcf541833fb57342cbbba.png

36V 4AMP Luna Mini Charger
https://lunacycle.com/36v-4amp-luna-mini-charger/

DIY Torque VESC
collections/featured-items/products/torque-esc-vesc-bldc-electronic-speed-controller
Miami Beach Benchwheel Controller
https://miamielectricboards.com/shop-1/handheld-electric-remote

DIY Single Drive Mechanical Motor Kit 
collections/featured-items/products/single-motor-mechanical-kit

In addition to these main parts i will also be getting (But not linking)
10AWG Battery Series Connector
XT90-S Anti-Spark Connector
Voltage Monitor
SPDT Switch
5s Battery Wire Balance Extender
XT90 Female-Wire
XT90 Male-wire
XT60 Connectors
12AWG Black Wire
12AWG Red Wire
 
Am i forgetting any important miscellaneous items or is there anything that you would advise me differently?

Thank you for reading this post and I appreciate all the help that you guys, the community, offers for us new builders. I really makes our introduction to electric boards and first build attempts much smoother.
```

---
## \#2 Posted by: MysticalDork Posted at: 2018-02-08T01:44:20.108Z Reads: 120

```
A good soldering iron and solder, heat shrink tubing, a deck, and an enclosure.
```

---
## \#3 Posted by: ArsenalMain Posted at: 2018-02-08T01:46:17.781Z Reads: 120

```
I have a soldering iron from a previous project. Im using using a board I already own, and I was thinking that I would just start with some plastic sealed food containers. And I totally forgot about heat shrink tubing. 
Quick question, what strength thread locker would you recommend?
```

---
## \#4 Posted by: mmaner Posted at: 2018-02-08T01:47:54.047Z Reads: 117

```
Blue loktite is all you need. Look at home Depot and Lowe's for plant trays.  They are typically stronger than tackle boxes and cheaper & better sized.
```

---
## \#5 Posted by: ZackoryCramer Posted at: 2018-02-08T01:50:49.415Z Reads: 111

```
If you are using 5 or 4 M screws. DONOT BUY red loktite. They will NOT come off. I learned it the hard way 😒
```

---
## \#6 Posted by: MysticalDork Posted at: 2018-02-08T01:51:32.556Z Reads: 106

```
Make sure your iron has enough power to solder 12awg wire - that's more than most radio shack pencil style irons can easily handle.
```

---
## \#7 Posted by: richardx Posted at: 2018-02-08T02:01:04.532Z Reads: 106

```
[This](https://www.amazon.com/X-Tronic-3020-XTS-Digital-Display-Soldering/dp/B01DGZFSNE) is the soldering iron that I got for higher wattage. I also have a 200W Weller soldering gun. 

You also might want to consider five of [these batteries](https://hobbyking.com/en_us/turnigy-5000mah-2s-7-4v-60c-hardcase-pack.html) instead of two of the Zippy packs for a thinner form factor and less voltage sag.
```

---
## \#8 Posted by: ArsenalMain Posted at: 2018-02-08T02:12:24.963Z Reads: 99

```
Does the batteries you recommended have less voltage sag because of the 300a discharge capability? Because the two zippy ones I have on the list can handle 240. Or am I missing the reason why. And ya I could definitely do that, put the 5 in series like @Namasaki did in his build.  How much more would you recommend that over tmy current batteries
```

---
## \#9 Posted by: ArsenalMain Posted at: 2018-02-08T02:14:03.991Z Reads: 102

```
Also, I was thinking about changing the motor to the diy sensored 6374 190kv motor. This is because I don't know if the motor I chose has a keyway and I don't know how to make one. Nt hold up is that it is ~1000w less power and cost 40 more. What do you guys think?
```

---
## \#10 Posted by: MysticalDork Posted at: 2018-02-08T02:20:13.790Z Reads: 98

```
Check out @scepterr's dark matter motors.
```

---
## \#11 Posted by: Namasaki Posted at: 2018-02-08T02:37:23.477Z Reads: 97

```
First of all you need to understand that multiplying the capacity and the C rating does not give a true current capability with Lipos.
I was not aware of this at the time I posted my Lipo build.
My 5ah 60C batteries can in no wise handle 300a
Neither can Zippy's 8ah 30C batteries handle 240a
And 5ah 20C batteries will in no wise handle 100a
Still Lipos with higher C rating are better than Lipos with lower C ratings.
And I do get a some voltage sag with my 5ah 60C Lipos when climbing steep hills, maybe 1-1.5v off total 10s voltage but when accelerating on flats the sag is only about 0.5 volts off the total 10s voltage. 

SMC is the only company I know of that states true current capability for their Lipos

![22 PM|416x111](upload://e3o4egTYKnEPV2cBiAR1Kz1qqMm.png)
https://www.smc-racing.net/index.php?route=product/product&path=67_119&product_id=467
```

---
## \#12 Posted by: richardx Posted at: 2018-02-08T02:37:51.298Z Reads: 91

```
Yeah, that's why I got those batteries. I also heard that the Turnigy cells are more reliable than the Zippys. 

The SK3 6374 doesn't have a keyway. You have to grind flat spots into the shaft to get the pulley to hold.
```

---
## \#13 Posted by: ArsenalMain Posted at: 2018-02-08T03:23:32.080Z Reads: 84

```
I just checked my soldering iron, it is 110v, 60w with a temp range from 200-450c. Is this good enough for the 10 and 12awg wires?
```

---
## \#14 Posted by: ArsenalMain Posted at: 2018-02-08T03:26:55.380Z Reads: 85

```
My only hold up with those batteries is that the capacity is only 5Ah instead of 8Ah. Do you think the weight difference and lesser volt sag is worth the smaller capacity?
```

---
## \#15 Posted by: richardx Posted at: 2018-02-08T04:03:21.264Z Reads: 82

```
I'm not sure... 60W is probably passable but it'll be a little difficult. I doubt it's that much worse than the 75W one that I recommended.
```

---
## \#16 Posted by: richardx Posted at: 2018-02-08T04:03:35.131Z Reads: 79

```
How much range do you want/need?
```

---
## \#17 Posted by: ArsenalMain Posted at: 2018-02-08T04:12:08.246Z Reads: 77

```
I was hoping for around 30mph top speed and 15 mile range.
```

---
## \#18 Posted by: ZackoryCramer Posted at: 2018-02-08T04:13:48.774Z Reads: 72

```
250wh :ok_hand:
```

---
## \#19 Posted by: ArsenalMain Posted at: 2018-02-08T04:17:01.228Z Reads: 71

```
Im sorry, what do you mean by this? Im confused
```

---
## \#20 Posted by: ZackoryCramer Posted at: 2018-02-08T04:27:40.307Z Reads: 75

```
You should put together a battery pack with around 250 watt-hours, a unit of energy calculated by multiplying amp-hours and voltage. Or less technically do [mah] / 1000 * [# of cells in series] * 3.7 Judging from your 8ah 10s1p setup (296wh), you should get more than 15 miles.

This is estimated from my experience, I usually get a wh-to-mile efficiency of 13wh/mi at 17mph. Your results may vary depending on your weight, terrain, turbulence, and setup. So I assumed 16wh/mi for you. 

And since you are using 30c lipos for energy reservoir your speed should only be bottle-necked by your Esc(Vesc hopefully), motor, and mechanical setup. :grinning:
```

---
## \#21 Posted by: gee Posted at: 2018-02-08T04:32:28.515Z Reads: 68

```
get yourself some bms man. just trust me on that. save you a lot of plugging and unplugging.
```

---
## \#22 Posted by: ArsenalMain Posted at: 2018-02-08T04:36:46.407Z Reads: 65

```
ya, im actually getting the DIY vesc, sensored motor, and single motor mechanical kit. And I was curious because @richardx was recommending the 5x 2s 5Ah batteries instead of the current 2x 5s 8Ah batteries  on the list. Any idea what you would choose between?
```

---
## \#23 Posted by: ArsenalMain Posted at: 2018-02-08T04:37:35.842Z Reads: 63

```
Ya, on my list above I listed this BMS:
http://www.electric-skateboard.builders/uploads/db1493/original/3X/d/0/d01297cebb990b052debcf541833fb57342cbbba.png
Im already ordering it.
```

---
## \#24 Posted by: ZackoryCramer Posted at: 2018-02-08T04:42:29.082Z Reads: 61

```
I would choose a lion setup to TBH. Have you worked with lipos before? They are really sensitive to output usage. You can easily get someone here to make a pack for you(u living in the states?). But if you insist, I would go with 5 x 2s 5ah lipos since they are thinner and can be cheaply replaced.
```

---
## \#25 Posted by: ArsenalMain Posted at: 2018-02-08T04:57:12.689Z Reads: 52

```
I was thinking about a lion settup, but I have no idea how to wire a lion setup to a bms and isnt lion alot more expensive?
```

---
## \#26 Posted by: ZackoryCramer Posted at: 2018-02-08T05:09:32.015Z Reads: 50

```
In the DIY world, Samsung 30Q 18650's are the way to go and would cost just as expensive or less for the same 296wh. But since you aren't into DIY'ing batteries packs, you can either buy one, which would cost about >$250 including BMS, or just stick with the lipo setup. Keep in mind that lipo'd only last about 200~300 cycles, or 4000 miles compared to >500 cycles for lion's(commonly referred to as 18650).
```

---
