# Battery In Parallel - push more amps brainstorming

### Replies: 24 Views: 674

## \#1 Posted by: skatardude10 Posted at: 2019-02-01T00:34:50.135Z Reads: 169

```
I'd like to restart this discussion. 

Bottom line: there's gotta be a way to add more batteries in parallel hot swap style to push more amps on the fly. 

I've done a ton of research and reading on this forum and others, but I haven't been able to come to a conclusion, so I'd like to restart the discussion here. To be upfront, I know it's dumb, just build a bigger P pack you say, but I can't right now and I'd like to put all my extra less capable cells to use if I can.

I remember (I think it was) stooge talking about lipos and liions in parallel, and how the lipos lower resistance allows them to take all the extra amps that the liions can't safely push, just naturally.

I want to be able to parallel some old  cells to push 20-30A more on my 10S setup. 

I started to consider safe ways to limit the current drawn from the additional parallel cells, and looked into current limiting resistors. For the right kind, they are either way too bulky, can't handle enough wattage, or are prohibitively expensive... Like new 12S8P expensive, defeating the purpose... Being cheap!

My thoughts- can the wire itself limit the current? 16 guage to the additional lower amp capable pack, and 10 guage from the main pack that pushes 80A? The idea is that if the current can't pull from the higher guage wire due to increased resistance under load (gotta get the resistance just right), it will just pull the remaining current from the main pack, just as intended.

Does anyone else have any ideas how to safely limit current over one set of wires to supplement a higher current pack besides higher guage wires or current limiting resistors?
```

---
## \#2 Posted by: Gamer43 Posted at: 2019-02-01T00:43:52.048Z Reads: 160

```
I'm sorry, but this is just not a good idea.

Never mix cells of differing internal resistances in parallel. (Or in series for that matter, but it is just *slightly* less dangerous for the cells).

What ends up happening is the higher drain cells (ones with lower internal resistance) end up taking the brunt of the load and are cycled several times more frequently than the lower drain (higher internal resistance cells). 

My friend tried this, he mixed drill 18650s with laptop 18650s. **His battery pack failed (catastrophically!) within four weeks.** (the cells were testing around 90% capacity, too so they had a bit of life left in them)

And in the case of lithium-polymer vs 18650s, the lipos are already designed for high power at the cost of cycle life, using this kind of setup would just degrade their life even faster. You'll be left with dead lipos and barely cycled 18650s.

Just a by the way, the internal resistance of the cells will naturally balance the load shared between two unmatched power sources in parallel, so the less powerful power supply delivers proportionately less of the load.

My advice is always build battery packs with well-matched cells, and always keep the 20% engineering headroom rule of thumb when designing for current draw.
It's better to spend more for a working battery pack than spend less for a dead battery pack.
```

---
## \#3 Posted by: ZachTetra Posted at: 2019-02-01T01:01:23.936Z Reads: 132

```
You can have them in parallel and use 2 high voltage high amperage relays with a not signal to swap to lipos if you pull more amps than the li ions and back to the li ions when the amperage drops below...but you'd need hella anti spark and surge protection
```

---
## \#4 Posted by: Lionpuncher Posted at: 2019-02-01T01:05:44.155Z Reads: 126

```
I would recommend you not use small wires to limit the current. You’ll just end up heating the wires significantly and likely melting solder, or causing a short generally speaking. Very important to have proper sized wiring.
```

---
## \#5 Posted by: skatardude10 Posted at: 2019-02-01T01:23:01.144Z Reads: 116

```
Okay. I've been discouraged from doing this before... As much as it would be nice, I might just need to make a larger more capable pack from scratch. 

If anyone else has any thoughts though, in favor of somehow drawing less amps from one pack and more from another in parallel, please feel free to post your thoughts. The consensus seems to be strongly in favor of simplicity and designed for the purpose from the start.. I'll point out diy powerwalls though, they use all sorts of different cells, just similar total ah for each parallel group in series. I know that due to the high P # and comparatively lower amp draw per cell it's not a huge deal though.
```

---
## \#6 Posted by: ZachTetra Posted at: 2019-02-01T01:26:20.107Z Reads: 97

```
You cannot do this without a full disconnecting of one battery and connecting of the other...anything you do with them connected will degrade them
```

---
## \#7 Posted by: Gamer43 Posted at: 2019-02-01T01:38:57.252Z Reads: 104

```
If you put two battery packs in parallel, ohms law will do the load balancing for you.

Like, drill (high drain) 18650s will have like half the internal resistance of laptop 18650s (something along those lines).

This means if one were to connect a pack of drill 18650s in parallel with a pack of laptop 18650s, the load will draw twice as much current from the drill pack. e.g. load draws 30A, drill pack supplies 20A, laptop pack supplies 10A. 

If both packs have roughly equal internal resistances, and your application requires that one pack supply significantly more current than the other, then you'll have to first measure the battery packs' internal DC (maybe even AC impedance if your load involves switching) resistances and inline the appropriate low resistance power resistor(s) with the lower supply pack and deal with the power losses incurred. 
One way to measure their relevant resistance is to measure the voltage drop when connected to the load and use ohms law.
You can get 50miliohm 10W power resistors for $3 off digikey, so it wouldn't be too expensive, but 10W (14A) of power is a lot of heat that needs to be diverted away from the battery pack and power electronics.

DiY powerwalls get away with it because their current draw when in use is fairly constant, and very low compared to their maximum current output capability. It is bad for an EV because EVs don't see constant load, they see bursts of high current draw, which after some complex circuit behavior, results in the higher drain cells being cycled several times more often. 
(TBH, powerwalls aren't particularly practical except for off-grid applications, so idk if they even see ANY significant current draw when in use.)

I would still recommend building one, well-matched battery pack suited for the application, it'll cost more, but it's less work, more reliable, and won't leave you with a dead battery pack when everything is said and done.

Remember, the battery pack needs to be capable of continuous load draw, that is, the current it have to sustain for more than a minute, bursts shorter than 1s will be handled by the bypass caps, and bursts of 10-15s, shouldn't overload the batteries, but they may shorten the life by just a little a bit. 

If current capability is really needed, just go for a lipo battery pack. if you have the space, the SPIM08HPs on ebay really pack the punch at a good price.
```

---
## \#8 Posted by: skatardude10 Posted at: 2019-02-01T02:06:47.111Z Reads: 81

```
@Gamer43, thanks 

Alrighty, I'm steering away from lipo for longevity and durability, and since I intend to stay with 2wd, and 8P 30Q will max out both focboxes at 60-80A.

If I can take this another direction... Say I have an 8P group, I want to pull 120-160A. One layer of nickel strips across the P group doesn't seem like enough, or is it? I heard nickel strips don't like to weld to themselves, if I get a weak spot welder that can at most weld 0.15mm nickel strip and marginally if not not double up on 0.15mm nickel strips, do you see an issue with having a single layer of 0.15x8mm nickel connecting the 8P cells and quite a lot of braided copper soldered to the strips to bridge the S groups pushing up to 160A? 

Or should I just look for a more powerful spot welder that can sufficiently layer nickel on nickel on nickel successively more until the soldered bridge between S's
```

---
## \#9 Posted by: Gamer43 Posted at: 2019-02-01T02:10:20.049Z Reads: 70

```
How long are you trying to pull that current?

You would need 00 AWG to handle that current for more than 30s O_O.
If you can get a solid weld onto the cells, soldering some copper braid on top of the nickel doesn't sound like a bad idea. Be wary when using braid, the flux is REALLY messy, so just bare copper wire would be better.

I soldered my pack together, I probably hurt the cells a bit when I soldered the negative ends since I used solder braid and didn't do it correctly the first couple times X_X.

Pack still tests at nominal capacity :man_shrugging:
```

---
## \#10 Posted by: skatardude10 Posted at: 2019-02-01T02:17:21.597Z Reads: 65

```
Nice. Yeah, maybe 10 seconds max, conservatively?

Besides the charge wiring (fused), I've heard the thought that the lower guage, lower resistance, lower heat, less voltage drop, all the more the better. I've got a ton of 10G silicone wire, why not  buy some 8, 6, 4, 2 or 0, or some braided flat copper equivalent? People who push 300+ amps on lipo aren't just using 5mm bullet connectors for series connections are they?  I'm looking forward to mostly eliminating voltage drop cause by my wiring.
```

---
## \#11 Posted by: Gamer43 Posted at: 2019-02-01T02:28:03.945Z Reads: 66

```
It'll take a lot of space, and silicone wire at those sizes tend to get pretty expensive.

Also, it's important to make the distinction between MOTOR current and BATTERY current.
Since brushless motors are orders of magnitude better than the brushed crap you find on cheap scooters.
160A means you are applying FULL torque while at FULL speed.
But if you need full torque, but at a stand still, the motor phases see 80A, but the battery may only see 16A (going to that one motor, double if two motors). 

Unless you are going to be climbing hills at 80% of your top speed, I honestly think stripping bare some 10 AWG to solder on top of the nickel strips and 8AWG for chassis wiring would be more than sufficient. And your battery pack, at 8 cells in parallel, will handle the current draw just fine.

If you are going off-road and rough-riding, lipos are really the way to go, 18650s are just not suited for that kind of application.
When I went from 18650s to the SPIM08HPs on my mountainboard, it went VROOOOM up the hill xD.
```

---
## \#12 Posted by: Marsen Posted at: 2019-02-01T03:45:53.754Z Reads: 65

```
Batteries of similar type but of different capacity will work in parallel as the voltage across them is the same. With different internal resistance the amount of current each provides is proportional to the capacity and the SOC,state of charge, will be equal (percentage value not Ah value) 

# ASK THE EXPERTS: Batteries in Series &amp; Parallel

 

[Share](https://www.homepower.com/articles/solar-electricity/design-installation/ask-experts-batteries-series-parallel#)

[Email](mailto:?subject=HomePower.com%20Article:%20ASK%20THE%20EXPERTS:%20Batteries%20in%20Series%20&amp;%20Parallel&amp;body=Hey!%20Check%20out%20this%20article%20link%20from%20HomePower.com,%20the%20website%20of%20renewable%20energy%20and%20home%20efficiency%20technologies.%20https://www.homepower.com/articles/solar-electricity/design-installation/ask-experts-batteries-series-parallel)[Print](https://www.homepower.com/articles/solar-electricity/design-installation/ask-experts-batteries-series-parallel?v=print&amp;print=true)

By: 

[Hugh Piggott](https://www.homepower.com/profiles/hugh-piggott)

**Published In:**

Issue #122, December / January 2008

[![](https://www.homepower.com/sites/default/files/styles/article_gallery_active/public/articles/images/battery_wiring.jpg?itok=PNB8LNQS)](https://www.homepower.com/articles/image/11097/5402?width=750&amp;height=600&amp;iframe=true&amp;template=colorbox)

Two options for wiring the cells of a battery bank together.

**What happens to the battery bank capacity, and the charging and discharging characteristics, when you connect a 12-volt (V), 100 amp-hour (AH) battery and a 12 V, 200 AH battery in series? Conversely, what happens when they are connected in parallel?**

**Sid Baxter • Pocatello, Idaho**

 

Connecting two battery banks of different amp-hour capacity together in series is a bad idea. The problem is that the battery charging controls will operate based on the average battery voltage and the two batteries will have very different voltages because their capacities are different. The 100 AH battery will become fully charged long before the larger one. The combined voltage will rise, but by the time the controller turns off the charging sources, the 100 AH battery will be overcharged. Meanwhile, the 200 AH battery will not get fully charged. When the bank is being discharged, the 100 AH battery will go flat and its voltage will fall well before the 200 AH battery. The inverter will eventually cut out but not before the 100 AH battery is excessively drained.

Connecting two banks with different capacities in parallel is technically fine since the batteries will be operating at the same voltage. Charge and discharge current will be shared, based on capacity. It is best if the batteries are of the same type and age. For example, avoid combining a sealed (gel or absorbed glass mat) battery with a flooded (conventional) battery because they have different charging setpoints. Broadly speaking, you can parallel batteries without problems, and the charge controller will look after them.
As the article states paralleling different capacity cells does work. 

[quote="Gamer43, post:2, topic:82755"]
And in the case of lithium-polymer vs 18650s, the lipos are already designed for high power at the cost of cycle life, using this kind of setup would just degrade their life even faster. You’ll be left with dead lipos and barely cycled 18650s.
[/quote]
I don't understand how the LiPO's will cycle more than the Li-ion cells if that is what you mean. The cycle of charge/ discharge is voltage related and the voltage will be the same in parallel. ie 4.2V fully charged for LiPo and Li-ion and discharged 2.5V for LiPO and Li-ion. They will cycle the same. Yes the LiPO's will be pretty much shot after 150 cycles ( SOH below 70% original capacity) and the Li-ion will still have another 150 cycles till they reach 70% SOH (state of health). 
I do think the difference between LiPO's and Li-ion would cause an issue and would  **not** recommend mixing the two. The other option which others have tried is to fit a Buck Boost DC to DC converter and plug it into the charge circuit to trickle feed the main battery. Good for range but no good if you are looking for more amps in the 20-30A range.
```

---
## \#13 Posted by: skatardude10 Posted at: 2019-02-01T04:17:55.913Z Reads: 49

```
Yep, already do trickle charge via dc-dc boost converter from power tool batteries mostly. Does work great for range- never a dead battery, but additional amps ... 5A less sag (noticeable) from the charge current at best.
```

---
## \#14 Posted by: Gamer43 Posted at: 2019-02-01T04:49:30.872Z Reads: 47

```
the article you referenced talks about Lead-Acid chemistry, where the general trend is higher capacity -> lower internal resistance.

(not to mention lead-acid is much more rugged)

For lithium-ion chemistry this is not necessarily the case. (and the article makes note of the analogous case with lead -acid, i.e. gel vs flooded).
For example an 18650 you might find in a drill has a capacity of 1.3Ah but an internal resistance of say 15 miliohms, while an 18650 you'd find in a laptop would have a capacity of 2.2Ah but an internal resistance of say 30-40miliohms.

(however, as the technology matures, we are approaching that generalization)

And this perfectly illustrates what I mean with using lipo and 18650 in parallel.

Let's say we have two 10s battery packs, one lipo one 18650, both have a nominal capacity of 10Ah.
Clearly, the lipo pack will have a lower internal resistance.
let's say the lipo pack has an Ir of 50 miliohms and the 18650 pack 100miliohms and we connect them in parallel.

Let's now burst load the two packs which are now connected in parallel with a 100A load for several seconds at a time, with several seconds of rest in between.
Here's what happens:
lipo pack supplies 67A, 18650 pack supplies 33A.
Already we can see that the lipo pack is being cycled more, since more current is being drawn from it despite the same capacity.
because of the internal resistance, the terminal voltage across the entire setup drops by 3.3V. Let's say both packs were charged to 42V at the start, this means both packs now output 38.7V under load.

Load is removed. the 18650 pack returns to just under 42V, BUT because the lipo pack was supplying MORE current at the SAME capacity (thus dissipated more charge), its voltage returns to significantly more below 42V.
Now what happens is the 18650 pack starts to recharge the lipo pack, cycling it even further.
Basically, the lipo pack, or whatever pack has the lower internal resistance (without the same proportional increase in capacity) is forced to act as a super-capacitor bank, which it is NOT designed for.

What my friend did was put 8 laptop 18650s (2.2Ah) in parallel with a drill 18650 (1.3Ah) in a 8S9P battery pack.
Four weeks later the drill 18650 in one of the layers failed short and caused a catastrophic failure of the battery pack.

To be fair,  he was using the piece of sh!t known as the brushed motor with an even worse pwm controller (with no current limit, it didn't even have synchronous rectification SMH!) in a scooter and full throttling the thing constantly.
```

---
## \#15 Posted by: Marsen Posted at: 2019-02-01T05:24:45.752Z Reads: 33

```
If the two packs are still connected in parallel, load or no load, then the voltage at the positive and negative terminal is the same across both batteries in parallel. Would that mean that the 18650 cells would be charging the LiPO cells when at rest? With a potential difference between the two current would flow.
```

---
## \#16 Posted by: Gamer43 Posted at: 2019-02-01T05:26:56.120Z Reads: 45

```
[quote="Marsen, post:15, topic:82755, full:true"]
If the two packs are still connected in parallel, load or no load, then the voltage at the positive and negative terminal is the same across both batteries in parallel. Would that mean that the 18650 cells would be charging the LiPO cells when at rest? With a potential difference between the two current would flow.
[/quote]

If left unconnected to the load, then yes, their voltages would be the same and no current would flow between them. 
If they were repeatedly loaded and then unloaded (as typically seen in EV applications and especially here in esk8) then their resting voltages would quickly deviate from each other because one pack was discharging a larger percentage of its capacity every time they were loaded.
However, when the packs are loaded, their terminal voltages are the same, but only because the internal resistances and their differing current contributions cause them to balance out.

If the the load were a constant current load, and not the burst loading seen in this application, then it would be (significantly?) less of a problem.
which is why powerwalls can get away with it, they see essentially constant current loads and not repeated burst loads.
Under a constant current load, they theoretically should be cycled at the same rate, one will just hit the undervoltage cutoff sooner.
ERR I should say, once Unndervoltage Lockout is triggered, the higher internal resistance pack will recover to a higher resting voltage.
In burst loading, this situation where the resting voltage of one pack is higher than the other is encountered multiple times per discharge cycle (which results in the lower IR pack being cycled more), while in constant current loading, this situation is encountered once per discharge cycle.

The worst case is encountered when each time the packs are unloaded, their resting voltages are allowed to reach equilibrium each time before the next loading session, and this happens dozens, maybe even hundreds of times before undervoltage cutoff happens.
In this worst case, the lower IR pack will be cycled proportionately many more times than the higher IR pack, the proportion being the ratio of their Internal Resistances divided by the ratio of their Capacities.

e.g. in the worst case, a pack with quarter IR but double capacity will be cycle twice as often. 
or packs with same IR but one with triple capacity, the smaller one will be cycled three times as often

And again, this explains the situation with my friend, he would intermittently full throttle his scooter countless times before he would charge it (it was only exacerbated by the fact the capacities were egregiously different).
```

---
## \#17 Posted by: Marsen Posted at: 2019-02-01T05:37:49.600Z Reads: 44

```
I have a bunch of LiPO's and Li-ion cells, if I had time I'd build a setup and experiment to see the effects and how much it damages the cells. I'm certainly of the opinion that LiPO cells and Li-ion cells in parallel definitely constitutes different type and should not be done because as you say their IR is too different.
Interesting topic :slight_smile:
```

---
## \#18 Posted by: pat.speed Posted at: 2019-02-01T10:29:37.483Z Reads: 41

```
So what happens when the packs reach and equal IR? The they would theoretically drain the same amount thus no cells charging the other
```

---
## \#19 Posted by: deucesdown Posted at: 2019-02-01T18:40:54.483Z Reads: 39

```
I think this idea would work fine if you get the proportions correct. It might help to think about hypothetical extreme cases. This is all in my fantasy brain lol.

If lipo pack has zero IR and 18650 pack has infinite resistance, the full discharge load would be carried by the lipo pack. Therefore, ignoring capacity for now, if you size the lipo pack to be able to take the full load, you'll never exceed the whole pack's capability.

The other extreme is if both packs have the same IR. In this case both packs would share the load equally. So you have to size the 18650 pack to be able to take 1/2 the total discharge to cover the worst case.

(I know there's one other extreme, 18650 zero resistance, lipo infinite resistance, but that's really not a possible case unless there's a failure)

So if you want 100a out of the pack, covering both worst cases, you can put together a lipo subpack with 100a discharge capability, and 18650 pack with 50a discharge capability.

Regarding capacity, the lipo pack will supply more watt-hours during high discharge, but when the load is off, the 18650 pack will charge the lipo pack. The trick is, you have to somehow not discharge the lipo pack too far. I'm not sure how to get a handle on this. Can probably put an ammeter inline for both subpacks and log to sdcard or something... Then you can develop an idea about the behavior of the system, and adjust your trigger finger.

Lipo pack will wear out faster, and it'll be difficult to judge how worn out. Maybe every 50 cycles or so run a discharge test on a hobby charger. Swap out the lipo pack when it's worn out.

Safety wise, if anything fails in the system, you can have many different disaster scenarios. This is a good reason not to do this.

But I think the idea has merit and can work. Just have to work out the safety factors.

EDIT disclaimer -- lithium ion/poly internal resistance is very dynamic, changing with temperature, load, state of charge. It's useful for theoretical discussion, but cannot be relied upon to predict full system behavior IRL.
```

---
## \#20 Posted by: funkychiken86 Posted at: 2019-02-03T01:25:22.925Z Reads: 26

```
So I currently have 2x HRB 22000mAh 25C 6S 22.2V EC5 LiPo Batteries in my board with 2x 154kv belt motors. It hauls ass but I want it to haul more ass. Am I limited to 30mph with this setup? I'm not sure how my Vesc6 was tuned as I had no clue how my friend did it. I still can't wrap my head around it to retune everything.

What are the possibilities of slapping a car battery on this bitch? Would I fry my motors or my Vesc?
```

---
## \#21 Posted by: Gamer43 Posted at: 2019-02-03T02:53:09.351Z Reads: 26

```
The Lipos currently on it will perform better than a car battery.

What are you trying to get out of it? Higher Top speed or high acceleration/hill climbing ability?
```

---
## \#22 Posted by: funkychiken86 Posted at: 2019-02-03T04:00:28.419Z Reads: 22

```
I was hoping for a higher top speed. I wanna make sure to really eat shit when I wipe out X-D
```

---
## \#23 Posted by: deucesdown Posted at: 2019-02-03T04:01:37.873Z Reads: 24

```
[quote="funkychiken86, post:20, topic:82755"]
2x 154kv belt motors
[/quote]

can try 170kv for a bit more top end, without giving up too much torque. Or 190-200kv but you give up a lot of torque, so probably will need to upgrade everything else.
```

---
## \#24 Posted by: funkychiken86 Posted at: 2019-02-03T04:13:32.787Z Reads: 23

```
Hmm. Alrighty then. I think I'll just stick with what I have considering wheelies are fun and it's a head Turner :) ty!
```

---
