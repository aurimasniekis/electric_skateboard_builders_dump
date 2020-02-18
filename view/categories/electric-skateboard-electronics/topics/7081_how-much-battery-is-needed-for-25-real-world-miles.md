# How much battery is needed for 25+ real world miles?

### Replies: 58 Views: 3271

## \#1 Posted by: smurf Posted at: 2016-08-03T18:27:13.514Z Reads: 345

```
I want to make a battery pack out of 18650's like 10s5p will make it bigger up to 8p to get the range I want.
how much battery is needed for 25+ real world miles?
```

---
## \#2 Posted by: Jinra Posted at: 2016-08-03T18:31:46.204Z Reads: 341

```
General rule of thumb is 10wh per km, on flats. Hills and air resistance will heavily affect the range you're able to output on your pack. 10s5p should get you 28 miles on flats. Drastically lower if you go up a bunch of hills or face a lot of air resistance/bad roads.
```

---
## \#3 Posted by: PLEB Posted at: 2016-08-03T18:44:21.547Z Reads: 339

```
I thought it was 1,000mAh is about one mile.
```

---
## \#4 Posted by: Jinra Posted at: 2016-08-03T18:47:35.583Z Reads: 336

```
no, that doesn't include working voltage which is just as important for range estimation. You compare with watt hours, which is amperage multiplied by nominal voltage.
```

---
## \#5 Posted by: chaka Posted at: 2016-08-03T18:50:29.443Z Reads: 330

```
In my own experience you want to have at least 60 cells in a pack made of 18650's regardless of discharge rating. Anything smaller will die an early death and be a waste of investment. A year ago people thought this was ridicules but we are starting to see smaller packs die sooner than expected. Heat is the killer and larger packs just don't get as hot as when pushed hard.
```

---
## \#6 Posted by: Kaly Posted at: 2016-08-03T18:50:45.439Z Reads: 320

```
What's the capacity of the cell you'll use ?
```

---
## \#7 Posted by: willpark16 Posted at: 2016-08-03T18:51:42.375Z Reads: 313

```
true however the possibilty of a short or bad cell also increases
```

---
## \#8 Posted by: chaka Posted at: 2016-08-03T18:52:45.132Z Reads: 306

```
A proper pack is built with cell level fusing. :stuck_out_tongue:
```

---
## \#9 Posted by: willpark16 Posted at: 2016-08-03T18:53:21.347Z Reads: 298

```
hmm never thought bout that
```

---
## \#10 Posted by: NAF Posted at: 2016-08-03T18:54:51.740Z Reads: 292

```
[quote="Jinra, post:2, topic:7081"]
General rule of thumb is 10wh per km, on flats
[/quote]

Somehow this rule works only for belt drives. Hub motors seem to chew up a little bit more juice.
```

---
## \#11 Posted by: Jinra Posted at: 2016-08-03T18:56:18.476Z Reads: 282

```
Probalby due to the higher current needed to push hub drives to speed. If you were to be at speed 100% of the time, you'd probably see similar results.
```

---
## \#12 Posted by: Jinra Posted at: 2016-08-03T18:57:20.990Z Reads: 282

```
Time for 26650 to replace 18650's for esk8.
```

---
## \#13 Posted by: smurf Posted at: 2016-08-03T18:57:55.377Z Reads: 280

```
Is there a significant amount of energy efficiency with a single motor?
```

---
## \#14 Posted by: chaka Posted at: 2016-08-03T19:05:53.277Z Reads: 273

```
18650's have a longer track record. 26650's also die early if driven past 1C for too long. Ideally you want to cruise at 0.5C and burst no more than 2C. High discharge cells do not last long when pushed hard till DOD. They work in power tools but they are allowed to cool between driving screws etc...
```

---
## \#15 Posted by: Jinra Posted at: 2016-08-03T19:09:36.489Z Reads: 265

```
Guess we'll have to follow up with @Namasaki in a couple months to see how his pack is lasting :)
```

---
## \#16 Posted by: chaka Posted at: 2016-08-03T19:14:02.045Z Reads: 271

```
I well designed pack should last at least 3 to 4 years. At least that is my design goal.
```

---
## \#17 Posted by: longhairedboy Posted at: 2016-08-03T19:41:17.202Z Reads: 261

```
430 watt hours will do it in a typical 15/36 belt drive system street build with 83mm wheels and 190kv motors. I did it on a 12S build. As long as you're mostly on flats, you can get 25 miles while doing 15-20mph easily. I've actually achieved close to 25 miles on a 360 watt hour lipo pack while keeping it around 15mph, that was on a similar set up but at 6S with NTM 5060 270KVs.
```

---
## \#18 Posted by: Mrmoonlight Posted at: 2016-08-03T19:58:54.577Z Reads: 257

```
Depends on how/where you ride too. With hub motors you don't have nearly the resistance from the motor, so you can cruise much farther without power. On my belt drive, there are grades where I needed power to go down, whereas my hub does it at good speed without. You can also push a hub almost like a regular board if you need to increase your range.
```

---
## \#19 Posted by: Namasaki Posted at: 2016-08-03T20:09:27.522Z Reads: 252

```
I don't think I could fit 60 cells on my deck with electronics. 
I barely fit 20 26650's
```

---
## \#20 Posted by: flatsp0t Posted at: 2016-08-03T20:12:50.170Z Reads: 246

```
Then it is time to go to larger decks.

I had to built one by myself to fit 72, it is definitely very large and very heavy.
I think it is no solution for an everyday commuter, as you do not want to carry it around, but very nice for long distance driving for fun.
```

---
## \#21 Posted by: Namasaki Posted at: 2016-08-03T20:13:05.343Z Reads: 229

```
I don't know what belt system you have but my belt drive has no more drag than my hub motor system did. 
And I get rolling too fast down hills and have to ride the brakes.
```

---
## \#22 Posted by: flatsp0t Posted at: 2016-08-03T20:14:16.084Z Reads: 234

```
Maybe he needs steeper hills.

I think a 9 mm belt setup is noticeable less drag than a 12 mm setup.
```

---
## \#23 Posted by: Namasaki Posted at: 2016-08-03T20:55:51.955Z Reads: 231

```
I'm using dual 9mm belts. 10% grade, gotta use brakes
```

---
## \#24 Posted by: flatsp0t Posted at: 2016-08-03T20:57:07.417Z Reads: 230

```
That is what i am getting too, maybe he is on 12mm, or got it too tight?
```

---
## \#25 Posted by: Namasaki Posted at: 2016-08-03T20:57:12.633Z Reads: 236

```
[quote="flatsp0t, post:20, topic:7081"]
Then it is time to go to larger decks.
[/quote]
I've already got 33" wheelbase
<img src="/uploads/db1493/original/2X/a/a16a281d1dd16adcafaab7de3c1421e2e0f31df0.jpeg" width="374" height="500">
```

---
## \#26 Posted by: Jinra Posted at: 2016-08-03T21:14:23.035Z Reads: 225

```
For me, my GT with dual 15mm belts has pretty similar rolling resistance (very low) as my dual 9mm belt DIY board. However, since the width of GT belts is so wide, I have them looser as well.
```

---
## \#27 Posted by: saul Posted at: 2016-08-03T21:59:57.860Z Reads: 216

```
I've done 25+ miles in a day using 2 x 12s 5200 mah lipo packs. About 500wh total, each pack gets 10-15 miles, then I can switch back up to full speed and do it all over again!  I think I can push a few more miles, low voltage limits are still pretty high...

Swappable packs is the way to go. I can keep one in my bag or just use one pack for normal rides.

Keeps weight down, but wiring can be more complicated.
```

---
## \#28 Posted by: Stevemk14ebr Posted at: 2016-08-03T22:23:57.754Z Reads: 206

```
Two 12s packs in parallel, or two 6s in series?
```

---
## \#29 Posted by: Namasaki Posted at: 2016-08-03T23:59:38.349Z Reads: 206

```
I used to use a similar setup with a clam shell enclosure and buckle straps holding the lid on for quick access. 
I put 2  6s/5000 together to make a 12s set and I had 3 sets. 
I got 12 miles per set. Seems like I never wanted to ride more than 12 miles so it became pointless for me to have multiple sets. 
Pound for pound, Lipos certainly deliver more power than Li-ions but charging and storing them safely is a hassle.
```

---
## \#30 Posted by: chaka Posted at: 2016-08-04T00:08:07.662Z Reads: 195

```
18650's actually have a higher power density than prismatic lipo's by as much as 10 or 20 percent. Lipos generally have a higher C rating but low cycle life.
```

---
## \#31 Posted by: Stevemk14ebr Posted at: 2016-08-04T00:11:20.959Z Reads: 196

```
Would be nice if battery manufacturers made some large square cells and filled them with the same stuff in 18650's. Would be a lot more space efficient
```

---
## \#32 Posted by: Mrmoonlight Posted at: 2016-08-04T00:13:23.654Z Reads: 205

```
I have and EGO, used to have a Gen2 Evolve, and tried a Boosted too. All had a considerable amount of drag compared to my Carvon Hub. The Carvon is also the only Hub I've ever rode. So not much experience there. Haven't had the chance to try many DIY builds. 

I commute with my board, so I'm always taking the same route. On quite a few places where there are slight downhills (1%-2%) sort of grades, I still need power to keep up my speed (around 14mph or so) on my belt drive systems. On my Hub motor, I can cruise without power and go faster.
```

---
## \#33 Posted by: Jinra Posted at: 2016-08-04T00:15:53.306Z Reads: 203

```
I dont think it'd be structurally safe. The corner edges end up being failure points on the cells.
```

---
## \#34 Posted by: chaka Posted at: 2016-08-04T00:25:10.185Z Reads: 204

```
This deck has a 33-34 inch wheelbase and fits 60 to 72  cells depending on how crowded you want to get. At 60 cells the central compartment can be used for electronics alone. The board in the photo has 72 cells 8 of which needed to be placed in the central compartment. If you use 3500mah cells you can get around 930 watt hours! Isn't that efficient enough?!

This board weighed in at 22 lbs with dual motors.

<img src="/uploads/db1493/original/2X/8/89bf3ca5eef4d8ce71f0567d5d600d0ccc4a0e60.jpg" width="648" height="500">
```

---
## \#35 Posted by: Randyc1 Posted at: 2016-08-04T01:47:13.129Z Reads: 196

```
Chaka ,Do you use the Panasonic GA cells ?

And what is you pack ?S ?P ?
```

---
## \#36 Posted by: CSN Posted at: 2016-08-04T01:49:56.536Z Reads: 201

```
Drool

Chaka do you recall how many watt hours in my board? I seem to recall 800 wh or so.

If the Evolve GT with 370 wh's has an ~30 mile max range.


Doing 40 miles on mine is realistic at a semi spirited speeds.

I can't see how I could get 60 miles unless it was mostly downhill with tailwind.

Do they have some secret sauce? smaller motors?
```

---
## \#37 Posted by: Stevemk14ebr Posted at: 2016-08-04T01:49:58.571Z Reads: 201

```
Very impressive! Imagine what you could do with a large square shape though! Such large batteries are not really practical for boards with alot of flex, so even the shape of a cell becomes important. In japan they grow their watermelons in squares to save space and make them easier to stack.


http://lubbockonline.com/sites/default/files/photos/blogs/62710/square-watermellons_1.png
```

---
## \#38 Posted by: Namasaki Posted at: 2016-08-04T01:52:28.059Z Reads: 193

```
I had an ego as well. They do have a lot of drag. 
My diy dual belt drive has much less drag than the ego and feels about the same as my dual Carvon system was.
```

---
## \#39 Posted by: Randyc1 Posted at: 2016-08-04T01:56:38.849Z Reads: 191

```
The older Evolve Carbon had a 10s 6p pack ,...now they only have a 370 wh ???
```

---
## \#40 Posted by: CSN Posted at: 2016-08-04T01:57:45.737Z Reads: 193

```
Maybe I have that wrong.

I thought the new GT was 370 wh's

Anyone know?
```

---
## \#41 Posted by: chaka Posted at: 2016-08-04T02:13:14.264Z Reads: 194

```
@CSN

I think your board is about 770 watt hours. The 30 mile range of the GT is a best case scenario, light weight rider, lots of stops which allow the battery to cool, low average speed,  etc... 

@Randyc1

The board in that photo is sporting a 12s6p LGHE4 system Panasonic GA's work well in a pack this large too. MJ1's are another that have similar specs to the GA.

@Stevemk14ebr 18650's are ubiquitous and have been around for a long time so they have already been proven within a specific criteria. I am all for improvement and optimization but when it comes to investing several hundred dollars in a power source I think it is best to stick with a proven source. Tesla for instance is leading the way in battery assembly, they use 18650's and provide an 8 year warranty on their packs! Of course the empty space around the cells in a tesla pack is used for cooling fluid so a solid block of square cells may end up running much hotter than cylindrical cells.
```

---
## \#42 Posted by: NAF Posted at: 2016-08-04T02:20:23.150Z Reads: 188

```
how wide is it ?
```

---
## \#43 Posted by: Randyc1 Posted at: 2016-08-04T02:23:53.854Z Reads: 186

```
LG HE4 are 20A continuous , GA are only 10A continuous , should the pack be able to provide what the motor can handle ..70-80A ??
```

---
## \#44 Posted by: chaka Posted at: 2016-08-04T02:29:47.263Z Reads: 186

```
@NAF About 10 inches.

@Randyc1 you can actually use recycled laptop cells once you get into packs this large but the voltage will sag a bit more than higher discharge cells while climbing or accelerating heavily. This is from personal experience and not just speculation.
```

---
## \#45 Posted by: Mrmoonlight Posted at: 2016-08-04T04:58:02.776Z Reads: 172

```
Good to know. I should be getting an extra motor when I upgrade my Carvon to the V2.5. Was thinking of putting it on a belt drive, but like the way the single Hub feels.
```

---
## \#46 Posted by: Namasaki Posted at: 2016-08-04T05:13:41.864Z Reads: 174

```
What's amazing about the Carvon hubs is the way they feel under power. Acceleration is very positive because there's no belt flex.
```

---
## \#47 Posted by: Namasaki Posted at: 2016-08-04T05:18:49.134Z Reads: 177

```
What amount of voltage sag have you seen with the LG 18650 cells when going up steep hills?
How low would you recommend letting a li-ion pack go before charging it, 10% 20%?
```

---
## \#48 Posted by: chaka Posted at: 2016-08-04T05:37:37.223Z Reads: 180

```
You are usually safe taking cells down to 3.3v per cell under load, once you go lower heat will build quickly in your pack so it is best to go lighter on the throttle and nurse yourself home at this point to keep the pack from heating up and deteriorating.

Voltage sag is relative to the size of the pack and the resistance of the cells as well as the size of the load so it is difficult to give hard numbers that will translate to smaller packs. Needless to say the voltage sag is almost nil with 72 LGHE4 cells. It is quite impressive.
```

---
## \#49 Posted by: Namasaki Posted at: 2016-08-04T05:53:58.301Z Reads: 177

```
I was wondering about the voltage sag because with my 10s 2p with the basen 4500 near full charge and going hard up a fairly steep hill my total voltage sagged about 4 or 5 volts. I thought that was a lot but i'm not sure. Do you think that is a lot or does that sound about right for a pack this size?
```

---
## \#50 Posted by: chaka Posted at: 2016-08-04T06:41:59.301Z Reads: 194

```
That sounds about right. The easiest way to get your head around what is happening is to see that voltage sag and heat build up are linked. One important aspect of going big is the fact that voltage sag is decreased allowing us to discharge a pack more deeply before triggering a low voltage event which increases range. In theory doubling a packs size while keeping the load the same will result in more than double the range because voltage sag will be halved. Heat will also be lower so the pack will deteriorate more slowly resulting in more charge cycles before noticeable loss in capacity.
```

---
## \#51 Posted by: devin Posted at: 2016-08-04T12:08:48.170Z Reads: 189

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#52 Posted by: laurnts Posted at: 2016-08-04T13:02:51.792Z Reads: 183

```
I think at minimum 20000mah  - 25000mah on 6s lipo packs single drive belt setup.
```

---
## \#53 Posted by: anorak234 Posted at: 2016-08-04T16:38:12.303Z Reads: 176

```
That rule is more accurate with 6s. 12s 5000mah will get you much more than 5 miles
```

---
## \#54 Posted by: smurf Posted at: 2016-10-19T08:32:21.789Z Reads: 134

```
I would like to thank everybody you guys sent me down the right path of researching.
```

---
## \#55 Posted by: trbt555 Posted at: 2016-10-19T09:08:46.716Z Reads: 132

```
In my experience: yes.
I started off with a single motor setup, and later decided to add a second motor to the existing setup see what the difference was.
More uphill power, better acceleration but my range dropped noticeably, I'd say around 20-25% at least.
More strain on the batteries too.
```

---
## \#56 Posted by: smurf Posted at: 2017-06-25T02:24:00.082Z Reads: 96

```
Have you joined the 30q bandwagon or do you prefer a deferent 18650 battery for your six parallel builds?
```

---
## \#57 Posted by: mmaner Posted at: 2017-06-25T02:37:04.195Z Reads: 98

```
I have a 10s2p made with x10 2s lipos (x5 in each parallel series) that's gets 20 + miles.  I haven't actually pushed it to the limit because after 20 miles my legs are like jelly 😀.  But I think it will do 25, just guessing though.
```

---
## \#58 Posted by: chaka Posted at: 2017-06-25T14:54:48.555Z Reads: 89

```
I am on the Sanyo 20700 bandwagon right now. Our Pikes Peak edition FreeRide uses them and has 24 Ah @ 36v. 

I like LG HG2 or LG HE4 if using 18650's. It is a big jump in price to the 21700 size cell but it is worth it for the extra capacity and still be able to fit inside a 33inch wheelbase.
```

---
