# What is the thinnest VESC possible?

### Replies: 8 Views: 1227

## \#1 Posted by: evoheyax Posted at: 2016-03-01T17:44:36.203Z Reads: 91

```
I'm curious to those who are supplying the community with vesc's, what is the thinnest you can get a VESC? I am researching to build a 15mm thick board from maple vinears and will be using 10 mm think lipo cells.

Can it be split into 2 boards?

Can you use more, smaller, thinner, capacitors?
```

---
## \#2 Posted by: thomwithah Posted at: 2016-03-01T21:39:38.987Z Reads: 75

```
My thoughts are that it's less than 15mm now, probably 13-12 MM thick looking at the ones in my Raptor dual. I'd guess adding a couple of mm to your board might be a better solution than a custom VESC unless your working with unlimited resources and strictly convicted to the 15mm thickness. Even with that, depending on your specific board materials and design 15mm *may* be possible with currently sourceable VESCs. I'm sure @onloop and other vendors will be able to provide and exact thickness for you. In the mean time maybe the information I shared will give some food for thought, or piece of mind.
```

---
## \#3 Posted by: onloop Posted at: 2016-03-02T00:08:14.752Z Reads: 62

```
The vesc will not get any thinner than what it currently is. 15mm is about it.
```

---
## \#4 Posted by: evoheyax Posted at: 2016-03-02T01:24:53.957Z Reads: 58

```
@onloop is that a limitation with the current design of the VESC or just, this is the thinnest it can be because the components need to be close enough to each other?

I know in some cases, certain chips need to be close or you get more latency, but I'm not sure if that's true with the VESC.

If vedder did a new design of the VESC, do you think that it could be made thinner?

The way I see it is that you have chips on both sides of the VESC. Moving all chips to one side would mean it would be wider and/or longer but maybe 5 mm thinner
```

---
## \#5 Posted by: torqueboards Posted at: 2016-03-02T01:52:48.092Z Reads: 54

```
@evoheyax - You could make it thinner.. as you mentioned. You would have to re-design the PCB footprint but then you would probably want to replace that height with a nice heat-sink to be able to push more amps through. So in the end it would be about the same size.
```

---
## \#6 Posted by: Hummie Posted at: 2016-03-02T02:08:21.773Z Reads: 52

```
A lot,of the height is plugs.  Plugs you're unlikely to use. I think if u knew what u were doing u could heat he board and suck out the solder or so,ethi g and remove them.  Or convince someone to not put them on to begin with and sell it to u.  Or make your own the vesc and omit the plugs and I think they make flat capacitors...at least skimmer is out here.  At the least u can have the plugs mounted horizontally
```

---
## \#7 Posted by: trbt555 Posted at: 2016-03-02T10:18:46.893Z Reads: 44

```
I did some probing on one of my own VESCs with my calipers.
The connectors, wires  and caps aside, it's 10mm thick at the thickest end, where the mosfets are.
It won't be comfortable but I think you could get away with 11 mm in total if you leave off the connectors and use smaller caps in parallel.
```

---
## \#8 Posted by: massy Posted at: 2016-03-02T18:41:32.066Z Reads: 29

```
[quote="evoheyax, post:4, topic:1617"]
The way I see it is t
[/quote]

Just had a look at mine and it seems you could save maybe 2mm on one side doing this, then the height of necessary components get in the way.
```

---
