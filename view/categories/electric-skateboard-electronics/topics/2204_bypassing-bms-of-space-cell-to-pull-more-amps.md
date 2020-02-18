# Bypassing BMS of space cell to pull more amps

### Replies: 34 Views: 4571

## \#1 Posted by: evoheyax Posted at: 2016-04-06T20:42:34.932Z Reads: 295

```
So I'm getting ready to mod my space cell to pull 60 amps instead of 30 amps.

BMS can tax a max of 30 amps, so I need to pull power before the BMS instead of after.

**Do I need the bms powered off while pulling 60 amps before it?**
Maybe my image how electricity flows is incorrect. But the way I see it is, if I'm pulling 60 amps before the bms, the 60 amps will go through the bms still if the bms is powered on. If it's powered off, there would be no issue. Is this a correct interpretation?

This would imply I can't power the battery while the board is on.

I just want to make sure I don't blow out the bms by wiring around the bms.

Would buying a 60a 10s li-ion bms be a better idea to maintain functionality or is it unnecessary?
```

---
## \#2 Posted by: onloop Posted at: 2016-04-06T22:15:03.881Z Reads: 293

```
I have never done this before, so this is an experiment, I imagine just solder another set of wires directly onto the battery where the existing discharge wires are coming from, bypassing the BMS.

Please be sure to set the current limit in the vesc so you don't cook your pack trying to pull too many amps.

then you will have two sets of discharge wires, one that is BMS limited ones that are not. this way you can choose.
```

---
## \#3 Posted by: evoheyax Posted at: 2016-04-06T22:23:00.480Z Reads: 288

```
Could you imagine this damaging the cells, by not pulling through the bms? 

I'm going to buy a bms in the group buy on here that can pull 80 amps, so everything can be wired through a bms, but in the mean time I still need power, so I'll try out what you suggested.
```

---
## \#4 Posted by: onloop Posted at: 2016-04-06T22:24:22.033Z Reads: 280

```
[quote="evoheyax, post:3, topic:2204"]
Could you imagine this damaging the cells, by not pulling through the bms?
[/quote]

yes, it is possible to damage cells if you discharge them too rapidly.
```

---
## \#5 Posted by: evoheyax Posted at: 2016-04-06T22:25:59.653Z Reads: 265

```
And that can be taken care of by setting the max dischanrge in the VESC.

Is the a max amps that these particular cells should be discharged at?

I know you said set them to 60, I was curious if they can take 80 continuously?
```

---
## \#6 Posted by: onloop Posted at: 2016-04-06T22:27:17.539Z Reads: 259

```
the vesc can control current from battery.
```

---
## \#7 Posted by: evoheyax Posted at: 2016-04-06T22:29:58.664Z Reads: 261

```
Yes, I get that.

But is 60a the max I should discharge from these cells? Or are they capable of 80a?
```

---
## \#8 Posted by: longhairedboy Posted at: 2016-04-07T18:56:06.226Z Reads: 248

```
soldering a set of leads directly from BMS where the pack leads go into the BMS should work, it will basically put the ESC in parallel with the BMS, which will allow you to balance charge and discharge while bypassing the BMSs safeties during riding discharge. 

Yes there is a very decent chance of over discharging your cells this way. I wouldn't pull more than 60 from them if you want them to last any length of time. i believe the cells individually are only capable of 25Amps burst, which would put them somewhere around 75A burst in the space cell's 3P config. I could be slightly off on that though. Either way expecting 80 amps out of them is potentially dangerous.
```

---
## \#9 Posted by: evoheyax Posted at: 2016-04-07T23:12:03.958Z Reads: 239

```
Could I over discharge if I set the lower voltage limit on the VESC? Are taking about the battery become unbalanced, even if I balance them from the bms at each charge?
```

---
## \#10 Posted by: TheWrongHombre Posted at: 2016-04-13T15:36:36.970Z Reads: 228

```
@evoheyax

Have you had any luck with this project?

Did you decide where to draw the line on output?  Are you thinking 60 amps?
```

---
## \#11 Posted by: evoheyax Posted at: 2016-04-13T15:42:33.526Z Reads: 227

```
Yes, its working great so far. I set each vesc to max of 25 amps, so 50 amps total. This DID fix my hill climbing problems.

**Before:**
<img src="/uploads/db1493/original/2X/a/a0d96027eb09473e7393a3db89155357ee980b07.JPG" width="375" height="500">

**After**
<img src="/uploads/db1493/original/2X/d/d8de502853218c7798c6c5313c7e9fbe80fc557b.JPG" width="375" height="500">
```

---
## \#12 Posted by: TheWrongHombre Posted at: 2016-04-13T15:56:55.076Z Reads: 222

```
Glad to see you got this working!

Have you put it through its paces yet?

Also, the new PRO4 states a peak output of 80Amps.  If you had the PRO4 would you have gone higher than 25Amps per vesc?
```

---
## \#13 Posted by: evoheyax Posted at: 2016-04-13T16:34:35.744Z Reads: 217

```
Yes. I would do 50 amps per motor if possible.

I did 1 good 5 mile hike with plenty of hills on it, and a bunch of flat ground testing. I can't say if this will last, its just kinda a hoping game now.

Since these cells can burst at 75 amps, I'm assuming the constant is closer to 45 or 50 amps, thus why I decided to settle on 25 each.
```

---
## \#14 Posted by: RunPlayBack Posted at: 2016-04-13T17:38:11.801Z Reads: 207

```
Very cool, can you elaborate on the improvements? Better hill climbing in regards to temperature? Noticeable speed increase?
```

---
## \#15 Posted by: evoheyax Posted at: 2016-04-13T18:25:58.062Z Reads: 208

```
I was never able to determine what caused the roll backing of speed on hills. There is a chance that allowing 25 amps instead of 15 is not really playing any role here, seeing as I also have chaka's heatsinks on these vescs. So it might have been a temperature thing all along. But I can go up hills of 7% grade on my route to school without an issues of slowing down. The ONLY limit I hit during my commute was a low voltage limit, which is a weakness of the battery again. Once I get to 30%, a hard trigger plug on a hill will sag it right down to 0%, causing the vesc to rollback. This is not too big of a deal, since I am over most of the hills by the time I starting having this problem.
```

---
## \#16 Posted by: onloop Posted at: 2016-04-14T23:19:28.589Z Reads: 196

```
[quote="evoheyax, post:15, topic:2204"]
The ONLY limit I hit during my commute was a low voltage limit, which is a weakness of the battery again.
[/quote]

might need to add another 10 cells.
```

---
## \#17 Posted by: evoheyax Posted at: 2016-04-15T02:30:13.395Z Reads: 201

```
Is that possible (considering the cells I have are not new anymore))?

Either way, I was planning on build my own pack sooner or later. I know I running the cells hard like this, and I don't expect more than 400 cycles. Been through 4 days of commuting (8 cycles, 5 miles per cycle, total of 40 miles). Had an issue today with the pins for the canbus port (I think that's the right name) of one of the vesc's broke off. I had to solder the wires to the bottom of the port, and used lots of hot glue to keep the wires between the vesc's in place. So for now, all is working great.
```

---
## \#18 Posted by: shred Posted at: 2016-04-26T19:08:21.531Z Reads: 191

```
I dont really have a clue but I think you might as well check and reinforce the connections between the cells, because (theoretically) if these are made out of normal nickel strips they might only support around 45A continuous, depends there are different ones out there, but I didn't find any which would support 60A yet. 

If you have a 3P and each single cell supports 20A continuous you could get 60 out of a "cell" while being sure you are not going to damage the actual cells.

just some thoughts guys.........
```

---
## \#19 Posted by: Kaly Posted at: 2016-08-06T16:20:56.267Z Reads: 156

```
Hello :slight_smile:
 
How is the battery holding up so far ? 

I'm planing on using this technique on my battery packs ( future and current ). 

IMO with the VESC voltage limit and choosing a safe overhead for li-ion. The discharging function of a BMS is just not that necessary. 

That way we can have smaller bms in the battery pack and bypass it to discharge.
```

---
## \#20 Posted by: evoheyax Posted at: 2016-08-06T17:57:34.100Z Reads: 147

```
So far so good. I have done around 100 charge and discharges like this and no issues what's so ever. 50 amps is for sure within these cells potential for continuous discharge. I do expect the battery to last less though. The VESC does a great job of slowly cutting me off as I approach the end of my space cells charge.
```

---
## \#21 Posted by: Kaly Posted at: 2016-08-06T18:00:42.772Z Reads: 129

```
thank you for the input.

the reasoning i have is that we can get a 15A bms and charger and not to break the bank.
```

---
## \#22 Posted by: evoheyax Posted at: 2016-08-06T18:02:56.397Z Reads: 134

```
That's a interesting idea. You should have no issues with discharging around the bms. My bms still works great on my space cell. I road with my laptop and the bldc program to Track my ride and see what amps I pulled, and I was consistently at 25-27 amp (per VESC, so 50-54 amps total) on steeper hills.

Personally, I like idea of discharging through a bms also. So if I bought a bms, I would likely buy one that can pull the amps I want. May I ask what bms your looking at buying?
```

---
## \#23 Posted by: Kaly Posted at: 2016-08-06T18:05:20.617Z Reads: 125

```
this one or something like it 
http://www.bestechpower.com/384v12spcmbmspcbforlifepo4batterypack/BMS-D105.html
```

---
## \#24 Posted by: Kaly Posted at: 2016-08-06T18:08:27.199Z Reads: 127

```
i have been using my batteries without a bms as for ever, but will like to make some packs for other people to use and that is when you need the easiest way to charge in order to minimize mistakes.

the inconvenience so far is that plug and play chargers with more than 5 Ah are really expensive and the space in the enclosure can be better use for more cells instead of a oversize bms.
```

---
## \#25 Posted by: evoheyax Posted at: 2016-08-06T18:08:31.517Z Reads: 127

```
That's actually a perfect solution to my problem right now. How much are those guys? (I couldn't find any prices)
```

---
## \#26 Posted by: Kaly Posted at: 2016-08-06T18:09:43.270Z Reads: 123

```
i need to email them.

but from a group buy that some guys did,  it's not that expensive
```

---
## \#27 Posted by: Kaly Posted at: 2016-08-06T18:11:10.136Z Reads: 120

```
this is what i like the most 
	
Size (L*W*T)
L70mm * W55mm * T7.6mm
```

---
## \#28 Posted by: evoheyax Posted at: 2016-08-06T18:11:47.347Z Reads: 119

```
I like the idea, becuase high amp 12s bms's are really big. I don't have that kind of space to spare right now.
```

---
## \#29 Posted by: Kaly Posted at: 2016-08-06T18:15:13.409Z Reads: 117

```
this is a 12s for lifep04 if you are working on 12S li-ion they have this one 
http://www.bestechpower.com/444v12spcmbmspcbforli-ionli-polymerbatterypack/PCB-D105.html

similar model but for li-ion
```

---
## \#30 Posted by: Kaly Posted at: 2016-08-06T18:21:36.693Z Reads: 112

```
My reasoning is that we are putting 3-4 cells in parallel and then attaching the balance leads to this pack, if a cell is to have any complication the BMS will not act on this because it takes the pack as a single cell. we are taking a average approach to each cell pack within the battery, so why not do it on the discharge of the whole pack and let the BMS just keep the cells balance and charge the pack.
```

---
## \#31 Posted by: evoheyax Posted at: 2016-08-06T18:29:16.429Z Reads: 107

```
That makes sense.  Discharging through the bms is pointless if you are using a VESC. I'm in the middle of figuring out how to keep my cells balanced, and I have little to no space to do this in.
```

---
## \#32 Posted by: Kaly Posted at: 2016-08-06T18:40:06.030Z Reads: 108

```
Then this small bms are the solution for our troubles :slight_smile:

you already have done the REAL WORLD test on the durability of the bms when use on this manner. for the discharging getting good cells and good VESC configuration will take care of that.

for balancing the cells, this bms have balancing function. 
from the web page : 

6.How balancing function works? after battery pack is fully charged. PCM will detect each cell's voltage and trim higher voltage down until other cells reach the same voltage level. Therefore, it helps cells have longer service life.
```

---
## \#33 Posted by: evoheyax Posted at: 2016-08-06T19:03:36.914Z Reads: 107

```
Have you found a good charger to use with the bms? That's the part I'm having trouble with.
```

---
## \#34 Posted by: Kaly Posted at: 2016-08-06T20:22:21.839Z Reads: 109

```
i order this one from this guys 
http://www.batterysupports.com/36v-42v-5a-lithium-ion-battery-charger-10s-10x-36v-lion-lipo-p-166.html

it's 5Ah
```

---
