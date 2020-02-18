# Soldering iron for 18650 packs

### Replies: 32 Views: 5563

## \#1 Posted by: Eboosted Posted at: 2017-03-06T05:08:04.400Z Reads: 428

```
I know the consensus here is to spot weld all battery packs with nickel strips however I don't plan to buy a spot welder at the moment.

I have a high wattage Weller soldering station and I already built a couple of packs which turn out perfect, been using the packs for several moths with zero issues.

I need some advice to solder cells together:

1. There are no youtube videos showing how to solder 18650s with nickel strips, have you got one with good quality results?
2. Soldering flexy silicone cables to 18650 cells is much easier to solder nickel strips, is this a good approach or should I stick with nickel strips?

Hope you soldering gurus could give me some input on this.
```

---
## \#2 Posted by: willpark16 Posted at: 2017-03-06T05:27:55.105Z Reads: 414

```
Just soldered a new pack gonna make it airplane travel safe I recommend wire if u wanna make it flex and it's easier high strand but u sacrifice space
```

---
## \#3 Posted by: Eboosted Posted at: 2017-03-06T05:58:46.707Z Reads: 408

```
Are you using 12AWG flex silicone wire?

Can you post a picture of your work?

Nickel strips seem almost impossible to work with a soldering iron
```

---
## \#4 Posted by: willpark16 Posted at: 2017-03-06T06:51:54.146Z Reads: 396

```
Nickel strips require lots of flux and heat along with some scuffing
```

---
## \#5 Posted by: willpark16 Posted at: 2017-03-06T06:53:54.486Z Reads: 383

```
My work is in one of my previous threads, I used 12 awg but I don't recommend that
```

---
## \#6 Posted by: Eboosted Posted at: 2017-03-06T07:00:16.426Z Reads: 375

```
What would you recommend then?
```

---
## \#7 Posted by: willpark16 Posted at: 2017-03-06T07:01:21.139Z Reads: 371

```
What size pack are u making?
```

---
## \#8 Posted by: Eboosted Posted at: 2017-03-06T14:18:17.842Z Reads: 369

```
I'm working on a 10s4p
```

---
## \#9 Posted by: Norco Posted at: 2017-03-06T15:04:29.035Z Reads: 386

```
This is the build of my 10S4P using a soldering iron and nickel strips. 
http://www.electric-skateboard.builders/t/pork-chop-express-comet-loki-motor-6374-vesc-10s4p-diy-18650-pack-benchwheel/13106/18

I would say pre soldering the strip helped and plenty of flux was useful. You need to be in and out quick to stop the battery heating up. I hot glued my cells together first and would recommend doing this. You will probably want to reinforce the nickel strip with single core copper across the series connection.
```

---
## \#10 Posted by: jaykup Posted at: 2017-03-06T15:59:09.269Z Reads: 386

```
**Equipment**

* **80-100w soldering iron** - you want to solder hot and fast.  10 seconds or so on the battery so you don't heat the battery up too much

* [**12awg flat copper braid**](https://www.mcmaster.com/#grounding-braid/=16gi4yq) - for series connections

* [**8 AWG solid copper wire**](http://www.homedepot.com/p/Southwire-By-the-Foot-8-Solid-Bare-Copper-10632890/204632160?cm_mmc=Shopping%7cTHD%7cG%7c0%7cG-VF-PLA-D27E-Electrical%7c&gclid=CK2Rz8qcwtICFcKEswodG2QELQ&gclsrc=aw.ds) - for parallel connections

* [**Sticky Insulators**](https://www.fasttech.com/product/2157501-paper-insulation-gasket-for-flat-18650-battery-50) for positive terminals

* [**rosin core solder**](http://www.digikey.com/products/en?keywords=24-6337-0027)

**Steps**

* Put the sticky insulators on.  These prevent the hot wire from melting through the 18650 insulation and shorting the battery.

* [Pre-tin the batteries with solder](http://www.electric-skateboard.builders/uploads/db1493/original/3X/4/3/436315d51709a98123ea378d0e2f7a2c6fc8d4cb.JPG)

* [Set strips of copper braid onto the batteries](http://www.electric-skateboard.builders/uploads/db1493/optimized/3X/2/c/2c82d491beeb484f6d5cb01978b99af51265ddc0_1_690x460.JPG), put soldering iron on top, add a little solder and let it melt onto the battery.  Use a screw driver or something to hold the strip into place until it cools.

* [Fold the battery over if necessary.](http://www.electric-skateboard.builders/uploads/db1493/original/3X/1/4/14bc2bf416aa73fd5bbc2ad5d998442b27e07819.jpg) - [pic2](http://www.electric-skateboard.builders/uploads/db1493/original/3X/6/a/6a5853a376668db4b737ca7c6a2ace50e31b7313.JPG)

* [For parallel connections, use a higher AWG wire - 8 AWG solid is what I used.](http://www.electric-skateboard.builders/uploads/db1493/original/3X/5/4/540ce1b672408e945628bb4de37c699c513af820.jpg)

**Notes**

I did some testing on Nickel strips I got off eBay.  at 12v 10 amps they got hot, and at 20 amps they discolored and began to fail.  At 40-50v 20A I don't think they will work well at all. nickel (or nickel plated steel like most eBay strips are) don't conduct electricity well.  If you are going for 18650 batteries, it's probably because you want a premium battery.  One that can output a ton of current, so it's worth making sure all the connections can handle the current.  The 12 AWG wires will handle 20A no problem.  The [8 AWG will handle 60-70A](http://www.powerstream.com/Wire_Size.htm) no problem.  Might be able to go to 6 AWG if you have more than 4 in parallel.  The concern of soldering batteries I believe is over-rated.  As long as you are careful not to overheat the battery, I don't see the problem.
```

---
## \#11 Posted by: Tobi Posted at: 2017-03-06T16:34:08.946Z Reads: 350

```
i just used normal 1,5mm copper wire for my 10s3p and iam happy with that , no issues so far.
```

---
## \#12 Posted by: willpark16 Posted at: 2017-03-06T17:25:23.623Z Reads: 341

```
But much tbh
```

---
## \#13 Posted by: willpark16 Posted at: 2017-03-06T17:27:03.315Z Reads: 350

```
Get some 14awg high strand awg and decent flux, some nice solder and a Denzel with sand bit and ur good to go this is what 12awg looks like<img src="/uploads/db1493/original/3X/1/a/1af37822c73a113a63bac03a5f63faf8c3406471.PNG" width="281" height="500">
```

---
## \#14 Posted by: KTMinni Posted at: 2017-03-08T13:03:54.899Z Reads: 325

```
How necessary are sticky insulators? And where did you buy the copper braid?
```

---
## \#15 Posted by: jaykup Posted at: 2017-03-08T14:45:53.003Z Reads: 322

```
[quote="KTMinni, post:14, topic:18626"]
How necessary are sticky insulators?
[/quote]

I read somewhere, on Endless Sphere I believe?, a story of a guy's 18650 pack using nickel strips.  When he was using a lot of current from his battery, the strips got so hot they melted through the plastic insulation on the 18650 cells and shorted them out.  The picture below shows the positive and negative are actually right next to each other, only separated by a thin plastic insulation.  If that's damaged or melts, the cell will short out.

<img src="/uploads/db1493/original/3X/3/5/35de07654afc69724a44a176c0f3f29b0ba99f47.jpg" width="400" height="300">

The idea behind the sticky insulators is that they protect against heated connections, either through the soldering process or thin nickel strips that heat up under high current loads.

[quote="KTMinni, post:14, topic:18626"]
And where did you buy the copper braid?
[/quote]

The copper braided wire was ordered form McMaster Carr - the link is in my post above.  You can also find copper braid from eBay, but I found it's sometimes a lot thinner and may not be 12AWG equiv.
```

---
## \#16 Posted by: KTMinni Posted at: 2017-03-08T16:26:50.347Z Reads: 307

```
Thanks for the quick and informative reply!
```

---
## \#17 Posted by: KTMinni Posted at: 2017-03-08T16:30:33.746Z Reads: 307

```
Sorry I also forgot to ask of rosin core solder is particularly important, as I do not have access to that at the moment.
```

---
## \#18 Posted by: jaykup Posted at: 2017-03-08T17:01:09.790Z Reads: 304

```
My understanding is that rosin core solder is just solder with a type of flux built into it.  It helps the solder "stick" to whatever you are soldering.  I don't see a reason why you couldn't just use flux and regular solder together.
```

---
## \#19 Posted by: longhairedboy Posted at: 2017-05-08T14:32:31.006Z Reads: 289

```
you can totally use flux and regular solder. You can also use flux and rosin core for stuff that's giving you a hard time.
```

---
## \#20 Posted by: longhairedboy Posted at: 2017-05-08T17:34:29.355Z Reads: 283

```
also.. if you buy flux in bottles like i do...

https://www.amazon.com/gp/product/B00UG08QDC/ref=oh_aui_detailpage_o01_s00?ie=UTF8&psc=1


these are awesome. and dirt cheap. and they don't really seem to clog much with dried flux for some reason. 

i got some of these and a solder pot for tinning big wires and now tinning is no longer a hassle. its actually kind of fun watching the flux boil out of the wire as the 50/50 wicks up the 10awg wire like oil in a lamp wick. 

The solder pot i got was $20 on amazon too. along with a big bar of 50/50 solder to go in it.
```

---
## \#21 Posted by: Sebike Posted at: 2017-07-16T10:53:21.036Z Reads: 245

```
[quote="jaykup, post:10, topic:18626"]
12awg flat copper braid - for series connections
8 AWG solid copper wire - for parallel connections
[/quote]

Why using bigger dimensions on the parallel connecting wires than on series connections? 

Load on series connections are bigger right, so the other way around would make more sense, wouldn't it?
```

---
## \#22 Posted by: Eboosted Posted at: 2017-07-16T16:15:21.764Z Reads: 224

```
Hey @longhairedboy what bland of oil solvent and flux do you use? Do you clean all your solder jobs with oil solvent after finish soldering or you use it before applying heat?
```

---
## \#23 Posted by: Alan_Smithee Posted at: 2017-07-16T18:08:55.687Z Reads: 225

```
Instead of nickel strips I just [0.2mm copper sheet.](http://www.ebay.de/itm/1pcs-99-9-Pure-Copper-Cu-Metal-Sheet-Foil-0-2-x-100-x-1000-mm-/271577611541?hash=item3f3b497d15:g:vPwAAOxy~dNTJ1aE).

Its much easier to solder than nickel strips and for the same area can carry more current iirc.

You can go thicker than 0.2mm but that thickness is easy to cut with regular scissors to any size you need.
If I need higer current I just use double or triple layers.
```

---
## \#24 Posted by: Surfer Posted at: 2017-07-16T18:34:53.316Z Reads: 221

```
Copper has like 5 times better conductivity than nickel, I use copper braid, also with braid is easier to make it a bit more flexible the 🔋. Some flux and 100+watts solder and ready to go.
```

---
## \#25 Posted by: longhairedboy Posted at: 2017-07-17T15:02:56.539Z Reads: 225

```
i use liquid flux in a little needle tipped squirt bottle. Cleanup i use rubbing alcohol and a clean white rag. 

https://www.amazon.com/gp/product/B005T8KZ0I/ref=oh_aui_search_detailpage?ie=UTF8&psc=1

and i pour it into this for application during jobs:
https://www.amazon.com/gp/product/B00UG08QDC/ref=oh_aui_search_detailpage?ie=UTF8&psc=1

i use rubbing alcohol to clean up the tips on the bottles as well.
```

---
## \#26 Posted by: jaykup Posted at: 2017-07-17T16:28:36.794Z Reads: 221

```
[quote="Sebike, post:21, topic:18626"]
Why using bigger dimensions on the parallel connecting wires than on series connections? 

Load on series connections are bigger right, so the other way around would make more sense, wouldn't it?
[/quote]

In this case for a 12s4p battery:

Series connections - 4 x 12 awg wires, one on each series line (**6 awg equiv**)
Parallel Connections - 1 x **8awg** wire

so technically the series has a better connection than parallel like you said.

Load per series is 20A x 4 which 12awg x 4 will handle, and load on parallel is 80a which 8awg, while a little undersized for continuous load, should handle.  VESC 4 will likely overheat before the wires do, though the VESC 6 may change things.

Some pics to clarify:

http://www.electric-skateboard.builders/uploads/db1493/optimized/3X/1/5/154a7070c89196cf2892ace326b542a92ef117a6_1_331x500.png

<img src="/uploads/db1493/original/3X/d/9/d96240b4746f482215540a59bee3ed1420018c45.png" width="690" height="460">

12awg on the series lines

http://www.electric-skateboard.builders/uploads/db1493/optimized/3X/5/4/540ce1b672408e945628bb4de37c699c513af820_1_667x500.jpg

8awg on the parallel lines
```

---
## \#27 Posted by: darkkevind Posted at: 2017-07-17T16:51:57.562Z Reads: 220

```
The problem with using wire and solder directly to the battery ends is that for a low guage wire (12/14 awg) you need A LOT of heat to melt a large amount of solder to engulf the whole wire **and** make it grip to the cell. 
The problem with that is, the batteries are great conductors of heat and most of the heat from the soldering iron gets conducted into the metal of the cell, thus damaging the inners of the cell.

If you want to make a flexible battery but still use solder, the best option is to weld small tabs of nickel to the ends of the cells, with enough nickel so that it can be slightly bent away from the cell, then rough up that nickel with a sharp end or sand paper and solder to that. The nickel basically absorbs most of the heat and much less dissipates to the cell.

You can make a spot welder from a car battery, a solenoid relay and some heavy guage cable for next to nothing, like mine...

<img src="/uploads/db1493/original/3X/3/b/3b45741d696e67f9d2a959142ece89230d5a55bf.jpg" width="690" height="388">
<img src="/uploads/db1493/original/3X/d/4/d49e6bcdd54d105be47decab6483c189a2150c8b.jpg" width="690" height="388">
```

---
## \#28 Posted by: Jinra Posted at: 2017-07-17T17:18:41.032Z Reads: 210

```
My cell fused parallel lines are running 22awg from cell to buss bar and used the .016" x .5" buss bar for series
```

---
## \#29 Posted by: jaykup Posted at: 2017-07-18T02:28:18.134Z Reads: 209

```
Soldering can be tricky - but I've found a good way to keep the battery temps low.

Use a ~100w soldering iron in an effort to be quick.  Pre-tin the cells with solder+flux, only takes a few seconds to get the solder on and to stick with the big soldering iron.  Cells get warm, but not too hot to hold.  Then, with the braided wire, just set it on top of the pre-tinned solder, put the soldering iron on top of the braided wire, and let it melt in using a little bit of rosin(flux) core solder to start the process.  Takes a few seconds and the cells don't even get warm.

The 8awg wire was a bit trickier to keep the cells cool, but pre-tinning both the batteries and the wire separately, then soldering together worked well.

I decided to look through my VESC tool - I've got 632 logged miles on the battery so far, so about 35-40 discharge/charge cycles with no BMS and just a meanwell adjustable 50v 4a bulk charger (I know, I know) but all the Samsung 25R cells still check out as follows:

Bulk Charger set to 49.6v (4.133333333v)

4.14
4.14
4.13
4.13
4.14
4.13
4.15
4.14
4.13
4.14
4.14
4.13

The pack has never been balanced.

**A quick pivot table of the CSV files I found some more specs to see how the battery has been used:**

Number of ride logs: 98
Total Distance: 632 miles
Max motor amps: 95.03 (single 6374 motor)
Max Battery amps: 54.61 (13.6a per cell)
Max Watts: 2283
Max (GPS) Speed: 30.1 mph / 48.17 km/h *
Min volts (not counting disconnects): 37.4 (3.11v / cell)**
Min Temp: 6.8c / 44.24v (cold morning test ride)
Max temp: 81.4c***

*this is all it will do at 95% duty cycle. Should go faster with taller gears.

**this was one or two rides I managed to kill the battery completely after 22 miles and was trying to get something out of the battery to get home.  VESC protection prevented me from going any lower.

***vesc de-powered on a LONG uphill run on a hot day

**Overall - I believe this style of battery building holds up extremely well, provides plenty of large pathways for high power capacity, and carefully soldering the cells doesn't have any impact on performance or longevity.**
```

---
## \#30 Posted by: gogomrrobot Posted at: 2017-10-10T20:51:37.875Z Reads: 159

```
https://www.mcmaster.com/#grounding-braid/=16gi4yq -- these guys are legit. Ordered this morning and received today. Maybe it's my proximity. Thanks for the link.

Do you heatshrink or electrical tape the copper braided flat wire or just leave open?
```

---
## \#31 Posted by: jaykup Posted at: 2017-10-11T03:01:13.236Z Reads: 150

```
I'd be worried about the longevity of electrical tape, and the heat resistance.  

The plan was to buy some large heat shrink and encase the entire battery in that.  For some reason I just never got around to doing it.  Since it's enclosed in a plastic case, it may not be necessary to cover the battery.  The connections won't move if soldered correctly, and there is nothing metal to touch.

There are some vendors on eBay that sell large diameter shrink tubing.  A paint gun (or hair drier in a pinch) would do the trick.

This **probably isn't the right size**, but it was what I saved in my bookmarks a few months ago.

http://www.ebay.com/itm/6-FT-OF-BLACK-4-41-112MM-PVC-HEAT-SHRINK-4-BATTERY-PACKS-USA-SELLER-/380807205162?hash=item58a9e0d12a:g:GDgAAOSwsB9WACUb
```

---
## \#32 Posted by: hj01 Posted at: 2017-10-11T18:13:53.020Z Reads: 134

```
Hey, i've just read the entire thread and it's super informative, thanks.

regarding the thickness of the wire in the parallel connections - you said that you've used an 8 guage wire. Isn't that a problem if one of the cell will get bad and shortout ? 
In that kind of situation the other cells in the group will pump the faulty cell and get ruined themselves.

In my understanding it is better to use a thick wire for the series connection and to isolate each cell with a thinner wire for the parallel connections. 

would like to hear you opinion, thanks.
```

---
