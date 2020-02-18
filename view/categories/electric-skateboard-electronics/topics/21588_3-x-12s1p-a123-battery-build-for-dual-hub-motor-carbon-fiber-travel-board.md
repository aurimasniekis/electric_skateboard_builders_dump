# 3 x 12S1P A123 battery build for dual hub motor Carbon fiber travel board

### Replies: 14 Views: 2391

## \#1 Posted by: BigBoyToys Posted at: 2017-04-23T06:08:52.186Z Reads: 301

```
Hey all,

I wanted to run my latest project by you all to gather some input and ideas on a few of the build details.

I'm going to attempt to take this board on planes with me weekly with the batteries removed and kept in my carry-on bag.

Planned major components:
1. Torqueboards 33" CF deck with integrated enclosure.
2. Vesc-X (2)
3. A123 LiFePO4 cells (36)
4. Three small 12S BMS(s) bypassed for charging only.
4. Torqueboard hubs or Carvon V3 hubs. Both should arrive next month so probably which ever comes first.

My biggest concern at this point is how to navigate the battery build around the following issues.

1. Problem: 100whr battery capacity limit on planes.
           Solution: Create 3 separate 12S1P battery packs.

2. Problem: 0.15mm Nickel strips don't support enough current to spot weld the pack together while still using the A123 cells to their full potential.
           Solution: Soldering columns of 6 cells end to end using a PVC jig then using 1/2" wide tinned copper braid to connect pairs of 6 cells to get 3 separate 12S1P battery packs.

3. Problem: A simple, safe and reliable battery charging method is needed.
         Solution 1: Squeeze three small 12S BMS's into the enclosure (bypassed for charging only).
         Solution 2: No BMS and just remove the batteries for balance charging on my Thunderpower TP1430 when I'm home.

Let me know what u all think about my proposed solutions and any thoughts or concerns you have related tof my build. 

Cheers!

<img src="/uploads/db1493/original/3X/4/b/4b45e00a346b583d2d48b2c9681e66030dee5b64.jpg" width="281" height="500"><img src="/uploads/db1493/original/3X/7/5/75d5d6964b2aa5ca0530791eb9b6bc5614306a58.jpg" width="690" height="388">
```

---
## \#2 Posted by: monkey32 Posted at: 2017-04-23T07:01:40.720Z Reads: 272

```
12s3p no? 12 sets of 3 hooked in parallel all connected in series?
```

---
## \#3 Posted by: monkey32 Posted at: 2017-04-23T07:02:41.226Z Reads: 263

```
Nevrmind I get it
```

---
## \#4 Posted by: Pantologist Posted at: 2017-04-23T14:17:37.593Z Reads: 243

```
Seal it up and point an official looking 99Wh sticker on it. You don't have much space to work with to put individual packs in there. 

Also why not make 3 4s3p packs in series so you only need to connect one BMS?
```

---
## \#5 Posted by: Eboosted Posted at: 2017-04-23T15:11:35.392Z Reads: 232

```
Can you show us your proposed battery layout?
```

---
## \#6 Posted by: Eboosted Posted at: 2017-04-23T15:21:13.024Z Reads: 228

```
Lifepo4 A123 cells have 2500mAH, for 12S1P you will have 3.3V nominal * 2.5mAH * 3 cells in parallel = 99WHr, that's perfect. 

The problem would be connecting 3 parallel groups of 12 series in parallel, if has been advised to be parallel first and then series because of excessive high current discharge on the former
```

---
## \#7 Posted by: BigBoyToys Posted at: 2017-04-23T17:05:54.543Z Reads: 224

```
@Pantologist

I kinda pulled that angle with my Galaxy note 7 by putting a case on it that cover the designation but I fly 60+ times a year so it kinda wore on my conscience and I switched back to my old S6 after a few weeks.

I considered 4S3P and 3S4P packs but couldn't figure out a good wiring setup considering the cells are orgainzed 6 cell x 6cells  lengthwise in then enclsoure. The enclosure is (170mm) so I can't fit 3 cells across which would have made those better options imo. 

Benefits of the 12S configuration idea I was planning:

1. With 12S battery packs I would still have a functional board with 1, 2 or 3 battery pack in use.
2. The 12S configuration would allow the use end to end soldering which will keep the resistance of the series cell connections to a minimum.
3. Less space would be required since there would be nothing between the cells besides solder and a balance lead( No bulky 10gauge wire or copper braid)
4. The only wire on each battery would be an inch or less on one end for the XT-60 connector to attach to and once piece of tinned copper braid at the opposite end to join the two halves.

The drawbacks I see to this design would be:

1. Long skinny battery packs (16") with almost zero flexibility. (I think I can deal with this since they would still fit in my backpack or carry-on).
2. This would require the use of 3 BMS's. (They are only $15 so no the only real issue is space but I think they will fit).

Excuse the rudimentary drawing, but it's just<img src="/uploads/db1493/original/3X/e/f/ef2182460cba2a29f59ebd6ff65744bc5eab98ba.jpg" width="281" height="500"> to give u an idea of the configuration I'm referring to.
```

---
## \#8 Posted by: BigBoyToys Posted at: 2017-04-23T17:13:12.571Z Reads: 201

```
@Eboosted 

I included a basic idea of the configuration above, thoughts?

When it comes to 12S1P vs 4S3P, my brain says 12S1P has more voltage but less  potential current discharge?  The 4S3P pack with 3 parallel rows has triple with amps available doesn't it?
```

---
## \#9 Posted by: Eboosted Posted at: 2017-04-23T18:21:12.645Z Reads: 197

```
I think you should build 3 packs of 3 parallel and 4 series each, then connect them in series using 5.5 bullet connectors, this way you would only use 1 bms, less cables runing inside and you would keep the recommended "parallel-then-series" setup, you will loose the possibility to run 12S1P or 12S2P but, come on, those are options you won't ever use or if you do you will feel incomplete and anxious.

BTW where did you buy your a123 lifepo4s? I've heard there are a lot of fake ones out there, how much did you pay for them? 

Do you usually travel in a specific airline?
```

---
## \#10 Posted by: BigBoyToys Posted at: 2017-04-23T19:20:22.314Z Reads: 200

```
I fly domestically with Southwest almost exclusively.

Before it got stolen I took my boosted board on the plane 3 or 4 times without any hassles.

Can you take a look at the way the batteries fit in the enclosure in the picture and give my an idea of how I'd configure and wire up 4S3P? As far as I can tell I'd either have to have 1 of the 3 packs a different shape than the other two, or I'd have to turn the battery cells 90 degrees from how the are in the picture, in which case only 24 cells would fit since I cant fit 3 cells across in the 170mm width.

If was was riding the board locally there's no doubt I'd want all the battery packs in the board, but I have other boards I'd rather ride if I was home (4wd hub 12S6P build or my evolve CGT). So this board would really get used primarily while traveling or for quick trips around town. Since I have to pull the batteries out to get through TSA anyway I'm really considering not using BMS's at all.

Im actually using the older A123 ANR26650m1-A cells which are 2.3 AHr's as opposed to 2.5 AHr for a total of 6.9 AHr's. That should give my about 10 miles considering my weight and riding habits. I bought them off ebay here for $6.75 a cell shipped.

http://www.ebay.com/itm/201498063622

I also have 24 Basen Black 4.5AHr cells that I can use for a 9AHr 12S2P pack, but from what I read those actually only support 23A(46 in 2P config) continous which is a little low for my likes. Anyone have personal experience running those? I'm having trouble believing I will get double the range with half the number of cells without some kind of drawback like heat, voltage sag and a massive drop in battery longevity.

I'm also thinking I will shrink wrap the packs in clear so the cell types are easily distinguishable in case there was any question as to the capacity of the battery pack.  Do guys think that will make them look more or less sketchy considering the fact that there will be balance leads visible through the shrink?

<img src="/uploads/db1493/original/3X/3/7/371a8c618fa74d2e79e7c64ddabde018d5148ca8.jpg" width="281" height="500">
```

---
## \#11 Posted by: Eboosted Posted at: 2017-04-23T19:48:00.262Z Reads: 182

```
Have you seen my build?, you could use the bullet connectors like I did.

https://www.electric-skateboard.builders/t/travel-safe-battery-design-v2-10s4p-360whr-for-loaded-vanguard/19535
```

---
## \#12 Posted by: BigBoyToys Posted at: 2017-04-24T04:31:31.875Z Reads: 168

```
I have seen your build,  that cold work but I don't trust myself  with banana connector long term. I'd probably use xt-60 so I can't reverse the polarity while rushing.

Biggest issue I see with that is it still 6 6S1P packs or 3 12S1P packs and I'd have to connect all the cells with 10G wire since 0.15mm strips can't move all the current the A123'same have to offer :(. I do like that the packs would be roughly square though as opposed to 2"x15" with the way I'm planning them.

Have you had a chance to take them on a plane yet?
```

---
## \#13 Posted by: BigBoyToys Posted at: 2017-09-07T18:08:03.970Z Reads: 147

```
Here are some pics of the <img src="/uploads/db1493/original/3X/0/7/0753d00edb2cdb135b4b779cba0fdbabb6dba9eb.jpg" width="374" height="500">batteries.

<img src="/uploads/db1493/original/3X/b/f/bf4109a9263092027e14af7afeb3691b10d11e8e.jpg" width="374" height="500"><img src="/uploads/db1493/original/3X/a/1/a17ec9cc0ea2399ade628fed60a5a087f5dcd834.jpg" width="374" height="500">
```

---
## \#14 Posted by: drone001 Posted at: 2019-01-10T18:02:07.389Z Reads: 48

```
I have a CF deck evolve cgt. I plan to swap out all electronics also the battery. Is it a good idea to drill holes for a possible battery enclosure?
```

---
