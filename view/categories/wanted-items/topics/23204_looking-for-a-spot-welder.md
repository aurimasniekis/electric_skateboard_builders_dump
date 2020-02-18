# Looking for a spot welder

### Replies: 18 Views: 1481

## \#1 Posted by: KTMinni Posted at: 2017-05-16T13:52:28.738Z Reads: 141

```
Hey guys, I recently tried soldering my 18650s together, it worked for a while but now the solder is snapping off.  So I was wondering if anyone would be willing to let me use/rent their spot welder.  I'd even buy a used one if the price is right.  Hell if I could send my batteries out to someone who would weld them I'd do it.

My location: St. Paul, Minnesota
```

---
## \#2 Posted by: Namasaki Posted at: 2017-05-16T14:10:37.088Z Reads: 138

```
Get a 60amp welder. 
The 30a welders don't cut it.
```

---
## \#3 Posted by: KTMinni Posted at: 2017-05-16T14:17:48.384Z Reads: 134

```
I'm not sure if it is worth it to invest that kind of money buying some thing I might use only once or twice.
```

---
## \#4 Posted by: ekitesurfer Posted at: 2017-05-16T14:24:57.454Z Reads: 131

```
https://malectrics.eu/product/diy-arduino-battery-spot-welder-prebuilt-kit-v2-1/
```

---
## \#5 Posted by: aigenic Posted at: 2017-05-16T14:49:40.740Z Reads: 119

```
I saw someone offering his spot welder for 80€ on this forum few days ago...
```

---
## \#6 Posted by: Okami Posted at: 2017-05-16T14:53:31.332Z Reads: 117

```
Someone was proposing ''traveling'' spot welder .. after you are done, just sell it further :D maybe even decreasing price a bit every time.
```

---
## \#7 Posted by: aigenic Posted at: 2017-05-16T14:54:30.466Z Reads: 116

```
[quote="Okami, post:6, topic:23204"]
Someone was proposing ''traveling'' spot welder .. after you are done, just sell it further :smiley: maybe even decreasing price a bit every time.
[/quote]

Great idea! I would hook up
```

---
## \#8 Posted by: KTMinni Posted at: 2017-05-16T15:03:00.473Z Reads: 113

```
That's such a good idea!  How would we get that started though?
```

---
## \#9 Posted by: jaykup Posted at: 2017-05-16T15:14:41.612Z Reads: 111

```
Sounds like you have cold solder joints.  A good solder joint on a battery will bend or damage the battery significantly if you try to remove it - or the solder it's self will break, leaving half still on the battery.

I did a lot of testing getting solder to stick to 18650 cells using dead laptop cells.

I found that a 80-100w soldering iron with rosin/flux core solder worked best.  The little 30-40w soldering irons lose too much heat and don't produce strong solder joints.  You have to heat it long enough for the solder to "flow" across the batteries surface, I find about 10 seconds with a 100w gun?

I pre-tin the cells, then come back and solder the wire to it.

https://www.electric-skateboard.builders/uploads/db1493/optimized/3X/0/7/073ccd3c8d40cfbc4a0b9fb5e43fc4611db9ce8e_1_666x499.jpg

https://www.electric-skateboard.builders/uploads/db1493/optimized/3X/2/c/2c82d491beeb484f6d5cb01978b99af51265ddc0_1_690x460.JPG

I was inspired by @chaka - he's soldered more packs than I can count.

[quote="chaka, post:8, topic:7571"]
I use an 80 watt for thick gauge and a couple of smd stations for everything else. You can use a brass wire sponge to clean your tip when it is hot and it will make better contact. Adding solder to the tip before soldering is actually bad practice since it will lead to pitting the iron tip and eventually eroding with use. Guess it doesn't matter much to most people since they don't solder often but it does if you are soldering daily.
[/quote]

[quote="chaka, post:10, topic:381, full:true"]
Those smd stations are great for small stuff but you really should have a large 80watt chisel tip for soldering large gauge power cables to pcb's or connectors. The smd stations are for soldering small things like smd chips, imagine that? SMD soldering stations can solder larger connections but you need to apply heat for so long that you end up cooking everything around it. Best to apply a lot of heat for a very short period of time.
[/quote]

[quote="chaka, post:9, topic:3744, full:true"]
No need to scuff the cells, you are soldering nickel to nickel. Use a good liquid flux and pre-tin your cells with a little pool of solder hitting them with a wet sponge after removing the iron.  We only scuff metals that have oxidation, remember soldering is not a mechanical bond.

And please use at least an 80 watt iron to do this. You have to get in and out quick. If you use a little smd iron you will need to let the iron dwell for much too long and the cell will get hot.
[/quote]

You can pick up a chinese 80-100w on ebay for around $30
```

---
## \#10 Posted by: KTMinni Posted at: 2017-05-16T15:25:58.689Z Reads: 104

```
I actually used a 250w gun for these joints so I don't know why they are breaking.
```

---
## \#11 Posted by: Jinra Posted at: 2017-05-16T15:37:30.197Z Reads: 101

```
Are you using flux and/or rosin core solder?
```

---
## \#12 Posted by: jaykup Posted at: 2017-05-16T15:49:14.724Z Reads: 105

```
One of these things?

http://www.stevenjohnson.com/soldering/pics/weller-8250a-kitsm.jpg

I haven't had any luck with those
```

---
## \#13 Posted by: chaka Posted at: 2017-05-16T15:49:23.588Z Reads: 106

```
It's better to solder to spot welded tabs if you have access to a spot welder. You still need to be quick when soldering to tabs since they will transmit plenty of heat into the cell if given the chance. Ideally you would solder fuse wire to a parallel buss bar connection just in case a cell decides to go thermal later in life. Using cell level fusing also allows the parallel packs to flex without breaking connections, I assume it helps with vibratory stress also.

On the subject of broken connections and vibration. It is a good idea to stabilize all wired connections with a natural cure silicone to keep the soldered connection from repeatedly bending or vibrating excessively. This stuff can be hard to find, if you need something found locally you can use [Versachem Mega Grey](https://www.amazon.com/Versachem-99939-Mega-Grey-Silicone/dp/B005CAKLRK). It is important that you do not use regular silicon since it can cause corrosion from the curing process.
```

---
## \#14 Posted by: Jinra Posted at: 2017-05-16T15:51:57.883Z Reads: 107

```
To add to this, some of my cell fuses broke due to excessive vibration and rubbing against the deck. +1 on the recommendation to secure any fusing with a shock absorbent material like silicone. I also padded my pack with some quarter inch soft craft foam as well and it's been holding up great!
```

---
## \#15 Posted by: chaka Posted at: 2017-05-16T16:15:48.140Z Reads: 103

```
I like to use 2 layers of fishpaper with adhesive backing. One under the bussbar and one on top. I fold about 1/8th of an inch over the edge of the cells to prevent the fuse wire from shorting out. The whole package is then shrink wrapped and siliconed in place to prevent shifting. 

It is important that some air gap is left around the fuse wire 

<img src="/uploads/db1493/original/3X/6/7/678e60cc49ace8b1f999c7301d96e00fa3af7a91.jpg" width="690" height="388">
```

---
## \#16 Posted by: KTMinni Posted at: 2017-05-16T18:05:10.868Z Reads: 98

```
I currently use both.
```

---
## \#17 Posted by: Cjnutts Posted at: 2017-05-22T15:15:02.643Z Reads: 77

```
 I'm buying a spot welder this morning. I jumped on here quick to see if there was any  recommendations between the 709 in the 788.   I don't know if you got your issue resolved but I'll have it in a couple days and I can show you how to solder so it sticks.    I'm in East Bethel Mn.<img src="/uploads/db1493/original/3X/1/f/1fe93d45055d8a844a5aa02b095866266bec0824.JPG" width="666" height="500"> i've built this girl yesterday.
```

---
## \#18 Posted by: KTMinni Posted at: 2017-05-22T15:34:26.802Z Reads: 74

```
Hell yeah!  I'm in North St. Paul, shoreview area
```

---
