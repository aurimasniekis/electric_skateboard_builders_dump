# Battery pack layout: use balance leads for parallel connections?

### Replies: 4 Views: 638

## \#1 Posted by: deucesdown Posted at: 2017-08-18T19:13:31.095Z Reads: 108

```
Okay, I'm thinking about building another pack, and as usual I'm making myself crazy. :slight_smile:

The things I'm trying to achieve are:
* 12s voltage
* lots of current handling
* ability to use balance charger (my charger is 8s)
* ability to monitor individual cell health

I see most packs being built with spot welded nickel strips, and the resistance of these strips seems really poor. Like poorer than the 22awg wires on typical balance leads.

22awg silicone allows maybe 10A, and the typical JST-XH are rated for 3A. If these are too wimpy, can upgrade to JST-VH rated at 10A per pin, which'll probably allow 20awg silicone.

Soo, I'm thinking about building 12s3p with modular subpacks.

* build 6s1p subpacks, six of them. I guess these will behave more or less like lipo packs
* 7 conductor balance leads, 22awg + jst-xh, or 20awg + jst-vh
* connect cells with spot welded nickel with copper wire/braid on top ala whitepony
* xt60 connector, 12awg wire for charge/discharge
* probably sammie 30q but but the 20700/21700 stuff's making me crazy

Hook up pairs of these in series for 12s, and hook up corresponding subpacks via the balance leads so each cell is parallel with its 3 neighbors. I'll build a strip board with paralleled JST headers.

I think electrically this makes sense, with the weak point being maybe increasing resistance on the JST pins over time. I'd skip BMS and maybe twice a month parallel charge on the hobby charger. And maybe every 2 months, do a single cycle with graphing on each subpack to measure capacity, check internal resistance, etc.

Does this sound like a terrible idea?

I guess it would be similar to using 6s1p lipos, and connecting their balance leads together.

As I understand, most of the current is flowing through the series connections, and just a wee bit through the parallel.
```

---
## \#2 Posted by: Deckoz Posted at: 2017-08-18T21:07:03.631Z Reads: 84

```
I use balance leads for parallel balancing connections but have primary terminals for current<img src="/uploads/db1493/original/3X/1/0/1040a505bac23eb068443d28450ef5a89f6eb2f8.jpeg" width="295" height="500">

I build mine modularly to be able to remove the 10s modules as 100wh packs for traveling via airliner
```

---
## \#3 Posted by: deucesdown Posted at: 2017-08-18T22:55:59.083Z Reads: 76

```
Nice, that's pretty much the idea. Your cells are stacked 2 high? Must have tall wheels :)
```

---
## \#4 Posted by: Deckoz Posted at: 2017-08-18T23:22:13.355Z Reads: 74

```
They're stacked in triangle configuration.

Running 83mm wheels on 1/8" risers on 44rear/50front calibers on a loaded vanguard. Plenty of clearance. Its shorter then the boosted board battery pack.
Old pic from before it was finished but its all I have on my phone
<img src="/uploads/db1493/original/3X/7/0/705b5c2985d9468432a48d86d12ee1a43baa677f.jpg" width="295" height="500">
```

---
