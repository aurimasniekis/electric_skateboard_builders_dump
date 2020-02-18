# Vedder sparkswitch 25$ chaka&rsquo;s revision

### Replies: 36 Views: 3073

## \#1 Posted by: Shogu12 Posted at: 2017-04-12T23:30:04.327Z Reads: 322

```
Selling completely  surface mount  soldered sparkswitches. You only need a button/ switch and a fuse (if you chose to use one).<img src="/uploads/db1493/original/3X/3/e/3e9c1d907b1fb13f06b04c291689940f31528d57.jpg" width="666" height="500"> add your own wires last time to many people wanted something special.  2$ us shipping 5$ Europe. 50 Available  will ship instantly.  I can add awg10 wires (non silicone) to both sides if you wish. I have 5 led pushbuttons left and can add them to the switches for 3$.The flip switch would be 1$ <img src="/uploads/db1493/original/3X/d/6/d6bf7e3cadc21a195601e818bd2d9017fc126e6e.jpg" width="666" height="500"> Trying to get more $$$ for motormounts so I'm  pricing to move.
1 per Switch 25$
2 per Switch 23$
5 per switch 20$
10 per switch 18$
```

---
## \#2 Posted by: Pantologist Posted at: 2017-04-12T23:33:14.945Z Reads: 301

```
Just curious, what is the heated bed for?
```

---
## \#3 Posted by: Shogu12 Posted at: 2017-04-12T23:39:18.080Z Reads: 297

```
Preheat the bottom of the pcb's to reduce the heatstress on the fets from the heatgun.
```

---
## \#5 Posted by: RootedSuperuser Posted at: 2017-04-24T19:25:45.339Z Reads: 246

```
Was this made with the 2oz copper?
Does this have the **75V** IRFS7730-7?
<img src="/uploads/db1493/original/3X/6/a/6a35b500b5be99b3fa539b4d8d2accf340392e2a.jpg" width="138" height="500">
```

---
## \#6 Posted by: sl33py Posted at: 2017-04-24T20:58:38.977Z Reads: 224

```
Most likely not - Vedder's BOM lists the IRFS7530TRL7PP.

You'd need to ask the experts if it's as simple as swapping in the higher voltage 7730 you mention.  There may be other components you need to replace as well to make this worthwhile?

I've seen some go to 3 FETs as insurance to make them more durable if you are pushing the higher voltages.

GL!
```

---
## \#7 Posted by: Shogu12 Posted at: 2017-04-24T21:22:31.109Z Reads: 209

```
Its 2oz copper and the 60v mosfet.
```

---
## \#8 Posted by: RootedSuperuser Posted at: 2017-04-24T22:26:28.012Z Reads: 204

```
"I've seen some go to 3 FETs"
Where?....
```

---
## \#9 Posted by: RootedSuperuser Posted at: 2017-04-24T22:28:33.983Z Reads: 204

```
Whats the cost without the fet's?
I need the 75V's and that another 16 bucks for me.
I'm pushing 14S @ 30A and the fet you are using is rated for 12S 30A.
```

---
## \#10 Posted by: Shogu12 Posted at: 2017-04-24T22:44:04.130Z Reads: 196

```
@RootedSuperuser  If you're  pushing 14s then these are still fine, fully charged 14s  is 58.8V which is only right after charging that being said I still can make you one with everything but the mosfets for 12$. You could  always use 2 if you're unsure.
```

---
## \#11 Posted by: RootedSuperuser Posted at: 2017-04-24T22:54:35.714Z Reads: 192

```
 
"I still can make you one with everything but the mosfets for 12$"
**YES**, I have a TESLA module from a 90D showing up tomorrow and need this for the battery build.
I will PM you and go from there with my personal email.
I do not trust public forum servers for security reasons.
Lets get rocknin on this.....
```

---
## \#12 Posted by: Pantologist Posted at: 2017-04-24T23:09:55.114Z Reads: 182

```
Oooo. Are you making like a gigantic pack? Those Tesla cells have like 10A continuous discharge ratings.
```

---
## \#13 Posted by: sl33py Posted at: 2017-04-24T23:12:03.097Z Reads: 187

```
[quote="Shogu12, post:10, topic:20894"]
If you're  pushing 14s then these are still fine, fully charged 14s  is 58.8V
[/quote]

I politely disagree or maybe better raise this as borderline possible.  

I've heard of users who had theirs fail at 12s, and 14s likely will exceed...  But though i've reflowed some v1.3 Vedder anti-spark switches (i sent Ben 1/2 of all profits and helped purchased a reflow oven w/ my part), i'm no EE.  So i defer to the experts.

I saw a github w/ a triple FET when searching for Vedder's BOM to clarify the FET used.  THey are out there, but not sure if anyone here is selling "kits" or spare PCB's.

Having sold some "kits" - unsoldered... I'd caution folks who aren't familiar with SMD soldering (reflow oven/skillet or hot-air) to not try.  Ham-handed soldering this with an iron will not work well.  My experience, but only my .02 and opinion.  You may be an expert w/ a solder iron and perfectly able...
```

---
## \#14 Posted by: RootedSuperuser Posted at: 2017-04-24T23:19:11.771Z Reads: 177

```
444 Cells in 1x 90D module. TESLA NCA chemistry, same/similar discharge curve to the Sanyo NCR18650GA cell and amp range @ 3550mAh.
The big difference is TESLA has a 2000 duty cycle and Panasonic/Sanyo cells (B/GA) have a 500 charge/discharge duty cycle. But that all depends on how you treat your cells.
I'm building 2 packs, 14S6P for me, and 20S8P. The 20x8 will use a golf cart solenoid, it will go onto a stretch cruiser, Edge 1500W hub.
```

---
## \#15 Posted by: RootedSuperuser Posted at: 2017-04-24T23:28:18.762Z Reads: 171

```
Yes, I can reflow.
I've spent 1 week + researching this item, I haven't found ANY 3 fet units. **LINK?**
Also, Emery paper glued onto a very flat surface, or using a diamond sharpening stone, flatten out both fet surface's, use Thermal Adhesive to apply a Heat Spreader.
A build upgrad may even include a DC fan when turned on, such as some BEC's have.
```

---
## \#16 Posted by: sl33py Posted at: 2017-04-24T23:37:23.562Z Reads: 173

```
Nice!  I'm an old school IT guy and have lapped a CPU a time or three to improve cooling (Air and Water - never went dry ice or immersion cooling).

I had a buddy send me a triple FET he was developing - as yet untested since i've been working and not playing w/ esk8 as much as i'd like.  I have one more to reflow for him.  Let me see where my spare is at.  Maybe i could send it to you to torture test at 14s?  I'll shoot you a PM.  This is not to sell it (there are 2...), and not trying to step on Shogu12's toes!
```

---
## \#17 Posted by: RootedSuperuser Posted at: 2017-04-24T23:41:45.123Z Reads: 177

```
I'm already looking at 25mm cooling fans with heat spreaders.
Ya, I'll give it a go, PM me.
I'll take a unit from Shogu12 as well, as a BU.
```

---
## \#18 Posted by: RootedSuperuser Posted at: 2017-04-26T00:46:42.727Z Reads: 176

```
And now the teardown and rebuilding begins.
<img src="/uploads/db1493/original/3X/d/8/d8ffedd1edd548c74fe47b102949e3cbb6e5db1a.jpg" width="690" height="388">
444 cells / 3 banks = 148 x 3.5v = **518 Volts, 30 Amps** nom, 60 Amps Peak.
There are 16 of these in 1 pod. for a total of 900 Volts, 400 Amps.
The - and + are unprotected, Anyone up for a dare?
```

---
## \#19 Posted by: Shogu12 Posted at: 2017-04-26T00:48:01.313Z Reads: 173

```
I envy you honestly. I did the same thing with 8 segway batteries but they  were a pain in my ass.
```

---
## \#20 Posted by: Pantologist Posted at: 2017-04-26T02:13:13.906Z Reads: 173

```
I wouldn't leave that much power sitting on my kitchen countertop if I were you!
```

---
## \#21 Posted by: TarzanHBK Posted at: 2017-04-26T06:58:21.679Z Reads: 167

```
throw some copper over that for protection!





(No pls don´t do that :smiley:)
```

---
## \#22 Posted by: RootedSuperuser Posted at: 2017-04-26T10:20:19.018Z Reads: 169

```
[quote="TarzanHBK, post:21, topic:20894, full:true"]
throw some copper over that for protection!
(No pls don´t do that :smiley:)
[/quote]

I threw some copper on it just as you mentioned.
Each cell is wired with a fusible link that should be blown. Best way to do this is to short out the poles.....

<img src="/uploads/db1493/original/3X/f/e/fe2ca4d65723ad996750b38b3ea22d5de8333ac7.jpg" width="690" height="389">

<img src="/uploads/db1493/original/3X/e/9/e9e2bb6b64852f9f275d383abc6288a0c93e7ab5.jpg" width="690" height="389">

<img src="/uploads/db1493/original/3X/7/e/7ee428a569c3c0249ec9ae9c1dd10e44c625f9c8.jpg" width="690" height="389">

<img src="/uploads/db1493/original/3X/2/b/2b68cab311c52628a6582ed252604c5166d98c13.jpg" width="690" height="389">


<img src="/uploads/db1493/original/3X/2/3/2319726c38b752c79111d27f9fa9e25a759fe0e9.jpg" width="690" height="389">

<img src="/uploads/db1493/original/3X/6/b/6bddb3dac969dcf02c2d0e2d6064629ee7b0a148.jpg" width="690" height="389">

At 518 volts and 60 Amps, my booster cable copper ends vaporised.
I just ripped the covers off in the end, just as quick, not so dramatic.

<img src="/uploads/db1493/original/3X/1/e/1ea169402aed6e85cb6e82288abf745dbe6370c4.jpg" width="282" height="500">

***EDIT***
And this is the fruit of labor.
<img src="/uploads/db1493/original/3X/1/c/1c19afd9f304a5674002c1ee387a023eba094216.jpg" width="690" height="389">
```

---
## \#23 Posted by: Maxid Posted at: 2017-04-26T10:47:37.918Z Reads: 159

```
why should the fuse wires melt when you touch the positive and negative of the entire pack?
The current going through a single cell should not be even close to melting the wire.
```

---
## \#24 Posted by: TarzanHBK Posted at: 2017-04-26T10:48:51.513Z Reads: 159

```

:joy::joy::joy::joy::joy::joy:
LOL! That made my day! Hope there´s nothing damaged... but yeah should work fine, if the fuse wire really protects the cell, that they don´t suffer under a too high current
```

---
## \#25 Posted by: RootedSuperuser Posted at: 2017-04-26T11:10:18.992Z Reads: 162

```
[quote="TarzanHBK, post:24, topic:20894, full:true"]

:joy::joy::joy::joy::joy::joy:
LOL! That made my day! Hope there´s nothing damaged... but yeah should work fine, if the fuse wire really protects the cell, that they don´t suffer under a too high current
[/quote]

Nothing wrong with the cells, I pulled 38 tonight, all fine.
My booster cable, both -'s are vaporised.
Shudda used welding cable without 1 end.
I'm cutting a snip from the video and will up it soon.

In the meantime, here are 2 other guys dead shorting a pack as well.
https://youtu.be/_IYXxGQ6Giw
```

---
## \#26 Posted by: Print3r Posted at: 2017-04-27T06:49:29.257Z Reads: 158

```
Looking to buy one of these switches in September for a 7s6p INR 18650 pack (20A continuous from each cell, 2500mah for each cel) setup. Will this be fine (don't want any sparks on my first build) - I have had enough magic smoke and am looking to avoid it!
```

---
## \#27 Posted by: Shogu12 Posted at: 2017-04-27T07:35:35.596Z Reads: 159

```
Yes it can absolutely handle that pack all sparks will be gone and everything gets powered by the push of a button.
```

---
## \#28 Posted by: RootedSuperuser Posted at: 2017-04-27T14:19:11.284Z Reads: 156

```
[quote="Print3r, post:26, topic:20894, full:true"]
a 7s6p INR 18650 pack
Will this be fine
[/quote]

Your best indicator of compatibility with any battery pack is the **BMS** that is in the pack you are building or considering.
The ASW is rated at 30A, the BMS must not exceed 30 Amp output.
This has nothing to do with the cells capacity as any Parallel group may exceed the 30 Amp capability of the ASW.

Volts increase in the Series, Amps stay the same.
Volts stay the same in Parallel, Amps increase.
You have S,20A*6P=120A is the unregulated total output (Not peak output).

In Theory:
If your battery pack BMS is delivering 25V 60A, you will need 2 of these in Parallel to not burn them up.
If your battery pack BMS is delivering 25V 30A, you will need 1 of these.
If your battery pack does not have a BATTERY MANAGEMENT SYSTEM, the total PEAK output is what you will be putting through the circuit, that will be over 120 Amps.
The final determining factor is what's the total draw of your system, if all the system can take is 5 Amps, well then you're fine, if your system can eat 60 Amps, but is throttled by a BMS @ 30 Amps, your marginal, but within the rated specs.
If you are running a motor that eats 60A nom and 90A peak, and you have a battery pack at 25V 120A without a BMS......TOAST, Well Done Toast.
```

---
## \#29 Posted by: Print3r Posted at: 2017-04-27T19:05:58.050Z Reads: 141

```
I was planning on using the VESC in my setup to limit the current and do not expect too much cell voltage drift (I will have 6 cells in parallel then connected in series 7 times - each lot of 6 cells with have the same voltage) and I will be balance charging them. I have decided to go for a (http://www.screwfix.com/p/schneider-electric-easy9-50a-single-pole-type-b-mcb/9688p) as they are relatively cheap, local and I will set up my VESC so that the current cannot go above 45A. Please let me know if you think my plan is crazy and that I am asking for a fire!
```

---
## \#30 Posted by: RootedSuperuser Posted at: 2017-04-28T06:11:09.440Z Reads: 129

```
[quote="Print3r, post:29, topic:20894"]
I am asking for a fire!
[/quote]
Yes you are.
```

---
## \#31 Posted by: Print3r Posted at: 2017-04-28T06:43:11.002Z Reads: 129

```
I don't really understand as I will also be using a Low Voltage Alarm Buzzer Indicator Meter (the alarm used on lipos which are triggered at 3.3V). These alarms constantly check the voltage of all the cells you are using in series and sound an alarm if they go under 3.3V - the equivalent of 1.8Ah used of total 2.25ah under 5A load per cell - 30A at 29.4V in total. So I won't be draining my cells excessively - no fire risk and I will be charging with a balance charger (they won't get overcharged) - no fire risk. Where is the fire risk if I have set my vesc to limit the current output?
```

---
## \#32 Posted by: Shogu12 Posted at: 2017-05-10T00:58:00.818Z Reads: 123

```
Bump still have a bunch available.
```

---
## \#33 Posted by: Jinra Posted at: 2017-05-10T01:13:41.287Z Reads: 130

```
If you don't use a fuse do you simply connect the 2 pads?

Could you provide a labeled picture of the finished product. Trying to visualize where all the wires go.
```

---
## \#34 Posted by: Shogu12 Posted at: 2017-05-10T01:26:02.871Z Reads: 130

```
Yes you connect the two pads and if you bought one of my switches the visualized image is on the back of it.
```

---
## \#36 Posted by: WrinklyWink Posted at: 2017-08-22T05:20:46.715Z Reads: 87

```
im interested in purchasing one. are they still available for sale?
```

---
## \#37 Posted by: nw-esk8 Posted at: 2017-08-22T08:23:12.460Z Reads: 80

```
perhaps +1... but did I read right that the amp limit on them are 30A?
```

---
## \#38 Posted by: banjaxxed Posted at: 2017-08-22T15:03:10.883Z Reads: 71

```
@Shogu12 is not around these days, a GB went tits up and he's gone awol
```

---
