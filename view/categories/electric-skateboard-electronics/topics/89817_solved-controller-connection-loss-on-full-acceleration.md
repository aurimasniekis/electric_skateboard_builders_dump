# Solved! Controller connection loss on full acceleration

### Replies: 20 Views: 668

## \#1 Posted by: ElectricHabitatLeaf Posted at: 2019-04-08T16:32:29.788Z Reads: 135

```
I just built a board using the single motor esc substitute from eBay. 
I get an issue where the power cuts out when I'm accelerating. 
Then the controller stops responding as if it lost connection. 
Then I have to completely stop and wait like 3sec and the controller will reconnect and the board will go. 

Happens 10x per trip. Only under hard acceleration. 
Often times I'm accelerating up to 42km/h 26mph and its fine, no cutouts. But then I'll stop and as soon as I start going the thing cuts out just as soon as power kicks in. 

The power only cuts out when controller is in high mode. Medium mode is smoother acceleration and the power doesn't cut out. 

My setup: esc substitute. Same esc and controller as meepo boards. Allows up to 1350w power.
-6364 190kv motor 2000w
- 9s battery 5000mah 20c 

The esc has a receiver built into it, and the receiver has a long antenna. I had the antenna close to the esc before, but then moved it away from esc and motor but still the power cuts out. 

Anyone experience this? 

![IMAG0061|689x390](upload://5XSkSm25BT55mDOaXVZVDT1GCfl.jpeg)

****UPDATE**** Fixed lose Connection, and not cutting out anymore. Read below for details. 

I noticed burnt plastic insulation on one of the motor to esc wires. So it’s turned out to be a lose connection that sparked and burnt the insulation. I crimped it more thoroughly, and even soldered it. Will test it soon and see if it stops cutting out. It didn’t cut out when I first built this thing so the connection must’ve come lose over time. It also lost brakes when it would cut out, so that’s how I knew that it wasn’t hitting voltage cutoff, because low voltage cutoff lets you use brakes but not the throttle.

Pics of the lose connection : You can see the burnt insulation. That connection was lose as heck.

![IMAG0064.jpg](https://www.electric-skateboard.builders/uploads/db1493/original/3X/f/6/f6c54f3e5fb347ca593060b9042b1d746bbe253e.jpeg)

Don't mind the electrical tape hack job. I'm gonna replace that as time goes on, just a temp fix.
```

---
## \#2 Posted by: threebysix Posted at: 2019-04-08T16:35:26.978Z Reads: 123

```
What's your cut off voltage set at? Could be your cutoff voltage set too high and your voltage drops during hard accelerations
```

---
## \#3 Posted by: Sn4pz Posted at: 2019-04-08T16:35:59.631Z Reads: 118

```
Im no scientist but maybe your s9 battery isnt compatable with the meepo ESC, which runs 10s natively.

You could be dipping below the voltage cut off too, another likely option.

Other than that how are your connections?
```

---
## \#4 Posted by: ElectricHabitatLeaf Posted at: 2019-04-08T16:38:46.143Z Reads: 113

```
The voltage cut off is at 3v per cell. I'm running 9s, and the esc is made for 10s.
```

---
## \#5 Posted by: venom121212 Posted at: 2019-04-08T16:39:31.025Z Reads: 109

```
Probably hitting low voltage cutout on hard acceleration
```

---
## \#6 Posted by: ElectricHabitatLeaf Posted at: 2019-04-08T16:41:37.529Z Reads: 106

```
Yeah the esc is 10s version. With voltage cutoff at 3v per cell. But even fully charged my battery indicator shows 75% charged since I got 10s, and it still cuts out. 
And when the battery is almost dead the cutouts are less.
```

---
## \#7 Posted by: venom121212 Posted at: 2019-04-08T16:42:45.489Z Reads: 96

```
When you accelerate hard, your voltage drops rapidly before slowly going back up to regular voltage level (coasting)
```

---
## \#8 Posted by: Sn4pz Posted at: 2019-04-08T16:43:36.136Z Reads: 92

```
[quote="ElectricHabitatLeaf, post:6, topic:89817"]
75% charged since I got 10s, and it still cuts out. And when the battery is almost dead the cutouts are less.
[/quote]

This doesnt matter, Im assuming that because you didnt list another spec after your 9s battery, that the parallel count is 1. A 9s1p pack is going to sag like a titty if the cells are only rated for 20c :sweat:


imo, your options are: 

1: get a 10s battery

2: take one of the 3s lipos off and buy the 6s esc ( make sure you get the correct one, hub vs belt) and youll be all set

3: continue on as you are :joy:
```

---
## \#9 Posted by: ElectricHabitatLeaf Posted at: 2019-04-08T16:44:11.037Z Reads: 85

```
I guess that could be the case. I also fell hard going 40km/h and the controller took full force of my hand. It's got a nice scrape on it. I took it apart and it seems to be ok inside. 
Before that fall the board didn't cut out. But it also didn't start cutting out right after the fall. So I'm confused a bit.
```

---
## \#10 Posted by: Friskies Posted at: 2019-04-08T16:45:41.759Z Reads: 83

```
This sounds like an ESC DRV error more than a remote error. Sounds like the ESC is failing under load(High amps) and the board is probably restarting or something.
```

---
## \#11 Posted by: thisguyhere Posted at: 2019-04-08T16:45:48.374Z Reads: 84

```
in addition to voltage cutoff, power wires emit enough emf to interrupt radio signals.  

like...if your controller wire is crossing the main power leads, the emf coming off the power leads can cause enough interruption to mess up the controller connection.
```

---
## \#12 Posted by: ElectricHabitatLeaf Posted at: 2019-04-08T16:50:11.967Z Reads: 82

```
Yeah well I guess I can just ride it in medium mode for now. It still goes fast just the power doesn't kick in as rapidly. That's what's causing the cutout, the moment the power kicks in in high mode. 

Maybe a vesc is in order. This Chinese rec substitute is not even programmable.
```

---
## \#13 Posted by: ElectricHabitatLeaf Posted at: 2019-04-08T16:53:37.116Z Reads: 80

```
I moved the antenna away from the power leads. Still same thing.
Here's the ghetto setup pic:

 ![15547423235051346026345|282x500](upload://4CCH1rjGtDPg3ucJTxAYycraCPm.jpeg)
```

---
## \#14 Posted by: ElectricHabitatLeaf Posted at: 2019-04-08T16:56:30.472Z Reads: 78

```
I was considering that too because the motor is rated 2000w and battery can deliver 1850w. But the esc has a max of 1350w. 
Also maybe the esc max amperage is lower than the battery? But how is that possible if the rec is  made for 10s battery and I have a 9s.
```

---
## \#15 Posted by: banjaxxed Posted at: 2019-04-09T02:38:23.045Z Reads: 70

```
Checked that the capacitors are not loose?
```

---
## \#16 Posted by: M.Hboards Posted at: 2019-04-09T03:10:14.780Z Reads: 71

```
Check if the breaks still work when the powercuts out as you are prob hitting the low voltage cut of of the esc due to you useing a 9s battery. these esc's leave the breaking even when it cuts acceleration due to hitting the cutoff. if the breaks are still there get a 10s battery and it should be be good to go if not you have some other problem.
```

---
## \#17 Posted by: Friskies Posted at: 2019-04-09T04:33:35.831Z Reads: 62

```
Oh you also have a9s battery with a 10s controller. If you pack sags under load it will cause a cutout too :(
```

---
## \#18 Posted by: ElectricHabitatLeaf Posted at: 2019-04-10T01:04:27.546Z Reads: 54

```
Update: 
I noticed burnt plastic insulation on one of the motor to esc wires. 
So it's turned out to be a lose connection that sparked and burnt the insulation. 
I crimped it more thoroughly, and even soldered it. 
Will test it soon and see if it stops cutting out. 
It didn't cut out when I first built this thing so the connection must've come lose over time. 
It also lost brakes when it would cut out, so that's how I knew that it wasn't hitting voltage cutoff, because low voltage cutoff lets you use brakes but not the throttle.

Pics of the lose connection : 
You can see the burnt insulation. That connection was lose as heck. 

![IMAG0064|689x390](upload://zd2bS3xqCuvX937ADmXcaojiJXw.jpeg)
```

---
## \#19 Posted by: mynamesmatt Posted at: 2019-04-12T04:36:47.509Z Reads: 45

```
i rekon its hitting cutoff like the others are saying.
if it's in the high mode like you said, it'll draw more current, and make the battery sag more. At 10s, the cutoff voltage is most probably 32v ish.
![Screenshot_20190412-143515_Calculator|414x493](upload://gjSIx9lUgkywsLUkxrhKm5u52pd.jpeg)
so once your 9s battery hits about 3.6-3.7v per cell, the esc thinks its a 10s battery with low voltage. A relatively full (75% like you said) battery may sag to this point easily
```

---
## \#21 Posted by: ElectricHabitatLeaf Posted at: 2019-04-13T01:27:09.707Z Reads: 31

```
Read the Update. it's not voltage sag. I fixed the connection from esc to motor. there was a lose connection. now it's not cutting out anymore.
```

---
