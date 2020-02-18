# Bypass Bestech BMS for dischage, wiring scheme - help please

### Replies: 19 Views: 2596

## \#1 Posted by: thisguyhere Posted at: 2017-07-03T07:14:36.336Z Reads: 342

```
planning wiring for a 12s pack with a bms.  this is first time using a bms and need some help.

i'm just using the bms for charging and bypassing it for discharge.

found this diagram to be pretty useful but the bestech bms has an additional C- port.

would this wiring work? if someone using a bestech bms could kindly chime in?

<img src="/uploads/db1493/original/3X/f/8/f8f79f6ea7a371e63e1e993fd77654909d9ecefa.jpg" width="690" height="389">

<img src="http://www.electric-skateboard.builders/uploads/db1493/original/2X/2/2094476139b90c721d4eb45ce2f0ec8150c53642.jpg" />

Wiring scheme from mfgr:

<img src="/uploads/db1493/original/3X/a/8/a85c1512e5ce9129b706fa88f24451d8b2081016.jpg" width="500" height="500">
```

---
## \#2 Posted by: IsTalo Posted at: 2017-07-03T11:03:04.397Z Reads: 309

```
Why bypass a 80a Bms?
```

---
## \#3 Posted by: rpn314 Posted at: 2017-07-04T17:56:52.896Z Reads: 297

```
I think you've got 3 different schematics there, and the only one that would work for anything is the one from the manufacturer (which doesn't bypass for discharge)

Generally there's 3 ports on a BMS for the following:

- 1 for Negative terminal of battery pack (looks like B- for this pack)
- 1 for the negative terminal of the charger input (I think that would be P- for you)
- 1 for the negative terminal of the load (the VESC or anti-spark switch, which I think is C- for you)

The positive terminals are then just connected together.

If you want to bypass then you just ignore the one for the load and connect the negative terminal for the load straight to the battery pack.

Though I would second @IsTalo's point. If you have a good BMS (60A+, which this looks to be) I don't know why you'd want to bypass on discharge.
```

---
## \#4 Posted by: Namasaki Posted at: 2017-07-04T18:07:20.237Z Reads: 285

```
I'm gonna third @IsTalo comment.
Why in the world would you bypass a bms capable of 80a cont and 240a peak
You would be throwing away a lot of protection for no reason.
Bypassing is a compromise when using a small low current bms
```

---
## \#5 Posted by: thisguyhere Posted at: 2017-07-04T18:20:43.081Z Reads: 282

```
yea after sleeping on it decided to just use the bms for discharge as well.

i didn't want the bms to limit discharge in anyway but since it's such a high amperage unit it shouldn't be a problem.  may consider bypassing if after vesc monitoring find amp draw nearing or exceeding bms rated discharge amperage.

found this diagram to be useful so should be ok.

the mfgr's diagram is useful for balancing lead connections but found the wire ports confusing as hell.

anyway, thanks for the input.

<img src="/uploads/db1493/original/3X/d/4/d49ed811b9536efbebb6e8feeb362ba58762eaee.png" width="690" height="319">
```

---
## \#6 Posted by: rok Posted at: 2017-07-04T19:28:37.345Z Reads: 257

```
Can someone please tell me how to discharge? Why and with what? How often?
```

---
## \#7 Posted by: oyta Posted at: 2017-07-04T20:08:46.949Z Reads: 251

```
@rok I am not sure what you are asking. Normally discharing is done by riding your board :slight_smile: Depending on your battery type and  setup there are different lower threshold for discharging. E.g battery type Samsung 25R, data sheet here: https://www.imrbatteries.com/content/samsung_25R2.pdf, has a end voltage at 2.5V but you will not go as low during your rides. You can see the discharge curves in the data sheet and it drops really fast around 3.1V. You can use a VESC and BMS as follows:

* Using a VESC you can set it to slowly reduce power between 3.3V and 3.1V where at 3.1V you do not get any more power.

* If you have a BMS you would set the BMS discharge voltage to a lower voltage than the VESC e.g. 2.6V to have a margin to the end voltage. The VESC should anyhow stop discharging at a higher voltage.
```

---
## \#8 Posted by: oyta Posted at: 2017-07-04T20:10:08.615Z Reads: 244

```
This looks correct.
```

---
## \#9 Posted by: rok Posted at: 2017-07-04T20:29:32.524Z Reads: 239

```
Ok i think i get it now, cuz i thought you need to somehow discharge your battery if you don't use up all the juice at the end of the day or something...pretty noob 
I do indeed have a 10s4p pack with samsung 25r cells with a basic chinese bms so i will bypass it and then set the vesc right. 
Your post is very helpful, thanks! I might contact you again once the time comes to set up my vesc.
```

---
## \#10 Posted by: oyta Posted at: 2017-07-04T20:38:15.080Z Reads: 231

```
Remember when you have 10s the voltage is 10 * battery voltage. If nominal voltage of the battery is 3.6V the 10S battery pack is 36V nominal. Then the numbers I used as an example in the previous post must be multiplied with 10. I.e. the end voltage is 25V and the VESC settings should be at 33 and 31 Volts.
```

---
## \#11 Posted by: psychotiller Posted at: 2018-03-22T21:17:09.665Z Reads: 166

```
Because the 80a bms constantly cut out. And a cutout/reset at 30+ mph is dangerous.
```

---
## \#12 Posted by: Namasaki Posted at: 2018-03-22T22:18:41.923Z Reads: 158

```
[quote="psychotiller, post:11, topic:26659, full:true"]
Because the 80a bms constantly cut out. And a cutout/reset at 30+ mph is dangerous.
[/quote]

I haven't had a problem with mine cutting out except once when I ran the battery all the way down and once when one of my battery connections broke loose.
```

---
## \#13 Posted by: psychotiller Posted at: 2018-03-22T23:07:17.708Z Reads: 158

```
I've had issues with probably 5 of the last 8 that i used. We have since gone to charge only wiring. some of them probably do work. Quality control may be the issue. Or maybe some just aren't actually 80a continuous capable. At any rate, too many have failed for me to use them anymore.
```

---
## \#14 Posted by: rockon915 Posted at: 2018-08-26T01:20:54.494Z Reads: 105

```
Would anyone know why the bestech12s bms would cause me to have an early low voltage cutoff? Usually around 44.4V. 12s5p to bestech 12s bms(HCX-D223v1) to 80 amp antispark (from eskating.eu) to dual focbox to dual TB6374. Running 60A motor max 30A battery max. voltage cutoff on focbox start set to 41.0V and end set to 39.0V.

antispark link https://eskating.eu/product/anti-spark-power-switch/

bms link https://eskating.eu/product/12s-bestech-bms-80a-12s4p-5p/

Any input would be great as i would like to go for a ride without unexpected cutoff and support hasnt been of much help yet. hopefully they will get back to me with more info.
```

---
## \#15 Posted by: rockon915 Posted at: 2018-08-26T01:21:41.914Z Reads: 105

```
Note that each cell is verified at 3.7V per cell
```

---
## \#16 Posted by: hyperIon1 Posted at: 2018-08-26T02:25:25.325Z Reads: 102

```
You want to use that bms but on a bypass setup?
```

---
## \#17 Posted by: rockon915 Posted at: 2018-08-26T05:23:21.042Z Reads: 97

```
i would like to not have to bypass as its keeping my batteries balanced perfectly but im getting a cutoff at 44.4v or 3.7v per cell. I just had someone tell me that my cutoff was set to high so i changed it to 38v start 34v end and had the exact same issue leading me to believe it is my bms causing the issue
```

---
## \#18 Posted by: hyperIon1 Posted at: 2018-08-26T06:26:25.555Z Reads: 93

```
Well, to be clear when I say bypass I mean discharge only. A lot of builders are going to a charge/ balance bms. Due to the cut out issue. 
In your case it can be done with that bms. It’s eazy to do and you won’t have the cut out problem. You still get the charge/ balance/ over charge functionality you just lose the discharge protection. Your esc can do that. 
In every pack we build we bypass discharge and use a smaller bms like the d140 or d163. 
If you do decide to try the direct discharge setup let me know and I will pm you a diagram.
```

---
## \#19 Posted by: rockon915 Posted at: 2018-08-26T15:44:45.330Z Reads: 88

```
yeah im deffinetly going to try bypassing the bms for discharge i beleive i just undo the negative off the bms and disconnect the negative off of the antispark to bms and attach those but a diagram would be great to verify
```

---
