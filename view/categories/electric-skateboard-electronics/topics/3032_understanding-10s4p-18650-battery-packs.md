# Understanding 10s4p 18650 battery packs

### Replies: 67 Views: 24214

## \#1 Posted by: DougM Posted at: 2016-05-09T17:23:47.360Z Reads: 1178

```
I'm assuming that 10S4P above means you have 4 sets of 10 cells?  How do you tie the packs together?  Do you charge all packs and then just close your eyes and attach the wires?  Do you discharge all packs?  I would think that any voltage difference between the packs could make for some pretty dramatic correction when you connect them?

Or is it not a concern?  I ask because I just took delivery of my first set of 12 18650's for a 12S1P but I could see a 2P in my near future.

Thanks,

DougM
```

---
## \#2 Posted by: Hummie Posted at: 2016-05-09T17:31:34.368Z Reads: 1106

```
Yea u can have a spark when connecting the packs of they are slightly different voltages.  U could integrate the parallel connections within the series chain and avoid sparks that way.  I'll post a pic what I did later tonight. 

Endless sphere for sale section has the best deal on awesome 3500mah cells but they are 10amp cells so you'll need to make a bbbbiiiggg pack otherwise suffer possible lower cell cycle life and voltage sag. 
Otherwise I think the of hg2 is a great choice.  For smaller packs you'll need higher discharge cells of
Course and they're only possible in 2500mah
```

---
## \#3 Posted by: treenutter Posted at: 2016-05-09T17:47:12.480Z Reads: 1082

```
@DougM [quote="DougM, post:1, topic:3032"]
I'm assuming that 10S4P above means you have 4 sets of 10 cells?
[/quote]

Not quite; it means you have 10 sets of 4 cells wired in paralell. Then you connect those 10 sets (with 4 each) in a series to increase voltage.

[quote="DougM, post:1, topic:3032"]
I would think that any voltage difference between the packs could make for some pretty dramatic correction when you connect them?
[/quote]

Ideally the cells begin with the same voltage and the same capacity, and then a BMS balances them during charging. You can test them with a multimeter before you connect them to makes sure there are no duds and to assure that they're already close to balanced.
```

---
## \#4 Posted by: Jinra Posted at: 2016-05-09T18:31:31.430Z Reads: 999

```
What if you **did** have 4 sets of 10 cells (10 cells in series then parallel them with 3 other sets)? Would you just have a pack that can't be balanced by a BMS?
```

---
## \#5 Posted by: DougM Posted at: 2016-05-09T18:39:08.027Z Reads: 987

```
I picked up the LG HG2's since I read somewhere they were pretty solid cells.  The packaging says they are certified OEM but I'm a little suspicious because they are rated 3000mAh but when I drain tested them at 1A I got slightly less than that.  I would have expected slightly more out of a brand new cell.

Thanks for the input - it does make more sense to do it the way @treenutter describes - 4 parallel then tie those together in series.  That way the potential V delta is much much less than 12 series tied to another 12 series.  I'll do that :slight_smile: 

so far I've been balancing my LiFePo's during charge with a balance charger, which is easy since I have a few very large cells, but I guess it's time to start looking at BMS for this transition.

Thanks,

DougM
```

---
## \#6 Posted by: treenutter Posted at: 2016-05-09T18:54:00.300Z Reads: 909

```
[quote="Jinra, post:4, topic:3032"]
What if you did have 4 sets of 10 cells
[/quote]

@Jinra OK I'll take a shot at answering this, but I'm not the resident battery expert! Essentially, you'd have a 4s10p pack that has a discharge rate that is too high for our purposes. Let's say you used Samsung 25R 18650 cells. The specs are 20A(continuous),100A(burst) 3.7V, and 2500mAh.

So if you built a pack as you described above, the pack would have a continuous discharge rate of 20Ax10= 200A,  **10,000A burst rate**, a capacity of 2500mAhx4=10000mAh, and a voltage of 3.7x4 = 14.8V.

So essentially you'd have a pack designed to fry your ESC :slight_smile:
```

---
## \#7 Posted by: Jinra Posted at: 2016-05-09T19:02:31.583Z Reads: 876

```
Bit of a misunderstanding. I mean having 10 cells in **series** then putting 4 of those packs in parallel, so there would only be 1 parallel bridge.
```

---
## \#8 Posted by: lox897 Posted at: 2016-05-09T20:23:28.738Z Reads: 846

```
@treenutter He is talking about series and then parallel. Don't put cells in series first. There is a whole argument on ES on why you shouldn't, something to do with science. Parallel and then series.
```

---
## \#9 Posted by: Jinra Posted at: 2016-05-09T21:01:03.075Z Reads: 816

```
Thanks for the info :) Was just curious on what would happen.
```

---
## \#10 Posted by: DougM Posted at: 2016-05-09T21:16:25.669Z Reads: 824

```
It makes sense - the voltage differential of any 2 fully charged cells is maybe max 100mv but the voltage differential of 10 or 12 in series would be 10 or 12 times that much, so when you attach them in parallel they will try to equalize instantly, causing a lot of smoke and grief.

This is what I was trying to understand in my initial question :-)  

The only other option would be to attach the series packs via some very large resistors so they equalize more slowly.

DougM
```

---
## \#11 Posted by: Ulfberht Posted at: 2016-05-09T22:30:57.707Z Reads: 821

```
A super simple way to visualize your battery pack is to look at the parts in terms of cells. 
For a 10s4p pack, you will need 10 packs, wired in series. 4 batteries wired in parallel each pack.
So visualize your 4 battery parallel connection as one "cell". This will determine your packs overall capacity in Mah as well as the total amperage that you can safely draw from the pack. More capacity, more amps!! 
Once you have your "cell" planned out, you need to bring the overall pack voltage up to the desired level to efficiently operate your motors and ESC. Running 10s or 10x4parallel cells will give you about 36v. As long as you follow this formula, you can build any size pack at any voltage you desire. 
Have fun, but be safe too!!
```

---
## \#12 Posted by: Kaly Posted at: 2016-05-10T00:26:08.158Z Reads: 795

```
http://www.ebikeschool.com/how-to-build-a-diy-electric-bicycle-lithium-battery-from-18650-cells/
```

---
## \#13 Posted by: Ulfberht Posted at: 2016-05-10T03:05:45.729Z Reads: 790

```
Here's the best write up I've been able to get my paws on. ESK8 specific and inspiring as hell!! IMO
https://endless-sphere.com/forums/viewtopic.php?f=35&t=72026&sid=708fbd95e09b3518f8802cd57d24072d#p1088195
@whitepony Props!! Thank you very much for posting this and other threads!!
```

---
## \#14 Posted by: Racetored Posted at: 2016-11-20T20:36:43.511Z Reads: 707

```
Hey guys, I was just on here looking for some battery build tips, and I'd like to point out that this comment from treenutter :"Not quite; it means you have 10 sets of 4 cells wired in paralell. Then you connect those 10 sets (with 4 each) in a series to increase voltage"... is wrong according to Jason Potter's (onloop) site. 

Regarding the Spacecell 10s4p he states: 
The battery is 10S4P meaning it has a total of 40 Cells, 4 Parallel groups of 10 cells in series.  Samsung 25R Cells.

So now as Ali G says "I's well confused!"

10 Cells of Samsung 25r's in series (nominal voltage of 3.6 per cell at 2500 mAh) would produce a single pack of 36volts and 2500 mAh (or 2.5wh) correct?

Wiring 4 of those 10 series packs in parallel gets me 36volts and 10,000 mAh (10wh) of power, correct?

Conversely, 4 of the same cells wired in Parallel gets me a 3.6volt pack with 10,000 mAh of power. 10 in series gets me to 36volts at 10,000 mAh of power.

So my question is, is the advantage to have more packs for a BMS to manage? The more micro-managing that can be done the longer the pack lasts? 

Or am I missing an advantage in Discharge Rate? From what I've read, Samsung 25r cells have a 5c discharge rate. Thats 5 times the capacity of 2500, or 12.5 Amps. Multiply that times the number of parallel groups correct? This would be a max "c" discharge rating of 50Amps for the battery built with 4 parallel groups of 10 in series, and the same for the pack made with 10 4 cell parallel packs in series? Just remembering that cells in series increase voltage and cells in parallel increase capacity.

It seems to me there is no advantage either way? Am I missing something? I'd like to get started on a build but the conflicting information out there has me confused a bit....
```

---
## \#15 Posted by: treenutter Posted at: 2016-11-20T21:20:31.739Z Reads: 628

```
@Racetored apologies if my comment caused any confusion; I think it's a problem with "order of operations" when you read my statement. The way I read it, My comment and Jason's are the same. Let me try to break it down:

"4 cells wired in paralell:" - each one of these is 4 cells wired in paralell:
<img src="/uploads/db1493/original/3X/5/0/5052b6632edc53788fe2efcffc5fdd51717422a4.jpeg" width="500" height="500">

in a  10s4p pack you have ten of these paralell packs, lined up like this:

<img src="/uploads/db1493/original/3X/2/e/2eb3f01e435699c885732e30f9704e747fb67b20.jpeg" width="500" height="500">

...and from here you make the serial connections to bridge together all the packs:<img src="/uploads/db1493/original/3X/c/8/c869b4ff4afeefcd0b97835e9a5a3bbc4b91f49c.jpeg" width="500" height="500">

Imagine my quote with these parenthesis : 
 "...you have 10 sets of (4 cells wired in parallel). Then you connect those 10 sets (with 4 each) in a series to increase voltage"

So parallel increases capacity, series increases voltage.

In the case above (10s4p) you get 4x the capacity of the cell (2500mah) to equal 10,000mah. Then you multiply the voltage of of each pack (4.2V max) by the number of packs in the series (10) so you get 42V max.

You could also express the voltage as nominal voltage, then it would be 36V.

Hope this helps, and I'm very open to being corrected so could someone pls double-check me?
```

---
## \#16 Posted by: Racetored Posted at: 2016-11-20T22:26:58.631Z Reads: 597

```
I totally get that. Jason clearly says 10 cells in series in 4 parallel groups. After doing the math it reall seems like "half a dozen of this, six of the other." The math all seems to add up the same, I was just looking for some clarity as to if there was a benefit to one over the other. There was an earlier comment here that a pack built on 4 parallel groups of 10 cells in series would produce a battery with too high of a discharge rate. 

Btw, thanks for those great photos! Is there somewhere here with a detailed bms wiring description?
```

---
## \#17 Posted by: Racetored Posted at: 2016-11-21T05:03:46.726Z Reads: 592

```
So, just to clarify a wiring diagram...this pack would be a 10s3p, or this would be a 3s10p? From what I gather, this is the wiring diagram used in the 10s3p Spacecell. Is this right anyone? <img src="/uploads/db1493/original/3X/6/0/6099a951b7b5614520e838db303f31fe4fc93184.png" width="690" height="426">

I'd love some clarity on how to wire a BMS as well! I have a charger for my RC helicopters that has balancing functions, but I don't think it can go up to 10s.
```

---
## \#18 Posted by: Racetored Posted at: 2016-11-21T05:06:39.005Z Reads: 580

```
I just realized that the parallel connection between pack 1 and 2 is wrong ...I would just flip the arangement of the first 10 cell pack...I am aware but this is the idea...
```

---
## \#19 Posted by: lox897 Posted at: 2016-11-21T05:13:08.492Z Reads: 583

```
No, that is incorrect. 3 batteries are joined in parallel. Then make 10 of those and wire them in series.
```

---
## \#20 Posted by: lox897 Posted at: 2016-11-21T05:14:47.624Z Reads: 603

```
This is a 10s4p:
<img src="/uploads/db1493/original/3X/1/9/1981de739604e2d86da82ea20a8c3d56e60e5876.jpeg" width="690" height="175">
```

---
## \#21 Posted by: Racetored Posted at: 2016-11-21T06:19:00.780Z Reads: 595

```
Awesome thanks man. Now BMS leads go where?
```

---
## \#22 Posted by: lox897 Posted at: 2016-11-21T07:17:12.126Z Reads: 589

```
The Bs on the diagram represent the balance leads. Credit to @whitepony for the diagram
```

---
## \#23 Posted by: treenutter Posted at: 2016-11-21T14:10:53.781Z Reads: 592

```
@Racetored check out the Beautiful Diagrams thread there are diagrams of all the common battery layouts. BMS wiring is shown there as well. Note that there is variation in the way you wire BMSs, they aren't all the same (some use the same ports for charging and discharge, others don't, for example) Any BMS you buy should give you instructions.

http://www.electric-skateboard.builders/t/beautiful-diagrams-no-words-just-pics/3179
```

---
## \#24 Posted by: Hockingham Posted at: 2017-02-21T23:15:52.739Z Reads: 541

```
Hi,  I'm not sure if this is the right thread to be posting but you guys all seem battery savy, I'm a carpenter not an electrician so struggle with the workings. 

I'm thinking of making a battery pack 5s4p with these batteries :  

Panasonic NCR18650B 3.7V 3400mah Li-on Battery

- Low discharge rate, no memory effect. 
 	SPECIFICATION
Description
Capacity (Ah): 3.4 Ah
Charging Voltage (V): 4.2 V
Energy (Wh): 12.2 Wh
Energy Density (Wh/L): 730 Wh/L
Nominal Voltage (V): 3.7V
Weight (g): 45 g
Diameter (mm): 18.3 mm
Height (mm): 65 mm
Model: NCR18650B
Made in Japan
Made by Panasonic

I can get 20 of these including postage for £75

So I'm asking are their any issues using these for a build and if not does the price seem fair?
```

---
## \#25 Posted by: Pantologist Posted at: 2017-02-21T23:18:01.617Z Reads: 497

```
Bad idea. The discharge current is probably only 10A at the most. 4 in parallel is only 40A. Not enough to minimize voltage sag.
```

---
## \#26 Posted by: Hockingham Posted at: 2017-02-21T23:22:13.782Z Reads: 480

```
I don't fully understand your comment as I'm a novice on all things that spark,  
what would be your choice of battery for the job?
```

---
## \#27 Posted by: Hockingham Posted at: 2017-02-21T23:23:54.569Z Reads: 481

```
Also am I right in assuming mah is increased by reducing discharge rate?
```

---
## \#28 Posted by: Pantologist Posted at: 2017-02-21T23:56:13.418Z Reads: 474

```
As batteries hold more energy, they cannot discharge as much current. Yes that is correct.
```

---
## \#29 Posted by: Pantologist Posted at: 2017-02-21T23:57:49.551Z Reads: 454

```
Samsung 25R, LG HE4, HG2s. These are all 2500mAh+ cells with 20A discharge rates.
```

---
## \#30 Posted by: Hockingham Posted at: 2017-02-21T23:58:43.025Z Reads: 446

```
Super,  thanks for the advice.  I'm off  shopping.
```

---
## \#31 Posted by: PXSS Posted at: 2017-02-22T00:14:09.977Z Reads: 443

```
Hey. I know it's been a while since you posted this but can you link the thread on ES which says you shouldnt put cells in series and then parallel? 
I do it all the time with no ill effects.
```

---
## \#32 Posted by: Pantologist Posted at: 2017-02-22T01:00:45.246Z Reads: 435

```
How do you balance them? That is the reason.
```

---
## \#33 Posted by: PXSS Posted at: 2017-02-22T01:33:03.175Z Reads: 428

```
Same way you balance the same pack thats connected first in parallel and then in series.
Not the reason
```

---
## \#34 Posted by: Pantologist Posted at: 2017-02-22T02:21:30.437Z Reads: 443

```
Oh okay. Could it have been that if a cell went bad in a series pack, it would bring the voltage of the whole pack down, but if a cell goes bad in a parallel pack, the capacity drops, not voltage. 

http://batteryuniversity.com/learn/article/serial_and_parallel_battery_configurations

Edit: 

"A cell that develops a high resistance or opens is less critical in a parallel circuit than in series configuration, but a failing cell will reduce the total load capability. It’s like an engine only firing on three cylinders instead of on all four. "
```

---
## \#35 Posted by: PXSS Posted at: 2017-02-22T02:41:09.590Z Reads: 441

```
Nope. If a cell goes bad in a soldered/welded parallel batch, you wont realize it's bad until all of them are bad and you have to dispose of the whole batch. 

If a cell goes bad in a soldered/welded series batch, you will realize as soon as you charge as the one cell will have higher IR and its voltage will be different than the good cells. In this case you can cut out the bad cell and keep going with the others as they have not been affected. 

E: I see what they are saying. If a cell is going bad in a parallel pack, the other ones will compensate as the weak cell will match the voltage of the good cells. 
If it goes bad in a batch of series cells, then your total voltage drops and it would underpower your system. 

This is all true, but as stated above, you would quickly realize you have a bad cell in a series pack by checking voltages. You wouldn't realize it as easily in a parallel pack unless you're constantly measuring capacity.
```

---
## \#36 Posted by: Pantologist Posted at: 2017-02-22T03:01:40.884Z Reads: 422

```
I'm still curious how you plan on hooking up a BMS to it. All BMSes are wired for parallel first battery packs because it is easier to wire.

In a series format, you will overcharge the pack that contains a dead cell with the same charger voltage. You'll end up damaging the rest of the cells in the series pack before realizing.
```

---
## \#37 Posted by: willpark16 Posted at: 2017-02-22T03:03:22.566Z Reads: 414

```
Where did U get that 100 for a 10s 8ah deal
```

---
## \#38 Posted by: PXSS Posted at: 2017-02-22T03:08:23.376Z Reads: 455

```
Each series pack has a balance port. All you need is this guy to connect to bms. $8 on amazon I think. 
<img src="/uploads/db1493/original/3X/0/f/0f1797d09a2a618f2306c80a4b6adcfe5b14d007.jpg" width="375" height="500">
I would post a pic of it all connected but it's work related. 

As for charging. No, I would not blow anything up before I realized I had a bad cell. I dont charge connected straight to a brick charger (that is idiotic). If you used a BMS, it would not let you overcharge any single cell, if you use a balance charger, it shows all of your voltages like below. 
<img src="/uploads/db1493/original/3X/e/9/e96b4f4096eb13871548bf940db14401064acafe.jpg" width="375" height="500">

E: This is why I want to see the ES thread @lox897 mentioned. I want to see if there is any actual science behind it for me to learn. If it's just because doing parallel and then series is easier then I dont really care lol
```

---
## \#39 Posted by: Pantologist Posted at: 2017-02-22T03:30:14.922Z Reads: 432

```
Other than having the bad cell drops voltage vs drops capacity, I don't think there is anything else. 

This just makes the pack more complicated and harder to manufacture. When making a pack of these dangerously powerful batteries, simpler the better.
```

---
## \#40 Posted by: PXSS Posted at: 2017-02-22T03:38:58.269Z Reads: 452

```
Yeah, there are pros and cons to each method. I make all kinds of crazy packs for work (up to 10S10P Li-ion setups). I'm just looking to further my knowledge :stuck_out_tongue:
```

---
## \#41 Posted by: Pantologist Posted at: 2017-02-22T03:41:23.210Z Reads: 437

```
Haha, we are all here to learn ;)

@willpark16 They are packs of new drill batteries. Ryobi 40V packs. I got them for less than 50% of regular price from an overstock seller on craigslist. I bought him out :grin:
```

---
## \#42 Posted by: PXSS Posted at: 2017-02-22T04:06:15.102Z Reads: 442

```
Do not get 25Rs if you can avoid it. They are rated for 20A but are no better than Sanyo GA cells which are rated to 10A with respect to power output. 

I recommend Samsung 30Q cells. They can be found somewhat cheap in eu
```

---
## \#43 Posted by: lox897 Posted at: 2017-02-22T04:42:52.441Z Reads: 473

```
@PXSS I saw it here: https://endless-sphere.com/forums/viewtopic.php?f=35&t=72026 

It's at the bottom of the first page and a bit of the second page. @whitepony 's thread
```

---
## \#44 Posted by: jaykup Posted at: 2017-02-22T06:30:27.900Z Reads: 487

```
> Do not get 25Rs if you can avoid it. They are rated for 20A but are no better than Sanyo GA cells which are rated to 10A with respect to power output. 

I'm not following.

**25R vs GA**
[Samsung 25R](https://www.e-cigarette-forum.com/forum/threads/samsung-green-25r-25r5-20a-2500mah-18650-bench-retest-results-a-great-20a-battery.706485/) discharges 20A at 77C while maintaining 92% of the rated 2500mah life (2300 total)
[Sanyo NCR18650GA](https://www.e-cigarette-forum.com/forum/threads/sanyo-ncr18650ga-10a-3300mah-18650-bench-retest-results-a-great-12a-battery.774493/) discharges 20A at **113C** while maintaining only 78% rated 3300mah capacity (2600 total).

The 25R looks quite a bit better than the Sanyo?

**25R vs 30Q**
25R discharges 20A at 76C and has about 2300mah capacity
[30Q](https://www.e-cigarette-forum.com/forum/threads/samsung-30q-20a-3000mah-18650-bench-retest-results-a-great-20a-3000mah-battery.727190/) discharges 20A at 83C and has about 2550mah capacity

25R pulse discharges 50A at 80C for 14.5 min
30Q pulse discharges 50A at 84C for 16 min

So the 30Q has slightly better capacity, but runs slightly hotter and costs significantly more in the US

25R - $3.50-4.00/cell - 2300mah @ 20A - 77C - $1.74/Ah
30Q - $5.60/cell - 2550mah @ 20A - 68C - $2.19/Ah

10S4P cost
40 cell pack 25R - $160 @ $4.00 368wh
40 cell pack 30Q - $224 @ $5.60 408wh

I think either the 30Q or 25R is a solid battery and it's probably worth getting which ever one is cheaper.
```

---
## \#45 Posted by: PXSS Posted at: 2017-02-22T07:01:47.168Z Reads: 482

```
Dont forget our aplication is constant power and not constant current. Voltage drop plays a very big role in this scenario. 

Voltage drop for a given current per cell. 
25R vs GA:
0.2A
<img src="/uploads/db1493/original/3X/8/9/89012a290880c60a55e014a25051584de0225e16.PNG" width="690" height="387">

5A
<img src="/uploads/db1493/original/3X/c/4/c4b54b359d2db5bf52e26579bbff58889fb630b2.PNG" width="690" height="387">

10A
<img src="/uploads/db1493/original/3X/c/e/ce0186ef42bf16dc88c5d83bea0fea9b1ca032e0.PNG" width="690" height="387">

The voltage sag is slightly worse in every scenario in the 25Rs. That means that for the same power setting, you will have to pull more amps on the 25R than on the GA up to 10A. This also means that the 25R is more inneficient. Most people do not run continuous power at current draws larger than 40A. It's usually just bursts which the GA cells can do just fine while staying under 60C. 

If you're drawing 20A average per cell while riding then I would not recommend the GAs, if you're drawing 10A on average then the GAs have 33% more energy than the 25Rs. 


-------------

25R vs 30Q
0.2A
<img src="/uploads/db1493/original/3X/e/c/ec7e0e701b906ba06b0008c781b0d7c1421b5bec.PNG" width="690" height="387">

5A
<img src="/uploads/db1493/original/3X/7/0/70bce96ef522a72085d47b1d1f6cfd0ab1fd66d9.PNG" width="690" height="387">

10A
<img src="/uploads/db1493/original/3X/f/0/f0d9077fc91d1255c056758c42b1541895b77a44.PNG" width="690" height="387">

15A
<img src="/uploads/db1493/original/3X/f/5/f50db86d3d411f0b89292b0b1fe8408e544b18e2.PNG" width="690" height="387">

As you can see, the voltage sag on these cells is significantly lower than on the 25Rs. This means that these cells will run at a lower current for a given power setting, not stall during hard acceleration due to power drop, and still have a significant amount more of capacity over 25Rs at high average current draws. 

I can easily source these under $4 per cell, both in the US and EU

E: Another good set of comparisons. This is the discharge energy at a specific current.
25R
<img src="/uploads/db1493/original/3X/8/8/882c86ecebfe9c1adcde7270dc69cf20911611ec.PNG" width="690" height="387">

30Q
<img src="/uploads/db1493/original/3X/1/5/155f46e971fc40a5f17ff274ce3760bac491b350.PNG" width="690" height="387">

GA
<img src="/uploads/db1493/original/3X/7/5/753826e4b4a6b56571359dae3697bd9059ac0902.PNG" width="690" height="387">
```

---
## \#46 Posted by: jga Posted at: 2017-02-22T08:01:27.551Z Reads: 402

```
https://eu.nkon.nl/rechargeable/18650-size/samsung-inr-18650-30q-3000mah.html
https://eu.nkon.nl/rechargeable/18650-size/samsung-inr-18650-30q-3000mah-button-top.html

These 30Q seem to be the same on Nkon, but the price is very different. Is that only due to the fact that the second has button-top?
Is it worth paying more for that?
```

---
## \#47 Posted by: PXSS Posted at: 2017-02-22T08:02:14.644Z Reads: 408

```
Thanks for the link! Really interesting conversation that went on. Learned somethkng about not welding directly on the center of a cell maybe? I need to go verify this on the webs.
```

---
## \#48 Posted by: lox897 Posted at: 2017-02-22T09:49:54.656Z Reads: 417

```
You dont need button top
```

---
## \#49 Posted by: Norco Posted at: 2017-02-22T10:05:48.846Z Reads: 425

```
Its threads like this that get me thinking. I have created a 10s4p pack as per diagram below.

<img src="/uploads/db1493/original/3X/e/4/e4aad598e2c23ba8c3a9706bf7b1179cdcc96f11.jpg" width="619" height="500">
(ignore the balance connector marks I know they are backwards)

I am not planning on having a bms and just using a brick charger with cutoff and then periodically checking the cells are balanced. I soldered the pack making sure that each connection was solid. (build of pack [here](http://www.electric-skateboard.builders/t/pork-chop-express-comet-loki-motor-6374-vesc-10s4p-diy-18650-pack-benchwheel/13106/23)) 

Now my question is what happens if the connection to a cell in a parallel group goes bad? How would I know before it is too late? I am assuming that the voltage across the parallel group would still be consistant with the other cells and the capacity would be reduced. Would that mean that I would just be overcharging the battery each time and destroying them without knowing? How would a BMS stop me doing this? (maybe I just suck it up and fit one and divert the BMS for discharge) 

I am not worried about a series failure as its hugely unlikely and rolling to a stop isnt the end of the world!

Norcs
```

---
## \#50 Posted by: jaykup Posted at: 2017-02-22T15:39:42.656Z Reads: 402

```
Interesting on the 30Q voltage drop.  Is that due to the fact that it has more total capacity though?  I would expect a cell with lower voltage drop to run cooler?

The 30Q still gets a lot hotter than the 25R, looks like lygte's tests had to stop at several high amp tests due to temperature?

I'm not sure that a small voltage drop will have any impact in practice?  It would need more amperage, but a very small amount?  

Due to duty cycle, actual battery draw is usually pretty light so maybe looking at it from a high amperage point of view is a bad approach and I should be looking at it from a capacity POV?

Overall the feeling I'm getting is the 30Q has a bit more capacity but struggles with high currents, and the 25R has lower capacity but handles high currents like a champ.

Thanks - now I have more questions than answers haha.  Good discussion though.  NKON has the 25R at 3.69 vs 3.99 for the 30Q.  That price is about right for the differences we see in performance.  Still having a hard time seeing a clear winner - will have to do some more research!
```

---
## \#51 Posted by: Maxid Posted at: 2017-02-22T16:01:03.945Z Reads: 377

```
[quote="jaykup, post:50, topic:3032, full:true"]
I'm not sure that a small voltage drop will have any impact in practice?  It would need more amperage, but a very small amount?  
[/quote]

You can't just replace voltage with current.
```

---
## \#52 Posted by: TarzanHBK Posted at: 2017-02-22T16:03:17.383Z Reads: 366

```
I think the only reason is the lower internal resistance of the 25r. 
The 30Q is a really interesting, underrated battery and we´re group buying a few from nkon.nl for EU guys for 3,55€ at the moment :slight_smile:
```

---
## \#53 Posted by: jaykup Posted at: 2017-02-22T16:28:07.421Z Reads: 358

```
> You can't just replace voltage with current.

I think at 100% motor load you are correct, but at less than 100% load the motor will just draw more amps if the voltage is less.  Since we are talking 0.1v per cell I'm not sure there would be any noticeable difference while riding since most riding is done under 100%
```

---
## \#54 Posted by: jaykup Posted at: 2017-02-22T16:32:13.786Z Reads: 350

```
Nice group buy!  Very attractive battery at that price
```

---
## \#55 Posted by: Maxid Posted at: 2017-02-22T16:38:14.875Z Reads: 362

```
[quote="jaykup, post:53, topic:3032, full:true"]
I think at 100% motor load you are correct, but at less than 100% load the motor will just draw more amps if the voltage is less.
[/quote]

That is not possible. The ESC basically just shorts the battery to the motor in a controlled way. The current that flows is not pushed but is the max current that can flow due to the internal resistance of the motor at that voltage. If your voltage is less you can not make up for that by "pushing" more amps. I have a 10S3P pack with 25Rs and I get voltage sag from 37V down below 33V. 0.1V multiplied by the number of cells becomes 3-4V in the end.
```

---
## \#56 Posted by: PXSS Posted at: 2017-02-22T16:54:52.579Z Reads: 373

```
Ask @evoheyax about his experience with a 25R pack. I bet he won't agree with you. 

The 25Rs do not handle high currents like a champ. 
At 50% (1.25Ah) used capacity. If you draw 15A, you will sag  from 3.7V to 3.2V. In a 10S4P pack that is a loss of 5volts, what should be outputting 2220W is now only doing 1920W. That is a power loss of 13.5%. If you're trying to climb a hill, it will stall. 

On the other hand, 30Qs drop to 3.45V at 15A draw with 1.25Ah consumed. In a 10S4P pack, this means 2070W. That is an improvement of 8% over the 1920W the 25Rs output. Things get much worse for the 25Rs the further down you move on the curve. 

Yes the 25Rs might run cooler. They still have less power output at any setting than the equivalent 30Q pack. 

Not only that, the sag means that you can only run it hard for about 50% capacity without hitting your lower voltage limit. Using 30Qs expands this to 80ish%
```

---
## \#57 Posted by: jaykup Posted at: 2017-02-22T16:57:07.507Z Reads: 359

```
@Maxid How are you doing the full quote?

All cells will sag quite a bit when under load, so 37 to 33 is pretty normal.  The 25R just sags 0.1v more than the 30Q under the same load, so 37 to 33 on 25R vs 37 to 34 (10x0.1) on 30Q.

I think what you are saying is the motor always takes the same amount of amperage, but the amperage is switched on and off by the duty cycle, so you'd have to have a higher/longer duty cycle at lower voltage to get the same wattage output, but the amperage wouldn't change - correct?

But isn't amperage = voltage / resistance?  

40v / 1ohm = 40 amps?
50v / 1ohm = 50 amps?

So what I was saying before is backwards, lower voltage would also lower your total amperage?

Sorry - thinking out loud here, just trying to understand.
```

---
## \#58 Posted by: PXSS Posted at: 2017-02-22T17:24:04.468Z Reads: 340

```
Power is constant. 
P = V*I
V = I*R
V is a variable
I is a variable
R is mostly a constant.
```

---
## \#59 Posted by: Hummie Posted at: 2017-02-22T17:28:32.658Z Reads: 361

```
talking about the different ways to wire up 10s4p, either in a 10s chain and those in parallel or 4p all wired in series, the obvious benefit is with the 4 all connected in parallel they will balance each other and you now have 12 cells effectively to really worry about as apposed to 40....but....when I say worry, this method is safer in that the cells will balance each other but also it has a liability in that you dont know the individual cell voltages and neither would a bms and if there's a dud in the pack of four you wouldnt know and you'll get reduced output from the pack of 4 as the one sinks all the rest.   a bms would likely need to do the 4 cells wired together as if all the cells are individual as in the 10s wired then in parallel would be too many individual cells for it to monitor so with a bms it's not an option anyway but the  point is when you put cells in parallel you dont know how they are individually doing anymore and you could be suffering from reduced output as apposed to when using 10s chains then wired in parallel.  

also someone said when you were to put 10s chains then in parallel it will be a lot more current going through than the current going through with the 4 single cells being paralleled. true but it would have many more cells for that current to go to and ultimately it would be the same inrush of balancing current per cell.  How much variance in voltage between the cells being parallleled is too much I'd like to know.  in theory even if the cells being paralleled had a slight variation in current and paralleled it would be a huge current inrush.  when cells are charged appropriately with a regulated supply they are limited to a constant current to avoid the high current that would be generated from a higher voltage connected to a cell

parallel connections pass very little current and its just the series chain that it runs in so the 4p then put in series would very likely also have reduced resistance with it's reduced series chain wiring,..four times less
```

---
## \#60 Posted by: ralphy Posted at: 2017-02-22T22:58:22.686Z Reads: 340

```
What did you get as far as capacity? I did a 2p6s pqck and its only takjng 4000mah
```

---
## \#61 Posted by: DougM Posted at: 2017-02-22T23:20:25.328Z Reads: 337

```
I don't know - I had to take that board offline for another issue, then winter hit.  Hopefully by the time I get back to it in the spring @raphaelchang's BMS will be ready to go, then I'll let you know.
```

---
## \#62 Posted by: jga Posted at: 2017-02-23T19:53:49.703Z Reads: 355

```
Where is that GB?
```

---
## \#63 Posted by: TarzanHBK Posted at: 2017-02-24T07:37:27.530Z Reads: 368

```
http://www.electric-skateboard.builders/t/18650-group-buy-eu/12067/

We´re at 3,55€ for 30Qs atm and like to order in a few days.
```

---
## \#64 Posted by: Hockingham Posted at: 2017-03-04T22:53:55.228Z Reads: 367

```
Thought this may be interesting 
https://www.youtube.com/shared?ci=qic5xFpiZxc
```

---
## \#65 Posted by: Hockingham Posted at: 2017-03-04T23:05:43.161Z Reads: 361

```
Also proves the point you guys were saying when I suggested these exact batteries
```

---
## \#67 Posted by: PXSS Posted at: 2017-03-14T16:11:10.451Z Reads: 339

```
Those batteries are the old version of the Sanyo GA cells I talk about above.
```

---
## \#68 Posted by: Adir Posted at: 2019-10-25T09:48:04.490Z Reads: 37

```
If you want calculate battery pack parameters:
(calculates: voltage, capacity, energy, discharge current, etc.) up to 9999s 9999p packs ;)

I suggest install free Android app: “**Battery pack calculator**” . 
Built-in database of 37 popular, branded batteries and the ability to define your own battery cells.
```

---
