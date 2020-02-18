# LiFePO4 cells, who uses them?

### Replies: 182 Views: 7248

## \#1 Posted by: banjaxxed Posted at: 2018-03-04T15:01:37.943Z Reads: 433

```
After jumping in a couple of threads today with irrelavancies (wristslap), I was looking at a 12v battery I have that's lightweight, good energy density & a long lifespan.

So why aren't they more popular? BMS charge/cutoff problems?

This looks promising, anyone used this company?
https://www.ev-power.eu/LiFePO4-small-cells/LiFePO4-High-Power-Cell-3-2V-20Ah-Alu-case-CE.html?cur=1#tab2
```

---
## \#2 Posted by: Exiledd_Top Posted at: 2018-03-04T15:35:07.407Z Reads: 396

```
LiFePO4 Don't need a bms there chemical chemistry  self balance them self. That battery only has 3c discharge that you listed .  I think the major reason we don't use them or most  of us is because there big and bulky compared to 18650 cells.
```

---
## \#3 Posted by: linsus Posted at: 2018-03-04T15:45:49.738Z Reads: 399

```
LiFePO4 usually boasts a higher current draw. But are far from the density of top 18650 models. 
LiFePO4 might be abit more robust but they do still need balancing.

They were abit pricy for awhile, not sure if they still are.
```

---
## \#4 Posted by: PXSS Posted at: 2018-03-04T15:55:46.093Z Reads: 394

```
EV Power LiFePo Cell
---
Dimensions:
Length: 178 mm
Width: 71 mm
Height: 28 mm
Volume: 353.86 cc/ml
Weight: 650g

Electrical properties:
N Voltage: 3.2v
Capacity: 20Ah
Energy: 64Wh
Max Discharge: 200A
Power: 640W

Energy Density: 180Wh/L
Power Density: 1800W/L
Specific Energy: 98Wh/kg
Specific Power: 980W/kg

---

Samsung 30Q
---
Dimensions:
Length: 65mm
Width: 18.3mm
Height:  18.3mm
Volume: 21.76785 cc/ml (**assuming it's a cube**)
Weight: 47g

Electrical properties:
N Voltage: 3.6v
Capacity: 3Ah
Energy: 10.8Wh
Max Discharge: 20A
Power: 66W (20A at 3.3V)

Energy Density: 496Wh/L
Power Density: 3031W/L
Specific Energy: 230Wh/kg
Specific Power: 1404W/kg

---
In conclusion, that specific LiFePo battery has less energy and less power per cubic centimeter and per kg added to your board than a 30Q battery. 
---
30Q pack is 2.75 times more energy dense and 1.68 times more power dense. It has 2.38 times higher specific energy and 1.43 times higher specific power.


They are not popular because of this. It would mean for the same battery size and weight, you would have less energy and power and nobody wants that. Except for boosted boards... They're weird...

---
E: added A123 cells from post below to keep it all in one post and modified the power data for 30Qs based on discharge curves. 

---
A123 26650 LiFePo
---
Dimensions:
Length: 65.15mm
Width: 26.62mm
Height: 26.62mm
Volume: 46.16688 cc/ml (assuming it’s a cube)
Weight: 70g

Electrical properties:
N Voltage: 3.3v
Capacity: 2.3Ah
Energy: 7.59Wh
Max Discharge: 70A (***No discharge curve provided above 40A***)
Power: 231W (***Extremely inflated as the cell sags 0.6V at 40A***)
Realistic power: 108W (***Based on discharge curve on datasheet, 40A at 2.7V***)

Energy Density: 164.4Wh/L
Power Density: 5004W/L (3.3v and 70A)
Realistic Power Density: 2339W/L (based on 40A discharge curve)
Specific Energy: 108.4Wh/kg
Specific Power: 3300W/kg
Realistic Specific Power: 1543W/kg

---
The A123 compared to Samsung 30Q:
Energy density ratio (30Q/A123): 3.02
Power density ratio (30Q/A123): 0.606 (based on 70A and 3.3V)
Realistic power density ratio (30Q/A123): 1.296 based on discharge curves. 
Specific Energy ratio (30Q/A123): 2.12
Specific Power ratio (30Q/A123): 0.425 (based on 70A)
Realistic Specific Power ratio (30Q/A123): 0.91 (based on discharge curves)
```

---
## \#5 Posted by: eb1925 Posted at: 2018-03-04T16:14:13.499Z Reads: 351

```
They are rated for a LOT of charge/discharge cycles.
```

---
## \#6 Posted by: ATLesk8 Posted at: 2018-03-04T16:23:16.135Z Reads: 347

```
I believe Metroboard uses LifePo correct?
```

---
## \#7 Posted by: Nordle Posted at: 2018-03-04T16:27:02.584Z Reads: 347

```
A123 cells also have life chemistry if i remember correctly
```

---
## \#8 Posted by: Fatos Posted at: 2018-03-04T18:30:46.478Z Reads: 337

```
I use them. A123 26650.They are great but they have their drawbacks also.
Lower energy density compared to liion. Very few producers. And pretty high priced.

But man they are rigid. I have tortured them in all possible ways. They are safer. I have discharged them to 0.5V many times. They don't show any wear. I have used them for spot welding also  :). 
They are pretty much fire safe.  They have high discharge current and really flat discharge curve.
I like them a lot honestly. I run them without any type of balancing and they are still in 0.05V different.

I hear people call boosted board stupid for using them but I can disagree.
```

---
## \#9 Posted by: E1Allen Posted at: 2018-03-04T21:03:43.459Z Reads: 318

```
There is a thread here where someone uses these

http://www.evassemble.com/index.php?main_page=product_info&cPath=2&products_id=19

I did the price comparison based on using 12s3p of 30q to
14s1p of these and it was about $70 more and 7 lbs heavier.  Maybe the higher Ah cells would be another option but would for sure make a heavy board.
```

---
## \#10 Posted by: banjaxxed Posted at: 2018-03-04T21:05:07.757Z Reads: 303

```
That is the answer that makes sense, thanks you

[quote="PXSS, post:4, topic:48126"]
30Q pack is 2.75 times more energy dense and 1.84 times more power dense. It has 2.38 times higher specific energy and 1.56 times higher specific power.
[/quote]
```

---
## \#11 Posted by: b264 Posted at: 2018-03-05T05:03:13.930Z Reads: 277

```
[quote="ATLesk8, post:6, topic:48126, full:true"]
I believe Metroboard uses LifePo correct?
[/quote]

Their Shortboard uses a 12S 5Ah LiFePO4 battery, yeah.  They are also more rugged and last longer and have a smoother power curve; they stay near nominal voltage for longer during their discharge cycle.  But yes, of course they are less energy and power dense than most 18650 cells.  For a shorter-range board that needs to be RUGGED they can be ideal in certain narrow circumstances.  My daily driver is one of these, modified slightly
```

---
## \#12 Posted by: deucesdown Posted at: 2018-03-05T07:01:16.362Z Reads: 261

```
There's a big difference between generic lifepo4 and A123's implementation. I've run my 12s2p pack for one year of almost daily commutes. Ridiculous batteries. Saved me from myself many times. Runs ruthlessly in the frozon nyc winters.

Pros:
- can take abuse wrt discharge and charging - can take 10c charge, overvoltage on charge, trickle charge.
- If abused to failure tends to die nicely
- 1000+ cycle life
- low internal resistance
- very good voltage sag characteristics
- works okay in cold
- can crank the regen current

Cons:
- expensive per WH
- low WH per volume
- nickel strips won't handle the current?
- heavy
- weird voltage
- hard to correlate state of charge to voltage

I think a 14s1p of A123 can fully feed just about any motor used for eskate. Nothing can touch it for regen, so amazing for hub motors.

I'll run the numbers against 30q ala @PXSS if I remember.
```

---
## \#13 Posted by: lock Posted at: 2018-03-05T07:57:44.240Z Reads: 242

```
I've looked, but am generally of the opinion you can forget about _non-a123_ LiFePO4 cells. The 200a EV cells sound impressive, but for a 12s setup that's 7.8kg of battery! Admittedly the 20Ah will get you a fair distance, but being able to travel 40km on a single charge hasn't been too high up on my list of priorities.

Specific power of the a123 26650 cell is listed at 2600 W/kg; that's a bit higher than quoted for the 30q above (1532W/kg). _a123 cells actually have a higher power to weight ratio_, so Boosted may not be so weird after all :wink: 

Then there's the nail penetration tests that make an interesting comparison. Not saying this is particularly relevant, but it certainly highlights the difference in stored energy density.
https://www.youtube.com/watch?v=f30fBFitkSM
https://www.youtube.com/watch?v=rb_J2QQ0k-4
```

---
## \#14 Posted by: PXSS Posted at: 2018-03-05T12:49:52.619Z Reads: 227

```
E: Look at post 4
---

I went looking for the A123 cell datasheet and found it here.
http://www.sullivanuv.com/wp-content/uploads/2014/06/A123-Cell-Datasheet-2008-08.pdf

So here's the same analysis:

Dimensions:
Length: 65.15mm
Width: 26.62mm
Height: 26.62mm
Volume: 46.16688 cc/ml (assuming it’s a cube)
Weight: 70g

Electrical properties:
N Voltage: 3.3v
Capacity: 2.3Ah
Energy: 7.59Wh
Max Discharge: 70A (***No discharge curve provided above 40A seems fishy, no temperature profile accompanying the data either***)
Power: 231W (***Extremely inflated as the cell sags 0.7V at 40A***)
Realistic power: 104W (***Based on discharge curve on datasheet***)

Energy Density: 164.4Wh/L
Power Density: 5004W/L (3.3v and 70A)
Realistic Power Density: 2253W/L (based on 40A discharge curve)
Specific Energy: 108.4Wh/kg
Specific Power: 3300W/kg
Realistic Specific Power: 1486W/kg

---
The A123 compared to Samsung 30Q:
Energy density: 30Q is 3.02x higher
Power density: 30Q is 0.66x lower based on numbers. 
Power density: 30Q is 1.47x higher based on discharge curves. 
Specific Energy: 30Q is 2.12x higher
Specific Power: 30Q is 0.464x lower based on numbers
Realistic Specific Power: 30Q is 1.03x higher basedon discharge curve. 

---
~~There is a caveat with the realistic numbers!!!
It is based on the discharge curve of the A123 but not the 30Q. So my 30Q numbers could have also been a little inflated. I must go to work so I will not be able to adjust those numbers until tonight. I don't expect it to change drastically. Maybe ~8% lower.
30Q avg voltage is 3.3V at 20A, not 3.6. So yes, 8% lower is correct~~
Data added to post # 4
```

---
## \#15 Posted by: banjaxxed Posted at: 2018-03-05T13:09:31.611Z Reads: 214

```
Maybe a monster Trampa build with 200mm+ tires would make sense. That EV pack comes to 7.8kg as mentioned which is a lot of weight for a pack on top of the rest of the running gear. in general ATB packs tend to be around a 3-4kg, so this is doubling on weight.

Price is very good for the amount of Ahrs you get €258 & assembly and protection woould be a breeze in this form factor

Where you get A123s and their price is another matter

**Edit:** Ok a123 on our old favourite
https://www.nkon.nl/rechargeable/26650/a123-systems-anr26650m1b-a-grade-3-3v-a-grade.html

I've decided to pull apart the Veruzend pack and liberate 72 30Q cells based on the above, more 18650 cells down the road
```

---
## \#16 Posted by: banjaxxed Posted at: 2018-03-05T13:31:07.152Z Reads: 202

```
hub motors eh? A123 cells mmmm interesting.
```

---
## \#17 Posted by: biggdaddyhawk Posted at: 2018-03-05T16:44:50.076Z Reads: 198

```
I've recently decided to use a123 cells on all my boards cause I don't trust my kids to not make a mistake when riding and charging when I'm not there. They might smoke for a second but they won't catch fire. Still wondering how many layers of 10mm x .15 nickle would be needed for the current. Really thinking of soldering gold coated copper battery bars like back in my old rc car days.
```

---
## \#18 Posted by: banjaxxed Posted at: 2018-03-05T16:48:51.382Z Reads: 202

```
If you run different voltages with different chargers & the risk is a random charger plugged into a random board then use different conectors for each board? better than a fire or a smokebomb.

https://endless-sphere.com/forums/viewtopic.php?f=14&t=58541
_Nickel strip amperage = SA(mm)x19/4. It's quite low. Ie 8mm x.15mm nickel = approx 6amps_

nice chart here
https://endless-sphere.com/forums/viewtopic.php?t=68005


about 10A with 0.15mm X 10mm pure nickel
http://www.electric-skateboard.builders/t/battery-building-what-nickel-strips-do-you-use/6202/4?u=banjaxxed

And a resource on-site here
http://www.electric-skateboard.builders/t/how-much-current-can-nickel-strip-handle/43081
```

---
## \#19 Posted by: biggdaddyhawk Posted at: 2018-03-05T16:53:43.925Z Reads: 188

```
Good idea. All the kids have 6s packs and they have their own chargers with a serious training lesson. I'm harvesting these cells from electric bus batteries and got the price down to 1.50 per cell.
```

---
## \#20 Posted by: AndyL Posted at: 2018-03-05T17:41:44.429Z Reads: 185

```
Are the cells still in good condition with good lifespan though? Read that the electric buses put considerable strain on these batteries, even if they're highly rated a123 cells
```

---
## \#21 Posted by: biggdaddyhawk Posted at: 2018-03-05T17:48:35.985Z Reads: 167

```
Out of 96 cells you must find the culprit cells which made them decommission the block. I had about 6 cells with no voltage. The other 90 cells are pristine holding 3.66 volts perfectly balanced I might add. I have yet to find a way to check them with the ohm meter on my voltmeter.
```

---
## \#22 Posted by: deucesdown Posted at: 2018-03-05T18:20:41.941Z Reads: 166

```
[quote="banjaxxed, post:18, topic:48126"]
If you run different voltages with different chargers & the risk is a random charger plugged into a random board then use different conectors for each board? better than a fire or a smokebomb.
[/quote]

The interesting thing with A123 voltages is 12s is very very close to 10s lithium ion, and 14s -> 12s.
```

---
## \#23 Posted by: deucesdown Posted at: 2018-03-05T18:23:59.965Z Reads: 168

```
[quote="biggdaddyhawk, post:21, topic:48126"]
I had about 6 cells with no voltage.
[/quote]

There's a decent chance these can be saved. A123 are crazy cells...

[quote="biggdaddyhawk, post:21, topic:48126"]
have yet to find a way to check them with the ohm meter on my voltmeter.
[/quote]

I think a charge/discharge/charge cycle on a hobby charger... Less than 70% of spec capacity, it's kaput.
```

---
## \#24 Posted by: deucesdown Posted at: 2018-03-05T18:31:10.024Z Reads: 157

```
Super awesome post as usual. We need to get your title set to Myth Buster (@treenutter? )

I think where I'm getting tripped up is I'm comparing 1 cell to 1 cell, where I should be comparing by volume and perhaps weight. The 3.3v vs 3.6v nominal makes a big difference in the energy delivered.

Still, A123 has stunning advantages in certain situations. Like a tiny high power pack or airplane friendly pack (12s1p 99wh, and can feed 2 motors).

14s1p seems a very good match for a single high power motor. @BigBoyToys (miss you bro) was heading down the path of independent 14s1p per motor, including VESC, receiver, bluetooth module, and bms.
```

---
## \#25 Posted by: PXSS Posted at: 2018-03-05T18:34:25.473Z Reads: 157

```
I updated post 4 with A123 vs 30Q data :)
```

---
## \#26 Posted by: deucesdown Posted at: 2018-03-05T18:36:15.675Z Reads: 162

```
Can you do 20700, 21700 and make it a sticky? :) (I feel like 18650s win easily)
```

---
## \#27 Posted by: biggdaddyhawk Posted at: 2018-03-05T18:42:31.670Z Reads: 173

```
Yea the lower voltage starts to add up when building packs with a123 cells. My 8s pack come in at 29.4 which is the same as a 7s lithion.
```

---
## \#28 Posted by: Hummie Posted at: 2018-03-05T18:43:05.599Z Reads: 179

```
it was maybe already said but the cycle life of the iron is about 4x more than for ion which is pretty awesome and makes the price much more reasonable.  

the headway red cells are awesome with their bolt connectors and 200 amp ability.  theres video of liveforphisics from endless-sphere over charging them and shooting them with his crossbow and other stuff
https://www.youtube.com/watch?v=52h8IK0IdqI&t=225s
https://www.youtube.com/watch?v=8IBapfB0Imo
great piece of mind there.  also really hard to damage them by over discharging and they pop back up
```

---
## \#29 Posted by: PXSS Posted at: 2018-03-05T18:47:06.682Z Reads: 166

```
I feel like I've alreadt done 21700 in a different thread. I'll look for it. If not, I'll try to get to it tonight. I keep meaning to do a full on wiki for batteries but I just don't have the time.
```

---
## \#30 Posted by: PXSS Posted at: 2018-03-05T18:50:18.548Z Reads: 168

```
There's also a video of him trying to prove how 18650 Li-ions are unsafe by overcharging them, hammering them, drilling them and doing more stuff to them I cannot remember. In the end the cell did not blow up. He still concluded that the cells were too dangerous to use.

He is extremely biased, even when experiments dont go his way, he manages to twist the data to support his theories...

His videos are ***very very*** entertaining though
```

---
## \#31 Posted by: deucesdown Posted at: 2018-03-05T18:51:51.663Z Reads: 165

```
[quote="Hummie, post:28, topic:48126"]
it was maybe already said but the cycle life of the iron is about 4x more than for ion which is pretty awesome and makes the price much more reasonable.
[/quote]

This is a trap in a way. For example, 12s2p A123 at $10/cell is $240. Money equivalent 30q pack is 10s7p ($240/$3.5 == 69 cells)?

The A123 pack is 198wh. The 30q pack is 777wh.

So you get almost 4x capacity in 30q, which offsets the 4x cycle life of A123.

Plus with 30q packs you typically don't drain it all the way, and usually don't need to charge to 4.2/cell, which can greatly increase cycle life.

Sorry @banjaxxed we're derailing your anti-thread-derail thread.
```

---
## \#32 Posted by: Hummie Posted at: 2018-03-05T19:00:24.511Z Reads: 155

```



and they have a great discharge curve holding a higher voltage level before dropping off.  better than ion.


or even better deal!!!:
17$ each
http://evassemble.com/index.php?main_page=product_info&cPath=2&products_id=20

and that's single cell price and they do packs.
```

---
## \#33 Posted by: biggdaddyhawk Posted at: 2018-03-05T19:01:15.509Z Reads: 152

```
So the price of used harvested cells are 1.50 each and the price for new a123 cells are around 6.00. Also they don't catch fire.
```

---
## \#34 Posted by: deucesdown Posted at: 2018-03-05T19:39:21.357Z Reads: 161

```
[quote="biggdaddyhawk, post:33, topic:48126"]
the price for new a123 cells are around 6.00.
[/quote]

This seems misleading to me. New cells ("B" type) are around $9-10:

https://www.buya123products.com/goodsdetail.php?i=6

https://ru.nkon.nl/a123-systems-anr26650m1b-a-grade-3-3v-a-grade.html

The older "A" type with less capacity can be found on ebay, at qty 60 or 100, for about $6 per cell, but they're new old stock, sitting around on shelves for a few years.

If you have a source for new "B" cells link us up.

@hummie i don't know why I hadn't noticed those red Headways. But they're HUUUGE! 38mm x 120mm (173.28cc assuming cube as above), 330g. Compared to 30q at 18mm x 65mm (21.8cc assuming cube as above) 47g. About 7 times bigger/heavier. Thicker than a double stack 18650. Gonna have to topmount on your deck with hella riser :slight_smile:
```

---
## \#35 Posted by: banjaxxed Posted at: 2018-03-05T20:44:55.625Z Reads: 151

```
derail away, a pure stream of consciousness is always entertaining
```

---
## \#36 Posted by: banjaxxed Posted at: 2018-03-05T20:46:28.671Z Reads: 150

```
those headways would get you shot in a portable body-belt pack, 12s1p = 4.32kg uuuufff. But cheap enough $200, weightwise against 12s3p 30Q..must check, checked, about 1.72kg..heavy man
```

---
## \#37 Posted by: Hummie Posted at: 2018-03-05T20:52:06.774Z Reads: 152

```
theres a photo somewhere I saw years ago on endless-sphere of a cnc'd aluminum deck with the red headways on the bottom sitting there exposed bolted on the deck somehow and it looked fantastic.  they're big but doable with the right deck.

I spent a lot of time designing a connector for those cells that would bolt to the board.  could be really simple to both connect the cells and mount them to the deck...and I think no enclosure necessary with these like the set-up with the aluminum deck I was writing about above.  I think it's a super clean nice look.  I like to see them
```

---
## \#38 Posted by: banjaxxed Posted at: 2018-03-05T20:53:13.930Z Reads: 143

```
I like the bolts, so easy
```

---
## \#39 Posted by: Hummie Posted at: 2018-03-05T20:55:26.357Z Reads: 146

```
and then if the bolts connect to your own metal fixture that bolts into a deck would be super slick.   maybe a cast copper bracket or something.  It was so long ago I was going to do it I forget what I was going to do in the end but sure there'd be many ways to do it.
```

---
## \#40 Posted by: banjaxxed Posted at: 2018-03-05T20:59:00.850Z Reads: 150

```
ah memory loss, such a curse, what were we talking about again?
```

---
## \#41 Posted by: E1Allen Posted at: 2018-03-05T21:13:43.902Z Reads: 149

```
http://www.electric-skateboard.builders/t/using-lifepo4-battery/9781/16

![IMG_4542|281x500](upload://98kJITLxyyi2asl8Q0lRjOvwxjb.jpg)![IMG_4543|281x500](upload://gKPOZXmUudw2lGtRP1IlaK8lCbg.jpg)

Here are those boards and the thread associated.
```

---
## \#42 Posted by: PXSS Posted at: 2018-03-05T21:41:14.673Z Reads: 140

```
Funny how the threads titles are nearly identical.
```

---
## \#43 Posted by: Hummie Posted at: 2018-03-05T22:11:38.760Z Reads: 141

```
What are those brown cylindrical lipo?!
```

---
## \#44 Posted by: cosmicc89 Posted at: 2018-03-05T22:37:19.428Z Reads: 143

```
That battery and rail system is dope
```

---
## \#45 Posted by: b264 Posted at: 2018-03-05T22:49:06.937Z Reads: 143

```
[quote="cosmicc89, post:44, topic:48126, full:true"]
That battery and rail system is dope
[/quote]

I can't get beyond picturing all the rocks and sticks and screws hitting it and cringing
```

---
## \#46 Posted by: E1Allen Posted at: 2018-03-05T23:01:57.652Z Reads: 140

```
[quote="b264, post:45, topic:48126"]
I can’t get beyond picturing all the rocks and sticks and screws hitting it and cringing
[/quote]

That may be an uncovered shot.  However a plastic guard to cover components could be easily added.  

I'd prefer a board to fit the cells the other way to hopefully fit 14 to match 12s
```

---
## \#47 Posted by: cosmicc89 Posted at: 2018-03-05T23:06:32.706Z Reads: 137

```
I was thinking the same thing. I'd rather have them perpendicular to the board
```

---
## \#48 Posted by: cosmicc89 Posted at: 2018-03-05T23:12:39.307Z Reads: 131

```
Has anyone on the forum done a mountainboard with LiFePo cells?
```

---
## \#49 Posted by: Dyspro Posted at: 2018-03-06T13:28:31.062Z Reads: 128

```
Oh man, Lithium Iron Polonium is much different from Lithium Iron Phosphate!
```

---
## \#50 Posted by: biggdaddyhawk Posted at: 2018-03-06T21:05:57.453Z Reads: 126

```
So is lithium manganese... made for extreme cold.
```

---
## \#51 Posted by: Dyspro Posted at: 2018-03-06T23:00:45.568Z Reads: 125

```
Don't forget about aluminum and sodium hydroxide, for those who are most cold.
```

---
## \#52 Posted by: eb1925 Posted at: 2018-03-07T02:24:51.587Z Reads: 125

```
My friend did all the maths and came up with a lifetime 6x as long for the A123 cells vs 30q
```

---
## \#53 Posted by: mmaner Posted at: 2018-03-07T02:43:22.317Z Reads: 126

```
I'd be very interested to see that math.  It seems it may not account for peak amount drains. The A123 cells lifetime don't fair well with huge amp drains...as I understand it.
```

---
## \#54 Posted by: eb1925 Posted at: 2018-03-07T03:02:56.204Z Reads: 124

```
That's true, what I've seen other places (not sure if it's credible) is that a123s drop off badly after 40 amps discharge.... he did not factor that in, but used the manufacturer provided lifetime discharge curves.
```

---
## \#55 Posted by: mmaner Posted at: 2018-03-07T03:28:30.826Z Reads: 124

```
I'd definitely see if I could find data on 40a plus usage.
```

---
## \#56 Posted by: ATLesk8 Posted at: 2018-03-07T03:29:17.022Z Reads: 120

```
My metro board charger i believe says 43.8V
```

---
## \#57 Posted by: eb1925 Posted at: 2018-03-07T04:41:18.772Z Reads: 123

```
But, the argument for that is, if you have a 2p or up of these batteries, you don't even have to worry about getting above 40 amps because you'd fry most any VESC within the 80+ amps (due to the 2p or more) of "safe" range for the a123 cells. Now on 1p you cluld easily do it.
```

---
## \#58 Posted by: Jebe Posted at: 2018-03-07T06:52:16.679Z Reads: 123

```
Weight is ok for an electric outboard or electric go cart :)
```

---
## \#59 Posted by: PXSS Posted at: 2018-03-07T11:16:56.283Z Reads: 134

```
The thing is, with the money for a 14S2P, you can buy a 12S7P 30Q battery. You are talking about 3x the energy on the 30Q. If you load the A123 at 40A, it means you would only load the 30Q at 11.5A. With 4x the range, you could charge to 4V and discharge to 3.2V and still have more energy than the A123. Charging/discharging like so will increase your battery life at least 4x. So you went up to 1200 cycles with the 30Q pack, likely even more because you aren't stressing them that much at a max of 11.5A, while you would get reduced lifespan from running A123 from stress at a max of 40A. So we're talking same ballpark in lifespan with higher power and range available.

From Nkon:
A123 cost €8.5 = $10.57
30Q cost €2.75 = $3.42

---
So for the same price of ~$300:

A123 Configuration: 14S2P
A123 Nominal Voltage: 44.8V
A123 Current Capable: 80A
A123 Energy: 224Wh

30Q Configuration 12S7P
30Q Nominal Voltage: 43.2V
30Q Current Capable: 140A
30Q Energy: 907Wh
```

---
## \#60 Posted by: mmaner Posted at: 2018-03-07T14:05:08.785Z Reads: 126

```
@eb1925 yeah, that :slight_smile:
```

---
## \#61 Posted by: eb1925 Posted at: 2018-03-07T16:18:19.751Z Reads: 121

```
Hahaha this man is on top of some batteries. I agree, that's why I bought 30q's 😂😂
```

---
## \#62 Posted by: eb1925 Posted at: 2018-03-07T16:28:38.899Z Reads: 122

```
I believe you're correct and it's the same thing I assumed but wasn't sure, but if you factor out the part charge/discharge cycles the math is right, which we didn't even bother counting part charge/discharge... the problem for us is that we will have at least one half cycle every day when riding to class, if not a full cycle, and on the weekends when we go ride for fun it could be 2. We ride a lot, now mostly on normal boards, but soon on esk8's. I got 10s5p 30q from IMR and my buddy got 14s2p for about $20 more(they had good discount rates on bulk)... we didn't do Nkon because of stateside shipping etc. We are both on thane, so I assume my range will be 25+ miles, his looks like about 14 (not sure).
```

---
## \#63 Posted by: eb1925 Posted at: 2018-03-07T16:29:44.732Z Reads: 116

```
But when I need some info on the next new battery I'm know who I'm PM'ing haha😉
```

---
## \#64 Posted by: Exiledd_Top Posted at: 2018-03-07T16:36:26.628Z Reads: 116

```
[quote="eb1925, post:62, topic:48126"]
my range will be 25+
[/quote]

Well 12s6p 30q bypassed with 4wd carvon got 30 miles so you'd get more like 30+
```

---
## \#65 Posted by: eb1925 Posted at: 2018-03-07T16:38:27.410Z Reads: 113

```
I like it! I didn't want to be overly optimistic so I've been telling myself 25😂
```

---
## \#66 Posted by: PXSS Posted at: 2018-03-07T17:00:51.298Z Reads: 127

```
Assuming a 20Wh/mile consumption, a 14S2P A123 would get you 11miles, the 30Q pack would get you 45 miles... Your buddy would have to recharge his pack 4 times before you run out of juice...

This is for 14S2P vs 12S7P. 

10S5P has 540Wh. Still 2.4x more energy and 20A higher discharge capability. Although at 10S you are less efficient than him at 14S
```

---
## \#67 Posted by: Hummie Posted at: 2018-03-07T18:00:48.207Z Reads: 125

```
I don't see that low price on that site for the 30Q.  I got them recently as a group here for pretty cheap but forget what I paid.

but how bout a comparison with the red headway 38120hp which are likely a better deal 

16.50$ for 8ah is the best I see but bet you can find much better in bulk

http://evcomponents.com/lifepo4-cell/headway-38120hp-8ah-lifepo4-cell.html
```

---
## \#68 Posted by: PXSS Posted at: 2018-03-07T18:03:17.477Z Reads: 119

```
They've been at €2.75 for at least a year. The euro has been steadily rising against the dollar which sucks.
```

---
## \#69 Posted by: banjaxxed Posted at: 2018-03-07T18:08:43.979Z Reads: 123

```
an thank God for that (and other orangey deiities)
```

---
## \#70 Posted by: Hummie Posted at: 2018-03-07T18:09:04.239Z Reads: 126

```
ok I see it.  the 30Q is a great deal but having that relaxing feeling your board wont blow up has a value.  I know I think about it when I take my board some places and worry about leaving it other places.


but this deal is hard to beat and cells stated at 10amp continuous.
https://www.ebay.com/itm/NEW-Box-of-80-Fullriver-LiFePO4-26650-3-2V-3300mAh-Rechargeable-Batteries/191987482937?hash=item2cb3588139:g:vj0AAOSwUYNaAcNp

80 cells for 80$$ !!!!
```

---
## \#71 Posted by: longhairedboy Posted at: 2018-03-07T18:14:52.637Z Reads: 121

```
all of this is why i still have about 300 30Qs in a bin under my bench. I've given up finding a more cost effective cell. It doesn't exist. So i'm buffering my stock and telling people not to bother with anything else. 

according to the inventory of the people i usually buy from, a lot of other people are thinking the way I am as well.
```

---
## \#72 Posted by: Hummie Posted at: 2018-03-07T18:18:22.490Z Reads: 121

```
these fullriver cells are a steal though.  the downsides of lifepo4 being bigger and heavier still but watts for dollars these things surely win.
```

---
## \#73 Posted by: BenTheBarre Posted at: 2018-03-07T18:23:18.533Z Reads: 122

```
Are these fullriver cells reputable though? At 1 dollar per cell there must be a catch... And why do they look like the have a paper wrapping?
```

---
## \#74 Posted by: PXSS Posted at: 2018-03-07T18:34:51.654Z Reads: 123

```
[quote="Hummie, post:70, topic:48126"]
but having that relaxing feeling your board wont blow up has a value.
[/quote]

[quote="Hummie, post:70, topic:48126"]
NEW LiFePO4 26650Fe Li-Ion 3.2V 3300mAh Cylindrical Rechargeable Batteries. | eBay!

80 cells for 80$$ !!!
[/quote]
 ...
I don't know what to say...
Good luck with those not blowing up...?
```

---
## \#75 Posted by: longhairedboy Posted at: 2018-03-07T18:44:16.032Z Reads: 120

```
@Hummie  dude.. you crack me up. 

You have a set of lipos taped to the bottom of a deck and.. oh wait. I see what you did there.
```

---
## \#76 Posted by: Hummie Posted at: 2018-03-07T18:49:07.910Z Reads: 123

```
they look pretty legit to me.  find me something showing otherwise.   but discharge testing is hard to find.
But @longhairedboy is a thin kydex plastic cover over lipos taped to the bottom of a deck better?  the results are in and probably yes but not by a landslide.  in my defense I haven't done that in a while and moved on to lipos glued to the deck with carbon glued on top of them.   I don't like that really though as I cant feel them for temp
```

---
## \#77 Posted by: PXSS Posted at: 2018-03-07T18:59:31.086Z Reads: 122

```
[quote="Hummie, post:67, topic:48126"]
comparison with the red headway 38120hp which are likely a better deal
[/quote]

Volume: 176cc
Weight: 300g
Energy: 25.6Wh
Energy Density: 145Wh/L
Unrealistic Power Density: 2906 W/L (160A at 3.2V)
Realistic Power Density: 2400W/L (160A at 2.6V)
Specific energy: 85Wh/kg
Realistic Specific Power: 1387W/kg

30Q has 3.42x the energy density, 2.71x specific energy, similar power density and specific power probably. 

30Q costs $0.317 per Wh
Red Headway costs $0.64 per Wh. 

IMO, it sucks.
```

---
## \#78 Posted by: PXSS Posted at: 2018-03-07T19:00:43.004Z Reads: 122

```
[quote="Hummie, post:76, topic:48126"]
they look pretty legit to me.  find me something showing otherwise.   but discharge testing is hard to find.
[/quote]
Again, good luck. Lol
```

---
## \#79 Posted by: Hummie Posted at: 2018-03-07T19:05:34.386Z Reads: 125

```
on endless-sphere they're still doing discharge testing but other than that people who got them seem happy.
ive moved on from the headway and the watthours to dollar of the fullriver surely trumps as well as cyclelife
```

---
## \#80 Posted by: PXSS Posted at: 2018-03-07T19:20:13.458Z Reads: 126

```
Go buy AAs from walmart. Betcha their watthours/dollar trumps fullriver
```

---
## \#81 Posted by: Hummie Posted at: 2018-03-07T19:22:53.479Z Reads: 129

```
https://www.youtube.com/watch?v=3sPzWe3CsOM

not bad really as long as not at peak discharge too long

a good review and says get them before the great price is gone  but not good for a small board though with a pretty low discharge ability.  would need to be a pretty big pack to work half decently and they sag pretty badly

the headway are stout high power cells though
https://www.youtube.com/watch?v=MdhyOFeOqyE

but the steal of a deal is gone
https://www.ebay.com/itm/183036308132?ViewItem=&item=183036308132
but seeing how low these headway HP cells can be is encouraging
```

---
## \#82 Posted by: Jebe Posted at: 2018-03-09T21:23:27.994Z Reads: 122

```
https://www.ebay.com.au/itm/183099679811
24 Headway 10aH for $370 Australian Delivered !
```

---
## \#83 Posted by: sk8l8r Posted at: 2018-03-10T07:37:30.664Z Reads: 122

```
my Bajaboard gen3 uses 8x Headway 40152S 15ah LiFePO4 Cell

http://www.evassemble.com/index.php?main_page=product_info&cPath=2&products_id=175

I'm upgrading to the gen4 internals (totally different battery now)  am going to have this 'spare' sounds like its worth my time reusing the cells in a new build wasn't sure till i saw this thread :) 

![image|379x500](upload://2ouXjgIgGVk65RYpf1Q5TEVr5d9.jpg)
```

---
## \#84 Posted by: b264 Posted at: 2018-03-10T08:10:02.834Z Reads: 119

```
Those are perfect for a little shortboard or old-school deck because it's hard to fit too much in there when you have like 14.5" wheelbase
```

---
## \#85 Posted by: aigenic Posted at: 2018-03-10T09:18:30.809Z Reads: 116

```
I doubt that...if the dimesnions of the cells are 40x152mm then in flat configuration the pack would have dimesions 152x320x40mm...With 368mm wheelbase (14.5") you will not be able to fit motor...
```

---
## \#86 Posted by: cosmicc89 Posted at: 2018-03-10T14:32:24.704Z Reads: 118

```
Thanks, very cool! What do you think of the pack? Pretty good? 
I'm also wondering if it was difficult to mount and install such a big battery?
```

---
## \#87 Posted by: sk8l8r Posted at: 2018-03-11T09:01:28.271Z Reads: 120

```
I tested the size of 8 on my 80's Tommy Guerrero reissue they fit, would have to reverse mount motor behind the truck, was thinking hubs but I'm really enjoying belts+real wheels at the moment :)  

@cosmicc89 I've had to replace 1 cell in 2 years, I only learned about voltage sag after buying a Meepo :) 

I'm going to try mounting 8 flat on this, I have 10 in total but 10 def. wont fit :(  

![image|294x500](upload://6iKd9uWGy5j76yTqpkNNQNRZ0NK.jpg)
using the supplied holders they even cope with the decks concave :)  will take some pics later
![image|168x86](upload://uJETyrrsyjfcXjYIPdn1DLIJqZy.jpg)
```

---
## \#88 Posted by: PXSS Posted at: 2018-03-11T12:35:04.993Z Reads: 117

```
If 8 of those fit on there, have you looked at how many 18650 would fit on that same volume? You'll come out with a way better battery.
```

---
## \#89 Posted by: cosmicc89 Posted at: 2018-03-11T16:15:51.393Z Reads: 116

```
If you do end up doing it, post pictures, I'd love to see how it turns out.
```

---
## \#90 Posted by: b264 Posted at: 2018-03-11T20:09:34.138Z Reads: 113

```
That's a fly deck right there
```

---
## \#91 Posted by: Jebe Posted at: 2018-03-11T22:56:19.816Z Reads: 116

```
Did they use copper bus bars for connections? What thickness are they ?
```

---
## \#92 Posted by: sk8l8r Posted at: 2018-03-12T09:09:46.048Z Reads: 120

```
nope they screw together, when I found out I had to replace a cell I ended up here, I panicked a little when I saw some of the battery builds have to say as a first battery to have to fix it was great :)
```

---
## \#93 Posted by: cosmicc89 Posted at: 2018-03-12T14:38:59.129Z Reads: 118

```
The more I read about the Headway cells, the more I'm leaning towards them for my next battery. Since you only really need a 1p of them, they end up being similar cost to a li-ion anyway but are safer and easier to work with.
```

---
## \#94 Posted by: E1Allen Posted at: 2018-03-13T02:32:43.042Z Reads: 109

```
Like 3x heavier though.  Less range and more expensive.  However 1p and less cells.. so whichever.
```

---
## \#95 Posted by: cosmicc89 Posted at: 2018-03-13T02:35:05.171Z Reads: 109

```
I don't see the weight as too big of an issue. It would be on a trampa board, not meant to be carried anyway. 

I'm happy to give up some range for a safer, trouble free battery, though maybe I'm just paranoid.
```

---
## \#96 Posted by: E1Allen Posted at: 2018-03-13T02:35:53.520Z Reads: 113

```
Makes sense.  People are using them
```

---
## \#97 Posted by: banjaxxed Posted at: 2018-03-13T09:36:45.889Z Reads: 117

```
The weight thing is hard to get over, even on a ATB build which as far as carrying - the car boot.

What I learned from this thread though is that this could be really nice in a small deck with 1P, I'm visualising cells placed in a row down the deck with the ends pointing outwards with alternating polarity to allow a little bussbar or silcone wire to thread them together, could be mighty
```

---
## \#98 Posted by: Jebe Posted at: 2018-03-13T09:53:46.563Z Reads: 121

```
I have so many different ideas so the ability to disasemble and reasemble based on current need is really advantageous.  Will be running 10s 2 p on a trampa then strip down and run 14s 1 p for a street build then maybe a 12s2p for a go cart then maybe a 8s3p for an outboard motor.... so many different options!
```

---
## \#99 Posted by: sk8l8r Posted at: 2018-03-13T18:47:06.763Z Reads: 119

```
@banjaxxed a bit like this ... (just trying out a couple I had lying around for size) 

![image|340x500](upload://zQHC6dwo2FQw3xKchSxdehTpP4Z.jpg)

@Jebe I've started considering a battery I can swap between decks now, there is no solder at all needed to build the battery, it should be possible to create a battery you can unscrew a cell from your street board, drop in your trampa and your off (in theory) :) 

<in my head i just justified 2 more builds lol>
```

---
## \#100 Posted by: banjaxxed Posted at: 2018-03-13T21:15:00.722Z Reads: 113

```
Yeah that's it! Can you do 10a1p and electronics space wise like that? Ok I see the holders, maybe possible to stack without holders, that would be like 50mm or something. Otherwise a 'creative' layout
```

---
## \#101 Posted by: cosmicc89 Posted at: 2018-03-14T01:27:28.992Z Reads: 110

```
This would be such a killer setup!
```

---
## \#102 Posted by: sk8l8r Posted at: 2018-03-15T18:05:14.271Z Reads: 107

```
starting to wonder if I could do a 13sp1 with these cells on a bigger board hmmmmm
```

---
## \#103 Posted by: b264 Posted at: 2018-03-15T18:07:45.728Z Reads: 109

```
Finding a 46.8V charger will be the most difficult part of that
```

---
## \#104 Posted by: sk8l8r Posted at: 2018-03-15T18:11:13.535Z Reads: 113

```
if that will be the most difficult that sounds really promising 

one of these not do it?

http://www.evassemble.com/index.php?main_page=product_info&cPath=0&products_id=17
```

---
## \#105 Posted by: Colson003 Posted at: 2018-03-15T18:14:13.333Z Reads: 116

```
You don’t need to find one. You could make one:

http://www.electric-skateboard.builders/t/programmable-supply-power-60v-15a-35/36797
```

---
## \#106 Posted by: Hummie Posted at: 2018-03-15T19:36:26.204Z Reads: 110

```
or just get a bulk power supply that's adjustable!  you don't need the other fixins if this thing tells you the voltage

https://www.amazon.com/gp/product/B06ZYDZCG9/ref=oh_aui_detailpage_o00_s00?ie=UTF8&psc=1

ive got one trying to get rid of. new in box.
```

---
## \#107 Posted by: b264 Posted at: 2018-03-15T19:37:43.700Z Reads: 109

```
A power supply shouldn't be used to charge lithium cells unless it's designed to charge lithium cells.  They need a Constant Current charge until max voltage is acheived, then a Constant Voltage charge

A regular power supply does not do that.
```

---
## \#108 Posted by: Hummie Posted at: 2018-03-15T19:45:03.476Z Reads: 110

```
its not true.   that's often said but look at a charge graph  and the "constant current" is only intended to decrease the charge current but if you have cells that have no problem with the high current that your power supply is putting out you have no problem and why bother wasting your time.  Ive said this long winded thing so many times and it is a lot of info but the bulk chargers are different from a "charger" in only two ways, baring any other features that may be there beyond.    a power supply or pcu or bulk charger or whatever you want to call it is almost always "cv" and goes with ohms law to decide the current and when first charging it will put out more current than at the end of charge.  that's fine as long as the cells can take it.  
the only other lithium charger special feature is a charge cut-off when it gets very close to hitting full, which is often set at 4.20, but a power supply will let the cells float at and be constantly charging so if you set it to 4,20 it will hold them at like 4.19 forever while a "charger" will cut the current and let the cells drop back down as they do off a charge.  so they don't SIT ON 4.2 like a bulk charger power supply pcu or whatever you want to call it with just cv will do.  being on 4.2 isn't good for a cell either way it's done so that's why they cut the charge with the charger but if you were to set your bulk charger to 4.1 it can sit on that all day charging.  no problem.   you can even set it to 4.2 but having cells sitting on the 4.2 for time it is bad no matter what way it's done.

its very often done with diy ebikes

we use very high discharge ability cells almost always in a board with so little room and they also have a very high charge rate as well.  people typically are charging their cells at a fraction of the rate they could be charged and with no signs of degradation.  look at the big electric car makers, they try to charge as fast as possible and they do it and often studies show there's no significant deterioration of the batteries from it.  charging at one c is silly.

I feel safer with one of these and a hardwired wattmeter and the voltage set at 4.1 than I feel with some chargers.   most fires start when charging and faulty chargers are sometimes the cause.  I think the safest thing would be a temp sensor really...nothing is going up in flames without getting warm first.   And with lipo a bulging cell is an easy sign

but you must balance somehow with these.  a bms.  or balance discharger.  or even a quick discharge by sticking your tongue on the highest cells if you must.

theyre even calling this one a drok but still the same without cc.  
https://www.amazon.com/DROK-Adjustable-Converter-110V-220V-Transformer/dp/B0716XVR7P/ref=pd_sbs_23_1?_encoding=UTF8&pd_rd_i=B0716XVR7P&pd_rd_r=B0G043WXXYZ747486SYF&pd_rd_w=UtTti&pd_rd_wg=B4sIQ&psc=1&refRID=B0G043WXXYZ747486SYF

I recommend getting one with a higher voltage than you'll be using it for too for some safety headroom so it doesn't break.
these ones with the golden adjustable knob rock and have a voltage screen that's pretty accurate.  off by .2v
```

---
## \#109 Posted by: cosmicc89 Posted at: 2018-03-15T20:02:48.390Z Reads: 108

```
These power supplies are great, I use one with a BMS to charge Lipo cells, works quite well, no issues at all.
```

---
## \#110 Posted by: Hummie Posted at: 2018-03-15T20:04:37.908Z Reads: 107

```
and you can probably charge at like 5 times as fast as any "charger" available and I wouldn't say it's any less safe AS LONG AS YOU ARE AWARE OF EACH CELL'S VOLTAGE.  I stick on a 15$ cell tester/discharger and I'm aware of whats going on and discharging the highest cell slowly too
```

---
## \#111 Posted by: b264 Posted at: 2018-03-15T20:05:43.849Z Reads: 107

```
What you two (@Hummie @cosmicc89 ) are talking about is dangerous if not done correctly, and encouraging others to do it is negligent at least and malice at most.  If folks know enough about electric to know when it is and is not safe, then they don't need to know this.

All this will do is cause an accident.

Please be responsible.
```

---
## \#112 Posted by: cosmicc89 Posted at: 2018-03-15T20:07:05.233Z Reads: 103

```
How will charging cells with a BMS and a power supply cause an accident?
```

---
## \#113 Posted by: Hummie Posted at: 2018-03-15T20:07:22.316Z Reads: 102

```
but if someone is capable of figuring what voltage their cells are at ...and know that they cant go over 4.20....what else is there to know?
```

---
## \#114 Posted by: b264 Posted at: 2018-03-15T20:07:25.344Z Reads: 96

```
If you need to ask, don't do it.  Only use lithium chargers.
```

---
## \#115 Posted by: cosmicc89 Posted at: 2018-03-15T20:08:09.210Z Reads: 96

```
so you're saying that boosted board, hover boards, literally every electric bike ever, etc etc are all dangerously charging?
```

---
## \#116 Posted by: Hummie Posted at: 2018-03-15T20:08:46.879Z Reads: 95

```
do you know the difference between the two?  because it's almost the same and the safety of CC is a waste of time, and the charge cut-off..is also unless the cells are charged to full charge.  even having fully charged cells sitting around is worse than having them sit on 4.1 all day
```

---
## \#117 Posted by: b264 Posted at: 2018-03-15T20:08:47.277Z Reads: 92

```
No, because they use lithium chargers that have a constant current mode.  Don't change what I said.  I said what I said and nothing about Boosted.
```

---
## \#118 Posted by: Hummie Posted at: 2018-03-15T20:09:16.798Z Reads: 94

```
but constant current is just a current limiter...but we have cells that will do like 4x more.  
look at the charge ability of your cells
```

---
## \#119 Posted by: b264 Posted at: 2018-03-15T20:10:27.448Z Reads: 98

```
[quote="Hummie, post:118, topic:48126, full:true"]
but constant current is just a current limiter…but we have cells that will do like 4x more

look at the charge ability of your cells
[/quote]

*You literally have no idea what cells people have who might be reading this.*  Look at your own cells -- but don't make foolish suggestions that will cause someone else to have an accident.  You certainly don't know what cells I have.
```

---
## \#120 Posted by: Hummie Posted at: 2018-03-15T20:11:42.715Z Reads: 94

```
I'm not pandering to the incompetent.  if someone cant figure out what their cells are capable of charging at they shouldn't be doing anything.  knowledge is a good thing.
```

---
## \#121 Posted by: Hummie Posted at: 2018-03-15T20:16:03.003Z Reads: 87

```
especially as we're talking about iron cells....I think we'd have a hard time blowing them up no matter how incompetent we were or what rate we charged them at
```

---
## \#122 Posted by: scepterr Posted at: 2018-03-15T20:16:50.970Z Reads: 88

```
I think if people are capable and knowledgble enough to come up with their own charging solutions, that's fine, but the recommendation otherwise should be the safest and most simple option
```

---
## \#123 Posted by: Hummie Posted at: 2018-03-15T20:21:36.173Z Reads: 87

```
how are they going to become capable and knowledgeable enough if they aren't given the knowledge.  this isn't the builders-lite forum....we're here to figure out what is going on.   I bet you 99 percent of the people on this forum could charge their cells safely at double the rate if not more but they either cant find a charger to do it, or cant even find a 12s charger period, or are unaware of what safe is.  it's not unsafe to charge you cells with way more current and with a much cheaper device and while totally within the guidelines of the manufacturers.  but you have to at least know what cells you have and what they can do.
```

---
## \#124 Posted by: cosmicc89 Posted at: 2018-03-15T20:24:33.136Z Reads: 84

```
I would still like to be educated in how a standard DC switching power supply regulated by a BMS is dangerous. I never got an answer, only that I apparently shouldn't be asking.
```

---
## \#125 Posted by: Hummie Posted at: 2018-03-15T20:34:16.617Z Reads: 90

```
[quote="b264, post:107, topic:48126, full:true"]
A power supply shouldn’t be used to charge lithium cells unless it’s designed to charge lithium cells.  They need a Constant Current charge until max voltage is acheived, then a Constant Voltage charge

A regular power supply does not do that.
[/quote]

not wanting to sound like a dick but wanting to get the details clear: 
  the constant current mode goes until it can get to a constant voltage mode and not be putting out too much current, and then it will not be fully charged yet but charging with a cv, just like a pcu, and ohms law deciding the current, and then after it is really close to full charge and the difference in voltage is so small between the supplied voltage and the battery voltage that the current is a trickle, then a charger will shut off.   
there are only two things going on here beyond what a typical cv pcu will do.  the cc, which is OFTEN holding the charge back from what the cells could be taking, and the cut off, which is only good in that at full charge it wont be holding cells at high voltage instead of letting them drop naturally down to 4.1 or whatever where less damage is done.  any cell that has a max charge of 4.2 is not good to be sitting on 4.2 either while charging or after charging and it has the same effect.
but would like to hear contrary opinion or facts and I just pick up what I find
```

---
## \#126 Posted by: Acido Posted at: 2018-03-15T20:45:54.569Z Reads: 89

```
30Q can go up to 4A per cell in the sheets,5p pack and thats 20 fucking charging amps
```

---
## \#127 Posted by: Kug3lis Posted at: 2018-03-15T21:04:35.267Z Reads: 90

```
Most cheap ass BMS does not regulate charging at all... It will keep pushing until you disconnect it or like Li-Ion chargers, they turn off charging internally. So in your case, PSU will always power battery until something happens ;)

This does not apply BMS with MCU (like @JTAG DieBieMS)  which controls charging ;)
```

---
## \#128 Posted by: cosmicc89 Posted at: 2018-03-15T21:09:26.949Z Reads: 90

```
Thanks for the reply.

Doesn't the BMS stop bulk charging once it goes into balancing mode or when the pack's total voltage reaches the charger's total voltage?
```

---
## \#129 Posted by: Kug3lis Posted at: 2018-03-15T21:12:05.002Z Reads: 93

```
I don't know if I am correct but as much as I looked in the one people uses here (without can/uart/bluetooth or etc) does not even care what kind of voltage you use for charging. The balancing is a purely standalone single cell balancer chip which does not give a shit about anything around and MOSFET switch for overcurrent/under voltage shutdown.
```

---
## \#130 Posted by: b264 Posted at: 2018-03-15T21:14:54.410Z Reads: 94

```
[quote="cosmicc89, post:128, topic:48126"]
Doesn’t the BMS stop bulk charging once it goes into balancing mode
[/quote]

Yes, it slows it to 50mA, I think

[quote="cosmicc89, post:128, topic:48126"]
or when the pack’s total voltage reaches the charger’s total voltage?
[/quote]

I don't think so
```

---
## \#131 Posted by: lock Posted at: 2018-03-15T21:16:30.578Z Reads: 95

```
I’ve been using a [Meanwell LED driver](http://www.meanwell.com/webapp/product/search.aspx?prod=ELG-150) to charge my LiFePO4 pack. Adjustable voltage and current (just make sure you select the appropriate option). It operates in a CC/CV mode. I’m honestly not sure how it differs from a ‘proper’ charger, but the guys over on endless sphere seem to hold them in high regard.

Worked out well. Originally selected a model to exactly match the voltage of my 12s only to find out that it needed to supply an extra 3v for the DieBieMS to start charging. Adjusting the potentiometer fixed this up in no time.
```

---
## \#132 Posted by: b264 Posted at: 2018-03-15T21:17:48.581Z Reads: 87

```
Those look like they'd work very, very well.
```

---
## \#133 Posted by: b264 Posted at: 2018-03-15T21:19:19.068Z Reads: 86

```
@sk8l8r This ELG-150-48 will charge a 13S1P LiFePO4 battery
```

---
## \#134 Posted by: cosmicc89 Posted at: 2018-03-15T22:08:08.578Z Reads: 81

```
@b264 any input on the quality of Supower CC/CV chargers? Looking at this one:

http://www.batterysupports.com/36v-438v-5a-lifepo4-battery-charger-12s-12x-32v-life-charger-p-161.html
```

---
## \#135 Posted by: b264 Posted at: 2018-03-15T22:09:14.217Z Reads: 82

```
I haven't used them, but it's definitely the correct thing
```

---
## \#136 Posted by: Hummie Posted at: 2018-03-16T01:01:43.132Z Reads: 87

```
[quote="cosmicc89, post:128, topic:48126"]
doesn’t the BMS stop bulk charging once it goes into balancing mode or when the pack’s total voltage reaches the charger’s total voltage
[/quote]

Almost all the bms people are using don’t stop the charge.  The pack is still being charged and all the cells in it, the only thing balancing is a resistor that is burning off power from cells that are over 4.2.  So if ur bulk charging with high power u can still be overcharging the cell if it’s way out of balance . Look at what the bms balancer is discharging and mostly very little.
```

---
## \#137 Posted by: Hummie Posted at: 2018-03-16T01:08:28.952Z Reads: 87

```
There’s nothing incorrect about using a cv power supply or even without a charge cutoff when full.  Done all the time.  U can blow ur stuff up either way.
```

---
## \#138 Posted by: cosmicc89 Posted at: 2018-03-16T01:26:09.551Z Reads: 83

```
Makes sense, thanks. 

A Li-ion charger then has the advantage of stopping charge when the current cycle is done?
```

---
## \#139 Posted by: Hummie Posted at: 2018-03-16T01:30:21.918Z Reads: 85

```
Lithium charger yes. So U could charge to 4.2 a cell and it will cut off. If u don’t have the cutoff and charge to 4.2 then the cells will sit on 4.2 which it’s not good to do.  But just as bad as having a cell that’s not on a charger sitting on ur shelf at 4.2. The cut off allows the cell to drop back down as soon as it hits 4.2. Typically when charging to 4.2 if u pull it from the charge it drops down to maybe 4.15 and nicer for the cell

So charging to full 4.2 is much safer
```

---
## \#140 Posted by: b264 Posted at: 2018-03-16T02:13:20.779Z Reads: 86

```
[quote="Hummie, post:136, topic:48126"]
Almost all the bms people are using don’t stop the charge.  The pack is still being charged and all the cells in it, the only thing balancing is a resistor that is burning off power from cells that are over 4.2.  So if ur bulk charging with high power u can still be overcharging the cell if it’s way out of balance . Look at what the bms balancer is discharging and mostly very little.
[/quote]

I don't think that's how it works.  Once the BMS goes into balance mode, it does stop charging that cell, and, furthermore, limits the entire pack's charge current, even for cells that aren't full yet.
```

---
## \#141 Posted by: PXSS Posted at: 2018-03-16T02:29:05.395Z Reads: 83

```
Oh god.....
```

---
## \#142 Posted by: Hummie Posted at: 2018-03-16T02:49:36.052Z Reads: 88

```
  all the ones ive seen I think they keep charging and once a cell goes over 4.20 that cell alone is hooked to a resistor that burns the current off at the same time.  stuff going in and out at the same time

don't think there is a balance mode
```

---
## \#143 Posted by: Hummie Posted at: 2018-03-16T03:40:20.445Z Reads: 91

```
wait no.  the "current" cycle is just a limiting of current.  once the pack voltage has come up enough then it will go into the cv stage which is where it's just following ohm's law and tapering down in current as it comes to the set voltage.  just like a pcu at that point, until it cuts off current when it gets to a really small trickle, which the pcu wont do
```

---
## \#144 Posted by: b264 Posted at: 2018-03-16T04:26:45.908Z Reads: 89

```
If you don't know how they work or what's happening, I'm confused why you are trying to give advice.
```

---
## \#145 Posted by: E1Allen Posted at: 2018-03-16T04:32:34.404Z Reads: 90

```
http://www.electric-skateboard.builders/t/cheap-chargers-with-customizeable-end-of-charge-voltage/6902


Migrate
```

---
## \#146 Posted by: Hummie Posted at: 2018-03-16T04:34:09.223Z Reads: 84

```
what do you think I don't understand and what advice do you think i'm writing that is wrong?
looking at what you wrote I feel like I should be giving you advice as youre writing about lithium chargers but seems you don't know what the difference between them and a pcu is.  telling people not to charge lithium without a lithium specific charger...yea I think that's bad advice
```

---
## \#147 Posted by: b264 Posted at: 2018-03-16T04:36:25.063Z Reads: 88

```
[quote="b264, post:107, topic:48126, full:true"]
A power supply shouldn’t be used to charge lithium cells unless it’s designed to charge lithium cells.  They need a Constant Current charge until max voltage is acheived, then a Constant Voltage charge

A regular power supply does not do that.
[/quote]

[quote="Hummie, post:108, topic:48126"]
its not true.
[/quote]

Because I'm still on this.  Every time I correct one thing, you say ten more things that aren't true.  I'm not spending all night correcting you.  You still didn't listen to the first thing.
```

---
## \#148 Posted by: Hummie Posted at: 2018-03-16T04:37:30.347Z Reads: 82

```
they don't need constant current!  they don't need a shut off at full charge!  what else is there to say
```

---
## \#149 Posted by: b264 Posted at: 2018-03-16T04:38:34.783Z Reads: 86

```
I have lessons available for $100/hr.  PM if interested.
```

---
## \#150 Posted by: Hummie Posted at: 2018-03-16T04:39:50.536Z Reads: 91

```
to tell me what?  if you want I can link you to many discussions of people using bulk chargers to charge lithium.  I can also link you to discussions of the difference between a bulk power supply and charger and what cc is.  you can tell me here if you have something to say. ?
```

---
## \#151 Posted by: Hummie Posted at: 2018-03-16T04:40:27.828Z Reads: 96

```
and tell me the ten things I said that aren't true. 

hum no facts just talk telling me I don't know the facts!  bring it!!!
```

---
## \#152 Posted by: BoostedBuilder Posted at: 2018-04-17T17:27:54.464Z Reads: 90

```
Anyone interested in 12 x A123 cells from a recalled Boosted battery?  I don't know if they are worth much, so offer me something if interested : )

![20180417_175152|374x500](upload://78y1epbd59SasNLBKb0MueJEAdI.jpg)
```

---
## \#153 Posted by: b264 Posted at: 2018-04-17T17:32:23.673Z Reads: 87

```
What are the dimensions of those 6S1P bricks
```

---
## \#154 Posted by: BoostedBuilder Posted at: 2018-04-17T17:39:21.254Z Reads: 92

```
157mm x 68mm x 28mm

I can print you anything, for any configuration if you send me the designs.
```

---
## \#155 Posted by: Hummie Posted at: 2018-05-17T22:33:43.444Z Reads: 90

```

super cheap high discharge soft rectangles.

https://www.ebay.com/itm/20-SPIM08HP-3-7V-8AH-LITHIUM-POLYMER-BATTERIES-25C-200A-SUPER-CELLS-24V-36V-48V/173305036284?_trkparms=aid%3D888007%26algo%3DDISC.MBE%26ao%3D1%26asc%3D50543%26meid%3D89127248bd3a40cfb0099a0ee15daed1%26pid%3D100009%26rk%3D1%26rkt%3D1%26sd%3D112825062264%26itm%3D173305036284&_trksid=p2047675.c100009.m1982
```

---
## \#156 Posted by: aigenic Posted at: 2018-05-18T05:25:15.871Z Reads: 88

```
Hey boosted,
Do you still have the batteries? where are you from? How much for them?
```

---
## \#157 Posted by: BoostedBuilder Posted at: 2018-05-18T06:24:56.185Z Reads: 90

```
Yeah, still have them. I'm in Switzerland. I don't know, how much are you willing to pay for them?

I just ordered some heatshrink for the batteries, should be here in a week or two.
```

---
## \#158 Posted by: aigenic Posted at: 2018-05-18T08:36:56.555Z Reads: 90

```
Ok, give me week or two, I need to decide if i need them or not...in case someone else will be interested in them meanwhile, do not hesitate to sell it to him...
```

---
## \#159 Posted by: akelly Posted at: 2018-05-18T08:46:48.077Z Reads: 91

```
I have a lot of used A123 26650 LiFePo4 cells, pulled from a grid scale energy storage plant in 12S 8P packs. I'm putting some in my own board but I have way more than I need. [Here's the datasheet for the cell](http://lib.store.yahoo.net/lib/buddipole/ANR26650M1A-Datasheet-APRIL-2009.pdf), I have measured the capacity on half a dozen cells and they've all come in at 1400mAh so far. [Packs look like this.](https://www.ebay.com/itm/A123-Systems-Lithium-Ion-Cells-ANR26650M1A/222961186068)

![image|666x500](upload://pIZNw2AL5u54RoS6bJvlHCgJEch.jpg)
I still haven't figured out how to measure the capacity of the whole pack effectively, but I can easily measure the resting voltage of each parallel bank, and I'm making a circuit board that can measure the capacity of a bunch of individual cells independently. Anyone interested?
```

---
## \#160 Posted by: banjaxxed Posted at: 2018-05-18T09:06:26.911Z Reads: 90

```
hi what's your location? Member-wise we're split between EU Vs US/Can mostly. 
Flying these is not easy, no ship/overland route to EU anymore using uSPS sadly
```

---
## \#161 Posted by: akelly Posted at: 2018-05-18T09:08:15.320Z Reads: 90

```
I'm in San Francisco US, so yeah, shipping to the EU probably isn't feasible.
```

---
## \#162 Posted by: banjaxxed Posted at: 2018-05-18T09:09:03.324Z Reads: 92

```
:persevere::disappointed_relieved::sob::sob::anguished::anguished::scream::crazy_face:

Frisco gets all the neat stuff

For the guys in your hemisphere -
Are they welded in those cage?
How old?
Capacity of a pack/cell average would be great
```

---
## \#163 Posted by: lock Posted at: 2018-05-18T09:20:33.895Z Reads: 96

```
[quote="akelly, post:159, topic:48126"]
come in at 1400mAh
[/quote]

Typo? ... 2400mAh?  If they're getting only 1400 they've probably been around a while.

I paid a bit over 300 for the 24 in my board, unfortunately I'm in Australia otherwise I'd be all over it 😩.
```

---
## \#164 Posted by: akelly Posted at: 2018-05-18T09:29:36.336Z Reads: 94

```
1400mAh is not a typo, they were 2300mAh new. It might have just been the ones I tested, they were all part of one parallel group so I need a larger sample size. I'm willing to sell these pretty cheap because of the capacity though. I'll have to check the date codes when I get home, but I think they were made in like 2010. Yes they're spot welded into the pack, a group of us with these batteries have developed a method to tear them down, but it still takes a while.
```

---
## \#165 Posted by: banjaxxed Posted at: 2018-05-18T09:36:46.758Z Reads: 93

```
Probably better for a powerwall TBH
```

---
## \#166 Posted by: Hummie Posted at: 2018-05-18T17:06:40.133Z Reads: 97

```
repeat spam!:
https://www.ebay.com/itm/4-SPIM08HP-3-7V-8AH-LITHIUM-POLYMER-BATTERIES-25C-200A-SUPER-CELLS-24V-36V-48V/183036786061?_trkparms=aid%3D222007%26algo%3DSIM.MBE%26ao%3D2%26asc%3D44040%26meid%3D750ce93d5fe243ed8cfab1c9bcdc69e3%26pid%3D100623%26rk%3D2%26rkt%3D6%26mehot%3Dpp%26sd%3D173305036284%26itm%3D183036786061&_trksid=p2047675.c100623.m-1

  this is more energy and likely more power than anything on hobbyking and will likely last way way longer and cheap.  theres a couple options of cell quantity and maybe 14 would be ideal.  surprised more people arent syched on these.  nothing like them around Ive seen.  wont fit my board unfortunately.
```

---
## \#167 Posted by: b264 Posted at: 2018-05-18T17:23:29.822Z Reads: 90

```
Anyone who writes in all capital letters is trying to rip you off.
```

---
## \#168 Posted by: Hummie Posted at: 2018-05-18T17:29:16.998Z Reads: 87

```
great reviews.
```

---
## \#169 Posted by: deucesdown Posted at: 2018-05-18T23:36:51.507Z Reads: 87

```
Need more info, othewise it's a gamble. Questions like, What's internal resistance like? How consistent cell to cell? How many amps can they push continuously without getting hot? What do they look llike after 50 cycles? After 150? 300? What happens if you overcharge or overdischarge?

If you have links to reviews with data I'm super curious as usual. :)
```

---
## \#170 Posted by: telnoi Posted at: 2018-05-19T05:50:04.046Z Reads: 83

```
Hints of scamming behavior when looking at the negative ebay user reviews / selling second hand as refurbished, lower actual mah, no refunds.
```

---
## \#171 Posted by: Hummie Posted at: 2018-05-19T15:50:27.112Z Reads: 81

```
in my enthusiasm I bought two sets of these 20 cells and then realized they wouldn't fit my deck and returned them within an hour.  no prob.  but I'll look into the cells and reviews more.  the reviews seem damn good but haven't looked through the bad ones.  i don't think second-hand need necessarily be a sign of a scam.  i'll update this post when I read more.



there is no negative feedback and all good reviews.  cells tested for capacity and described as "like new"
```

---
## \#172 Posted by: telnoi Posted at: 2018-05-19T16:54:19.773Z Reads: 84

```
That was based on the user account, not the sales for this specific cell.

On endless sphere you will find a few reviews. What is common is that the capacity differs between cells, some being as low as 7000 while others are 9000. Also mentioned that capacity may increase after a few cycles.
```

---
## \#173 Posted by: Hummie Posted at: 2018-05-19T17:26:23.584Z Reads: 82

```
Can u link the endless-sphere thread please.  There are some reviews of the cells on eBay under the many diff listings and all I saw were good

https://endless-sphere.com/forums/viewtopic.php?t=93103
Looks all good from the little info here.
```

---
## \#174 Posted by: telnoi Posted at: 2018-05-19T17:30:15.533Z Reads: 84

```
Google the battery type and you will come across those. Can only use one hand/takes a shitload of time for me.
```

---
## \#175 Posted by: jbc289100 Posted at: 2018-11-15T01:14:29.976Z Reads: 56

```
![0916182017|281x500](upload://301wxzdcKW4E92PBr6PWmOvIlNh.jpeg)  This is a fully assembled and balanced 4s10p 80ah battery built with the SPIM08HP'S. As you can see it is sitting at 14.8 volts and has a very low internal resistance. I have been testing these for over 6 months. All cells were tested for capacity, cycled and parallel balanced before assembly. So far the highest load I have hit them with is 1000 amps and that tester didn't survive. I had a .8 volt drop from nominal voltage on that same draw and after the test completed, rebounded right back up to 14.7.
```

---
## \#176 Posted by: jbc289100 Posted at: 2018-11-15T01:15:21.717Z Reads: 56

```
![IMG_20180929_155553841|666x500](upload://lTsYgPTD4OSUIkx0qGUG5K5U6J6.jpeg)
```

---
## \#177 Posted by: jbc289100 Posted at: 2018-11-15T01:15:54.536Z Reads: 57

```
![IMG_20180929_155546569|666x500](upload://w1exCbRZhOEqAApfLlrBO5STpeZ.jpeg)
```

---
## \#178 Posted by: deucesdown Posted at: 2018-11-15T01:18:10.553Z Reads: 56

```
Omg I think I got a little wood. Pics of the testing rig?
```

---
## \#179 Posted by: jbc289100 Posted at: 2018-11-15T01:20:22.362Z Reads: 57

```
I hit this battery with a 500-600 amp load on the daily with 300 amps of continuous charge and it have never dropped below 14.8 volts resting. As of now, it is currently sitting at 15.0 volts resting and sees 15.2 volts on the charge. No issues with heat or cold. 10-20 degrees at night and in the morning it is sitting at 15.0. ![IMG_20180927_081136197|375x500](upload://lfsWLhNM0GVCnRQL4ddW7ByOMUk.jpeg)
```

---
## \#180 Posted by: jbc289100 Posted at: 2018-11-15T01:21:29.247Z Reads: 58

```
It runs my vehicle....for the past 6 months.
```

---
## \#181 Posted by: jbc289100 Posted at: 2018-11-15T01:22:54.597Z Reads: 63

```
![0527182044a|690x388](upload://y2P4gxVlNVZFzm5oEaiPwNgnZMf.jpeg) don't mind the other battery. It is no longer there. But it also powers my car audio.
```

---
## \#182 Posted by: Socrates Posted at: 2019-04-27T13:20:29.501Z Reads: 45

```
About the quality of the Headway Cells LiFePO4 model 40152S-15Ah compared with 30Q someone please could tell us if its good or not for 8s2p MTB ?

* 40152S-15Ah : Price by pc $ 20,5 Alibaba with shipping.

* Samsung 30Q : Price by pc Nkon $ 3,64 or € 3,29 with VAT.

Im thinking there isn't way yet, 30Q its much better, but LiFePO4 more safe e easy to handle it.
```

---
