# Opinions on schematic?

### Replies: 39 Views: 2171

## \#1 Posted by: Shiven Posted at: 2017-07-06T04:55:35.286Z Reads: 185

```
Hi there! I've been entertaining the idea of building a board and I've been trying to plan out the wiring. I made a (very crude) schematic of what I was thinking. Please let me know if it'll work or needs any improvement.

Additionally, I'm planning on having a 12s setup with a SK3 168kv motor. All XT90 connectors are going to be anti-spark also.

<img src="/uploads/db1493/original/3X/9/c/9cead5750ccfccfe25b48bc76706b8c0713b58ad.png" width="690" height="388">

New schematic based on the solutions given:

<img src="/uploads/db1493/original/3X/4/d/4d9ed6e86425006dd563d0ab6ebd03c04dbdd131.png" width="690" height="388">
```

---
## \#2 Posted by: wafflejock Posted at: 2017-07-06T05:02:56.181Z Reads: 164

```
Looks all fine to me not showing your receiver though.  Also good to keep in mind board flex and how you will hold the cables to the board, also best to keep them as short as possible from what I'm told and what I understand.
```

---
## \#3 Posted by: Shiven Posted at: 2017-07-06T05:19:23.061Z Reads: 152

```
The receiver totally slipped my mind, thank you! And yea, the wiring in the pic isn't exactly how it's going to be. Thanks for the response!
```

---
## \#4 Posted by: Namasaki Posted at: 2017-07-06T05:30:08.883Z Reads: 137

```
Those 10C multistar packs have been tried and reported as not a good option.
They're C rating is just too low making them a weak performer regardless of the high capacity.
```

---
## \#5 Posted by: Shiven Posted at: 2017-07-06T06:26:15.524Z Reads: 124

```
Oh man, really? Any recommendations?
```

---
## \#6 Posted by: pat.speed Posted at: 2017-07-06T06:44:43.435Z Reads: 121

```
I would have thought they are still decent because they can dump 100 amps which is more than the spacecell and most other li ion packs. I could be wrong tho
```

---
## \#7 Posted by: wafflejock Posted at: 2017-07-06T07:05:06.860Z Reads: 118

```
They worked okay for me for a short time but I pulled a cell too low and basically never properly recovered the pack after that (it could never fully bring that cell up to 4.2).  The amperage didn't seem to be a problem but they were also hefty and I didn't need the top speed it gives really.
```

---
## \#8 Posted by: Namasaki Posted at: 2017-07-06T15:59:04.646Z Reads: 106

```
I never tried them but people who have been on this forum longer I have, said that they are not good. 
The thing about C ratings (and this has been discussed in earlier threads) is that it is not a real number. 
And though I am a strong supporter of the use of Lipos for e-skate, I have to admit the C rating are not realistic. However, they do serve as a relative value when comparing similar Lipos to each other. 
Here is a prime example:
I use 5ah Lipos that are rated 60/120C
That's 300a continuous and 600 amp peak. 
That is just ridiculous. The main wires coming from those batteries are only rated for 75a
And when I go up a 10% grade, I still get a little voltage sag. 
So don't count on those multi rotor packs to be capable of 100a cuz you can bet they won't be anywhere near that
```

---
## \#9 Posted by: Namasaki Posted at: 2017-07-06T16:02:15.186Z Reads: 95

```
[quote="Shiven, post:5, topic:26892, full:true"]
Oh man, really? Any recommendations?
[/quote]

The Zippy flight max 8ah 30C would be a better bet
If your wanting a lot of range and power.
```

---
## \#10 Posted by: wafflejock Posted at: 2017-07-06T16:13:52.074Z Reads: 85

```
Yeah thing is I weigh like 120lbs or so and no hills here and with a 149kv motor my ammeter never showed above 20A draw even when I punch it so it still has plenty of headroom for pulling more power, that said they are huge and they probably don't dissipate heat that well especially from the cells in the center of the pack.

---

Even if the motor got the full rated power delivered at 40V to get around 2500W you'd have to be drawing about 80A I'm sure this has never happened.
```

---
## \#11 Posted by: Namasaki Posted at: 2017-07-06T16:35:51.561Z Reads: 83

```
Ok, 120lbs and flat ground won't require a lot. 
But if your 190 lbs and climbing steep hills, it's a whole different story.
```

---
## \#12 Posted by: faithfulpuppy Posted at: 2017-07-06T16:40:49.880Z Reads: 80

```
i'd put the battery meter after the circuit breaker so that it's not constantly on
```

---
## \#13 Posted by: Shiven Posted at: 2017-07-06T18:21:36.839Z Reads: 76

```
Awesome, I'll check em out! Oh, and I'm wanting to run a 12s set-up, hence the high capacity per li-po and two 6s ones, if that changes anything.
```

---
## \#14 Posted by: sl33py Posted at: 2017-07-06T19:02:02.910Z Reads: 77

```
Schematic looks good - i'd move the anti-spark XT90 to the end so it's what you plug in to power the VESC - instead of two anti-spark XT90's on each battery (though that works too, but you only need the last one you connect).  And if you connect those, then plug in the final single plug to power the ESC/VESC it will spark since the resistor to slow the inrush is bypassed when the plug is fully seated...

As for the Multistar 10Ah 10C packs - like almost all lipo's made - the C rating is usually MARKETING and should be questioned.  One of the reason i shoot for higher C packs so that the actual real-world performance is sufficient.  

The difference with li-ion vs lipo is i trust the actual tests of the 18650 cells done by Mooch and others on the candlepower and vape forums.  Heavy load tests around the 15-25+ Amps are great indicators for our use.

And on the flats and only 120lbs - i think the multistars will work fine for you.  I'd still watch out for over-discharging them, or under heavy use feel them to see if getting hot.  Inspect frequently when you charge and look for puffed cells and any that sag early.  Signs of a failing pack - stop using and charging!

GL!
```

---
## \#15 Posted by: Namasaki Posted at: 2017-07-06T20:03:19.149Z Reads: 70

```
Going higher voltage will definitely help because you will draw less amps.
The main thing as mentioned in another similar thread is to be careful to not discharge these batteries too low. 
Don't go below 3.6v per cell and if possible, you would do better to not go below 3.8v per cell.
With 12s and 10ah your max range would be apx  20 miles. 
If you can limit your ride to 15 miles it would be good.
```

---
## \#16 Posted by: Shiven Posted at: 2017-07-06T20:08:36.419Z Reads: 68

```
Duly noted! I plan on using Anti-spark connectors for all the XT-90s I use
```

---
## \#17 Posted by: Shiven Posted at: 2017-07-06T20:09:09.351Z Reads: 68

```
What do you mean when saying discharge? Like when I plug it into a balance charger or when using the board?
```

---
## \#18 Posted by: Shiven Posted at: 2017-07-06T20:10:14.666Z Reads: 70

```
Oh, i re-read the comment, thanks!
```

---
## \#19 Posted by: Namasaki Posted at: 2017-07-06T20:11:27.457Z Reads: 72

```
When using the board or draining it with a charger it would be best to not go below 3.8v per cell. 
Your battery will last a lot longer. 
Please read the edit to my last post
```

---
## \#20 Posted by: Shiven Posted at: 2017-07-09T23:42:39.934Z Reads: 66

```
well, I'm 130 and will be climbing a few hills. I got a SK3 168kv motor along with the batteries aforementioned earlier, will that work or will I have to get a different battery setup?
```

---
## \#21 Posted by: Namasaki Posted at: 2017-07-10T00:15:53.418Z Reads: 57

```
I have never tried using 10C multi rotor packs myself and have heard from old-timers on this forum that they offer weak performance.  I use 5000mah 60C batteries at 10s even with these, I experience some voltage sag when climbing hills.
At 130lbs, you might be ok with 10C packs but I can't say for sure.
```

---
## \#22 Posted by: Shiven Posted at: 2017-07-10T04:51:33.345Z Reads: 49

```
I may go for a lower capacity so I can get something that says it is 20-30C, just to be safe than sorry. Cheaper that way too. Thanks for the reply!
```

---
## \#23 Posted by: Jellybean Posted at: 2017-07-10T04:55:34.705Z Reads: 49

```
Aren't LiPos 3.7 volts per cell? So how can you only go to 3.6? Or does charging them put them over that 3.7v so 3.7v is resting?
```

---
## \#24 Posted by: Namasaki Posted at: 2017-07-10T11:28:57.121Z Reads: 49

```
Lipos and Li-ions are 4.2v per cell when fully charged. 
The voltage drops as they deplete. 
3.8v is storage voltage.
```

---
## \#25 Posted by: Namasaki Posted at: 2017-07-10T11:31:50.556Z Reads: 46

```
Check out Zippy flightmax 8000mah 30C
```

---
## \#26 Posted by: wafflejock Posted at: 2017-07-10T19:23:03.880Z Reads: 47

```
If you search around here or on manufacturers websites or in their datasheet on the various batteries you can see the voltage over the discharge for the particular cell chemistry you're working with.  Most Lithium Polymer variety of hobby RC batteries have like @Namasaki said 4.2V when fully charged and somewhere around 3.6V when fully depleted (depends on the specifics of the chemistry in the electrolyte, the anode, the cathode, and the arrangement/size of things, but general rule of thumb those numbers are correct for run of the mill RC LiPo bricks).

If you look at the discharge curves for the cells you'll see the rate of the power being dropped out of the battery depends on the amperage... meaning if you pull 10A for 1hr you'd drain more Amp-hours out of a battery than if you were drawing 5A for 2 hrs.  In theory those would be equivalent but in reality the higher drain on the battery means you end up reducing the voltage more quickly than if you have a lower current draw.  With all the lithium based stuff I've seen they have the same general characteristics to the curve though, quick drop off from 4.2 to around 3.9 then levels off to a somewhat linear voltage depletion until you hit somewhere between 3.6 and 3.3V at which point you hit a cliff and the voltage drops to near 0 pretty quickly.  If you ever have a cell go over that cliff it essentially means replacing the pack (unless you are going to do somewhat dangerous surgery on your pack and have the right solder and flux around... basically not worth it).

---

All batteries have slightly different curves but they will look something akin to below.

http://www.rctech.net/forum/attachments/electric-road/1104193d1377325541-benchmarking-best-2s-lipos-tp-extreme-5000-discharge-curve-graph.gif
```

---
## \#27 Posted by: Namasaki Posted at: 2017-07-10T20:59:02.948Z Reads: 42

```
I would like to add one observation if I may,
It did seem to me that when I compared 25C 5ah Lipos in a 12s configuration to 60C 5ah Lipos in a 10s configuration that the the 60C Lipos have a slower and more linear drop from 4.2v than the 25C Lipos. 
I am convinced that when using Lipos, the higher the C rating the better off you are. 
It's probably safe to say that drawing 30a from a 60C Lipo is like drawing 10a from a 20C Lipo
Or 5a from a 10C Lipo in terms of voltage sag.
```

---
## \#28 Posted by: Jellybean Posted at: 2017-07-11T05:03:58.958Z Reads: 40

```
Good to know. 
And thanks @wafflejock for the chart, that makes a lot more sense now
```

---
## \#29 Posted by: JdogAwesome Posted at: 2017-07-11T05:39:06.139Z Reads: 41

```
Personally im using 4x Zippy Compact 5Ah 3S Lipos for a 6S2P and they have been working very well. Personally I dont discharge past 3.7V though I have had a LiPo I accidentally took down to 2.6V a cell and brought pack without any noticeable difference in capacity, though time will tell because im sure it affected the IR of the cells. However I use to have 2x Turnigy 30-40C 5Ah 3S Lipos in series and eventually they started bulging and I replaced them with the Zippy ones when I re built my board. 

Also @Shiven please for the love of god dont use one of those "100 circuit breakers" they are TERRIBLE I use to use one and it was the worst part of my board! Either use a XT90 key loop, or a MOSFET switch. Also you dont need to use XT90 connectors XT60 are more then plenty as well as much cheaper.
```

---
## \#30 Posted by: Namasaki Posted at: 2017-07-11T05:41:04.540Z Reads: 39

```
I also tried to use one of those automotive breaker switches on my first 12s board and it did not hold up either.
The arcing between the contact points wore them out pretty fast..
```

---
## \#31 Posted by: JdogAwesome Posted at: 2017-07-11T05:43:12.465Z Reads: 39

```
I remember I was using it for a while and over time it started falling apart, a pin here and there then the entire top lid, kept fixing it. Then one day I went off a little curb and it hit the ground, it literally exploded it was hilarious, also sucked cause my board was no worky. Also the arcing was a problem had to clean the contacts once or twice though I was also only 6S and had a car ESC, nothing compared to 12S and a VESC capacitor bank.
```

---
## \#32 Posted by: Namasaki Posted at: 2017-07-11T05:46:55.743Z Reads: 41

```
believe me the spark at 12s is pretty intimidating. 
My points not only got burned up but the spring bar got weak from heating up and I started loosing connection while riding.
```

---
## \#33 Posted by: JdogAwesome Posted at: 2017-07-11T05:49:42.729Z Reads: 37

```
I see, but did yours explode? I DIDN'T THINK SO, TOPPED!
```

---
## \#34 Posted by: Namasaki Posted at: 2017-07-11T05:54:10.053Z Reads: 38

```
you got me there LoL
```

---
## \#35 Posted by: Shiven Posted at: 2017-07-11T06:09:45.180Z Reads: 44

```
No breaker switch, got it! Is there anywhere I can find a MOSFET switch for the vesc?
```

---
## \#36 Posted by: JdogAwesome Posted at: 2017-07-11T06:31:27.082Z Reads: 44

```
Yeah there's a bunch of people who sell them, including me though I'm out of stock ATM. Torque boards sells one for $60 which is a bit pricy but there's others to @goldenHusky husky sells his switch you can ask him about it or just search on this forum "Vedder anti spark switch" or "MOSFET switch" should return plenty of results.
```

---
## \#37 Posted by: wafflejock Posted at: 2017-07-11T14:21:07.983Z Reads: 42

```
Just use an antispark loop.... I don't get the "huge benefit" of one plug over two and don't think BMS is typically a good idea ( unless you're making a consumer board) more crap on the board is just more crap that will eventually shake apart or break in some other way.  If you make your own battery pack and need to put leads on their anyway it makes some sense to me but for lipos I don't get it.  Been riding with the same batteries for over a year and no corrosion of the leads ( I spray everything with corrosionx though and keep the balance leads mostly tucked into the battery enclosure)
```

---
## \#38 Posted by: Shiven Posted at: 2017-07-11T20:13:04.471Z Reads: 40

```
True. I was looking for a more elegeant solution and was planning on using this [switch](diy-electric-skateboard-kits-parts/electric-skateboard-on-off-power-switch/), but a loop would be cheaper.
```

---
## \#39 Posted by: mynamesmatt Posted at: 2018-07-02T09:00:21.800Z Reads: 19

```
cannot recommend these enough!! I run a 10S system with 2x5S 8ah FlightMax's and they run awesome!
```

---
