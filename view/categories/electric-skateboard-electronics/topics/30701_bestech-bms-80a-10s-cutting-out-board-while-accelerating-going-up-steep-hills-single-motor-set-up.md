# Bestech BMS 80A 10s cutting out board while accelerating/going up steep hills - single motor set up

### Replies: 58 Views: 3139

## \#1 Posted by: MontPierre Posted at: 2017-08-15T11:25:48.195Z Reads: 236

```
Hi,

I have just wired up my Bestech BMS 10s 80A. Board is running fine but when I accelerate from stop giving full throttle/accelerating up steep hill it cuts off whole board and I have to switch it off ( using built in BMS switch ) and switch it on again to resume riding. As it is 80A I'm surprised it cuts me off. I'm sure I'm not pulling 80A.

Here are my specs:

10S 8ah batteries in series ( Zippy Flightmax 30C - 40C Burst - all the same.)
SK3 6374 192 KV motor ( 80A)
FocBox
15mm belts

Cutting out happens while I have 38V or 42V ( fully charged) so it can't be over voltage protection ( I have 57V set up in BLDC). Running BLDC mode. I have done motor detection. Do I have to redo it when unplugging phase wires? 

Since I have two same BMSs( minimum order two) I have tried both thinking one can be faulty. Unfortunately it is the same behaviour on both.

I'm sure it has nothing to do with FocBox. I can't even read any fault codes as BMS cuts off power and faults are erased. I did check on bench motor with live sampling and with no load I'm pulling 3-5A. 

All connections ( phase wires, battery wires, etc)  are shrink wrapped and taped with electrical tape to avoid any possible shorts. 

Using @Ackmaniac software - moderate settings- here are screenshots. 

<img src="/uploads/db1493/original/3X/7/8/78a609b0aff3d50ad8ccb9bfd99ec63fd86efaee.png" width="690" height="391"><img src="/uploads/db1493/original/3X/b/d/bdde7d0191059737d663f8739add7ca2c1a0685e.png" width="690" height="382"><img src="/uploads/db1493/original/3X/b/9/b99784e4a2e666ab10882adc54cb162e7279d78d.png" width="690" height="386"><img src="/uploads/db1493/original/3X/5/a/5a34250362140c22c26d70c0c35813b9efc570ea.png" width="690" height="390"><img src="/uploads/db1493/original/3X/2/3/23c310fd745f7f973c92b722e41694bf9a6feb73.png" width="690" height="385">

Bestech specs

<img src="/uploads/db1493/original/3X/c/2/c2a3e17b68bbda5c0156d7fb727fff6f2715de3a.png" width="348" height="500">


Any idea on what can cause the cut off? Fuse on BMS is rated for 90 Celsius rather than Amperage but don't quote me on that.

@Namasaki have you had similar problems?
```

---
## \#2 Posted by: darkkevind Posted at: 2017-08-15T12:30:02.505Z Reads: 205

```
I'm sorry I can't shed any light on your particular problem, although it sounds very similar to my issue I'm having occasionally...

When I'm full throttle going up some kind of incline, my power will suddenly cut, throwing me forwards if I don't catch it in time...

I believe the VESC is cutting out though as when it happens I have no control, then a few seconds later I have control again so I think it's the VESC re-booting.

This also happens full brake going down hill sometimes... which is a little unnerving! :confused:
```

---
## \#3 Posted by: MontPierre Posted at: 2017-08-15T12:37:32.305Z Reads: 198

```
I completely loose all the power and have to reset switch and it all works fine afterwards. Maybe if I will wire BMS with bypass on discharge and test it again and it then cuts me out I will know it is Vesc. 

Actually before I had BMS wired up I was riding on same setup, same settings, same hills and never had any problems, no cut offs - it must be BMS since it all started happening as soon as I wired it in. Strage :confused:
```

---
## \#4 Posted by: Namasaki Posted at: 2017-08-15T12:56:41.818Z Reads: 190

```
I have not had this issue even when accelerating up steep hills. 
I believe the problem your having is due to abnormal voltage sag in one of your battery cells. If any cell drops to 3,0v the bms will shut down. One cell going too low likely won't trip the Vesc protection. 
I suggest not bypassing the bms. 
I suggest testing your batteries for internal resistance. 
I suspect at least one of your 10 cells will show high internal resistance. 
Replace the pack with the bad cell and your problem should be solved. 
One time I ordered 4 Zippy batteries and tested them and found 2 packs with bad cells right out of the box.

Up to 5 milliohms internal resistance is acceptable 
If any cell is showing 10+ milliohms I would replace that pack.
```

---
## \#5 Posted by: MontPierre Posted at: 2017-08-15T12:58:24.257Z Reads: 184

```
Thanks @Namasaki - what resistance should make me worry ? I'll connect them to balance charger and check all the values now.
```

---
## \#6 Posted by: Namasaki Posted at: 2017-08-15T12:59:40.559Z Reads: 176

```
I just added that info with edit
```

---
## \#7 Posted by: MontPierre Posted at: 2017-08-15T13:24:57.966Z Reads: 183

```
@Namasaki Thanks! I just took pictures and here they are. I know they are not balanced - I have tried with Bestech BMS but my charger just stopped feeding any current at 42V so for the moment I will be balancing them on Turingy balance charger separately. 

<img src="/uploads/db1493/original/3X/9/9/99568575d437a15126d7b939e62aba5d1fb59cac.jpg" width="690" height="496">
```

---
## \#8 Posted by: MontPierre Posted at: 2017-08-15T13:34:18.374Z Reads: 176

```
Everything is wired as per your diagram using 12 AWG wires to BMS and VESC ( apart of charge port - 22 AWG wires) 

http://www.electric-skateboard.builders/t/connecting-a-bms-quick-guide-how-to/6122/59?u=montpierre
```

---
## \#9 Posted by: Namasaki Posted at: 2017-08-15T14:11:50.006Z Reads: 172

```
Internal resistance although poorly matched is within acceptable limits. 
Still, voltage sag is the only suspect that I can think of. 
Do you have some way of monitoring voltage while riding?
```

---
## \#10 Posted by: MontPierre Posted at: 2017-08-15T14:14:28.312Z Reads: 169

```
@Namasaki Yeah, I have voltage meter attached. What should I look for? Voltage drops a little depending on how I accelerate but only around  0.1 0.2 of voltage before acceleration. It also rises then breaking - regen.
```

---
## \#11 Posted by: MontPierre Posted at: 2017-08-15T14:56:24.080Z Reads: 160

```
I'm on the board now and up a steep hill, slow acceleration I had a drop of voltage from 41.7V to 4.12V. I think that's normal right ? If it was much lower than this then I would be worried ...
```

---
## \#12 Posted by: Namasaki Posted at: 2017-08-15T15:35:16.022Z Reads: 154

```
Do the full throttle thing that makes the bms shut off and see what the voltage drop is. 
I think it's likely that cells with 5 milliohms are sagging more than the rest.

So you have 2 3s/8000/30c packs and
2 2s/8000/30c packs all in series?
```

---
## \#13 Posted by: Namasaki Posted at: 2017-08-15T15:48:00.835Z Reads: 148

```
[quote="MontPierre, post:11, topic:30701, full:true"]
I'm on the board now and up a steep hill, slow acceleration I had a drop of voltage from 41.7V to 4.12V. I think that's normal right ? If it was much lower than this then I would be worried ...
[/quote]
1/2 volt drop from total pack voltage is pretty mild sag.
```

---
## \#14 Posted by: MontPierre Posted at: 2017-08-15T15:48:40.836Z Reads: 147

```
Yes, to make 10s. 5s packs were to thick for my enclosure. 

Funny enough I can't replicate this cut off now. I will try later on when board "rests" for a bit :) From what I have seen before, voltage would drop half a volt and then BMS would cut off. It did not sag more than this.

How can I reduce sag? 12S? Add one more battery?
```

---
## \#15 Posted by: Namasaki Posted at: 2017-08-15T15:56:39.088Z Reads: 140

```
Maybe sag is not the issue here. 
Maybe you have a loose connection or faulty solder joint that causes intermittent lose of connection and throws the bms into protection mode. 
This happened to me once when the last pack in my setup developed an interment disconnect where the main positive wire connects to the solder tab inside the pack. I was cruising along and the bms shut down. When I got home a took a closer look I found that if I moved the wire around it would connect and disconnect randomly.
```

---
## \#16 Posted by: Silverline Posted at: 2017-08-15T15:57:43.578Z Reads: 140

```
I think it's because that your cells gets out of ballance to each other, because you are using two different batteries. With most likely different C ratings.
```

---
## \#17 Posted by: MontPierre Posted at: 2017-08-15T16:01:15.284Z Reads: 138

```
Well I don't think having different cells matters. All are the same brand, same C rating and capacity. Only difference is S count.  Also I'm positive it does not make them discharge unevenly. Even when you have same batteries in series they will discharge/charge unevenly to a degree.
```

---
## \#18 Posted by: MontPierre Posted at: 2017-08-15T16:01:47.682Z Reads: 137

```
I'll check wiring. Maybe thats the cause.
```

---
## \#19 Posted by: Silverline Posted at: 2017-08-15T16:02:27.137Z Reads: 136

```
But something is triggering the BMS
```

---
## \#20 Posted by: jmasta Posted at: 2017-08-15T17:09:54.834Z Reads: 156

```
[quote="Namasaki, post:4, topic:30701, full:true"]
I have not had this issue even when accelerating up steep hills. 
I believe the problem your having is due to abnormal voltage sag in one of your battery cells. If any cell drops to 3,0v the bms will shut down. One cell going too low likely won't trip the Vesc protection. 
I suggest not bypassing the bms. 
I suggest testing your batteries for internal resistance. 
I suspect at least one of your 10 cells will show high internal resistance. 
Replace the pack with the bad cell and your problem should be solved. 
One time I ordered 4 Zippy batteries and tested them and found 2 packs with bad cells right out of the box.

[/quote]


@Namasaki nailed it!

My board is now doing the same exact thing, with Zippy Compact 40C 6.2Ah batteries.  My pack is perfectly balanced at resting voltage, but under load, some of the cells rapidly drop to unsafe levels triggering the BMS cutoff.  I don't have my log book right now, but now 3 of the cells will drop from 3.85V resting to 3.2V with just 1A direct loading;  while the others might only drop to 3.7V under the same exact loading.  So under higher load, I am definitely hitting the 2.9V BMS cutoff with at least one cell

 Took me some time to diagnose the problem; however, I built a device to measure individual cell voltage with a constant load.  It has a calibrated voltage meter and can select 0A, 1A, or 2A loading.  What I learned from all this is even if your pack is "balanced" while resting, it could still be very unbalanced under load

TLDR -  Don't bypass your BMS. Especially with lipos!  I would have been unknowingly wrecking havoc on my batteries
```

---
## \#21 Posted by: psychotiller Posted at: 2017-08-15T17:32:03.601Z Reads: 142

```
I have one that does the same thing...Hoping to confirm it is cutting off lower than 80a because it will be going back to bestech for replacement.
```

---
## \#22 Posted by: MontPierre Posted at: 2017-08-15T17:38:11.556Z Reads: 141

```
I'm getting metr.at bluetooth which will allow me to log my data. Hope this will help me in troubleshooting.
```

---
## \#23 Posted by: psychotiller Posted at: 2017-08-15T17:41:12.571Z Reads: 140

```
Let me know!!!
```

---
## \#24 Posted by: SilentException Posted at: 2017-08-15T17:50:59.328Z Reads: 141

```
Whenever I want to know what the cells are doing I connect a parallel balance lead and [this guy](https://www.banggood.com/ISDT-BC-8S-Battery-Checker-with-Two-85dB-Buzzer-for-LiPo-LiHv-LiFe-LiIon-Batteries-p-1128253.html). It has a neat functionality of showing cell lowest voltage so you can see the lowest sag with ease.
```

---
## \#25 Posted by: MontPierre Posted at: 2017-08-15T18:09:39.439Z Reads: 139

```
That's a great find! Shame they don't do 10s variations. I guess I can use this on 10s, monitor 8cells and then other two on separate ride. Do I need parallel balance lead with this checker? I guess regular balance lead - male to female  extension would be ok?
```

---
## \#26 Posted by: SilentException Posted at: 2017-08-15T19:17:49.214Z Reads: 132

```
I guess your balance leads are connected to BMS? If yes, you will need parallel adapter first (one goes in BMS, one in meter). If not, you just connect balance plug to the meter. 

I your specific scenario you will probably need to make adapter 10s -> 5s, twice. First one for first 5 cells, second one for other 5 cells.
```

---
## \#27 Posted by: jmasta Posted at: 2017-08-15T22:17:58.115Z Reads: 127

```
[quote="MontPierre, post:22, topic:30701, full:true"]
I'm getting metr.at bluetooth which will allow me to log my data. Hope this will help me in troubleshooting.
[/quote]

I have Metr, and it's useful for diagnosing VESC faults.  But there is no real way to distinguish between a BMS cutoff and say a remote dropout.  I thought my GT2B was cutting out before I built the battery tester/discharger

I hate to say it, but I can almost guarantee it is your 30C lipo batteries.  I am in the same boat.... It only gets worse from here.   I was flying up hills for months, and now even a small incline can trigger the BMS cutoff if my battery is below 75%.  My board is crippled until I either buy new Lipos to replace the bad ones, or build a li-ion pack
```

---
## \#28 Posted by: MontPierre Posted at: 2017-08-15T22:30:10.501Z Reads: 125

```
Well it cant be remote as whole board switches off. Might be lipos but they are new and I only have done around 10 miles on the board so far. Well on my second ride today I didn't have any cut offs and I did try hard to replicate the problem - went full throttle on same road as before, same inclines. Might have been loose wire or so, I have opened her up and connected everything one again, not sure what was the issue.  In couple of days I'll do some more testing, I might get the cell checker - looks cool.
```

---
## \#29 Posted by: MontPierre Posted at: 2017-08-15T22:31:19.064Z Reads: 120

```
Btw- I thought Lipos have a lot less sag than li-ons.
```

---
## \#30 Posted by: Lionpuncher Posted at: 2017-09-26T14:51:17.072Z Reads: 115

```
So i had this problem yesterday while on a nice little rip. Build is still relatively new. First cut off was up an incline, had to more on flats? Battery (10s) was at approx 35.5 v. I have a Bluetooth mod and ackmaniacs app. Every cutoff would say under voltage fault. From what I'm gathering here that means i could have a faulty cell?
Edit: I have a bestech 10s Bms. On a tesla 10s4p battery. I know the batteries are fairly low discharge (10 a constant, 20 for 45 second bursts)  but i haven't really experienced much sag. Defo not enough to trigger a cut out at like 36 v...
```

---
## \#31 Posted by: Jinra Posted at: 2017-09-26T14:51:55.319Z Reads: 109

```
what's your minimum input voltage set to
```

---
## \#32 Posted by: Lionpuncher Posted at: 2017-09-26T14:55:33.590Z Reads: 109

```
 for the vesc? I still have to get into the tool and look, but i doubt i set the cutoff at anything above 31 v.
```

---
## \#33 Posted by: Jinra Posted at: 2017-09-26T15:02:26.971Z Reads: 106

```
Not cutoff, minimum input voltage. If you didn't change it, it should be 8v
```

---
## \#34 Posted by: Lionpuncher Posted at: 2017-09-26T15:05:37.796Z Reads: 103

```
 I'll look. At work right now. Try and do at lunch. If not later tonight.
```

---
## \#35 Posted by: Lionpuncher Posted at: 2017-09-26T15:41:07.146Z Reads: 104

```
Other thoughts that are starting to occur to me. Put the battery on charge last night. Selected 100% at 1A. Overnight it should have got to 100 %. Take it off the charger and it's at 38V. That's starting to point at me having lost a cell here isn't it?
```

---
## \#36 Posted by: Jinra Posted at: 2017-09-26T16:12:37.970Z Reads: 105

```
you gotta measure every parallel group to see what voltage they're all at
```

---
## \#37 Posted by: Lionpuncher Posted at: 2017-09-26T16:45:32.680Z Reads: 109

```
Ok. Stupid curiosity.... should be working and here i am ripping apart my board haha. :cold_sweat:
<img src="/uploads/db1493/original/3X/7/f/7faef8196bd0cbc4c853eaae4aec4e5e8fe69f3e.jpg" width="281" height="500">

1. 3.59v      7. 3.59
2. 3.68.       8. 3.67
3. 3.62.       9. 3.67
4. 3.65.     10. 3.67
5. 3.67
6. 3.67

Not sure what the tolerance is but doesn't look terrible to me...
```

---
## \#38 Posted by: Jinra Posted at: 2017-09-26T16:48:56.633Z Reads: 107

```
not terrible but also not balanced, my deviation is normally within .02v
```

---
## \#39 Posted by: Lionpuncher Posted at: 2017-09-26T17:01:27.322Z Reads: 106

```
 like would you say the bms isn't working?
```

---
## \#40 Posted by: Jinra Posted at: 2017-09-26T17:02:35.928Z Reads: 111

```
Could be, or a parallel group isn't fully connected. Try measuring each cell of the outlier groups (1st 3rd and 7th) and make sure you probe as close to the cell surface as you can.
```

---
## \#41 Posted by: Silverline Posted at: 2017-09-26T17:13:04.047Z Reads: 107

```
If one of the cells is missing, the bestech wont turn on. 
But maybe something happen to one of the cells under load, when you ride.
```

---
## \#42 Posted by: Jinra Posted at: 2017-09-26T17:16:15.844Z Reads: 104

```
What are your current limits at. If you're drawing too much for the cells you could be experiencing insane voltage sag
```

---
## \#43 Posted by: Lionpuncher Posted at: 2017-09-26T17:44:22.540Z Reads: 102

```
 Ill report back once home...
Really appreciate the help here guys. 
If the balance connectors weren't on well, the bms won't turn on, but wouldn't that mean my entire system won't turn on?
```

---
## \#44 Posted by: Lionpuncher Posted at: 2017-10-03T02:37:38.745Z Reads: 98

```
Sorry to disappear like that. Family stuff blah blah lol.
So I removed the BMS and charged my pack to 90%. It sort of charged more than that and the first group of cells were at 4.31 V. My battery guy us replacing the first group right now. I'm getting it back tomorrow. Would I be able to hook my 42 v battery charger to my vesc and use as a power source to look at my settings or is that a bad idea? @Jinra
```

---
## \#45 Posted by: Lionpuncher Posted at: 2017-10-03T02:38:40.823Z Reads: 92

```
Also, does the Regen setting affect how much it well the board brakes?
```

---
## \#46 Posted by: Lionpuncher Posted at: 2017-10-04T04:37:49.707Z Reads: 93

```
@Jinra, got my battery back, all is hooked up minus BMS. Gonna test tomorrow. Here's my VESC setup:

<img src="/uploads/db1493/original/3X/d/4/d47050aac4b1c6736f3e8ed57415af64514d1b17.PNG" width="690" height="350">
<img src="/uploads/db1493/original/3X/2/6/26f8c0ff7d2e86169015032030df18fe4d87c743.PNG" width="690" height="355">
<img src="/uploads/db1493/original/3X/b/3/b37c6f1bd0c5c6f105fb880ddbfeee9d765df5c5.PNG" width="690" height="352">
Any help and insight will be greatly appreciated.
```

---
## \#47 Posted by: Jinra Posted at: 2017-10-04T05:27:32.929Z Reads: 85

```
Be careful overcharging cells like that. Li-ion is a sensitive chemistry that does not like to be overcharged and it can damage the cell and shorten it's cycle life.

[quote="Lionpuncher, post:45, topic:30701, full:true"]
Also, does the Regen setting affect how much it well the board brakes?
[/quote]

Battery regen affects the high speed braking response, motor min affects low to mid-high braking. If those settings are for a single VESC you can go up to +4A per parallel cell, though with how regen works you can afford to go a bit higher as well for better braking.
```

---
## \#48 Posted by: Lionpuncher Posted at: 2017-10-04T14:33:01.813Z Reads: 79

```
Ok. So you figure the battery min is probably ok, but I'm overcharging? By that do you mean battery max and motor min/max? I'm pretty sure that's what happened. Screwed up a group of cells from over taxing. Would definitely like to avoid this happening. What parameters would you input?
Thanks
```

---
## \#49 Posted by: Jinra Posted at: 2017-10-04T14:35:29.331Z Reads: 79

```
you're settings are okay from what i see. You'll need the bms to prevent overcharging on your parallel groups.
```

---
## \#50 Posted by: Lionpuncher Posted at: 2017-10-04T15:03:10.709Z Reads: 79

```
When you're speaking of overcharging, are you referring to when I'm riding and using the brakes? Or when I'm actually charging the battery? I have a smart charger. I can select 80, 90, and 100% charge. And it's voltage is specific for 10s Li ion. Don't get me wrong, I plan on having a BMS one way or another, not sure if my bestech is toast or not. Have another coming. But I'm not certain where it really comes in handy still...
```

---
## \#51 Posted by: Jinra Posted at: 2017-10-04T15:04:09.113Z Reads: 76

```
When you're charging the battery. You mentioned that one group was at 4.31v which is very bad for the cell. You'll like never overcharge from regen as the energy you get back is minimal.
```

---
## \#52 Posted by: Lionpuncher Posted at: 2017-10-04T15:48:06.313Z Reads: 74

```
True. So strange it did that. To me, that seemed to be more to do with the cells in that group being bad. But I just don't know enough yet about battery charging and BMS circuitry to be sure. 
Thanks for your help man. 
Appreciated.
```

---
## \#53 Posted by: Jinra Posted at: 2017-10-04T15:48:39.133Z Reads: 72

```
If you had a BMS attached it would've stopped that parallel group from going over 4.2~v
```

---
## \#54 Posted by: Lionpuncher Posted at: 2017-10-04T15:50:12.012Z Reads: 74

```
But how come just the one bank? All others where at 3.9 V? That said, it is the pack that that the main negative lead comes off of.
```

---
## \#55 Posted by: Jinra Posted at: 2017-10-04T15:53:03.260Z Reads: 76

```
it could be that a cell in the paralllel group became detached meaning that group is charging faster than the others due to less mAh.
```

---
## \#56 Posted by: Lionpuncher Posted at: 2017-10-04T16:05:37.951Z Reads: 75

```
Very possible. Looks like 3 of the batteries started venting at some point. Still leaves me wondering what's going on? I'll have it all back together to test ride tonight. If that hitchy feeling is gone then I'll have to assume my BMS was screwed up? No point in drawing conclusions until I've given her a bit of a test drive.
```

---
## \#57 Posted by: JuanMontero Posted at: 2019-06-10T07:40:02.284Z Reads: 22

```
Did you finally diagnose the problem? I’m having the same issues! Is it a faulty bms? Or a problem with some of the batteries? Thank you
```

---
## \#58 Posted by: Lionpuncher Posted at: 2019-06-10T16:37:48.283Z Reads: 19

```
Damn dude, that was a while ago!
From what I remember, that batt caused a few problems initially. Had the battery repaired (bad cell in first p group), but didn’t bother with the bms for a while. That worked great but obviously not safe. Next season used a different bms and had no further issues. So it could be a battery issue (most likely) or a bricked bms. How long you been using it for? Who built it?
```

---
