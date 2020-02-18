# XYRS BOM for vedder&rsquo;s spark switch

### Replies: 24 Views: 2027

## \#1 Posted by: longhairedboy Posted at: 2016-09-13T18:51:19.413Z Reads: 163

```
I'm going to have some made to use in my builds and maybe sell as well, and throw Vedder some donations while I'm at it. 

The problem is the BOM on GitHub for the project isn't in the XYRS format that I need to have them made, so before i go and pay them extra to convert the existing BOM which is more of a simple parts list, could somebody tell me if this exists already somewhere?

Somebody, somewhere, has done this. They charge $75 an hour for this kind of thing, so i'd rather avoid it if possible. 

Whoever can hook me up with this will get a free switch or two when i get them in if it works.
```

---
## \#2 Posted by: JuniorPotato93 Posted at: 2016-09-13T18:59:42.839Z Reads: 157

```
I tried googling and brute forcing through a few pages of lists but I realized very quickly I was not going to be able to add any value. I'm afraid electronics daze and confuse my mind, I'm more of a mechanical creature.
```

---
## \#3 Posted by: DeathCookies Posted at: 2016-09-13T19:04:14.831Z Reads: 154

```
I had some problems inserting the BOM even if i have converted it to csv or something else....
You best bet is to open the bom and search for the five mouser numbers. :thumbsup:

_Currently i am going to make some myself and for the european room ;)_
```

---
## \#4 Posted by: longhairedboy Posted at: 2016-09-13T19:04:35.058Z Reads: 147

```
and i have zero experience with PCB layout despite being able to do all of this soldering and stuff myself if it comes down to that. I just don't want to do it myself. I'd rather use that time to come up with a better deck and box system or better battery pack layouts or better yet, chase my 2 year old around the house while he giggles wildly.
```

---
## \#5 Posted by: longhairedboy Posted at: 2016-09-13T19:06:12.809Z Reads: 146

```
i have the mouser numbers, i just don't want to order the parts and assemble it myself. It needs to be in this particular format or the place that will make them for me will have to do that work and charge me for it.
```

---
## \#6 Posted by: DeathCookies Posted at: 2016-09-13T19:10:10.858Z Reads: 146

```
Ah okay, now i got you. XYRS is a gerber file.

Maybe you can download gerber, import the switch and export it as XYRS ;)
```

---
## \#7 Posted by: longhairedboy Posted at: 2016-09-13T19:12:28.958Z Reads: 143

```
i'll see if i can do that... maybe that really is all there is to it.
```

---
## \#8 Posted by: smurf Posted at: 2016-09-13T19:12:46.379Z Reads: 144

```
I was thinking about making my own with this stuff

http://surplustek.ca/image/cache/data/Prototype-b-font-Copper-font-b-PCB-500x500_0.jpg
```

---
## \#9 Posted by: DeathCookies Posted at: 2016-09-13T19:30:46.910Z Reads: 132

```
[quote="longhairedboy, post:7, topic:9545, full:true"]
i'll see if i can do that... maybe that really is all there is to it.
[/quote]

Mhm...somehow it seems that it is not that easy...

Maybe this can help you
http://trickel.org/thomas/skc/Engg/ENGG_340/How_to_Eagle.txt
```

---
## \#10 Posted by: DeathCookies Posted at: 2016-09-13T19:53:07.555Z Reads: 133

```
Edit:
"Every CAD system can generate this information. The XYRS is simply the information needed to place (or find) a component on the assembly. The (XY) information is in inches, MM, or Mils; and is measured from a given board origin. The (R) rotation is in degrees clock-wise (0, 45, 90, etc.). The (S) side is usually defaulted to the top side, but can be expressed as Top/Bottom or even 0/1."
Source: http://aa-pcbassembly.com/resources/faqs/
```

---
## \#11 Posted by: elkick Posted at: 2016-09-13T21:28:03.827Z Reads: 125

```
You should use @chaka's template, it's more robust.
https://oshpark.com/shared_projects/XuqJkZzU
```

---
## \#12 Posted by: sl33py Posted at: 2016-09-13T23:29:59.829Z Reads: 117

```
[quote="elkick, post:11, topic:9545"]
it's more robust.
[/quote]


I didn't realize there is a v1.4 out there.  What's more robust specifically?
```

---
## \#13 Posted by: zmoney Posted at: 2016-09-13T23:58:50.413Z Reads: 114

```
It allows for heavier current on the PCB traces
```

---
## \#14 Posted by: longhairedboy Posted at: 2016-09-14T00:30:35.793Z Reads: 107

```
i have a face full of giant cheeseburger but I wanted to stop in and say I found it. Thanks!
```

---
## \#15 Posted by: longhairedboy Posted at: 2016-09-15T18:56:02.474Z Reads: 92

```
BTW four of these guys will be here in about two weeks for testing. I'm only going to need two of them for now so i'l be happy to let go of the other two to help recover my cost once i'm satisfied they're not crap. 

So if anyone is interested in a v1.4 vedder switch with 75v mosfets let me know and i'll sell you one and include a detachable rocker switch to boot. No heatsinks yet, but i'm going to try and figure something out for that when i get them in. 

my plan is to sell these and throw vedder some dough if they work out. He deserves our support for being so awesome and making so much of this shit we do possible.
```

---
## \#16 Posted by: sl33py Posted at: 2016-09-27T05:16:11.478Z Reads: 65

```
How does v1.4 differ from v1.3?  I was going to get some more kits and continue to send $ to vedder, but the github he has still shows v1.3 as most current.
```

---
## \#17 Posted by: lox897 Posted at: 2016-09-27T06:24:53.847Z Reads: 65

```
I think someone made the traces bigger to handle more current
```

---
## \#18 Posted by: DeathCookies Posted at: 2016-09-27T06:50:49.366Z Reads: 70

```
It was chaka:
https://oshpark.com/shared_projects/XuqJkZzU
```

---
## \#19 Posted by: chaka Posted at: 2016-09-27T07:26:44.624Z Reads: 70

```
I actually stitched the traces together to double the current capability of the traces.  Priory to the update some users were heating the traces up enough to dislodge the fets. No longer an issue with the added through holes.

 I have an updated gerber with jst-ph  ports instead of solder pads for the 3 pin switch if anyone wants it. I have been holding off on sharing the files since I have been working on incorporating a few other features to the pcb.

Here is the Osh link if anyone wants it.: <a href="https://oshpark.com/shared_projects/Ryc1HY3u"><img src="https://oshpark.com/assets/badge-5b7ec47045b78aef6eb9d83b3bac6b1920de805e9a0c227658eac6e19a045b9c.png" alt="Order from OSH Park"></img></a>
https://644db4de3505c40a0444-327723bce298e3ff5813fb42baeefbaa.ssl.cf1.rackcdn.com/85e5c91f2d194d8e5bddefbd1955473b.png    
https://644db4de3505c40a0444-327723bce298e3ff5813fb42baeefbaa.ssl.cf1.rackcdn.com/8e98a6af06a0c3ca38f416327afff0b6.png
```

---
## \#20 Posted by: sl33py Posted at: 2016-09-27T16:24:37.675Z Reads: 58

```
very cool.  Wouldn't a 2oz pcb vs 1oz also alleviate this?  

Thanks @Chaka!
```

---
## \#21 Posted by: chaka Posted at: 2016-09-27T17:58:05.704Z Reads: 55

```
Not entirely. I would still stitch them and add a heat sink to the back side.
```

---
## \#22 Posted by: SORRENTINO Posted at: 2016-09-27T18:13:13.113Z Reads: 53

```
SO SAME BOM AS 1.3 FOR CHAKA VERSION? JUST WANT TO MAKE SURE. :slight_smile:

THANKS MATT
```

---
## \#23 Posted by: sl33py Posted at: 2016-09-27T18:34:52.151Z Reads: 54

```
[quote="SORRENTINO, post:22, topic:9545"]
SO SAME BOM AS 1.3 FOR CHAKA VERSION? JUST WANT TO MAKE SURE. :slight_smile:

THANKS MATT
[/quote]


YES - SAME BOM.  (said in a LOUD voice kind of like yelling) :stuck_out_tongue_winking_eye:

[quote="chaka, post:21, topic:9545, full:true"]
Not entirely. I would still stitch them and add a heat sink to the back side.
[/quote]
@Chaka - i didn't realize you added the heatsink to the back.  I thought that was mounted to your FETs.  Neat idea, but you must cut the heatsink or how do you insulate so it doesn't short?
```

---
## \#24 Posted by: longhairedboy Posted at: 2016-09-27T19:56:31.897Z Reads: 48

```
i read elsewhere on here that part of the reason for doing that is that not enough heat is transferred through the front of the FET to make the heatsinks effective. So i'm also curious about heat sinks not shorting out the stuff they're attached to. 

Hopefully these guys will be showing up soon so i can play with them. 

In other news, i contacted that guy with the open source LiFePo4 BMS. He says he's still a few months out getting it functional and ready for testing, but i told him i'd be happy to have a few made and a test them out and give him some feedback as well as monetary support if they work out and can be sold. He also said modding it for Li-Ion would only require swaping a few resistors, so its possible to have a couple of different flavors. That's something that this community is in dire need of. A fully open source BMS solution with a feature set specifically geared towards electric skateboards. It really is the last piece of the puzzle. Between that and the VESC, its really all you need for a fully hackable system.
```

---
