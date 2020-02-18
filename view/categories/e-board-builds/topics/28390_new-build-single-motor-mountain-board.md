# New Build: Single Motor Mountain Board

### Replies: 19 Views: 2088

## \#1 Posted by: eTrader Posted at: 2017-07-23T19:01:40.230Z Reads: 260

```
This is my first build and my first post. My car broke down and I dont have the money to buy a new one so Im going to try and build a mountain board for commuting to work.I wanna keep the project around 1000$ I want to make sure all my parts are compatible before purchasing and want to make sure the board meets my requirements. 

My requirements:
 Top speed at or exceeding 30km/h
Minimum range 20km 

The Build
Board: 
MBS Colt 90X Mountainboard
https://www.amazon.com/gp/product/B0157CSIAY/ref=ox_sc_mini_detail?ie=UTF8&psc=1&smid=A39X64M46X4IIK

Motor Mount:
custom made

Belt and pully:
3M Pitch Nema23 Stepper Motor Timing Pulley Wheel, Axis Bore & Belt Set, Ratio 6:1 Reducer For DIY CNC Machine
https://www.aliexpress.com/item/3M-Pitch-Nema23-Stepper-Motor-Timing-Pulley-Wheel-Axis-Bore-Belt-Set-Ratio-6-1-Reducer/2052935069.html?spm=2114.search0304.4.18.wYaoNq

Battery: 2 in series 2 in parallel to make 12s2p
Turnigy Heavy Duty 5000mAh 3S 60C Lipo Pack w/5.5mm Connectors
https://hobbyking.com/en_us/turnigy-heavy-duty-5000mah-3s-60c-lipo-pack-w-5-5mm-connectors.html?___store=en_us


Vesc:
TORQUE ESC VESC ® BLDC Electronic Speed Controller
diy-electric-skateboard-kits-parts/vesc-the-best-electric-skateboard-esc/

Motor:
Electric Skateboard Motor 6355 190KV
diy-electric-skateboard-kits-parts/electric-skateboard-motor-6355-190kv/

Remote:
TorqueBoards 2.4ghz Nano Remote Controller
diy-electric-skateboard-kits-parts/torqueboards-2-4ghz-nano-remote-controller/

BMS:
Battery Management System (Battery BMS/PCM) for 12 Cells in series 44.4V Li-ion/Li-Polymer Battery Packs
http://bestechpower.com/444v12spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html

Charger:
43.2V 44V 50.4V 4A Lithium ion LiPO Battery Charger 12S 12x 3.6V
http://www.batterysupports.com/432v-44v-504v-4a-lithium-ion-lipo-battery-charger-12s-12x-36v-p-167.html

Switch:
ON/OFF Black Metal Shell with Blue LED Suitable for 19mm 3/4" Mounting Hole (Blue)
https://www.amazon.com/gp/product/B017KP67FY/ref=ox_sc_act_title_2?smid=AFILHMJZCK2VV&psc=1

Battery indicator:
DC Car Battery DC 12V 24V 36V 48V LCD Voltage Current KWh Watt Power Combo Meter
http://www.ebay.com/itm/DC-Car-Battery-DC-12V-24V-36V-48V-LCD-Voltage-Current-KWh-Watt-Power-Combo-Meter-/322598339972?var=&hash=item4b1c5c0584:m:mS_b9zui8fMxoo-3l_EWh5g

Anti Spark:
XT90-S Anti-Spark Connector (2pairs/bag)
https://hobbyking.com/en_us/xt90-s-anti-spark-connector-2pairs-bag.html
Also miscellaneous Connectors and wires.
```

---
## \#2 Posted by: jammin Posted at: 2017-07-23T19:41:03.099Z Reads: 204

```
For that mount, you'll need Caliber-style trucks:
https://calibertruckco.com/collection/#section_caliber_ii

That battery capacity tester won't work (since you're running at 12s).

And I believe that your current config (3 x 4s lipos) would make it 12s1p (with 6200mAh), if I understand correctly. That's all I can see at the moment.
```

---
## \#3 Posted by: eTrader Posted at: 2017-07-23T20:32:35.604Z Reads: 189

```
Hey thanks for taking a look! I changed the mount to custom so I can keep the original trucks,I changed the battery should I be worried about the c value? and I changed the battery display. If you have time would you mind reviewing it again?
```

---
## \#4 Posted by: MysticalDork Posted at: 2017-07-23T20:52:57.805Z Reads: 180

```
I think you need to rethink your belt and pulley selection. the ratio will result in a top speed of 67km/h. You'll need something along the lines of a 70 or 80-tooth wheel pulley, which with a 15-tooth motor pulley will give you a top speed around 50-58km/h. If you can get a 90-tooth pulley, you can get that down to 45 km/h. With pulleys that large, you are going to need a long motor mount. With a long motor mount, I recommend welding it just for the added strength and rigidity that gives. I'd recommend not going below a 14 tooth pulley because there just aren't that many teeth engaged, which could result in belt slipping.

The C rating should be sufficient.

You'll also either need a loop key or an anti-spark switch, that latching button won't be able to handle the current alone.
```

---
## \#5 Posted by: eTrader Posted at: 2017-07-23T22:49:04.489Z Reads: 156

```
I updated the pulley, I'll have to bore out the motor pully to be 8 mm but other then that it looks like it will work.The new top speed with weight should be 45 km/h. I also added an anti spark xt-90 Im just not sure how to install it. I know it goes in between the battery and the vesc just not sure about wiring ? Thank you for checking it out. If you have the time would you mind reviewing it again?
```

---
## \#6 Posted by: ShutterShock Posted at: 2017-07-23T22:51:12.308Z Reads: 147

```
I would say that the C rating is a bit low, my street board has a 25C set of 4 3S batteries.
```

---
## \#7 Posted by: eTrader Posted at: 2017-07-23T23:10:45.825Z Reads: 138

```
Im struggling to find a battery configuration that offers enough mah. How much are yours? The beginners guide c rating thread said that c rating doesn't necessarily matter is that true.
```

---
## \#8 Posted by: ShutterShock Posted at: 2017-07-23T23:13:22.079Z Reads: 140

```
Yeah that can be tough, the best thing I could suggest is looking up other emtbs on here to see what batteries they used.

Mine is 4x 3S 5000mah 25c each. Optionally, you may be able to pick up a custom one from someone on the forum.

The C rating is just for how many amps you can continuously discharge, and you may be fine, but I just suggested more seeing as it is an electric mtb rather than street board, one would expect a bit more performance requirements.
```

---
## \#9 Posted by: MysticalDork Posted at: 2017-07-23T23:46:33.972Z Reads: 143

```
Here's a decent image that I stole from johnny_261 on here for how to wire all the stuff. The loop key goes where the "Breaker" is in this image. <img src="/uploads/db1493/original/2X/2/20ca6e523e92861320cf17d3c032f52e7ac84013.jpg" width="333" height="500">
You'll have to modify it somewhat to incorporate dual motors and a 12s battery, but that's relatively self-explanatory. The vescs communicate between themselves via canbus, so only one of them needs to be connected to the receiver.

Taking another look at the BMS, it appears to have an e-switch built-in, so you can probably get away without a loop key, but being paranoid, I probably would still have one just as an oh-shit last resort to disconnect the battery physically.
```

---
## \#10 Posted by: eTrader Posted at: 2017-07-24T05:49:05.066Z Reads: 116

```
I changed the battery mind checking it out?Also is the c rating additive when wired in series ? Thanks again!
```

---
## \#11 Posted by: pat.speed Posted at: 2017-07-24T10:53:56.746Z Reads: 110

```
You should change the pitch of your pulleys to 5mm I have 3mm ones on my longboard and they slip on fast acceleration and strong braking. They won't be big enough for mountain boards
```

---
## \#12 Posted by: ShutterShock Posted at: 2017-07-24T17:48:12.268Z Reads: 97

```
Yeah that looks alright.  If possible I would still try to go for a higher c rating, maybe you'd be able to wire some smaller cells together in series and parallel to get a higher mAh as well.  You'll have to look around some more and I would suggest again, viewing some other builds.

The C ratings do not stack in parallel or series, so a 10C battery is a 10C battery no matter what. That is just how the actual cells are rated individually.
```

---
## \#13 Posted by: DilatedPupils Posted at: 2017-07-24T18:02:23.840Z Reads: 93

```
Discharge rate is affected by how many cells in parallel.
```

---
## \#14 Posted by: sprocket12 Posted at: 2017-07-24T18:11:01.623Z Reads: 87

```
Not sure what your batteries are at right now, but 10,000 mAh seems a little low for the distance you want to go with an eMTB.  The pneumatic tires will decrease distance due to the downward force. Of course, you get a much better ride too

I had a regular longboard with an 8s1p 8000 mAh lipo.  It did around 13 miles with lights, traffic, people, kids, etc
```

---
## \#15 Posted by: eTrader Posted at: 2017-07-24T18:15:31.508Z Reads: 85

```
Would charging with a bms work the same if I have 2 in series and 2 in parallel?
```

---
## \#16 Posted by: eTrader Posted at: 2017-07-24T18:16:57.565Z Reads: 78

```
Thanks! I'll look around and see if I can find anything .
```

---
## \#17 Posted by: DilatedPupils Posted at: 2017-07-24T18:26:34.798Z Reads: 79

```
I would suggest a bigger motor.  6374 would be great specially you're going single.
And 5m pitch 15mm wide belt.
```

---
## \#18 Posted by: ShutterShock Posted at: 2017-07-24T18:38:37.115Z Reads: 80

```
I agree here as well, I would go with 5m pitch and 15mm.  6374, you should watch the comparison video, I have a 6355 in mine and think it will be fine but if you really want power the 6374 will have you covered.
```

---
## \#19 Posted by: ShutterShock Posted at: 2017-07-24T18:41:50.591Z Reads: 89

```
Yeah it should be the same, you wire the BMS up to the balance leads and those are not used when you wire it in series or parallel so it shouldn't matter either way.

Here's a link to my build, you can see how it has been coming together, I also have my excel sheet of parts in my latest update :slight_smile: maybe that can help you a bit.  It's a street build but it all works together.  With my battery setup, some of the calculators say about 12 miles.

http://www.electric-skateboard.builders/t/razarac-quick-and-blue/26430/6?u=shuttershock
```

---
