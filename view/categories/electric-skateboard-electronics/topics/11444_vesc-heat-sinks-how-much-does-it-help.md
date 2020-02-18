# VESC Heat sinks - How much does it help?

### Replies: 49 Views: 4808

## \#1 Posted by: Pedrodemio Posted at: 2016-10-19T13:42:08.017Z Reads: 450

```
Hello guys, in my current build i have serious problem with over heating due to my enclosure being completely sealed and almost no air inside, very tight.

My plans for the next build is milling a heat sink that clamps to booth sides of the FETs and has the fins exposed under the board direct in the air stream. I know that the epoxy side has a poor thermal conductivity, but i think it's better than no contact with the outside

So for the people who tried heat sinks on the fets, it at least helps to get up some hills?
```

---
## \#2 Posted by: chaka Posted at: 2016-10-19T13:46:54.039Z Reads: 449

```
Heat sinks will help but it will just delay the onset if you do not have a fan to remove the heat or some passive airflow. Is this a single drive? You can also reduce your gear ratio, and top speed :sob: , but it will reduce your current consumption while climbing.
```

---
## \#3 Posted by: Pedrodemio Posted at: 2016-10-19T13:50:30.947Z Reads: 439

```
That's the idea, the fins will be outside of the enclosure, and i will also lower the gear ratio a bit, currently i'm on 2,78, just waiting for the pulleys to try 3,0, and yes, single drive, no money right now to go dual, unfortunately
```

---
## \#4 Posted by: SirDiff Posted at: 2016-10-19T13:55:55.020Z Reads: 432

```
Would something like [this](https://www.amazon.com/Gdstime-Small-Plastic-Brushless-Cooling/dp/B01DA3OFZE/ref=sr_1_9?ie=UTF8&qid=1476885278&sr=8-9&keywords=5v+fan) work?
```

---
## \#5 Posted by: chaka Posted at: 2016-10-19T14:04:21.110Z Reads: 430

```
If you can expose the fins then you should have good results.

@SirDiff Those little fans don't really push air too well. If you want results from an induction fan setup you need to run something larger off a buck converter.
```

---
## \#6 Posted by: saul Posted at: 2016-10-19T15:32:10.336Z Reads: 411

```
Might have to try this, I added a buck to power some 12v led strips but it runs hot too since 50v -> 12v. and it shares a box with my vesc....

this style fan moves more air and would work with a low profile...

https://www.amazon.com/Brushless-Fugetek-HT-07530D12-75x75x30mm-Computer/dp/B00B2ARV22/ref=sr_1_1?ie=UTF8&qid=1476891046&sr=8-1&keywords=12v+blower+fan
```

---
## \#7 Posted by: Quinlanbrown Posted at: 2016-10-19T15:46:59.057Z Reads: 393

```
After thinking of ways to cool my vesc would it work to use a pc liquid cpu cooling system for the top of the vesc and mount the back to an 1/8" peace of alumanum that's the top of my board, cause a have a corsair cpu cooler and I could replace it with a fan
```

---
## \#8 Posted by: chinzw Posted at: 2016-10-19T15:55:59.071Z Reads: 379

```
Im sorry to burst your bubble, but the heat transfer from the mosfet to the outside package  is very low, adding heatsinks will probably reduce your temps in the range of 1-3 degrees tops.
```

---
## \#9 Posted by: Mrmoonlight Posted at: 2016-10-19T16:24:43.979Z Reads: 378

```
I installed heatsinks on my mosfets and it made a substantial performance difference to me. As Chaka said, it only delays the onset, so heat eventually builds up. Wether it helps or not depends on how you ride. In my case, I have some longer hills followed by flats. Adding heatsinks enabled my board to barely make it up and everything cools off on the downhill. If the uphills were any longer, the heatsinks wouldn't be enough and I'd be pushing my way up those hills. 

Also note that different VESC's have different levels of performance.
```

---
## \#10 Posted by: chaka Posted at: 2016-10-19T16:25:40.703Z Reads: 369

```
That's why you need to use heat transfer plaster.  Sometimes you need to actually try things before spouting off. ;)

The key point is heatsinks wont lower temps unless you have some airflow. Without airflow you are simply adding more thermal mass which can help for burst currents ect..
```

---
## \#11 Posted by: chinzw Posted at: 2016-10-19T16:54:51.607Z Reads: 357

```
I'm not spouting off, its simple science. As per the mosfet datasheet, the Thermal Resistance to the case (in this mosfet it would be the underside pad) is 0.4 C/W, now the Thermal Resistance to ambien (in this mosfet that would be the package) is 40 C/W.

Adding thermal plaster will not lower that 40 C/W thermal resistance.
```

---
## \#12 Posted by: Pedrodemio Posted at: 2016-10-19T17:16:45.075Z Reads: 343

```
This 0.4 C/W would not be from the silicon die from the metal of the underside? And this 40 C/W would be from the epoxi to air, if we replace the air with a cooper mass, this value would not be much lower?
```

---
## \#13 Posted by: chaka Posted at: 2016-10-19T17:18:36.215Z Reads: 347

```
What I am saying is you are using a myopic view by siting the data sheet alone without actual experimentation i.e. "actual" science.  It has already been well documented that adding heat sinks with thermal plaster adds significantly to heat reduction.
```

---
## \#14 Posted by: IDVert3X Posted at: 2016-10-19T17:24:03.705Z Reads: 341

```
Heatsink = bigger surface to dissapate heat.
Plaster = better heat transfer between mosfet and the heatsink
```

---
## \#15 Posted by: chaka Posted at: 2016-10-19T17:25:35.409Z Reads: 339

```
You can also pack plaster into the void, bridging the gap between pcb and heat sink.

Thermal plaster is often used alone on smaller chips to provide better heat dissipation.
```

---
## \#16 Posted by: chinzw Posted at: 2016-10-19T17:26:44.792Z Reads: 343

```
So you're telling me if a stick a heatsink with thermal plaster outside my oven it will lower the internal temperature by a considerable amount? wow!
```

---
## \#17 Posted by: IDVert3X Posted at: 2016-10-19T17:33:12.731Z Reads: 346

```
No, I'm not. I'm just explaining heat transfer.
```

---
## \#18 Posted by: smurf Posted at: 2016-10-19T17:38:22.894Z Reads: 344

```
How about some kind of heat pipe and radiator  system?

http://www.myheatsinks.com/docs/galleries/home-featured/heat-pipe-assembly.jpg
```

---
## \#19 Posted by: chinzw Posted at: 2016-10-19T17:43:09.291Z Reads: 341

```
The problem is that the case epoxy doesn't have a high enough thermal conductivity to have a heatsink make a considerable difference. Lets see:

DYE --(40)--> EXPOXY --(0.3 aprox)--> (HEATSINK) ---> AIR

Now tell me, will the thermal resistance of the epoxy lower because there's a heatsink?
```

---
## \#20 Posted by: Jeff Posted at: 2016-10-19T23:00:53.247Z Reads: 331

```
To give you a real world test point, I have heat sinks on all my Ollin VESCs (the high-output package VESC from Ollin is the only speed controller I use on my builds). I weigh 225 lbs and rip up hills with no overheating issues. VESCs are in large, but sealed, enclosures.
```

---
## \#21 Posted by: chinzw Posted at: 2016-10-19T23:31:57.189Z Reads: 319

```
What are your settings? How many VESCs? There's a ton of things that will affect heating issues. I have no heating issues, and that's because i have conservative settings and good gearing ratio.
```

---
## \#22 Posted by: smudgeUK Posted at: 2016-10-19T23:52:05.961Z Reads: 318

```
Its a great idea and it would work for sure! The problem is you now need a reservoir/pump/radiator ... and you have introduced the potential for flooding your enclosures if not careful ;-)
Ive also thought about it but on a board it isnt the best solution. Using the airflow already provided makes much more sense
```

---
## \#23 Posted by: smudgeUK Posted at: 2016-10-19T23:53:07.224Z Reads: 315

```
See above :-)
```

---
## \#24 Posted by: chinzw Posted at: 2016-10-19T23:55:31.261Z Reads: 315

```
Heatpipes are not water coolers, they use gas to transfer heat away from the source quicker.
```

---
## \#25 Posted by: smudgeUK Posted at: 2016-10-19T23:57:43.418Z Reads: 314

```
Ahhh sorry my bad, i just looked at the pic and thought it was a cpu cooling system like @Quinlanbrown mentioned.
Is that a pressurised system then?
```

---
## \#26 Posted by: Jeff Posted at: 2016-10-19T23:58:05.596Z Reads: 312

```
Here is the single build (geared to 25 mph): http://www.electric-skateboard.builders/t/carbon-python-hi5ber-python-caliber-ii-s-single-6374-hi-output-vesc-12s-lipo/2208

Here is the dual build (since updated with 15mm belts, geared to ~33 mph): http://www.electric-skateboard.builders/t/street-missile-vanguard-42-flex-1-caliber-ii-s-dual-6354-dual-hi-output-vesc-10s-lipo/1886
```

---
## \#27 Posted by: Pedrodemio Posted at: 2016-10-20T00:34:25.127Z Reads: 307

```
Agreed, but i think it's the only way that it can be done, even if just delays the overheat, that's good enough, any other idea is appreciated

Things are starting to get very hot here, 41º today, so that doesn't help, in the winter I think I never had this issue

Other thing that I think it's going to help is my new batterys, the ones I'm using sag a lot, and so the current demand goes up
```

---
## \#28 Posted by: racidon Posted at: 2016-10-20T01:22:25.984Z Reads: 308

```
[quote="chinzw, post:24, topic:11444, full:true"]
Heatpipes are not water coolers, they use gas to transfer heat away from the source quicker.
[/quote]

They use liquid and gas to transfer heat from one area to another.
Which is similar to how a "water" cooled pc component works.

Would it be worth using PC water cooling? probably not.
If you used a passive system (no pump) then ultimately you're just using the exact same method (less effective mind you) then heatpipes and it would be bulkier.
The only time I would suggest water cooling is if you want your vesc in a closed area sealed off but would like heat disapation. It would allow for you place a radiator outside the enclosure without risk to the rest of the components. However if you don't understand water cooling a PC I again would advise against doing it near 35-60V of batteries and a component like the VESC.
In all honesty and practacality your best bet would be a protruding heatsink from your enclosure or with a vent that has a 1U fan sitting over it in "pull" (ensure to get one with reasonable static pressure) position like the following fans: 
<img src="/uploads/db1493/original/3X/2/a/2a9b6c1b193cfd25ca8df1e9c8764e361ca10be6.jpg" width="648" height="486">
```

---
## \#29 Posted by: Namasaki Posted at: 2016-10-20T01:54:01.550Z Reads: 284

```
I say, the heat sinks are an inexpensive add on so if they help at all, then they're worth having..
The problem with venting the enclosure is a lot of dust and dirt getting in.
```

---
## \#30 Posted by: smudgeUK Posted at: 2016-10-20T04:47:22.013Z Reads: 279

```
That picture smurf posted shows 2 pipes which are closed at both ends so there is no 'flow' of the liquids/gas ...? The heat isnt actively being removed from the area, just given a path which it can travel down to dissipate? hmmm
I think the most sensible and simple option would be to have the heatsinks protruding from the enclosure but sealed everywhere else then
```

---
## \#31 Posted by: smudgeUK Posted at: 2016-10-20T04:48:54.145Z Reads: 275

```
Has no one incorporated a simple air filter in an enclosure yet?
```

---
## \#32 Posted by: Mrmoonlight Posted at: 2016-10-20T07:33:59.259Z Reads: 272

```
I haven't checked any data sheets, but I've done quite a bit of testing with a different VESC's when it comes to heatsinks. Same ride, settings, and setup under the same conditions with different VESC's and adding heatsinks upped my performance substantially. If I were to ballpark it, I'd say it was the equivalent of raising your max temp roughly 10C.
```

---
## \#33 Posted by: chinzw Posted at: 2016-10-20T08:38:05.208Z Reads: 270

```
there is flow, the liquid gas evaporates and moves to the cooler zone and condenses. this moves the heat away from the heat source faster.
```

---
## \#34 Posted by: Pedrodemio Posted at: 2016-10-20T09:10:14.198Z Reads: 278

```
A heat pipe may make sense in a more massive setup, maybe a mountainboard, but when the vesc is so close of the outside I don't think is worth the trouble 

<img src="/uploads/db1493/original/3X/b/0/b03eccd99f699f5cc87c1ee706a15eb8f879a90e.JPG" width="690" height="425">
```

---
## \#35 Posted by: Quinlanbrown Posted at: 2016-10-20T13:21:55.702Z Reads: 266

```
yesterday i built a heat sink out of scrap aluminum i used a 1/8" pece for the bottom that was the size of the vesc and 2 strips of 1/4'' for the top and botom of the mosfets i wish i had a pic rn but im at school, i bulted it all together and it increased climbing hills alot i went up a hill that when my board was in erlyer prototype it stopped half way up but now at about 10-15mph
```

---
## \#36 Posted by: chinzw Posted at: 2016-10-20T17:39:42.065Z Reads: 254

```
Im def gonna make some measurements on this once im done with all the other work. It seems some people are running their vescs so close to the limit that 2-5 degrees actually makes a difference for some.
```

---
## \#37 Posted by: SirDiff Posted at: 2016-10-20T17:51:23.163Z Reads: 251

```
I'm really interested about this, vesc's heat is probably going to be one of my main problems on a single 6374 at 7s, even if I'm just 60kg. If anybody could do any scientific measurement that would be really appreciated!
```

---
## \#38 Posted by: smudgeUK Posted at: 2016-10-20T20:01:27.795Z Reads: 248

```
Interesting stuff ! Thanks, every day is a school day :-)
```

---
## \#39 Posted by: Quinlanbrown Posted at: 2016-10-21T18:01:45.983Z Reads: 250

```
I added a plate and didn't have airflow and it made a big change
```

---
## \#40 Posted by: sebaszz Posted at: 2017-01-01T20:38:49.075Z Reads: 241

```
Anybody i'm quite surprised mine vesc heats up so fast

This is on:
Single drive 
6374 sk3 192kv
12s
16/36 90mm
Rider 98kg, flat area

https://metr.at/r/atZJE

https://metr.at/r/cDQr7

https://metr.at/r/EtzsG
```

---
## \#41 Posted by: Ackmaniac Posted at: 2017-01-01T21:54:18.219Z Reads: 220

```
@sebaszz Well I can see that your hearing is too high for a single drive with your weight. It really depends how fast you want to go. If you want to reach around 50 km/h top speed then you should go for a 14-36 gearing.  Because I saw that you were at 76% duty cycle when you reached 50 km/h. If you would go with a 14 teeth motor pulley your heat would get much better and also the acceleration.
```

---
## \#42 Posted by: Skateman Posted at: 2017-01-01T23:02:08.430Z Reads: 224

```
Read @smudgeUK input about a simple air filter. I use an air intake with filter and an exhaust fan. My VESC seems to stay cool but I don't pull the amount of amps that a skateboard does. Designing my enclosure though, it seems like I needed to get air in and out since the enclosure would be completely sealed. Here is a couple of pics of my set up.





<img src="/uploads/db1493/original/3X/e/1/e1522c458df1fa39e5acf58063ba6d411eed91e0.JPG" width="375" height="500">


<img src="/uploads/db1493/original/3X/f/6/f6fd64cb668a40462dcc4e3d8b5ce69a5b3a5c2e.JPG" width="375" height="499">
```

---
## \#43 Posted by: sebaszz Posted at: 2017-01-03T11:27:45.896Z Reads: 208

```
thank you for your fast reply. 

that's a good idea, doesn't this cause any issues with 12mm width belt? (less surface for grip)
I originally posted this because looking only at current, temperature start to rise already quickly around 25-30A. I expected with a rating 50A continuous this shouldn't be a problem. Maybe the mistake I make is that the graph only shows batt current?
```

---
## \#44 Posted by: Ackmaniac Posted at: 2017-01-03T11:46:53.039Z Reads: 208

```
The motor current is what rises the temperature. And according to Benjamnin Vedder the standard VESC can only handle 23A contentiously. Luckily we don't drive contentiously with the same amperage. And the VESC can handle peaks up to 200A. I have a 10S with 15/36 Gearing and get temperature problems as well. I attached already Heatsinks but didn't really connect them with the correct paste or a thermal pad. I hope that the temperature will get better after i done those steps. I am also looking forward to the VESC-X as they come with big Heatsinks. Need to make some tests. And you are right. With 14 teeth you would have less surface which results in less grip. Better would be to have a bigger Wheel Pulley if the wheels are big enough. But they are not so easily available.
The easiest way to avoid the Temperature problems is to have dual drive. Never had a overheat with my dual.
```

---
## \#45 Posted by: sebaszz Posted at: 2017-01-04T23:02:56.027Z Reads: 195

```
thanx

i first try to improve the cooling and see how that works out. probably need to improve other things as well
```

---
## \#46 Posted by: Nickanzolas Posted at: 2018-07-13T13:39:50.232Z Reads: 72

```
what does everyone think about a liquid cooled heat sink so the board can still be sealed to the elements or “water resistant” not water proof
```

---
## \#47 Posted by: Kug3lis Posted at: 2018-07-13T13:45:16.649Z Reads: 73

```
I dont really see a point of warer cooling, I am running 4.5kW focbox in our case with max temp of mosfets 50ºC :)
```

---
## \#48 Posted by: FredrikHems Posted at: 2018-07-13T13:56:09.349Z Reads: 71

```
Is that 4,5kw on one focbox, or two? And is it while calculating with battery or motor amps?
```

---
## \#49 Posted by: Kug3lis Posted at: 2018-07-13T14:07:14.553Z Reads: 71

```
Single focbox in dual case I am calculating motor based on motor amps :)
```

---
