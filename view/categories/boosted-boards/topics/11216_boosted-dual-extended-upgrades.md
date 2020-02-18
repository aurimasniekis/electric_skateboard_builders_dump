# Boosted Dual+ Extended upgrades

### Replies: 37 Views: 7798

## \#1 Posted by: t0mmykn1fe Posted at: 2016-10-16T04:30:44.561Z Reads: 415

```
What have you done with yours?
```

---
## \#2 Posted by: t0mmykn1fe Posted at: 2016-10-16T04:31:15.491Z Reads: 420

```
Anyone put Abec 11 Flywheels on there's?
```

---
## \#3 Posted by: KMeyerson Posted at: 2016-10-16T05:13:47.214Z Reads: 414

```
Serious loss in torque reported by someone once upon a time.
```

---
## \#4 Posted by: KMeyerson Posted at: 2016-10-16T05:16:31.591Z Reads: 409

```
I am looking into replacing the original batteries with 10Ah (more than 4x the capacity) LiFePO4 Polymer Pouches.  I'm asking @jacobbloy if he knows whether or not the 70/120Amp A123 26650 discharge is critical to the boards design. If I am correct, we can get away with 50/100Amp discharge so we can maximize our range without increasing our foot print. With that said, the additional battery capacity will cost you 5 lbs of weight.
```

---
## \#5 Posted by: KMeyerson Posted at: 2016-10-16T05:31:47.846Z Reads: 402

```
[quote="jacobbloy, post:2, topic:11217, full:true"]
They have a current limit of about 45a per ESC. The current v2 99wh battery is still 26650 a123 but the new 199wh battery is a 54.4v 18650 pack so I would say is has 2x 1.8ah 18650 in parallel in a 13s2p the battery pack has a higher voltage to combat the steep discharge curve of an 18650 so the voltage is basically regulated at the 43v mark. 

I think they they get away with peak discharge rates of 35ah per motor.  The new motor cables that they use for the v2 are rated to 40A peak.

In the current V1 Battery case you can fit 10s2p of 18650. I looked into this a while ago.
[/quote]

So I will attempt this mod and report back. I am a little worried about the charging, but we'll have to see.

Edit:
Houston, we have a problem:
* 12s1p A123 26650 Cells arranged as (26*104*195mm)
* 12s1p Proposed Battery arranged as (25*240*260mm)

So it won't just neatly fit into the old compartment. Which does suck. I wish their dimensions were accurate.  Does anyone have a dead Boosted Board Battery enclosure they need to sell? I want to take the BMS out of it...
```

---
## \#6 Posted by: lox897 Posted at: 2016-10-16T07:23:27.215Z Reads: 338

```
@jacobbloy put mtb wheels on his.
```

---
## \#7 Posted by: KMeyerson Posted at: 2016-10-16T18:04:08.492Z Reads: 339

```
Damn, they have a next-level battery pack. Modding that is a no go.

The "What's inside" youtube show reveals the BMS. Its on an entirely different level than our DIY boards (I guess automotive engineers can do a lot better with time/resources).  The cells are welded together in the 1*4*3 grid but the solder tabs also stick up vertically. The rests directly on top of the cells and attaches to these tabs thus creating a battery unit.

Adding/Replacing batteries to this unit is not going to work. If I could get my hands on a dead boosted board battery, I would try it. The can bus/communication is probably required for the board which is why other boosted battery mods just connect to the ESC side's power leads.
```

---
## \#8 Posted by: Pantologist Posted at: 2016-10-16T18:11:35.810Z Reads: 326

```
I doubt the info Jacob has is correct. He has no idea. It would be cheaper and more logical to fit a 10S2P pack of 18650 2.5Ah cells. That equals it around 180Wh. Boosted usually rounds up a bit.
```

---
## \#9 Posted by: Pantologist Posted at: 2016-10-16T18:12:30.010Z Reads: 323

```
12S 10Ah cells will not fit under the board.
```

---
## \#10 Posted by: KMeyerson Posted at: 2016-10-16T18:34:12.003Z Reads: 331

```
You're making massive assumptions here. Please do some googling first before you make blind accusations.

I have connections with manufacturers from designing SAE Formula Cars in school.  Long story short, I can get LiFePO4s in about every shape you could ask for in various capacities and draws. To only see batteries in cylindrical shapes is your downfall because of how much space they waste.

I just checked, even without direct manufacturer connects you can buy "LiFePO4 Polymer Pouches" on eBay, Alexiexpress, BatterySpace, etc. 

To further prove my point, check out the below information I got from about 2.5minutes of surfing the first page of google.

**_Off the shelf Pouch Specs ([8 Cells for $70](http://www.a123rc.com/goods-1677-2015+lifepo4+8PCS+X+32V+33AH+30c+POUCH+CELLS+.html)):_**

Dimensions: 127x50x8.2 mm (3x, 2x, 2x for a total of 12s in the Boosted compartment of 26x102x260mm)
Weight: 100g (24g or 32% increase in weight compared to A123 26650)
Capacity: 3.3Ah (1Ah or 30% increase in capacity compared to A123 26650)
Max. Charge Rate: 1C (or 3.3amp)
Recommend Continuous Discharge Rate: 30C (99amp)
Pulse Discharge Rate: 50C (165amp)
Above charge/discharge are very similar to A123 cells for our purposes.


And in response to the first comment,

18650 cells are just as space wasting as 26650 cells. We chose to rely on them because they do not require any skills or prior knowledge to assemble. Their discharge rates may not be sufficient for the motors and since LiFePO4 chemistry has some short comings where density is concerned (very safe though), Jacobs battery specs make sense.
```

---
## \#11 Posted by: Pantologist Posted at: 2016-10-16T19:52:55.070Z Reads: 289

```
12 10Ah pouches will not fit in the same enclosure. Yeah 3.3Ah pouches will fit according to their dimensions. 

Not sure why you think I can only think in terms of cylindrical batteries... But okay.

We'll see what Boosted actually ended up putting in the extended range. 18650s are definitely easier to assemble. I think Boosted would continue to use cylindrical cells considering they struggle to maintain demands for orders even with the standard range.
```

---
## \#12 Posted by: KMeyerson Posted at: 2016-10-16T20:05:44.829Z Reads: 284

```
If the compartment was not so fixed in shape (thanks to its fiberglass construction), we could actually have crammed the 10Ah cells into the foot print of the enclosure. Not necessarily into the current battery compartment.

I find polymer pouches are harder to regulate but much easier to produce.  Given their strict QC, they're doing quite well.
```

---
## \#13 Posted by: Pantologist Posted at: 2016-10-16T20:10:07.169Z Reads: 278

```
I'm going to be honest. I don't see the point in doing all this work for a Boosted Board. If you want more range, I'd just developed a way to quick mount another parallel pack of A123s right next to the motor housing.
```

---
## \#14 Posted by: KMeyerson Posted at: 2016-10-16T20:24:46.118Z Reads: 271

```
The appeal of the Boosted Board is its streamlined appearance. You've got to admit, they built a killer body. The battery unit is surprisingly well sealed.

If I were to pursue this further, I would create another 12s1p pack as you suggested and connect it to the main board by tapping into the flat braids under the grip tape, not by soldering it to the ESC as popular mods would suggest. The problem is again how the Boosted boards aesthetic is reduced.  Honestly, I got the board for science. Now I'm selling it.  I only wish I could get my hands on a Carbon GT next.
```

---
## \#15 Posted by: t0mmykn1fe Posted at: 2016-10-16T20:35:49.868Z Reads: 261

```
Nice, let me know how you go.

I like the idea of the boosted board due to the amount of positive / lack of negative comments in respect to the battery sag and controller disconnection.

Just need a safe board after a recent faceplant lol
```

---
## \#16 Posted by: Mr_Mahal Posted at: 2016-10-19T00:25:46.749Z Reads: 243

```
I injured myself more on the GT than the Boosted in a matter of months/weeks. It's a thrilling machine, but it has it's quirks that some aren't willing to tolerate. I sold it since I don't need it for my commute to work anymore. Bought another Boosted and really missed the ease of use and weight.
```

---
## \#17 Posted by: t0mmykn1fe Posted at: 2016-10-19T00:53:47.602Z Reads: 248

```
Where are you based?
Not sure their shipping the Boosted board to Sydney Australia yet......
```

---
## \#18 Posted by: maxz Posted at: 2016-10-19T08:50:05.052Z Reads: 256

```
I don't know about australia but in NZ they have youshop which is a store based in the US that ships stuff to NZ. So if a product only ships to US we can use youshop. Maybe you have something similar?
```

---
## \#19 Posted by: boostedboard Posted at: 2016-10-22T13:03:19.324Z Reads: 249

```
Esk8 I watched all of ur vids and even saw you snap your evolve. Make more vids if u could!
```

---
## \#20 Posted by: evoheyax Posted at: 2016-10-22T16:29:10.416Z Reads: 242

```
[quote="KMeyerson, post:7, topic:11216"]
What's inside" youtube show reveals the BMS. Its on an entirely different level than our DIY boards (I guess automotive engineers can do a lot better with time/resources)
[/quote]


What makes you think it's on another level? It's closed sourced, runs in BLDC, not FOC. I don't see what's better about it (other than possibly size). Sinosidol waves are just better than trapezoidal waves, which is why I think the vesc is better.
```

---
## \#21 Posted by: KMeyerson Posted at: 2016-10-22T18:32:13.753Z Reads: 231

```
I actually believe it might be using FOC for low speed torque control. The boards are dead silent until you get around 11mph. 

I cannot speak for the ESC since i haven't seen the top or bottom of it, but the BMS system is incredible both in physical design and hardware. Essentially the 12 cells are welded with outward extending tabs. Thus the PCB slides on top of the battery such that the tabs fit through the PCB and are soldered then and there (virtually no balance leads), I believe each cell may feature thermal sensors, etc.  Boosted's use of the can bus isn't just to relay battery status. Their PIC based ESC has a primitive elegance at the ESC side making it a very inexpensive component to repair and replace. I believe that unlike the VESC which burns out all the time, the processing and bluetooth radio/nunchuck/remote and primary functions such as the odometer are actually integrated into the STM based BMS which is in a watertight container.

The ESC is very expendable and costs very little to replace because the BMS unit is the actual processing unit/brain. The ESC acts like a trained muscle - take input and modulate motor speeds and report back to the battery.

This is how an electric car works - its focused on the battery side, not on the motor side. Motors are cheap and easy to replace, batteries no so much. Their use of automotive grade components and design is not a coincidence.
```

---
## \#22 Posted by: evoheyax Posted at: 2016-10-22T18:59:00.900Z Reads: 208

```
[quote="KMeyerson, post:21, topic:11216"]
I actually believe it might be using FOC for low speed torque control.
[/quote]

I don't remember where I saw it, but boosted stated somewhere that their controller runs in BLDC. The sensors are why it has better torque at low speeds. Any specialized specific design should be better in a sense than a generic design. The tabs sound cool. But if a cell breaks, it can be more work to replace.

I've had issues with low quality vescs, never with a chaka vesc. I have 8 chaka vescs, and never had any issues. So to say they brn out all the time is not true.

How is the ESC expandable?

And why would you do logical processing on the BMS?

The ESC is generally the brain. When your doing calculations, you want the shortest bus possible. Separating this to the BMS via cables from the esc would slow the processing speeds way down (this is why you have multiple layers of cache on a processor for example)
```

---
## \#23 Posted by: Pantologist Posted at: 2016-10-22T19:24:52.332Z Reads: 193

```
[quote="KMeyerson, post:21, topic:11216"]
The ESC is very expendable and costs very little to replace because the BMS unit is the actual processing unit/brain. The ESC acts like a trained muscle - take input and modulate motor speeds and report back to the battery.
[/quote]

Yea I doubt this is case too. Their ESC looks like a full fledged unit to me. The BMS is also a smart BMS that lets the BMS and ESC communicate with each other.
```

---
## \#24 Posted by: KMeyerson Posted at: 2016-10-22T21:20:46.039Z Reads: 186

```
I'm thinking about this from a cost perspective.  When my board comes back with new motors, I plan to measure the Bluetooth signal. I suspect it'll be inside the BMS.
```

---
## \#25 Posted by: Pantologist Posted at: 2016-11-03T18:16:13.464Z Reads: 188

```
[quote="KMeyerson, post:10, topic:11216"]
Jacobs battery specs make sense.
[/quote]

I just found out that the V2 charger is outputting 50v. Safe to assume they are using a 12S2p battery now. 

Weird noise coming from V2 charger since day 1, possible cause of battery issues?

https://www.reddit.com/r/boostedboards/comments/5awu54/weird_noise_coming_from_v2_charger_since_day_1/
```

---
## \#26 Posted by: KMeyerson Posted at: 2016-11-07T03:17:40.357Z Reads: 172

```
Nevermind then. Voltage sag will continue to be a pain in cold weather.

No. Your listening to the buck converter switching action and probably some degree of harmonics caused by the EMF of switching system.

I suspect their cell quality suffered from counterfeit A123s OR the cell ratings for dis/recharge 18650 have a fraction of the 26650 dis/recharge and their math didn't account for this some how. Weird thing is, LiFePO4 can take a LOT of abuse before they get dangerous. Its a real mystery.
```

---
## \#27 Posted by: Pantologist Posted at: 2016-11-07T03:24:52.886Z Reads: 175

```
[quote="KMeyerson, post:26, topic:11216"]
I suspect their cell quality suffered from counterfeit A123s OR the cell ratings for dis/recharge 18650 have a fraction of the 26650 dis/recharge and their math didn't account for this some how. Weird thing is, LiFePO4 can take a LOT of abuse before they get dangerous. Its a real mystery.
[/quote]

100% doubt they are counterfeit. They buy directly from A123 at this point. Tens of thousands of cells can be purchased directly. 

LiFePO4s only last a few charge cycles if overcharged to 5v.(US Military study did an overcharge test with A123 18650s) If they are not limiting the charge current properly on the 50v charger, then the LiFePO4s will be charged to 4.2-4.5v. After about 10 charge cycles I am guessing that the cells are deteriorating enough to vent with little current draw.
```

---
## \#28 Posted by: KMeyerson Posted at: 2016-11-09T02:47:52.193Z Reads: 149

```
Good find on the study, got any links? I love LiFePO4 research.

Sourcing is a thing. The cells are made overseas. People swap goods all the time unfortunately, sometimes in the loading bay.
```

---
## \#29 Posted by: Pantologist Posted at: 2016-11-09T02:59:32.761Z Reads: 147

```
They are made in China, yes, but that doesn't mean someone is going to replace tens of thousands of cells with fakes.... 

Study: http://ecst.ecsdl.org/content/41/39/1.full.pdf
```

---
## \#30 Posted by: KMeyerson Posted at: 2016-11-09T03:12:07.963Z Reads: 142

```
Consider it this way - if you had access to packaging, you could swap high value authentic cells for cheap cells that look identical. 

You'd make a huge profit per cell in USD value. Ever wonder how some elcusive parts get out of factories to 3rd parties too fast? 

This isn't a racist/country thing. Its a greed and knowing profits thing.
```

---
## \#31 Posted by: Pantologist Posted at: 2016-11-09T03:21:07.592Z Reads: 138

```
Well we'll see what Boosted discovers in their investigation.
```

---
## \#32 Posted by: KMeyerson Posted at: 2016-11-09T03:34:49.546Z Reads: 150

```
Indeed. They made a gauge announcement today.

Fingers crossed.

Batteries are everyone's problems.
```

---
## \#33 Posted by: jacobbloy Posted at: 2016-11-27T13:16:01.115Z Reads: 160

```
The new charger is 54.4v that's basically 13x 4.18v logical for boosted to not charge there batteries to 4.2v. Boosted said 199wh so 13s2p of 1.8ah batteries sounds great. or they are using 15s lifepo4 safer and better life cycles and what they currently use. the reasons for increasing voltage,  basically if they have a torque control ESC then they can draw on the voltage and also stop voltage sagging from reducing the top speeds that they provide. Every thing is regulated. You buy a v2 with a 99wh battery the pack is still the same as the V1 but the charge voltage is 54.4. They have 2 depths of the charging port one for 43.2v so you can use your V1  charger and the second for 54.4v that runs through a regulator to then drop the voltage to charge the cells. 

The v2 has gone away from a decoder and now use hall sensors. Basically sanjay told me that it was a cost compromise and they felt that the control they can get from hall sensors is still great because there ESC is made for 1 motor so they can dial in on settings and others tellemitry.

In the v2 the have a larger diameter stator but shorter. This wasn't so much about torque increase it was about heat while using a sealed motor and while increasing the amount of plastic they used on the motor mounts to again to reduce cost. The V1 mounts where heat sinks. 

This is the thing that differs many companies every one is trying to get more power, range, reduce weight while boosted are refining what they have. There battery issue sucks but there service has been great. Evolves mounts snap (could be just as bad) and they say nothing about it.
```

---
## \#34 Posted by: huntercasillas Posted at: 2019-03-29T19:05:33.516Z Reads: 39

```
I have a V1 and V2 BMS if you’re still looking.
```

---
## \#35 Posted by: Dog Posted at: 2019-07-26T04:01:10.640Z Reads: 25

```
I’m interested in dead boosted batteries. Still have it?
```

---
## \#36 Posted by: huntercasillas Posted at: 2019-07-26T04:15:24.184Z Reads: 24

```
I tossed all the parts and recycled the cells unfortunately.
```

---
## \#37 Posted by: Sn4pz Posted at: 2019-07-26T21:20:52.089Z Reads: 16

```
I've got a boosted v1 battery + BMS that won't hold a charge, a cell or multiple are likely dead. You interested?
```

---
