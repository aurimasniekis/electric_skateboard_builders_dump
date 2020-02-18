# Disassembled and made safe, pre-balancing and float charging

### Replies: 74 Views: 1893

## \#1 Posted by: Chase Posted at: 2018-06-20T22:17:15.104Z Reads: 379

```
So after seeing @evoheyax 's beautiful board go out in flames, I realize I had no idea what I was doing when I made my first battery. I was basically on a month long drinking binge and just do not trust whatever has been done. I have to make this battery safe. Here is the issues that I have with the current 12s4p  30Q build:

![IMG_0559|666x500](upload://12t2sy6cKY7IHaYihebwQTNP3eW.jpg)

1. Did not use fishpaper. The only fishpaper was small pieces under the balance leads. 

2. No insulated caps on positive ends

3. I only used one layer of 12mm .15 mm nickel strips. The seller says they are rated at 40 amps but from the tables I have seen recently, it seems way to high. Even then one layer wouldnt be enough for this 4p setup.

https://www.ebay.com/itm/Solid-Pure-Nickel-Strap-Strip-Spot-Welding-battery-12mm-x-0-15mm-12x0-15-40A/263068537518?var=562069545322&hash=item3d401b52ae:m:mUyORsdr1PEgRuE9LsvRdkQ

![IMG_0567|666x500](upload://pIuiDfnAQDZuHPN0zYbUFxSbFJM.jpg)

4. Possibly most importantly, I dont trust the way I bridged my serial connections across the pack. I looked for several methods but I ended up just welding strips across then folding the pack outward to be flat like in the picture below. The first time I did this the stress of bending caused most of them to break off.

![IMG_0565|666x500](upload://y02Wm35PNVPQmsGLmfwZDnTS6Uf.jpg)



My ideas and questions.

1. At this point I would love to try to pull off the stripping and reuse the cells since they are new. Of course they would have little metal burs that would need to be smoothed out. I have gotten mixed responses on doing this. In the video below the guy uses a dremel. **Is this safe, or am I stuck buying new cells?**

https://www.youtube.com/watch?v=iScKCOH3eqA


2. What is the best way to bridge series across the pack? The way I did in this pic just seems like an issue waiting to happen. I like the way cell level fusing makes the connections across the top of the bus bars. Would it be stupid to make a nickel connection from each cell to a bus bar and then connect across the pack that way? If thats a bad idea, what is the absolute best way to make these connections?

![IMG_0565|666x500](upload://y02Wm35PNVPQmsGLmfwZDnTS6Uf.jpg) 

Any other advise or help is appreciated.
```

---
## \#2 Posted by: Randyc1 Posted at: 2018-06-20T22:22:16.744Z Reads: 336

```
Does you pack need to bend ?
```

---
## \#3 Posted by: Chase Posted at: 2018-06-20T22:25:01.527Z Reads: 336

```
No it does not.
```

---
## \#4 Posted by: Randyc1 Posted at: 2018-06-20T22:28:08.831Z Reads: 339

```
Do you have a diagram of how your cells are layed out in your pack ?...ok nevermind,.. i see how your pack is built in 1st pic
```

---
## \#5 Posted by: Chase Posted at: 2018-06-20T22:30:32.816Z Reads: 334

```
It’s just like this except 12s4p

![image|690x404](upload://iYxQmQyl8EO0085rqBVdqeB6Kfm.jpeg)
```

---
## \#6 Posted by: Randyc1 Posted at: 2018-06-20T22:37:43.097Z Reads: 306

```
My first pack was built the same way![20170530_134130-2016x1512|666x500](upload://ivycefEkT43hKVaVPgPbpDT8CBb.jpg) but I soldered a 12G solid wire on Edge of nickel strip (Before) spot welding on cells....I also did put 1 bending joint in middle of pack just to be sure
```

---
## \#7 Posted by: Randyc1 Posted at: 2018-06-20T22:42:05.898Z Reads: 302

```
Next pack will be made with these PCB glued on top of each parrallel pack.![70A3CB60-5486-4D21-A295-80A515549CCB|375x500](upload://orAEoUiAW7pMbTv1AModHWcEY0X.jpeg)
```

---
## \#8 Posted by: Chase Posted at: 2018-06-20T22:43:31.594Z Reads: 295

```
So you will essentially use that like a double bus bar to bridge the connections. I like it. Where can I find those?
```

---
## \#9 Posted by: moon Posted at: 2018-06-20T22:45:42.612Z Reads: 291

```
Think he made them
```

---
## \#10 Posted by: Randyc1 Posted at: 2018-06-20T22:46:52.200Z Reads: 291

```
From PCBway.com,.. someone i know ordered them for me .
```

---
## \#11 Posted by: thisguyhere Posted at: 2018-06-20T22:52:05.231Z Reads: 283

```
in terms of salvaging your cells, no problem grinding the terminals to smooth out the burrs from prying off nickel.  it's just you can't do it more than...once or twice since you'll be removing material from the terminals which are already thin.
```

---
## \#12 Posted by: Chase Posted at: 2018-06-20T22:54:53.444Z Reads: 275

```
Thank you. Any advice on the best way to bridge series across the pack? I just feel like bending nickel like in the above pics is reasonable or stable. Is this busbar idea reasonable? If so do you know a decent source for the small brass strips?
```

---
## \#13 Posted by: Randyc1 Posted at: 2018-06-20T22:59:04.518Z Reads: 269

```
Got mine from some huge 8 Guage scrap of  wire that had about 8 strand of these solid wires in it....otherwise you can just spot weld 2-3 more nickel strips on top to increase amp capacity.
```

---
## \#14 Posted by: thisguyhere Posted at: 2018-06-20T23:05:21.168Z Reads: 269

```
i'll take some photos tonight, i've got a pack in progress now.  my series connections are using flat copper strand.

i ran a 12s3p in exactly the same way you've constructed your pack and by the time i salvaged it, there wasn't a single visible problem with it.

that's to say, i don't think there's any obvious shortcomings with what you're doing but in the spirit of safety, at least insulate your cells better.  cap insulators, fish paper...hell, dime roll wraps.
```

---
## \#15 Posted by: Chase Posted at: 2018-06-20T23:07:02.568Z Reads: 262

```
Thanks you. I greatly appreciate this. I look forward to seeing the pictures.
```

---
## \#16 Posted by: Randyc1 Posted at: 2018-06-20T23:24:50.876Z Reads: 267

```
Also try to make nice solid spot welds to prevent issues![20160423_144858|690x388](upload://yQOPjeXD508xuIZtL4bkN5NNSYp.jpg)
```

---
## \#17 Posted by: thisguyhere Posted at: 2018-06-20T23:33:08.508Z Reads: 270

```
yea, those are nice beefy welds, evenly distributed.  good point.
```

---
## \#18 Posted by: Chase Posted at: 2018-06-21T01:56:57.938Z Reads: 263

```
In the meantime you guys have any good local US sources for adhesive backed fishpaper? I’ve found it in amazon but not adhesive backed
```

---
## \#19 Posted by: lrdesigns Posted at: 2018-06-21T02:49:22.511Z Reads: 268

```
Well good on you for taking the hard decision to rebuild the pack. I think the cells will be fine to reuse if your not too rough with disassembly. 

The thing that always freaked me out about some peoples packs is how close the nickel is to the - can where it welds to the positive terminal.
```

---
## \#20 Posted by: thisguyhere Posted at: 2018-06-21T04:10:28.847Z Reads: 269

```
here's P group, fish paper both ends, then clear pvc shrink:

![0620181836|281x499](upload://fsLTz2ztJO2FabTGegiJ1hjTQNn.jpg)

all cells have insulator caps, cut away pvc shrink, welded with tabs for series connection:

![0620181837|690x388](upload://93qsmoKOMUPpVCDxlFvjQ1GdfOI.jpg)

using copper strand for series connections, going to solder tabs to copper strand.

![0620181838|690x388](upload://lzZoVdaCWiZ4CcJpRiaFP8XTBs0.jpg)

when pack is complete, each 6s6p group will be shrink wrapped again and slots cut through to allow for some amount of flex:

![0620181839|690x388](upload://6sQx5njtTZYv77EZBMOPZWmVxB0.jpg)
```

---
## \#21 Posted by: deucesdown Posted at: 2018-06-21T04:33:09.295Z Reads: 246

```
It that hummie deck? Sweet. The only concern I have is carrying 6 cells worth of current through just 2 nickel strips: it's probably way fine in real life but I'm super cautious. Would be cool to do this foldover with like a 3 cell wide nickel sheet.
```

---
## \#22 Posted by: Chase Posted at: 2018-06-21T04:48:18.965Z Reads: 247

```
Where did you get that copper strand. Probably more conducive, but do you think it’s as stable as the flat sheets?
```

---
## \#23 Posted by: thisguyhere Posted at: 2018-06-21T04:57:12.982Z Reads: 245

```
[quote="deucesdown, post:21, topic:59532"]
The only concern I have is carrying 6 cells worth of current through just 2 nickel strips
[/quote]

my thinking is resistance increases over distance.  the tabs you see here are about 3mm so at that length ampacity should be well above average amp draw.  i mean, these cell fuses can do 20amp at short lengths so 10mm nickel should be able to handle it.  this is without any experimentation though.

i wouldn't run long lengths of nickel, like when making serial connections.

[quote="Chase, post:22, topic:59532, full:true"]
Where did you get that copper strand.
[/quote]

[ebay](https://www.ebay.com/itm/5-FEET-1-2-BRAIDED-GROUND-STRAP-GROUNDING-BARE-PURE-COPPER-FLAT-BRAID-IN-USA-/292009190103)

[quote="Chase, post:22, topic:59532, full:true"]
do you think it’s as stable as the flat sheets?
[/quote]

it's going to get secured down, insulated with kapton, the whole pack will be pvc shrinked again when it's complete.
```

---
## \#24 Posted by: Chase Posted at: 2018-06-21T08:27:52.932Z Reads: 218

```
Does this make sense being rated for 40 amps?

https://m.ebay.com/itm/Solid-Pure-Nickel-Strap-Strip-Spot-Welding-battery-12mm-x-0-15mm-12x0-15-40A/263068537518?varId=562069545322&_mwBanner=1&_rdt=1
```

---
## \#25 Posted by: lrdesigns Posted at: 2018-06-21T08:33:46.048Z Reads: 221

```
> Binge drinking and battery building. 

The obvious solution is to switch to the :japanese_ogre:'s :green_salad:
```

---
## \#26 Posted by: thisguyhere Posted at: 2018-06-21T16:00:15.859Z Reads: 212

```
technicaly yes, but you've got nickel, just use what you've got.

if you're concerned about long lengths of nickel, just double them up, and it doesn't have to be stacked the whole length either.  just double it up like half the length and it should up the ampacity.

![image|690x254](upload://s5ALeYmDfdLG2XbmTVGciqfd7Bd.jpg)

parallel lines on the bottom are nickel strips.
```

---
## \#27 Posted by: Chase Posted at: 2018-06-21T19:31:36.110Z Reads: 205

```
Thank you so much for all the advice and pictures
```

---
## \#28 Posted by: Chase Posted at: 2018-06-21T20:17:21.345Z Reads: 197

```
I live in California so your suggestion tends to be my oxygen. The drinking is just comes back to bite me every year or so and when it starts it takes a long time to sober back up.
```

---
## \#29 Posted by: Chase Posted at: 2018-06-21T21:30:04.523Z Reads: 189

```
Does it harm the cells at all if there was like a second long short/spark across two cells not connected in series? Was using scissors to remove some laptop and didn’t realize they had connected two cells. Quick spark. Still good cells? To be honest this happened a few times when I was inebriated as well just for brief seconds.
```

---
## \#30 Posted by: thisguyhere Posted at: 2018-06-21T22:13:12.856Z Reads: 185

```
nah, you're fine.  small sparks, as long as there isn't damage on the terminals, especially the positive (anode) end, are fine.

[quote="Chase, post:29, topic:59532"]
I was inebriated
[/quote]

i usually have a glass of wine around at all times but maybe not be shitfaced while you work in explosive batteries...
```

---
## \#32 Posted by: thisguyhere Posted at: 2018-06-21T22:42:25.927Z Reads: 182

```
i hear ya, i'm on about my 5th build and each build is an improvement over the one that came before it.

i think most people's first build is a bit of a mess then you go from there.

it's great you're doing your due diligence but there comes a point where you just have to build it.  and it being something you build, you can always improve incrementally going forward.
```

---
## \#33 Posted by: Chase Posted at: 2018-06-21T23:10:58.226Z Reads: 184

```
“As long as you don’t puncture a positive terminal”. When I was also a little out of it I decided to make a 10s1p, punctured the wrong part of the positive end. Started shootijg our flames. That’s partially why I’m so frightened to make my own stuff.

![image|375x500](upload://mtrNVc8bEgjKMeerXpCNwFGzTdd.jpeg) 

You can see the spot in the above pic where the problem occurred. Obviously I’ll be scraping this cell.

Grinding down terminals now. Re heat shrinking because most ripped off from the superglue
```

---
## \#34 Posted by: psychotiller Posted at: 2018-06-22T00:11:41.859Z Reads: 171

```
That whole shooting out flames thing is why I wouldn't grind down the ends of cells. $160 dollars worth of cells is a hell of alot cheaper than a house fire. If you've got the money, let somebody else do the ghetto shit.
```

---
## \#35 Posted by: Chase Posted at: 2018-06-22T00:53:53.397Z Reads: 162

```
So damn mad. Wasn’t paying attention accidentally stuck a battery facing the wrong way when I was stacking them in a box. Next thing I know the box has erupted in flames
```

---
## \#36 Posted by: lrdesigns Posted at: 2018-06-22T00:56:19.906Z Reads: 165

```
[quote="Chase, post:31, topic:59532"]
I missed important facts like abrasion
[/quote]

This is one thing that really stood out to me after my first build. I knew abrasion is a serious issue but I didn't realize how aggressive it could be on a skateboard from the vibration. 

On my first build the vesc caps where resting against the plastic enclosure, after not too many miles the vibration had worn a hole through the metal casing of the caps just from resting on plastic. Now I hot glue down anything that can move or be damaged from abrasion.
```

---
## \#37 Posted by: Sender Posted at: 2018-06-22T00:59:42.780Z Reads: 159

```
Pics or it didn't happen.
```

---
## \#38 Posted by: Chase Posted at: 2018-06-22T01:10:07.762Z Reads: 161

```
Well I’ve already tossed 6 the burnt batteries.
That being said if anyone has 5 to 10 30q they can sell lemme know. It was a stupid mistake and essemtially burnt the fuck out of the positive terminals.
```

---
## \#39 Posted by: Chase Posted at: 2018-06-22T03:06:40.568Z Reads: 165

```
So the cells that were involved in the small fire no longer hold voltage. After disassembled I check every voltage of the cells notninvokved in the incident. Most were at the 4.03 from a slight charge. Maybe 3 were at 3.4 and then two were all the way down to to 2.20 V. How low can these go when fully empty? Does this mean I need to scrap these cells? I’m just not too farmiliar with how to detect bad cells with the voltage values.
```

---
## \#40 Posted by: lrdesigns Posted at: 2018-06-22T03:18:00.748Z Reads: 160

```
2.5v is usually the minimum on the data sheet. 

The cells at 2.2v can still be recharged and used most likely, but there is a good chance that their internal resistance is higher than the other cells now. So if you use them in a pack they would discharge un-evenly.   

Edit. They might have already had an higher internal resistance, thats why they are at 2.2 and not at the same level as others. 

The only good way to check the health is with a smart charger that can measure capacity and internal resistance.
```

---
## \#41 Posted by: Chase Posted at: 2018-06-22T03:23:10.468Z Reads: 150

```
Yeah at this point I’ll just buy a pair from amazon to be safe. Thanks for your input.
```

---
## \#42 Posted by: Acido Posted at: 2018-06-22T06:05:51.348Z Reads: 149

```
its totally okay to disassemble and reassemble the packs
```

---
## \#43 Posted by: Chase Posted at: 2018-07-10T02:45:15.640Z Reads: 143

```
I’m having the worst luck with my battery builds. I just rebuilt the 12s4p with a new bestech D223 V1. Everything works as it should but when I plug in the balance wires to the bms, the bottom gets extremely hot! 

Any ideas of why would be extremely appreciated.
```

---
## \#44 Posted by: Lionpuncher Posted at: 2018-07-10T03:18:41.269Z Reads: 136

```
@Chase test your leads. What your describing can happen when the balance wires aren't in the correct order. I bet that's the issue.
```

---
## \#45 Posted by: Chase Posted at: 2018-07-10T03:36:51.985Z Reads: 133

```
Damn you were right. I can’t believe I missed that. Did it screw it up you think?
```

---
## \#46 Posted by: Lionpuncher Posted at: 2018-07-10T05:00:04.780Z Reads: 134

```
I doubt it. As long as you didn't try to ride it like that. Without a significant load, you were probs just really making one resistor work. Should be ok still. Monitor closely for the next few charges.
```

---
## \#47 Posted by: Chase Posted at: 2018-07-10T05:12:08.260Z Reads: 131

```
I just charged it up to 90%. Everything seems to be working fine, but shouldn’t all the cells read the same voltage?
```

---
## \#48 Posted by: legend27 Posted at: 2018-07-10T08:15:47.796Z Reads: 133

```
Don't think so. Think the bms has to balance all the cells. Pretty sure it will do that when 1 cell is at max capacity. It just takes some time. Can you post some pics of the new pack? And how did you do the series connections?
```

---
## \#49 Posted by: Chase Posted at: 2018-07-10T08:40:16.642Z Reads: 142

```
I think there must be some sort of language barrier with bestech because when I asked them why the first cell of the series is lower in voltage than the rest, they keep responding “make sure all the cells are matched” before assembling. Their all of course 30Q. The reason some of them were different voltages before I assembled it was because some were brand new and some were slightly charged. I told bestech this but they just keep saying make sure all the cells are matched before assembling.

The new pack pics below

Started by adding new heat shrink to the cells because the super glue pulled a lot of it off when disassembling. Then added cardboard rings and fishpaper. 
The parallel connections are made with 10mm nickel strips. 
The outer series are connected by 12mm nickel strip supported by 12 gauge solid copper along the edge. 
 Inner series are connected to a brass bus bar, then the series are bridges by two 14 gauge wires.

![image|375x500](upload://p8xrYy6yAYkqSMrwAVdaoIA7rlp.jpeg)![image|666x500](upload://pHV1JZmiclySm7ZxSUJRotRYjH.jpeg)![image|375x500](upload://dcCxNP8uMeYt1TDX86P7hJD54rB.jpeg)![image|375x500]
(upload://oKMIwUuTJ3LZ72qFHGhyQDmjqum.jpeg)![image|375x500](upload://bK6cMfUNTqX721esGSP6X307VXi.jpeg)![image|666x500](upload://xYMwrJpbajeKZqqLke7rIWtCr5c.jpeg)
```

---
## \#50 Posted by: sk8l8r Posted at: 2018-07-10T09:52:44.808Z Reads: 133

```
[quote="Chase, post:49, topic:59532"]
The reason some of them were different voltages before I assembled it was because some were brand new and some were slightly charged. I told bestech this but they just keep saying make sure all the cells are matched before assembling.
[/quote]

you could charge all the cells to the same level BEFORE assembly
```

---
## \#51 Posted by: Chase Posted at: 2018-07-10T10:05:06.813Z Reads: 134

```
But is that absolutely necessary for the bms to balance the cells correctly?
```

---
## \#52 Posted by: banjaxxed Posted at: 2018-07-10T11:26:50.312Z Reads: 133

```
It’s called float charging 
https://www.electric-skateboard.builders/t/float-charging-why-you-shouldnt-bypass-the-bms/39879
```

---
## \#53 Posted by: Chase Posted at: 2018-07-10T17:42:14.144Z Reads: 119

```
Thanks for the link. Looks like it may just take some time to balance these.
```

---
## \#54 Posted by: Hummie Posted at: 2018-07-10T19:02:00.875Z Reads: 123

```
[quote="Chase, post:33, topic:59532"]
Grinding down terminals now. Re jeatshironkojg because most ripped off from the super glue.

[![image|375x500](//www.electric-skateboard.builders/uploads/db1493/optimized/3X/4/a/4a96084aa9d2859e279a1a0bd8b078ebade9e3d1_1_375x500.jpeg)
7FC22447-3DD3-475B-BF6C-9BD5C98967EE.jpeg3024x4032 2.97 MB
](//www.electric-skateboard.builders/uploads/db1493/original/3X/4/a/4a96084aa9d2859e279a1a0bd8b078ebade9e3d1.jpeg)
[/quote]

holy hella dangerous looking all those cells without wrap together.  looks like one of them is practically shorting across the top of a couple even in the pic.   one big spark and then you knock the bong over onto all the cells and then you run out of the house screaming...run away never come back.
```

---
## \#55 Posted by: Chase Posted at: 2018-07-11T01:17:28.864Z Reads: 123

```
Yes that did happen actually. I learned very quickly how dangerous of a situation I had created once one of the negative ends lodged itself inside of the positive groove of another causing about 4 nearby cells to go crazy and almost burn my table down. I can honestly admit that I didn’t have enough hands on experience working with batteries to realize how dangerous these can be. Hopefully others can learn from my stupidity.
```

---
## \#56 Posted by: Chase Posted at: 2018-07-11T01:45:47.565Z Reads: 117

```
Ok so I have been reading about it and it looks like you are right. One cell needs to be 4.2 for balancing to begin. The weird thing is that none of the cells go above 4.1 by the time the charger light goes green (when indicator reads 90%). So does this mean that it won’t ever begin balancing? And why does my charger stop at 90% (48.0 V) when my charger is rated for 50.40 V?
First cell of the series is about 3.67 and the rest are right at 4.10.
```

---
## \#57 Posted by: sk8l8r Posted at: 2018-07-11T07:32:02.718Z Reads: 117

```
[quote="Chase, post:55, topic:59532"]
I can honestly admit that I didn’t have enough hands on experience working with batteries to realize how dangerous these can be. Hopefully others can learn from my stupidity.
[/quote]

I was racing through my current build when I saw this thread - decided to take an extra couple of weeks on my battery build - really glad I did I was about to do something stupid, I don't think I would have spotted it if I wasn't hyper paranoid about batteries now :)
```

---
## \#58 Posted by: Chase Posted at: 2018-07-11T08:45:16.804Z Reads: 114

```
Good that makes me feel like maybe all this trouble is worth something
```

---
## \#59 Posted by: legend27 Posted at: 2018-07-11T09:54:32.281Z Reads: 113

```
The same thing happened in another thread. To fix it he let the battery charge for a few hours when the light was green. It takes some time to balance. Let your battery stay in the charger when the light becomes green and the bms should do the rest. Don't leave the battery for 5 hours but see after an hour or less if something has changed.
```

---
## \#60 Posted by: Chase Posted at: 2018-07-11T19:25:41.817Z Reads: 112

```
Yeah I saw that post and tried that already. One cell got up to 4.2 V, 10 are at 4.1 Vbut the first one won’t change from 3.68 V. I talked to bestech and they said “check the cells in the first series because they Arlene abnormally low compared to the others”. But the cells in the first series are all brand new. Do I have to make sure they are all charged to the same voltage (or nearly the same) before assembling? I didn’t do this before making the pack because I thought that was what a bms was supposed to do.
```

---
## \#61 Posted by: legend27 Posted at: 2018-07-11T21:25:38.819Z Reads: 105

```
Pretty sure all cells has to be around the same voltage when you assemble it... Sadly. Don't know what you can do other than take everything apart again, charge all cells to max and assemble it again :frowning:
```

---
## \#62 Posted by: Chase Posted at: 2018-07-11T22:59:09.412Z Reads: 99

```
Well most of the others are at 4.10 V except for the one that's at 4.2. You think Ill  be able to get away with just charging the first set thats at 3.67 V to 4.10 V like the majority of rest of the cells? This way I can avoid having to disassemble the whole thing.
```

---
## \#63 Posted by: legend27 Posted at: 2018-07-11T23:20:49.774Z Reads: 93

```
Yea. Think that will do it. Just don't know how you're going to do it.
```

---
## \#64 Posted by: Chase Posted at: 2018-07-11T23:23:41.636Z Reads: 96

```
Yeah I bought a usb charger for them. I’ll just have to pull it out and monitor the voltage every so often until I reach 4.1 V on the first cell set.
```

---
## \#65 Posted by: legend27 Posted at: 2018-07-11T23:25:55.476Z Reads: 98

```
Try that :slight_smile:
```

---
## \#66 Posted by: Chase Posted at: 2018-07-12T19:56:50.002Z Reads: 96

```
Wish I had seen this first. This article explains my situation very well. 

https://www.orionbms.com/general/pre-balancing-cells/
```

---
## \#67 Posted by: Chase Posted at: 2018-07-14T17:25:58.423Z Reads: 95

```
It appears to have worked. Learning new costly lessons everyday
```

---
## \#68 Posted by: Chase Posted at: 2018-07-15T17:53:46.564Z Reads: 88

```
Changed the title of this thread to help others with the same issues. In order for the bms to balance my cells they had to be prebalanced. After prebalancing 11 of the series to 4.10 V, and the 12th reaching 4.20 V the bms started to balance the cells. It trims everything down to 4.08 V but this is not a fast process. It took about 36 hours after the charger light turned green.
```

---
## \#69 Posted by: Sender Posted at: 2018-07-15T18:23:50.264Z Reads: 83

```
Glad you got it worked out.  Learning is a painful and long process sometimes.  But fun. Super fun.
```

---
## \#70 Posted by: Lionpuncher Posted at: 2018-07-15T18:47:12.455Z Reads: 87

```
This has been helpful. Been struggling with my battery and I think this is the ticket. Been a good thread. Thanks
```

---
## \#71 Posted by: Chase Posted at: 2018-07-20T05:17:32.888Z Reads: 82

```
Well I went through the trouble of making this big battery and it doesn’t even fit. I guess I thought because of this image of the evo eboosted enclosure with a 14S, that I could fit a 12S4P and wedge the bestech up in the back. Nope about two inches two long.

![image|281x500](upload://ejMy85gYZj0yUEwAZyZMCsSk8Of.jpeg)

I guess my only option now is to sell it or make a new build that can fix it. Anyone want this or know if a good long deck that I might be able to fit it on? I’ll probably pair it with the carvon XL when I finally get it.

Or maybe I can just find a thin 12S bms to change to but I really don’t feel like having to change up this battery.

![image|375x500](upload://9Bg8SIfe75QujlX5TA5Gh1oZWkI.jpeg)
```

---
## \#72 Posted by: Hummie Posted at: 2018-07-20T06:24:44.110Z Reads: 75

```
looks awesome as is.  id skip the bms and hook up two 6s balance plugs and connect to this
https://www.ebay.com/p/HobbyKing-Turnigy-DLUX-Lipo-Battery-Cell-Display-and-Balancer-2s-6s/1180189308?iid=261667879653&chn=ps

and charge to only 4.1 probably.
```

---
## \#73 Posted by: Chase Posted at: 2018-07-20T18:57:57.678Z Reads: 67

```
Hmm that’s cool. I guess to use it I’d have to get a variable charger.
```

---
## \#74 Posted by: Sebike Posted at: 2018-07-20T19:19:34.721Z Reads: 69

```
No need to keep the charger plugged in after led has turned green for the balancing to take place. When bms starts balancing the cells, it will do so without the charger.
```

---
## \#75 Posted by: Chase Posted at: 2018-08-26T21:31:34.083Z Reads: 44

```
Figured I’d post this here just as a resource. Made a couple of batteries since and I really like this setup. Here’s my progress on a 12S6P.

![image|375x500](upload://ncAHRyIaKNfYkFeN8vUbFKaepgs.jpeg)

Still learning small lessons along the way. Used the high setting on my hot glue gun and ended up burning tiny lines through my original shrink wrappers when binding the parallel cells. Switched to the low temp and then half of them came loose I was adding my fishpaper strips. About to try to reinforce with super glue. These dual cell layers definitely need to be secure to each other.
```

---
