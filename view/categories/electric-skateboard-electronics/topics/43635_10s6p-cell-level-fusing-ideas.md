# 10s6p cell level fusing&hellip;. Ideas?

### Replies: 37 Views: 2455

## \#1 Posted by: trigger4point7 Posted at: 2018-01-13T18:21:30.556Z Reads: 293

```
I'm trying to reason about how to build a two layer pack with cell level fusing. Any ideas out there? I've been looking around and nothing so far. I've got to build this thing safe!
```

---
## \#2 Posted by: Lukas Posted at: 2018-01-13T18:23:14.062Z Reads: 293

```
Did you see this thread?
https://www.electric-skateboard.builders/t/ollinboards-cell-level-fuse/7392
```

---
## \#3 Posted by: trigger4point7 Posted at: 2018-01-13T18:41:55.628Z Reads: 283

```
I've read through it before but I don't remember anything about a double layer design.
```

---
## \#4 Posted by: michaelcpg Posted at: 2018-01-15T00:41:03.262Z Reads: 251

```
Here's a modular design I came up with a while ago. The sides of each group of cells is spot welded with a nickel strip thats folded over a sheet of fibreglass like this stuff:

https://www.ebay.com/itm/12x6-1mm-G10-FR4-Glassfibre-Sheet-Epoxy-Glass-Smooth-Fibreglass-Sheet-Board-/142465838559

Then I use brass bars as a bus bar on each side with the fuse wires soldered between the bus bar and nickel strips. Both the bus bar and nickel strips are held in place with plenty of hot glue (Doesn't look particularly tidy but it does the job). Then I glue another layer of fibreglass over the top to as a layer of protection/insulation.

![20170702_180937|690x388](upload://4IPSJHjp69X9ScG6fTbEcWUU8pu.jpg)![20170715_221526|690x388](upload://1QKvyT1MAWFoN9ELFae0E55JUW9.jpg)![20170719_204034|281x500](upload://Am0cPsEpb7lLfrXTGUosOSQzf4Y.jpg)![20170716_233553|690x388](upload://yC27nRq38TTk9nHODze5UOEtLgd.jpg)![20170716_233506|690x388](upload://3mcD9PV9jsFR0DSd4HqYSOGmknv.jpg)
```

---
## \#5 Posted by: trigger4point7 Posted at: 2018-01-15T01:00:36.316Z Reads: 228

```
Oh sweet! Cleaver design. What sort of enclosure did you put those batteries in?
```

---
## \#6 Posted by: michaelcpg Posted at: 2018-01-15T01:06:30.075Z Reads: 234

```
Cheers. These are being used on a Loaded Vanguard so I made a pair of enclosures out of ABS. 6 packs in one and 4 packs + ESCs in the other
```

---
## \#7 Posted by: akhlut Posted at: 2018-01-15T14:49:52.867Z Reads: 229

```
I'm working on a different approach.  Just spitballing now, but I really like the PCB that @Blasto and @Kaly are using.  Super reliable and easy to troubleshoot.  I'd like to modularize the idea to make it airplane safe and completely toolless.  Uses TE Micro Mate-N-Lok connectors for the balance leads.  Hopefully they're vibration-resistant enough for the application.  A 3D printed fixture may be added to secure these connectors in place.

Something like this:

http://a360.co/2DA2ONU

that implements this:

https://www.youtube.com/watch?v=c7PGLFgkdf4

I really like how @Kaly does his packs:

https://www.electric-skateboard.builders/t/no-words-just-pictures-delete-words-use-pm/2992/3035

I just need to work on the PCB's, which is easy.
```

---
## \#8 Posted by: trigger4point7 Posted at: 2018-01-20T21:04:58.009Z Reads: 208

```
Its so subjective, but what is the range your getting with the 6P pack?
```

---
## \#9 Posted by: sash Posted at: 2018-01-24T03:34:34.356Z Reads: 200

```
I am trying to figure out how to do cell level fusing for 10SP4 pack in 2 layers.   Thinking to cover positive ends of each P group by a PCB cut to its shape with 4 drilled holes for cathodes of the cells.   Then run fuse wires from the cathodes to the PCB.

Lot's of ideas in this thread:

http://www.electric-skateboard.builders/t/fishpaper-and-cell-level-fusing-use-it/35026
```

---
## \#10 Posted by: trigger4point7 Posted at: 2018-01-25T19:59:54.774Z Reads: 173

```
That's not a bad idea, I think that is what @michaelcpg achieved above. The only negative of that approach is having to make sure you have space for the extra length of the cell + the PCB or Fiberglass. If you have the space for it, do it. Are you pulling the trigger on it? Care to share some pics of the experience?
```

---
## \#11 Posted by: michaelcpg Posted at: 2018-01-25T20:22:58.054Z Reads: 169

```
I'm currently working on a 1.1Kwh mountainboard build and I've come up with a slightly more refined (and hopefully much simpler and quicker to build) design for the new pack. 

Although it's more designed for single layer packs, it could probably be fairly easily used on double layer packs with no issues and should only make the cells a couple mm longer. 

I'll see if I can find some time this weekend to draw up a model of the idea if anyone is interested
```

---
## \#12 Posted by: trigger4point7 Posted at: 2018-01-25T20:45:41.703Z Reads: 160

```
We're interested :slight_smile:
```

---
## \#13 Posted by: sash Posted at: 2018-01-26T05:21:41.031Z Reads: 150

```
I am interested too.
```

---
## \#14 Posted by: sash Posted at: 2018-01-26T05:35:16.320Z Reads: 152

```
Speaking about your double layered design above...

Why do you put fuses on both sides of cells?  It is enough to fuse only one side, right?

I am thinking about the following modification:   Put fiberglass plates and fuses only on one side of a pack.  Connect the other side by nickel strips as usual.  Make two packs like this and glue them by the sides that don't have fuses.   Then all fuses will be on the sides of the pack (mixed on pluses and minuses ).   It should be easy for inspection, replacement of fuses, etc.   

Hope it makes sense what I mean.
```

---
## \#15 Posted by: sash Posted at: 2018-01-26T05:45:04.336Z Reads: 146

```
... also instead of bus bar I want to use flat wire like this

https://www.mcmaster.com/#69925k66/=12w8di4

(because I already have it)

And instead of hot glue, I'll use neutral cure silicone.  (Hot glue is flammable.)
```

---
## \#16 Posted by: ZackoryCramer Posted at: 2018-01-26T06:04:10.300Z Reads: 147

```
If you don’t want to worry about taping and wrapping the batteries, you can use brackets as such. Looks clear and easier to handle. 
![image|620x500](upload://Uit6ZiYSKvWnRw32LJujsDbsat.jpg)
PM me if you want some.
```

---
## \#17 Posted by: Acido Posted at: 2018-01-26T06:08:38.111Z Reads: 135

```
It looks like small packages of coke with cables sticking out
```

---
## \#18 Posted by: trigger4point7 Posted at: 2018-01-26T06:22:46.788Z Reads: 135

```
The idea behind the trapizodial design is to save space. There aren't a lot or hardly any enclosures that fit 6P even with that design.
```

---
## \#19 Posted by: ZackoryCramer Posted at: 2018-01-26T06:24:07.767Z Reads: 137

```
Oh. Thanks. I didn't quite get it in the beginning :stuck_out_tongue:
```

---
## \#20 Posted by: sash Posted at: 2018-01-27T19:26:47.082Z Reads: 128

```
Still trying to decide if I'll go for cell level fusing, or just spot weld the cells as usual. Sure I'll post pics if I pull the trigger.
```

---
## \#21 Posted by: trigger4point7 Posted at: 2018-01-30T19:42:19.478Z Reads: 116

```
I'm warming up more and more to this idea. One question I have is are you doing anything to adhere glassfibre sheet to the P group? Or are you just relying on the nickel tabs to take care of that? Do you feel like it is secure enough if that is the case?
```

---
## \#22 Posted by: michaelcpg Posted at: 2018-01-30T20:22:35.327Z Reads: 124

```
The nickel strips themselves basically just hold the fibreglass sheets in place. Before I fold the nickel strips over the edges of fibreglass, I also apply a thin strip of hot glue along each long edge of fibreglass which you can kinda see in the last photo. 

This means that when you fold the nickel strips over, the bending angle of the strips isn't quite as sharp which should ideally create a little less stress in the bend but it also means when you solder the fuse wires to the strips, the glue underneath melts and helps to secure the strips in place.

Keep in mind that this battery build took a lot longer than I was expecting. Reproducing it now would take a lot less time due to the fact that I did a fair bit of prototyping with similar ideas and testing etc. 

To speed up the process even more though, I wouldn't worry about fuse wires on the negative terminals. Instead you could possibly just create a bus bar out of a bunch of nickel strips welded on top of each other and then spot weld each negative terminal directly to it. 

Also could be worth playing around with the idea of using flat copper braid instead of the 10AWG wire that I've used for the wire that runs up the side of the cells, should be easier to work with in regards to bending to the angles and will be a bit flatter/cleaner looking :)
```

---
## \#23 Posted by: Hummie Posted at: 2018-01-30T20:23:55.318Z Reads: 122

```
 The fuses open a circuit when a single cell in the p group shorts but when would a single cell short to begin with?  I'm wondering is this solely a safety feature for cells that are poorly manufactured and somehow have some conductive contaminant in a cell that surprises you later by shorting or are there other ways a shorting cell could happen?

  It's too late once a cell hits runaway, probably for the entire pack, but would a runaway cell be internally shorting or open?
```

---
## \#24 Posted by: scepterr Posted at: 2018-01-30T20:34:09.929Z Reads: 113

```
The only circumstance I can see a cell shorting is against another cell.

A runaway cell, i guess can be open and/or closed throughout the runaway?
```

---
## \#25 Posted by: Hummie Posted at: 2018-01-30T20:36:23.971Z Reads: 112

```
Yea that's hella common I bet. Done that. No fire just sound of vents opening and I ran it outside.
```

---
## \#26 Posted by: scepterr Posted at: 2018-01-30T20:39:20.312Z Reads: 109

```
I find the CID to be an adequate protection device, the only issue is not being able to visually tell if a cell in p group had it's CID triggered without taking the p group apart, or doing a capacity test on each P group
```

---
## \#27 Posted by: Hummie Posted at: 2018-01-30T20:44:16.446Z Reads: 112

```
But if the CID is triggered I imagine with the now decreased capacity of the p group the voltage will go higher than the rest when charging and lower when discharging than the other p groups and could be spotted
```

---
## \#28 Posted by: scepterr Posted at: 2018-01-30T20:46:02.691Z Reads: 108

```
Yeah that would be the effect
Though there could circumstances when that doesn't show, like if youre not draining the whole battery below the capacity of the affected p group. 

I gotta look back at all that tests I did when starting my PowerWall, 10000 mixed cells working in harmony 😃
```

---
## \#29 Posted by: michaelcpg Posted at: 2018-01-30T21:30:00.592Z Reads: 102

```
One easy to way to spot if you've got a broken fuse wire when using a BMS is you'll find that the BMS will cut the charge to the pack before you can charge the battery to 100%
```

---
## \#30 Posted by: michaelcpg Posted at: 2018-01-30T21:35:27.037Z Reads: 105

```
Another guess would be for when over time as cell resistances increase, if some cell resistances increase at greater rates than others, you'll end up with different current levels going through different cells. You could potentially get to the point where a significantly larger current, potentially greater than what the cell is designed to handle, is being drawn from a single lower resistance cell in a P pack.

Either way, there's obviously a reason why Tesla does it :p
```

---
## \#31 Posted by: scepterr Posted at: 2018-01-30T21:52:44.266Z Reads: 104

```
As for Tesla, last I can recall their cells don't have a CID, that mightve changed in newer models though, haven't looked in a while
```

---
## \#32 Posted by: trigger4point7 Posted at: 2018-03-25T21:19:00.336Z Reads: 94

```
@michaelcpg or  @scepterr I picked up this non-flamable industrial glue. I'm considering it to hold down the bussbar. Any reason I shouldn't or should I stick with the battle tested hot glue?
 ![15220125993874700034794462764653|375x500](upload://gZHQzqKUzgscbaM9KM9Wog21BMW.jpg)
```

---
## \#33 Posted by: scepterr Posted at: 2018-03-25T21:31:28.466Z Reads: 94

```
The description is deceiving, not sure what about is "industrial" lol. Pretty sure it'll burn off when soldering, 
![Screenshot_20180325-172858|281x500](upload://8pzkso5flyBdqpScZjDFOhKJOhI.png)

I would use a high temp safe epoxy or just some kapton to hold it down when soldering
```

---
## \#34 Posted by: michaelcpg Posted at: 2018-03-25T21:38:38.058Z Reads: 92

```
Neutral cure silicone is another good option which handles vibrations really well although it takes a while to set
```

---
## \#35 Posted by: moon Posted at: 2018-08-02T20:35:10.969Z Reads: 65

```
Did you get anywhere with this :)

edit - looked at the fusion file. Looks very promising
```

---
## \#36 Posted by: akhlut Posted at: 2018-08-02T21:00:17.510Z Reads: 60

```
abandoned.  too complex and ultimately unnecessary.

To to 10s6p fused just use two 3p backer PCB's and set them up for fusing.  Use braid between the 3p busses to get to 6p.  That's my plan anyway.
```

---
## \#37 Posted by: moon Posted at: 2018-08-02T21:08:04.312Z Reads: 60

```
Ok. I just liked the travel pack part of it the most

I think I have to to use those pcbs too but this is my first pack and can't seem to find many packs that use those pcbs you made. I am making a 10s3p 30q pack now

I have already welded the cells together with 1 layer 8*0.15mm nickel. I was hoping I could get some good advice on what I could do next.

I was planning on using 12awg or 10awg to solder onto the nickel that's welded to the batteries. Then solder the other side to the pcb, probably two connections on both the positive and negative side of the pack.like this image:
![image|375x500](upload://qV5tD7KxM0u22LEl8ZyfViUtF6s.jpg)

Then for balance wires I have no clue where to start😥
```

---
