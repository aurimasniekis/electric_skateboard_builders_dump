# LIPO vs LI-ION Amp Ratings

### Replies: 15 Views: 236

## \#1 Posted by: ghols Posted at: 2019-11-17T15:48:23.339Z Reads: 75

```
Hey guys,

I know this topic has been beat to death, but I'm having trouble wrapping my head around the whole battery thing. My goal is to build a board capable of hauling my extremely heavy frame around, so in order to do that, I'm going to try to avoid bottlenecks wherever possible. This means I want to be able to push my motors, vesc, and battery to their theoretical limits without damaging any component.

So here's my dilemma. Lipos offer high current so I'll never be bottlenecked when using them with the potential to push well over 100 amps continuous. But, I prefer the idea of a prebuilt 18650 pack LI-ION w/ built in BMS for convenience of charging. But, every prebuilt LI-ION pack I've seen has a stupid low max amp limit. For example:

This battery back is limited to 60A continuous and 150A peak. Meaning, I could only pull 30A to each motor. 

https:///collections/electric-skateboard-battery-pack/products/electric-skateboard-battery-epower-pack-12s4p

Let me know if I'm completely off here. I'm still learning and in the research stage of a build. Also, drop in some links if you know of higher discharge LI-ION packs. 

Thanks!
```

---
## \#2 Posted by: Benjo Posted at: 2019-11-17T16:39:37.461Z Reads: 71

```
Well, what kind of board are you building? For MTBs or similar you probably want to increase that "p". 12s6p to 12s8p. 4p just doesn't allow for high current.
```

---
## \#3 Posted by: Mr_McTurd Posted at: 2019-11-17T17:23:35.010Z Reads: 68

```
So if you want a samsung 30q pack that pushs 100+ amps of current without sagging horribly, then you will need a 12s8p pack. With a bms, that would cost around 500$ if you built it yourself, or 700-800 dollars if you buy it from a vendor. 

If you are looking for pure power with only 5 to 10 miles of range, lipos are a good choice. I would recommend the Turnigy Graphine brand. These packs only weigh about 2 pounds each, compared to a 12s8p pack that weighs 11 pounds. You can find those cells at https://hobbyking.com/en_us/catalogsearch/result/?q=graphine%206s.

There is a cheap alternative for lipos called SPIM08HP. Each cell can discharge 200a continuously and they only cost 6$. The only downside is that they are quite large and the cells were previously used, so you must buy a decent balance charger and lipo alarms.

link for SPIM08HP-https://batteryhookup.com/collections/frontpage/products/4-200a-lithium-polymer-3-7v-8ah-flat-pouch-cells-lipo-batteries
link for balance charger- https://hobbyking.com/en_us/turnigy-accucell-c150-ac-dc-10a-150w-touch-button-smart-balance-charger-us-plug.html
```

---
## \#4 Posted by: ghols Posted at: 2019-11-17T17:26:21.592Z Reads: 61

```
[quote="Benjo, post:2, topic:103956, full:true"]
Well, what kind of board are you building? For MTBs or similar you probably want to increase that “p”. 12s6p to 12s8p. 4p just doesn’t allow for high current.
[/quote]

Oh yeah you're definitely right. With a 4p build I'd only be able to have a continuous discharge of 60A if I went with 30q's. I've been looking at @psychotiller battery packs as well but I did see that the BMS was charge only. Would any discharge protection come from an inline fuse i'd have to place myself or would the VESC settings be sufficient?
```

---
## \#5 Posted by: ghols Posted at: 2019-11-17T17:30:00.278Z Reads: 55

```
I love the idea of these flat pack cells, but man, I'd be super out of my depth with diy battery building. I know the basics of configuration but buying a spot welder and safely routing wires is just a lot for my second build. I suppose if there was a reputable builder for these, they would fit my needs pretty well.
```

---
## \#6 Posted by: Benjo Posted at: 2019-11-17T17:34:02.540Z Reads: 54

```
The VESC will only limit the charge current and do a cut off on too low voltage. No balancing or anything is happening there of course.
A fuse triggers very late, it is a "very analog" process. A 80A fuse can take 100+A and more for a significant time until it blows. That won't protect your cells, it is just a safety measurement to prevent fire.
```

---
## \#7 Posted by: ghols Posted at: 2019-11-17T17:35:54.118Z Reads: 43

```
So the vesc won't limit the amount of amps it pulls from the battery or how much it can deliver to the wheels?
```

---
## \#8 Posted by: Mr_McTurd Posted at: 2019-11-17T17:37:28.319Z Reads: 44

```
I also forgot to mention that those flat cells are very easy to assemble. Each cell comes with holes on each terminal where you can clamp each terminal with screws and locknuts. I didn't even have to solder the balance wires or the main discharge wires because you can just clamp them down with washers. I'm an incompetent 14 year old and I was able to put these cells together without issues.
```

---
## \#9 Posted by: Benjo Posted at: 2019-11-17T17:43:22.874Z Reads: 45

```
Oh, sorry to confuse. Sure you can set a (separate) limit for the battery and motor current. It's just that this is different from a discharge BMS as it does not care about the individual cells, just the whole pack. But in general this is fine, as long as you always balance charge the pack and don't set the voltage cut off too low.

Edit: but note that longevity is better if you balance discharge as well.
```

---
## \#10 Posted by: ghols Posted at: 2019-11-17T19:15:57.762Z Reads: 42

```
[quote="Benjo, post:9, topic:103956"]
you can set a (separate) limit for the battery and motor current. It’s just that this is different from a discharge BMS as it does not care about the individual cells, just the whole pack. But in general this is fine, as long as you always balance charge the pack and don’t set the voltage cut off too low.
[/quote]

This may show my complete lack of experience, you would balance charge every time you charge the packs right?
```

---
## \#11 Posted by: Benjo Posted at: 2019-11-17T19:50:45.138Z Reads: 38

```
Yes, that's what you normally do with LiPos, the ESC draws from the whole pack without balancing, then you charge it with a balance charger like a regular hobby RC Lipo charger. Then the next time you ride all cells are perfectly balanced again. After the ride there might be some discrepancies which you then just balance away while charging.
```

---
## \#12 Posted by: pmouraguedes Posted at: 2019-11-26T13:45:46.116Z Reads: 23

```
With 21700 cells you can already get 100A continuous with a 3P configuration, for example with a Samsung INR21700-40T.
```

---
## \#13 Posted by: ghols Posted at: 2019-11-26T14:35:33.321Z Reads: 23

```
The only person I’ve seen building these packs so far has been eboosted out of Peru. Do you know anyone else who is building these packs with a charge only bms?
```

---
## \#14 Posted by: pmouraguedes Posted at: 2019-11-26T15:12:56.018Z Reads: 22

```
I just built a 10S3P flat pack with 18650 cells for a friend and I'm starting one for me with 21700 cells for a MTB (both with charge only BMS). 
Drop me a message if you're interested in one.
```

---
## \#15 Posted by: murdomeek Posted at: 2019-11-27T20:27:27.092Z Reads: 10

```
[quote="Mr_McTurd, post:3, topic:103956"]
So if you want a samsung 30q pack that pushs 100+ amps of current without sagging horribly, then you will need a 12s8p pack
[/quote]

30q's can be safely discharged at 20a as per many technical tests and graphs.

So for 100a continuous discharge, you will only need a 10s5p pack (or 12s5p).  This is a pretty standard pack and lots of people build these with BMS
```

---
