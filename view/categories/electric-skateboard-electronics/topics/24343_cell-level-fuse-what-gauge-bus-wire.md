# Cell level fuse, what gauge bus wire?

### Replies: 30 Views: 3233

## \#1 Posted by: thisguyhere Posted at: 2017-06-01T17:19:01.931Z Reads: 230

```
hello.

i'm planning a 12s3p build using lg hg2 cells.  these cells have continuous discharge rating of 20amp, and 3000mah capacity.

in 3p, continous disrchage will be 60amp with a 9ah capacity, bringing C rating to 6.7 (right?).

i want to employ cell level fusing like it's [described here](https://www.electric-skateboard.builders/t/ollinboards-cell-level-fuse/7392) (@chaka).

i have some [22awg bare bus wire](https://www.amazon.com/gp/product/B00B8866BA) but have concerns that it won't be thick enough to carry the amp output of each cell.

looking up wire gauge current ratings, 22awg seems to be rated at 7amps.  i know current capacity varies based on temperature but this should be a decent indicator.

i think the question answers itself, but it seems i should use 16awg to be able to carry the 20amp continous discharge these cells are capable of producing, right?  is there some nuance i'm missing?  also, would it be possible to coil this 22awg wire to double its carrying capacity?

<img src="/uploads/db1493/original/3X/c/d/cde7576d352fd81a156e5b0aabe094c7dcaa30d9.png" width="690" height="446">

<img src="/uploads/db1493/original/3X/2/9/29e470e1e5bd0dcd7cb15b29e9e444d021f37731.png" width="690" height="316">
```

---
## \#2 Posted by: chuttney1 Posted at: 2017-06-01T22:22:06.734Z Reads: 201

```
Use Aluminum wire. It's melting point makes it a good property in cutting off current without glowing like steel does.
```

---
## \#3 Posted by: chaka Posted at: 2017-06-01T22:26:55.012Z Reads: 197

```
Fuse size is a different spec than power transmission. FYI the smallest pack I have ever built is 10s6p. The cells will be under a larger load in a 10s3p so 22 awg may or may not be up to the task. The goal is to have a fuse that will still blow if a cell internally shorts. This becomes more difficult to spec in a small pack since you are relying on the remaining cells in parallel to produce enough current to blow the fuse on the offending cell.
```

---
## \#4 Posted by: thisguyhere Posted at: 2017-06-01T23:01:19.443Z Reads: 186

```
Got ya, thanks @chaka for chiming in.

I'm just going to double up the 22awg wire, twist it together, and try to run 20amp then a lot more than that as a test.  I'm hoping they'll hold up at 20amp, and blow at 30+amp.  We'll see.
```

---
## \#5 Posted by: Jinra Posted at: 2017-06-01T23:09:21.073Z Reads: 172

```
For me on 10s4p, 22awg tin-coated copper wire was sufficient.
```

---
## \#6 Posted by: thisguyhere Posted at: 2017-06-01T23:14:50.878Z Reads: 172

```
i'm just confused because these wire gauge specifications are saying 22awg is good for 7amp.  i'm confused.

@Titoxd10001 also told me 22awg is good on his 10s4p pack.  assuming motor max is 60amp, a 4p pack would mean 15amp draw for each cell.  my 12s3p pack will be 20amp draw.

yea, i think i'm going to twist 22awg wire together and test it.
```

---
## \#7 Posted by: chaka Posted at: 2017-06-01T23:15:11.740Z Reads: 167

```
22 awg nickle plated copper wire will blow at approximately 40 amps depending on the length of the fuse wire. If you double it up they probably wont blow.
```

---
## \#8 Posted by: Jinra Posted at: 2017-06-01T23:16:19.635Z Reads: 162

```
For tin wire it'll probably blow at lower amps. tin coated copper will blow at higher current.
```

---
## \#9 Posted by: thisguyhere Posted at: 2017-06-01T23:21:11.586Z Reads: 161

```
[quote="chaka, post:7, topic:24343"]
22 awg nickle plated copper wire will blow at approximately 40 amps
[/quote]

really?  if that's the case, then yea a single strand would work just fine.

[quote="Jinra, post:8, topic:24343"]
tin coated copper will blow at higher current
[/quote]

i think the ampacity charts must not be for tin coated copper...

ok, thanks for the input guys, i feel a lot better about this now.
```

---
## \#10 Posted by: chaka Posted at: 2017-06-01T23:24:47.840Z Reads: 151

```
Those charts are for actual wiring over long lengths. Longer the length the higher the resistance and the more it will heat up under load.
```

---
## \#11 Posted by: thisguyhere Posted at: 2017-06-01T23:25:28.680Z Reads: 148

```
makes sense, like for home and industrial wiring...

ok got all excited for no reason.
```

---
## \#12 Posted by: Titoxd10001 Posted at: 2017-06-01T23:31:03.088Z Reads: 151

```
I'm uing 22awg wire in my 11s4p pack and have pulled about 80 battery amps peak. Holding up good so far. Soldering was a pain over 200 joints I think lol

@chaka are you still using cell level fusing? And are you using cell holders still or a new method?
```

---
## \#13 Posted by: chaka Posted at: 2017-06-01T23:40:09.033Z Reads: 154

```
We are not using the cell holders anymore, switched to using fishpaper and dow corning 737 silicon to save space and make a thin pack.
```

---
## \#14 Posted by: Titoxd10001 Posted at: 2017-06-03T08:34:08.302Z Reads: 137

```
Cool. Do you have more info on how everything is secured. Is silicon​ holding the cells together? Fish paper has adhesive for the buss bar I'm guessing? And how do you secure battery packs to the board.
```

---
## \#15 Posted by: Jinra Posted at: 2017-06-03T08:42:04.431Z Reads: 138

```
My setup if you're interested.

<img src="/uploads/db1493/original/3X/d/8/d80afec8f5a781ec860a0d58991d39f2114bb805.png" width="375" height="500">

Some of those extra solder poitns you see on the buss bars are because the fusing broken (probably from vibration), so instead of lifting the buss bar to resolder underneath, I just soldered on top.
```

---
## \#16 Posted by: Titoxd10001 Posted at: 2017-06-03T18:28:08.002Z Reads: 130

```
Thanks, your images helped for my first battery build. What i wanted to understand is how chaka was keeping everything together because he no longer uses 3d printed cell holders

The fuse wire broke? It seems quite flexible. Do you have your cells and the bus bars glued down? Wondering​ if I should be worried about my pack now
```

---
## \#17 Posted by: thisguyhere Posted at: 2017-06-03T18:43:03.798Z Reads: 130

```
Mmmm sexy, the inside of my enclosure is SO MUCH more disorganized.

Is the bms underneath the anti spark switch?
```

---
## \#18 Posted by: Jinra Posted at: 2017-06-03T19:03:08.143Z Reads: 130

```
yep, though i ordered a different bms to replace it since that one doesn't balance.
```

---
## \#19 Posted by: Jinra Posted at: 2017-06-03T19:04:39.458Z Reads: 130

```
the bars are hot glued to the cell holders, but the pack is loosely sitting in the case. It could be higher internal resistance causing the wire to blow too, i did put two wires for one of the cells since it kept breaking.
```

---
## \#20 Posted by: Titoxd10001 Posted at: 2017-06-06T02:07:10.114Z Reads: 122

```
I wouldn't have thought vibration could break a wire. Your cells are glued to the cell holders? if not they can possibly rotate causing stress on fuse wire. I use 22 awg and working so far. I do have double side foam tape, maybe that adds a little extra dampening. The wires I can visually inspect look good and voltages looks good, but I'll try to monitor more closely. 

If your using two wires do think it would be better to just use silicone strand wire in thinner 16-20 gauge+bus bar since youre not getting fuse action but you can still solder easily.
```

---
## \#21 Posted by: Jinra Posted at: 2017-06-06T02:09:20.588Z Reads: 115

```
The cells are taped so they shouldn't be moving around. Also I had to measure voltages to find out a wire was broken, it's really hard to tell as it still looks like it's connected sometimes.
```

---
## \#22 Posted by: Titoxd10001 Posted at: 2017-06-06T02:36:41.305Z Reads: 116

```
You never know, I applied a little adhesive goop to be sure. I do check voltages before every charge. Do the fuse wires break in any general area like at the solder joints or right in the middle of wire, on the bends.
```

---
## \#23 Posted by: Jinra Posted at: 2017-06-06T03:50:25.449Z Reads: 115

```
I only have 3 out of the 80 break. however one of them was very stubborn and kept breaking over and over which is why I have two wires on it. it seems to be random where they break but I think it's most frequently at the solder joint
```

---
## \#24 Posted by: Titoxd10001 Posted at: 2017-06-07T01:31:48.102Z Reads: 114

```
Still think you should glue down your cells. Anyway just curious would you buy/make a spot welder next time or same method with different wire like silicone. Kind of like this method because with proper technique I don't think you'll damgae the cells and I don't make that many packs to invest in more tools. Spot welder would be nice though
```

---
## \#25 Posted by: longhairedboy Posted at: 2017-06-07T02:28:53.047Z Reads: 115

```
They've got that silicone @chaka was talking about here:
https://www.ellsworth.com/products/by-market/consumer-products/sealants/silicone/dow-corning-737-neutral-cure-sealant-silicone-clear-300-ml-cartridge/

I ordered some for my builds. If anyone knows of a less expensive place to buy it, hit me up. The price didn't seem too unreasonable.
```

---
## \#26 Posted by: longhairedboy Posted at: 2017-06-07T02:41:17.527Z Reads: 111

```
What eswitch is that?
```

---
## \#27 Posted by: ekitesurfer Posted at: 2017-06-07T03:09:42.615Z Reads: 111

```
Is hot glue a big no no?
```

---
## \#28 Posted by: longhairedboy Posted at: 2017-06-07T03:39:30.034Z Reads: 110

```
hot glue is fine. you can tack your cells into P groups with hot glue all day long, build your entire pack with it. That's what i do. 

using regular silicone, like the generic 100% clear silicone sealant for doors and windows, to seal a pack into a box seems to be the nono here. There's evidence that the vapors from the curing silicone can cause corrosion. It does seem to cause some kind of weird condensation on the heat shrink for sure. I've stopped using it and started using the 737.
```

---
## \#29 Posted by: Jinra Posted at: 2017-06-07T06:48:25.769Z Reads: 105

```
DIYES (torqueboards)
```

---
## \#30 Posted by: longhairedboy Posted at: 2017-06-07T19:12:59.728Z Reads: 101

```
it looks like a flyer and a vedder had a baby.
```

---
