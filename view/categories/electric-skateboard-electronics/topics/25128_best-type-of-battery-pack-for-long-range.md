# Best type of battery pack for long range

### Replies: 17 Views: 3978

## \#1 Posted by: Blucas Posted at: 2017-06-11T19:11:02.917Z Reads: 333

```
Hey all,
Very simple (at least I hope!), what battery pack would be the best for long range vs ease to charge, etc.? I keep seeing 10s3p and 12s3p popping up in various threads, and I haven't got the foggiest as to what they mean! :D

Any help would be greatly appreciated.

Blucas
```

---
## \#2 Posted by: Vinocity Posted at: 2017-06-11T19:21:33.070Z Reads: 324

```
10s means 10 batteries in series. So say a 3.6v 18650 liion cell in 10 series would equal 36v. (3.6x10=36v) and 12 is (3.6x12=43.2v)	

The 3p means 3 packs of 10 in parallel. Parallel means however many amps and amps per hour you have multiplied by how many parallels you have. So in this circumstance, a cell that has 3000mah in 3 parallels would be 9000mah. (3000x3)
```

---
## \#3 Posted by: Blucas Posted at: 2017-06-11T19:47:24.142Z Reads: 307

```
Does more mah = more range?
```

---
## \#4 Posted by: Vinocity Posted at: 2017-06-11T19:52:57.208Z Reads: 301

```
There is a lot of factors that add range. Mah means the juice that a battery can hold. Voltage and amperage play a factor in it as well. Say if you have a high amount of amperage and voltage. You don't need to use as much throttle causing you to go farther :slight_smile: I personally would get the samsung 30q cells in a 10s3p pack. Best way to go for eboards. It's got plenty of power 36v and the amperage can very between batches, 45-60amps, and 9000mah, if you use 10s3p. Should be able to go around 20 miles, and top speed should be around 25 mph, depends on your setup though. Also they are one of the cheaper high amperage liion cells.
```

---
## \#5 Posted by: thisguyhere Posted at: 2017-06-11T19:54:24.678Z Reads: 293

```
Essentially yes.

But really watt hours is the real measure of capacity. 

You get that from multiplying voltage x amp hour. 

https://milliamps-watts.appspot.com
```

---
## \#6 Posted by: Blucas Posted at: 2017-06-11T19:57:35.664Z Reads: 278

```
To create the battery pack, can I just solder them together, or do I need a spot welder (I think that's what I've seen mentioned in other threads).

Since I'm planning my first build, perhaps pre-built battery packs are the way forward for the time being?
```

---
## \#7 Posted by: Vinocity Posted at: 2017-06-11T20:01:14.920Z Reads: 265

```
I'm going to have to use a solder myself, mostly cause I don't want to shell out $100+ for a spot welder on a 1 time use. When soldering you have to be careful not to cover up the pressurized gas exhaust on the positive ends of the cells, and not to heat up the cells with the solder. Basically just apply the solder for as little time as possible. Heard people say a max of 3 seconds. I would do it under 2....
```

---
## \#8 Posted by: Vinocity Posted at: 2017-06-11T20:01:41.471Z Reads: 255

```
As long as you are safe, and just apply the solder gentle and quickly you should be fine :slight_smile:
```

---
## \#9 Posted by: Blucas Posted at: 2017-06-11T20:05:14.052Z Reads: 255

```
Maybe pre-built is the way to go :P I'd rather not ruin £160 of batteries (I'd need 30 of the samsung 30q's to make a 10s3p pack right?)

Time to see if any companies out there do custom battery packs :stuck_out_tongue:

P.S. Surely finding batteries with tags already on them would make things easier, right?
```

---
## \#10 Posted by: Vinocity Posted at: 2017-06-11T20:09:28.364Z Reads: 251

```
Well, I found these a few days back. I'm not completely sure about the company, but they looks good to me. Here is a video of what they do which might be perfect for what you are going for.
https://www.youtube.com/watch?v=9Pxq4Au5iuc

and the product: http://vruzend.com/product/vruzend_basic_kit/
```

---
## \#11 Posted by: smurf Posted at: 2017-06-11T20:56:47.446Z Reads: 239

```
I consider a 10s3p the minimum size for a 18650 battery pack. Now a 10s6p battery will not only have more range but will have a longer life span as well.
```

---
## \#12 Posted by: Blucas Posted at: 2017-06-11T20:58:45.563Z Reads: 237

```
Why a longer life span?
```

---
## \#13 Posted by: smurf Posted at: 2017-06-11T21:05:26.536Z Reads: 227

```
The higher the current draw from the battery the hotter it gets and heat is the real enemy to lithium batteries causing dendrite growth between the electrodes .
```

---
## \#14 Posted by: Smorto Posted at: 2017-06-12T01:40:24.401Z Reads: 215

```
That looks cool but it seem you can only make a rectangular pack like that. Like there is no way to connect cells end to end.
```

---
## \#15 Posted by: wmj259 Posted at: 2017-06-12T01:45:20.877Z Reads: 211

```
I would proceed with caution on that pack forming kit from vruzend. Mainly because noone here has used it and if your in the budget then I wouldn't risk it.
```

---
## \#16 Posted by: chuttney1 Posted at: 2017-06-12T03:14:29.934Z Reads: 199

```
I looked at it. The single reason why I would not use is that it's a few extra millimeters wider cell I do not need. Fine for Ebikes because they got extra space or a power wall. Serviceability is a major plus
```

---
## \#17 Posted by: Namasaki Posted at: 2017-06-12T04:13:12.364Z Reads: 192

```
[quote="Blucas, post:6, topic:25128"]
To create the battery pack, can I just solder them together
[/quote]


Welding is the quickest and easiest way to go however it makes the pack completely stiff and any flex in your board can be a problem.
 
You can solder the cells together for a more flexible pack however, you will need to use insulator rings on the positive ends of the cells and use insulated silicone wire 12ga or 10ga removing as little insulation as possible to solder to the cells.
I would also advise using a minimum 300w Weller soldering gun. Some peeps will disagree with me on that and say you can use your low temp soldering pencil. The reason I tell you to use a 300w gun is because with it you can get a good solder joint very fast. And the longer it takes to make the joint, the more area you heat up on the battery.
I used to solder Nicad cells together with thick gold plated bars long before Lithium batteries came on the scene and I did it with a 300watt Weller. The bars where a little tuff but soldering the supply wires on only took seconds.
```

---
