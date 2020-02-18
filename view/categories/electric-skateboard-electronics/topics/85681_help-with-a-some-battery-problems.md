# Help with a some battery problems

### Replies: 13 Views: 332

## \#1 Posted by: the1seabass Posted at: 2019-02-28T20:19:33.784Z Reads: 95

```
Hi guys so long story short last year had a working battery for a couple of months. Then it died due to it not being built the best. After back and forth with the builder not getting anywhere I decided to drop it and focus on some other stuff.
Jump to now almost a year latter and I still have the battery but disassemble. Should I
A. Sell for parts and try to buy a new battery 
B. See if I can find a spot welder somewhere and rebuild it/ see if some one can rebuild it for me
C. Scrap and just buy a new one.
Also for background info it was a 10s2p battery here it is now 
-thanks in advance![IMG_20190228_151549|666x500](upload://LzwSDQe2nOzEgpYhM9rV4FRm3A.jpeg)
```

---
## \#2 Posted by: Klaerke91 Posted at: 2019-02-28T20:32:45.733Z Reads: 90

```
well you said it yourself.

The battery died.

I wont use it after 1 year on the shelf
```

---
## \#3 Posted by: AlanZhou Posted at: 2019-02-28T20:50:30.119Z Reads: 84

```
[quote="Klaerke91, post:2, topic:85681"]
I wont use it after 1 year on the shelf
[/quote]

that depends.
```

---
## \#4 Posted by: pat.speed Posted at: 2019-02-28T21:06:24.475Z Reads: 77

```
What do you mean by died? What voltage was it at while sitting? Are the cells balanced? 

These all need to be checked before you go any further
```

---
## \#5 Posted by: the1seabass Posted at: 2019-03-01T15:56:30.829Z Reads: 57

```
So due to the spot welds not being done correctly it caused the nickle strips to pop off a couple of the cells thus not completing the battery circuit because of this the fully charged battery would jump from 100 down to around 14 percent and any time I would try and press the excererator it would drop to two and the motor would stall. I ended up figuring this out and used some electrical tape to hold the connection down but that would only work for so long before the it would come loose and I would have to take the board apart and start the process all over again. I tried to solder the connection together but decided against it due to the harm it might cause to the cells from the heat.

As for the cells now I just checked and they all seem to be around d the same charge except for a couple. Let me know what u think
```

---
## \#7 Posted by: sk8l8r Posted at: 2019-03-01T16:08:22.632Z Reads: 49

```
For such a small battery it I would look at these https://www.electric-skateboard.builders/t/n-e-s-e-nese-no-solder-module-battery-packs/36847

It's costly to buy a welder battery for it 
 etc I don't think it's worth it for you, unless your likely to build more batteries in future

Edit: if your cells are ok
```

---
## \#8 Posted by: the1seabass Posted at: 2019-03-01T16:17:44.642Z Reads: 49

```
Cell charge 
3.888   
3.833
3.819
3.801
3.803
3.729
3.807
3.820
3.808
3.816
3.808
3.801
3.888
3.808
3.803
4.400
3.810
3.834
3.752
36.0
The last one  not sure what's going on but I checked it a couple of times
```

---
## \#9 Posted by: skatardude10 Posted at: 2019-03-01T16:21:51.989Z Reads: 44

```
Someone feel free to roast me...


Imo these all seem great. I'd pick up something like the litokala li-500 that can test total capacity, internal resistance, then pair the batteries so that each P group comes out to closest to the same total mAh. 

I might be a tad worried about the 3.6v cell, but it might be fine, just cycle it and see exactly how much capacity it may have lost or how much higher the internal resistance is.

I agree with previous posts- NESE sounds like a great option for you. No need to scrap good cells, and I wouldn't sell them unless you cycle them and test them for capacity anyways. 

I always keep old cells unless they won't fully charge, lost more than 40% capacity or heat up excessively. There are so many things you can do with old cells, nice to have functioning cells on hand. 

Personally, I use old laptop cells that are up to 8 years old in charge packs for my boost converter to charge my board anywhere from a battery in my backpack in many # P configurations, low amp output stuff. The cells range anywhere from 1.5AH to 3AH, varying ages, etc... just paired to  match overall capacity with voltage monitor constantly watching each P groups voltage. Old cells aren't usually suited to continue on in high drain applications, but they are perfect for lower drain stuff. Either way, 1 year is far from old.

Check out https://secondlifestorage.com/repackr.php
```

---
## \#10 Posted by: Goonman Posted at: 2019-03-02T00:29:32.150Z Reads: 26

```
The 4.4 is a bit high. But you can balance them out. If you were going to scrap them I would probs just solder them. At you would have a battery pack that didn't cost so much. There are a lot of scaremongers who will tell you doing that will cause your house to burn down and loved ones to meet their demise. But do it right and it will be fine.
Otherwise send them off to a battery builder and get them to reconstruct it using the cells you already own.
```

---
## \#11 Posted by: skatardude10 Posted at: 2019-03-02T00:52:35.571Z Reads: 26

```
Oh man, I didn't notice the 4.4 one... that's strange!!
```

---
## \#12 Posted by: MysticalDork Posted at: 2019-03-02T01:12:20.094Z Reads: 23

```
If you plan to use them, definitely do like @skatardude10 said and discharge them all equally, then run them all through a charger that can measure capacity (Doesn't matter if the readings are accurate, just that they're consistent.) and group them so that the capacity of each P group is the same.

If you decide to solder, I'd recommend getting some junk cells from a trashed laptop or something to practice on. You want the absolute minimum time spent heating the cells, so you'll need a good quality iron with a decent size chizel or wedge tip (At least 60 watts and preferably temperature controlled), and some good flux. I use "ruby fluid" liquid flux, it's used for soldering copper pipes and it's more aggressive and faster to give good wetting on nickel-plated cell terminals than the rosin based stuff I've used.
You want to apply a drop of flux to the cell, then apply solder to the iron (Set hot, I usually go about 400c) and then touch the iron to the cell, while adding a little more solder. Remove the iron as quickly as you can while still having good wetting of solder on the cell - It should be less than one second. 
Let the cell cool, and tin the wire/strip/braid.
Once both are cool, load some solder onto the tip, and use it to press the two tinned areas together. Again, do this as fast as you can while still getting a good fusion of the solder between them, it should also be less than one second.
Allow the cell to cool completely before doing the adjacent cells. I've seen people use a large chunk of aluminum pressed against the joint to help conduct the heat out of the cell.
```

---
## \#13 Posted by: the1seabass Posted at: 2019-03-02T02:48:46.860Z Reads: 18

```
Thanks you for all of the help and suggestions guys but I think I'm just going to scrap the cells and either sell the bms or keep it if I every need a nother. This project was suppost to be cost effected( even though I'm already over budget) I would rather have a battery that I know works rather than one I put together and some what knows it work. Plus I don't have a lot of money to be going out and buying tool that I'm probably going to use once. That said if anyone wants cells 20 for 20 seems like a good deal
```

---
## \#14 Posted by: deucesdown Posted at: 2019-03-03T15:36:23.202Z Reads: 11

```
Imo you should keep the cells! But I'll happily take them $20 for 20.
```

---
