# Loaded Tesseract &#124; 12s5p VTC6 &#124; Dual TB VESC and Maytech 6355 170kv

### Replies: 21 Views: 1818

## \#1 Posted by: HummusDip Posted at: 2017-11-30T11:37:25.376Z Reads: 374

```
Hi everyone,

I had a very simple and very plug and play build running LiPos, but decided to revamp it, so here's the rundown my first proper/updated build.

**The bits (I have probably forgotten a couple of things here)**:
Deck - Loaded Tesseract
Battery Pack - 12s5p with Sony VTC6 18650s
BMS - Supower/Batterysupports 12s 30A BMS (using this for charge only, so ordered a lower discharge current rating).
Enclosure - Psychotiller's Knuckles enclosure
Trucks - Psychotiller's Ripba Dual 200mm Truck set (using half inch risers)
Motors - 2xMaytech 6355s from Psychotiller (using 12mm 16T 5mm HTD motor pulley)
Vedder Anti-Spark Switch from Psychotiller
ESC - 2xTorqueboards VESC
Wheels - ABEC11 97mm flywheels (with 36T wheel pulley from torqueboards).
Transmitter/receiver - GT2B with two corresponding receivers (using two receivers rather than CAN bus, one per VESC)

Pics of the progress so far.....

**Board with mounts/motors:**
<img src="/uploads/db1493/original/3X/7/b/7bf5cc7729900ada218f993465bf113467354905.jpg" width="372" height="500">
<img src="/uploads/db1493/original/3X/a/8/a8a3fe93b8b128adf157199581adbc8a59d00cd5.jpg" width="372" height="500">

Doggo hates it, she can remember the sound the Evolve GTX makes.
<img src="/uploads/db1493/original/3X/4/9/495eefe83615b6bd1e53642661705cbce881248e.jpg" width="372" height="500">

**Battery pack construction**

Parallel pack spot welded:
<img src="/uploads/db1493/original/3X/0/c/0cfc4faeaa2f3720558ea607c173222e3642ecae.jpg" width="670" height="500">

All connected up (lots of nickel strips stacked up on the series connections that go length-ways along the pack):
<img src="/uploads/db1493/original/3X/0/f/0f2ef04682f7d71ef3db0a8a7303786242d8e37f.jpg" width="690" height="460">

Did some insulating then folded the pack out:
<img src="/uploads/db1493/original/3X/6/f/6f4cf810648c373352fe8fbe944d0fe9e06f8e6a.jpg" width="670" height="500">

All wrapped up:
<img src="/uploads/db1493/original/3X/f/8/f8c1430837ec9c427b54146f65daa45b7c73aebe.jpg" width="372" height="500">

I've connected up the BMS and an XT90 off the battery pack and it is on its first charge as I write this, no pics of that yet.
All that's left now is attach the bits to the deck and attach the enclosure.
Big thanks to @psychotiller for answering many questions about the build!

Edit:
Had a little hassle when ordering stuff for the battery pack. Watch out for fake batteries, I got a fake bunch of HG2s from ebay (local seller in Australia and luckily they refunded quickly). Did some searching and found people on vaping forums recommending the seller Supersports600 (in Australia) who seems to do much more testing to weed out fakes. I ended up ordering my VTC6s from them and everything was good! Based on my experience, I'd recommend chatting to them if you're looking to order in Australia!
```

---
## \#2 Posted by: chrisongtj Posted at: 2017-11-30T14:22:52.513Z Reads: 305

```
Any pics of the final build?

What kind of insulation do you have between the two batteries? The middle row looks really close
```

---
## \#3 Posted by: psychotiller Posted at: 2017-11-30T14:31:33.051Z Reads: 296

```
Great job! Let me know if you needed anything else!
```

---
## \#4 Posted by: HummusDip Posted at: 2017-11-30T15:02:27.524Z Reads: 288

```
Nothing is attached to the board just yet, I'll hopefully drill and stick things to the deck tomorrow night, I'll get some pics as I go!

I did some extra polyamide tape, followed by some electrical tape. Added a layer of the little gaskets I used on the positive terminals and folded it open. I think it's enough, I did press it together after folding so there's a decent gap but yea it is a small gap. I also did some more gluing and taping after folding to try to make it a bit more rigid to reduce any movement that might wear the insulation.
```

---
## \#5 Posted by: HummusDip Posted at: 2017-11-30T15:04:09.958Z Reads: 268

```
Thanks mate! And No worries, will do :)
```

---
## \#6 Posted by: briman05 Posted at: 2017-11-30T19:19:57.084Z Reads: 255

```
That battery looks really nice awesome job
```

---
## \#7 Posted by: thisguyhere Posted at: 2017-11-30T19:37:02.832Z Reads: 249

```
lookin' good.

how's the wheel clearance?
```

---
## \#8 Posted by: HummusDip Posted at: 2017-11-30T23:51:13.557Z Reads: 245

```
If I remember I'll measure the clearance to the enclosure later, I have put half inch risers on and with 97mm wheels it should be reasonable. The deck is also pretty rigid, so that will help.
It should have better clearance than my evolve gtx, which I've bottomed out few times, in part due to the deck flex.
```

---
## \#9 Posted by: HummusDip Posted at: 2017-12-03T12:27:18.289Z Reads: 236

```
Grabbed a couple of pics:
<img src="/uploads/db1493/original/3X/c/3/c33aace1cb9fa948d6e836a73cca105acb1b971e.jpg" width="670" height="500">

Measured wheel clearance in direction of travel toward the flare and got about 70 mm (not a very accurate measurement, but gives some idea):
<img src="/uploads/db1493/original/3X/8/1/815db36325bb16acea1e65d9ea1b587a83e9683e.jpg" width="372" height="500">
```

---
## \#10 Posted by: HummusDip Posted at: 2017-12-16T23:24:02.530Z Reads: 217

```
Here are a couple of pics of the completed board (I've since added a couple more screws to the enclosure), and one of FET failure. 

FET failure happened while the board only just moving as I stood back onto it after a break. I had stopped riding for a few minutes, as I was about to get going again just getting back onto the board (had not yet used the remote), I heard a crackling noise from the board, and I turned it off straight away. I had to get picked up, since one motor was braking, so I couldn't just kick the board home (I suspected an ESC had gone and was shorting two of the motor leads somehow). When I opened it up later, it was evident one of the FETs had blown. 

Bit strange with the timing of the failure, it had been ridden fairly hard previously on the same day (testing out the acceleration/speed etc), but the riding for a good while before I stopped had been light/cruising, I had then stopped for a while and it happened while the board was barely moving as I went to stand back on it (no load from the remote, I had just stood on the board, so any motion as I got on it would generated a little current from the motor back to the VESC). I have ordered a couple of ollin escs a while back but haven't heard anything yet so I don't think they're on their way yet, but I'm sure I'll get them eventually, looking forward to having direct FETs! I passed up the recent FOCBOX deal knowing I had other good VESCs ordered, kinda wish I'd grabbed a couple now, so that I could have something in the meantime.
<img src="/uploads/db1493/original/3X/b/1/b1fa637e274c21cf735438396bff5d57c0b91911.jpg" width="375" height="500">
<img src="/uploads/db1493/original/3X/f/b/fb6c76bd6a595e61feb0e0a5b638686bafbf53e9.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/9/b/9bae53a24966bf5f162d36b8579f9d21855dd9c2.jpg" width="666" height="500">
```

---
## \#11 Posted by: willpark16 Posted at: 2017-12-17T03:23:53.905Z Reads: 197

```
That enclosure looks almost exactly like one I had made, did you make that your self?
```

---
## \#12 Posted by: HummusDip Posted at: 2017-12-17T03:36:55.792Z Reads: 187

```
I grabbed it from @psychotiller (the knuckles enclosure). Was just right for my stacked battery pack!
```

---
## \#13 Posted by: Movation Posted at: 2018-07-24T20:59:20.073Z Reads: 127

```
Great build working on a similiar one, just tested some hg2's from australian ebay seller with 99.9% positive feedback their capacity topped out at 2550mah. Out of desperation more than anything i spotted some 4ah battery packs at aldi for $22 i grabbed 6 that gave me 60 samsung 2000mah cells these will do while i sort out my ebay refund. Going to grab that enclosure
```

---
## \#14 Posted by: HummusDip Posted at: 2018-07-25T23:53:23.231Z Reads: 116

```
Yea, the one I originally bought from was highly rated at the time, I see they've dropped to 99.8% now though. Won't name names on the negative side here. Sorry to hear you got bitten too, but good that you've found a short term fix.

But on the positive side...
Once I got the refund, I bought from supersports600, sent him a message on ebay and he did me a better deal as I was buying a bit of bulk. Maybe there are cheaper genuine ones around, but I just didn't want the hassle/uncertainty, and the price was still reasonable.

Minor update on the build:
* Now have 2xFOCBOX for the VESC, because I blew a FET on the torqueboards ones. I had settings within specs, but I had been riding it hard on and off. It blew as I stood back on the board after it had been resting for about 5 minutes, which seemed a bit weird, I might have been holding the brake on as I got on, can't really remember. In order to connect to the existing motors I just changed the motor-side connectors out on the FOCBOX to the same size bullets the motors were (**for anyone considering, apparently doing this voids warranty**). 

* I got an anti-spark switch from antisparkheaven, I got the biggest one at the time, it looks like he has upgraded the product since then to handle current even better. The current I was wanting to run was too high for the old anti-spark, so I swapped in the antisparkheaven one when I put in the FOCBOXs.
```

---
## \#15 Posted by: lambievu0916 Posted at: 2018-11-19T20:56:08.375Z Reads: 76

```
Where did you get your bms?
```

---
## \#16 Posted by: lambievu0916 Posted at: 2018-11-19T20:56:31.469Z Reads: 75

```
Also! Do u have pics of how u connected the switch?
```

---
## \#17 Posted by: silaczdotoalet Posted at: 2018-11-19T21:31:22.755Z Reads: 70

```
VTC6 are one of the best cells (despite VTC5A) but have higher density of energy:)
```

---
## \#18 Posted by: HummusDip Posted at: 2018-11-21T08:32:12.371Z Reads: 64

```
It was just from ebay,  here's a pic!
It's wired only for charge, not discharge, so I didn't need higher amp.
![SmartSelect_20181121-193242_Gmail|610x500](upload://jq8UbfKRSYSUCgPIGCh0h1vBh7k.jpeg)
```

---
## \#19 Posted by: HummusDip Posted at: 2018-11-21T08:33:27.679Z Reads: 61

```
No, sorry. Might be able to take one as I just blew a focbox last weekend!
![20181118_194927|666x500](upload://45xeRxxvG6dhSdmZEn2EkgbkxHa.jpeg)
```

---
## \#20 Posted by: MannyM0E Posted at: 2018-11-21T08:42:44.967Z Reads: 56

```
😳😳 how did this happen ?
```

---
## \#21 Posted by: HummusDip Posted at: 2018-11-21T08:59:35.432Z Reads: 56

```
Board was off for maybe 5 mins, had been riding it fairly hard before, but I've done that a lot before. Was going to take off, so I started it, lifted back off ground to spin motors to check remote was connected and heard a snap, crackle, pop haha!
```

---
