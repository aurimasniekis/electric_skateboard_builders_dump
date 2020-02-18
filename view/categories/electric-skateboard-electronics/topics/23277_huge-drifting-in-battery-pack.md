# Huge drifting in battery pack!

### Replies: 32 Views: 1801

## \#1 Posted by: Tuomalar Posted at: 2017-05-17T06:18:20.357Z Reads: 193

```
Hi. I bought batterypack from last group buy. It was wery low quality and i took it apart. 2 series were drifting all the time and now i did measure cell voltages. I wonder if this is caused by bad welding or crappy cells? 8 of the 4 sets (8s4p) were all 3.82V per cell and these 2 were drifting like crazy. 

When i connect them in parrallel it should balance itself all 4 cells?
<img src="/uploads/db1493/original/3X/d/9/d97e5f9bc588308442f5cddd877c4af53ba2989d.JPG" width="432" height="500"><img src="/uploads/db1493/original/3X/c/0/c0294480df9c5a657045ae940fe5da305f362a12.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/f/5/f5998e6f2f9207d1b61dab87c9fabee3cf6c0675.JPG" width="375" height="500">
```

---
## \#2 Posted by: Maxid Posted at: 2017-05-17T06:41:50.892Z Reads: 175

```
don't just connect drifted cells together in parallel. They will balance themselves but your have no control over the current flowing from the "charged" to the less charged cell. 0.1V or so doesn't matter but I see you have 4.07 and 3.69V cells there - that is too much. Either connect only similar level cells together or discharge/charge them one by one.
```

---
## \#3 Posted by: Tuomalar Posted at: 2017-05-17T06:57:47.614Z Reads: 165

```
That's what thougt. Just need to find something how i can charge/discharge them individually.
```

---
## \#4 Posted by: Eboosted Posted at: 2017-05-17T07:10:01.559Z Reads: 156

```
What would happen if you just connect them together? You might have a very small undetectable micro spark but I'm guessing it won't damage the cell at all.
```

---
## \#5 Posted by: Maxid Posted at: 2017-05-17T07:54:00.243Z Reads: 155

```
As I said - you don't have control over the current and the current might go above the charge current the cell is rated for.
A 25R is rated to 4A charge current. It can discharge a lot more so in a worst case scenario there could be more than the 4A flowing from the charged to the less charged cell. How much current there actually is I don't know. But I don't want to be the one finding out ;)
```

---
## \#6 Posted by: TarzanHBK Posted at: 2017-05-17T07:59:53.164Z Reads: 147

```
a simple trick would be a really thin cable. Just hook your cells up in parallel with it and you have kind of a fuse to avoid higher currents
```

---
## \#7 Posted by: Tuomalar Posted at: 2017-05-17T08:09:49.803Z Reads: 139

```
Very good idea!
```

---
## \#8 Posted by: Maxid Posted at: 2017-05-17T08:23:16.907Z Reads: 135

```
Or use a light bulb to discharge the pack to a similar level as the lowest cell
```

---
## \#9 Posted by: Tuomalar Posted at: 2017-05-17T08:37:32.336Z Reads: 133

```
I don't have any. But this works. Single strand from balance wire
 <img src="/uploads/db1493/original/3X/6/4/64a84a808127cad5bfe40791cb01f3fc3515fb24.JPG" width="375" height="500">
```

---
## \#10 Posted by: Norco Posted at: 2017-05-17T09:15:32.714Z Reads: 121

```
This is with a BMS too? Sorry to see you haven't had much luck with this pack. Without a BMS I have only seen drift of about 0.12v between parallel groups. I only charge to 40 volts anyway so no issue for me. Plan to check the pack once a week from now on.
```

---
## \#11 Posted by: Tuomalar Posted at: 2017-05-17T13:20:35.299Z Reads: 106

```
No bms have no effect on this. Problem is that 2 of 4-packs are actually only 3p because of bad weldings. So those two charge and disharge faster than the others. I haven't had any drift (0.0V) expect those two which were always +-0.2-0.4V
```

---
## \#12 Posted by: Norco Posted at: 2017-05-17T13:26:47.077Z Reads: 102

```
Might be easiest to discharge to the point where they are all even and then repair the pack and start cycling from there?
```

---
## \#13 Posted by: Tuomalar Posted at: 2017-05-17T13:32:34.367Z Reads: 101

```
Look that pic above. I balanced those 2 drifted packs and both balanced to 3.83 and 8 of them are 3.82 so i'm going to charge them with bms and then go without and check them every week.
```

---
## \#14 Posted by: KTMinni Posted at: 2017-05-17T13:35:34.781Z Reads: 101

```
Highly recommend picking up an imax b6 charger for like $20 just so you can slowly charge and discharge the cells.  Doing this at 1A will reveal any broken cells.  Nothing should happen if it is a good cell.  It's also possible to measure the internal resistance I believe.

Edit: PXSS recommends matching the cells by internal resistance so they don't drift unevenly.  i.e. they will be very similar in parallel.
```

---
## \#15 Posted by: Tuomalar Posted at: 2017-05-17T13:54:33.038Z Reads: 96

```
I do own one but it's broken. How does it reveal when battery is gone? I can measure resistance with my multimeter.
```

---
## \#16 Posted by: KTMinni Posted at: 2017-05-17T14:15:21.592Z Reads: 97

```
Internal resistance is a bit different.  It's a physical limit of the battery itself, so it effects the max discharge, how fast it discharges etc.  Ultimately the IR is an important factor of how you should group your batteries.  If they do drift, they will more likely drift as a pair and keep the same/similar voltage.  But you should pick up another imax b6 or something like that.
```

---
## \#17 Posted by: Tuomalar Posted at: 2017-05-17T14:33:31.244Z Reads: 88

```
But how does imax reveal broken cells? It just doesn't charge or can't balance or what?
```

---
## \#18 Posted by: KTMinni Posted at: 2017-05-17T14:36:00.587Z Reads: 88

```
Oh!!!  Ok yeah, basically high IR = bad low IR = good match them alike.  But also charging and discharging at 1A will reveal any bad cells because it is such a safe procedure (less than 1C) if any cells get hot or go el combusto on you are **probably** bad.
```

---
## \#19 Posted by: KTMinni Posted at: 2017-05-17T14:43:27.871Z Reads: 84

```
And if you want to go the cheap route you can also use a voltmeter and a resistor to calculate it.
```

---
## \#20 Posted by: Namasaki Posted at: 2017-05-17T15:00:55.226Z Reads: 82

```
[quote="Tuomalar, post:17, topic:23277, full:true"]
But how does imax reveal broken cells? It just doesn't charge or can't balance or what?
[/quote]
Usually, a bad cell will have much higher IR than normal. 
I got a couple bad Lipo packs from HK once. 
Each had a bad cell that where below 3.0v and with very high IR
```

---
## \#21 Posted by: Tuomalar Posted at: 2017-05-17T15:35:00.070Z Reads: 70

```
Any idea what is good value for IR?
```

---
## \#22 Posted by: Namasaki Posted at: 2017-05-17T17:03:35.064Z Reads: 69

```
It varies. 
For Lipos anything under 5 miliohms per cell.  
Li-ions that I have tested where much higher. 
You would need to test all your cells to get an average.
```

---
## \#23 Posted by: KTMinni Posted at: 2017-05-18T00:25:41.028Z Reads: 62

```
As namasaki said, you should test all of your cells and look for outliers.  If anything is abnormally high comparatively then you have a bad cell.
```

---
## \#24 Posted by: Norco Posted at: 2017-05-18T10:32:08.272Z Reads: 53

```
Thinking about stripping down my pack and rebuilding when I get a run of wet days and time. Idea will be to better match the batteries into packs and see if there are any with high IR so that I can swap them out with a couple of spares I have. I have an iMax B6 so will use this for the discharge/charge and IR. I'll document how I do this on my build thread when I get round to it.
```

---
## \#25 Posted by: PXSS Posted at: 2017-05-18T11:40:24.996Z Reads: 54

```
[quote="KTMinni, post:14, topic:23277"]
Highly recommend picking up an imax b6 charger for like $20 just so you can slowly charge and discharge the cells.
[/quote]

Do not get a knock off b6. They are known to overcharge batteries and will damage them in the long run. If you're going to buy a b6 make sure its the real thing from skyrc (it's usually about $40-50)

[quote="KTMinni, post:14, topic:23277"]
PXSS recommends matching the cells by internal resistance
[/quote]

That's only if you're building a pack from scratch with new batteries. In this case he already has the batteries wired in. 

[quote="Tuomalar, post:15, topic:23277, full:true"]
I do own one but it's broken. How does it reveal when battery is gone? I can measure resistance with my multimeter.
[/quote]

You cannot measure battery IR with a multimeter. How an rc charger does it is by rapidly increasing the current draw from 0A to 5A and measuring the voltage drop. R = V/I. They do this at several currents and get the average. 

Another reason not to get a fake charger is sinse their voltage sensors are crap, you never know if the IR measurements are accurate. 

[quote="Norco, post:24, topic:23277"]
if there are any with high IR so that I can swap them out with a couple of spares I have
[/quote]
Mixing new and old cells is bad. I would never recommend doing this.

@Tuomalar. It looks like you had some shitty welds which is probably the most common cause of drifting cells. I recommend you get the charged cells back in line with the others and then re welding the pack.

 I only recommend you ride with a BMS as if this happens and you ride your battery until it's fully depleted then the three cells that have to compensate for the missing cell will be at a much lower voltage and probably damaged. @Eboosted had several cells go all the way down to 0V a while ago because of the exact same issue and not using a BMS.
```

---
## \#26 Posted by: KTMinni Posted at: 2017-05-18T12:11:30.607Z Reads: 50

```
Tried to quote but I'm on mobile.  If he has the skyrc 12V switching power supply he can buy the imax for $20.  That's what I was getting at.  Also he had taken the batteries out of the pack, so I was saying he might as well match them.
```

---
## \#27 Posted by: Tuomalar Posted at: 2017-05-19T06:41:23.677Z Reads: 51

```
[quote="PXSS, post:25, topic:23277"]
I only recommend you ride with a BMS as if this happens and you ride your battery until it's fully depleted then the three cells that have to compensate for the missing cell will be at a much lower voltage and probably damaged. @Eboosted had several cells go all the way down to 0V a while ago because of the exact same issue and not using a BMS.
[/quote]

I never rode battery pack below 36.5V and so far charged batteries only 6 times. All cells seems to be okay.
New welding paid 10e with 10mm/0.2mm nickel strips from local battery store.

Problem with BMS is that massive size. I could use it as a deck :D
```

---
## \#28 Posted by: Norco Posted at: 2017-05-19T19:35:23.146Z Reads: 44

```
Quick question. I've just taken apart my 10s4p as I suspect one of the parallel packs has died. I haven't had chance to take them all apart but before I do, what would you suggest for next steps? I have 2 new batteries - I'm thinking of building a test rig and  marking them all up by capacity and IR then rebuild the battery. If 4 cells are a complete loss. Would you go 9s4p, 10s3p (current thought) or order another few batteries and rebuild as a 10s4p.
```

---
## \#29 Posted by: SirDiff Posted at: 2017-05-19T19:46:52.564Z Reads: 41

```
How would they have died?
```

---
## \#30 Posted by: Norco Posted at: 2017-05-19T22:57:59.566Z Reads: 37

```
I think 2 of the solder joints detached when I went over some rough ground and so the V on the other cells over discharged. Hot to touch when I got back :thumbsdown:
```

---
## \#31 Posted by: SirDiff Posted at: 2017-05-19T22:59:01.224Z Reads: 36

```
Were you using a bms?
```

---
## \#32 Posted by: Norco Posted at: 2017-05-20T11:10:51.745Z Reads: 32

```
No. Probably a lesson learnt there too.
```

---
