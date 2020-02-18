# Easy DIY Battery Pack Idea - Individually Fused, Cheap, No welder required, Somewhat Modular

### Replies: 13 Views: 261

## \#1 Posted by: Vykku Posted at: 2019-04-30T20:14:57.897Z Reads: 112

```
Looking for some feedback from more experienced people on what they think of method of building a battery pack, as I haven't seen anyone do this yet.

Nkon offers welded solder tags on cells for pretty cheap (0.55€ per cell). I thought of using these cells on a PCB by soldering these tags. To hold them in place,  a 3d printed support can be used, together with zipties, like in the following pics. 

On the PCB, it is easy to add SMD fuses for every single cell. To connect each parallel pack together, I would use multiple thinner wires instead of one thick one to make it slightly more flexible. I haven't done any calculations yet for the wire thickness yet, as it still requires some work.

Here is a very quick rough render (only spend about 5 mins on the design, still needs a lot of polishing) of what I mean: 

![image|544x500](upload://xteS7jVFCKs6GZZ00S6Ak3k2gBF.jpeg) 

The extra bits of nickel strips can be cut of after soldering so they don't protrude.

This is a quick sketch of what the underside would look like:

![image|690x463](upload://al9riJYVxi7VsO1Ys6OjT95fXR0.jpeg) 

I forgot to add a place to hook up balance wires in this sketch.

And here is what the 3d printed part would look like (it still needs some way to clip into the PCB so it wouldn't try to move):

![image|690x303](upload://78PPZmWkdKnYluj92I1sPIzHySb.jpeg) 

The advantages over NESE modules is the cost, and the cells are fused. These modules also use much less space.

The disadvantage is that it is harder to replace a cell. However people don't have to replace cells too often, and to do this all you need to do is desolder 2 connections and solder the new cell (and the fuse if it is blown).

The only issue I can think of is that the cells come with 8x0.15 nickel strips, which might not be able to handle the current required.

Using this method, the total cost additional to the cells for something like a 10S4P would be  ~£20 for solder tags, £10 for PCBs, ~£3 for filament, and then the cheap consumables like wires, fuses and heat shrink which I guess would add up to about ~£15, so about £40-50 total.
```

---
## \#2 Posted by: brenternet Posted at: 2019-04-30T20:20:15.325Z Reads: 107

```
[quote="Vykku, post:1, topic:92361"]
The only issue I can think of is that the cells come with 8x0.15 nickel strips, which might not be able to handle the current required.
[/quote]

I think this is the biggest hurdle here. I like your thinking though.

What we really need is what @topcloud is arranging but on a DIY level. We need a talented DIY battery guru to start producing P packs for us to buy and put together into batteries ourselves. If you think about it, welding is the most stressful/expensive part of the build. If we could buy premade P packs and then solder and assemble we'd be golden.

@pjotr47 - Do this in the EU ;)
```

---
## \#3 Posted by: Grozniy Posted at: 2019-04-30T20:21:17.583Z Reads: 107

```
@pjotr47 please do
```

---
## \#4 Posted by: moon Posted at: 2019-04-30T20:22:11.696Z Reads: 103

```
Like what @thisguyhere is doing?
```

---
## \#5 Posted by: brenternet Posted at: 2019-04-30T20:22:16.716Z Reads: 97

```
Imagine the convenience for the battery builder too. All they need to do is mass produce P packs and not worry about all the fiddly stuff, list them on a site as is, no negotiation or size requests. The rest is up to the user.
```

---
## \#6 Posted by: brenternet Posted at: 2019-04-30T20:22:44.676Z Reads: 96

```
I didn't know he was doing that, sweet.
```

---
## \#7 Posted by: thisguyhere Posted at: 2019-04-30T20:34:53.141Z Reads: 89

```
thanks for the shout.

yea, i find getting a welder and associated supplies to go along with it is the biggest hurdle.

so this service is cells welded in to 3, 4, 5p - then bound to a PCB:

http://esk8life.com/samsung-30q-18650-cell

then you can solder it together.
```

---
## \#8 Posted by: Vykku Posted at: 2019-04-30T20:41:13.615Z Reads: 82

```
I had no idea he does that. His solution does seem pretty nice, and the price that he charges is much lower than I would have expected for this service, but seems he is not doing them at the moment, and international postage for batteries is a pain.

I was thinking maybe once everything is soldered together, it might be possible to add solder with a good iron to the nickel to allow more current to flow. The PCB might act as a bit of a heatsink so slightly less heat would go into the cell. Not a perfect solution, but it should increase the current capacity while hopefully not damaging the cells.
```

---
## \#9 Posted by: ZachTetra Posted at: 2019-04-30T21:07:31.241Z Reads: 75

```
What would it be for a 12s4p p-pack if we already own the cells?  Still on the fence about getting a welder
```

---
## \#10 Posted by: pjotr47 Posted at: 2019-04-30T21:07:38.795Z Reads: 72

```
It is no problem for doing this. Thnx for the tag everybody! & thnx for the tip

When I have my company fully running. I will think about listing that on my website. 

Welding a pack take not the much time. It is all the other stuff. Glue the cells, add fishpaper, cut the nickel and the sharp corners. Place the BMS and route those wires very clean
```

---
## \#11 Posted by: thisguyhere Posted at: 2019-04-30T21:27:51.175Z Reads: 62

```
i charge $4.2 for bare cells, then it's an additional $2.2 for 4p group build.

so, $2.2 * 48 = $105.6, plus shipping if you supplied the cells.

this includes pcb, fishpaper, nickel and adhesives.
```

---
## \#12 Posted by: thisguyhere Posted at: 2019-04-30T21:29:33.487Z Reads: 62

```
[quote="Vykku, post:8, topic:92361"]
international postage for batteries is a pain
[/quote]

i've had a package containing battery be outright denied by US postal service.  at the moment shipping lithium cells is a massive grey area.  i think it's because some of it is shipped via air.
```

---
## \#13 Posted by: Vykku Posted at: 2019-04-30T21:42:12.193Z Reads: 52

```
@thisguyhere  I'm located in UK so unfortunately can't buy any from you. The price is extremely reasonable, and I would have bought enough for a battery instantly if I could.
```

---
