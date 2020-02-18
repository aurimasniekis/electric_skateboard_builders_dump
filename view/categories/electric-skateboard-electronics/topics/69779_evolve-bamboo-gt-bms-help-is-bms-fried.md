# Evolve Bamboo GT BMS help (is BMS fried?)

### Replies: 30 Views: 794

## \#1 Posted by: Steven1 Posted at: 2018-10-01T20:41:59.461Z Reads: 114

```
After browsing through previous Evolve GT battery upgrades on this forum I tried doing it myself. Everything was going smoothly until I hooked up my balance wires to the BMS and the BMS started getting too hot to touch. When I noticed this I immediately disconnected the BMS but now Im unsure whether it's fried or could still function. I redid the wiring and checked the voltages on the balance leads and they seem to be in order but the same problem persists when I connect the balance plug - the BMS gets hot. Any troubleshooting suggestions? 

![MVIMG_20180930_194654|374x500](upload://wzhEEJb2eAyzVvmxT1yjxLnF8IT.jpeg) 



![MVIMG_20181001_203429|374x500]


![IMG_20181001_215311|375x500](upload://A6dcyxszjnDpjh43vU4ZQdcy5Zw.jpeg) (upload://x886j4TKwbHbPXM05aPPmycxo7M.jpeg)
```

---
## \#2 Posted by: mccloed Posted at: 2018-10-01T21:52:29.601Z Reads: 103

```
It could be that your cells are out of balance and its balancing them. That would get the mosfets warm or hot. Maybe @psychotiller could shed some light?
```

---
## \#3 Posted by: Steven1 Posted at: 2018-10-01T22:12:40.133Z Reads: 101

```
Thanks for the reply, I hope that's the case. Thing is, the board won't turn on either, so I'm guessing I still did something wrong. I'm pretty sure the balance leads are ok now since I double checked they were hooked up correctly (going from B0 to B10 starting from left to right seen from BMS viewpoint) and had the right voltages. 

The BMS weirdly only gets hot on the right side though where you see the cylindrical thing with the volt measure on it (yeah i'm new :P), you can see the orange "glue" being burnt there as well. I'm guessing if it was a BMS balance plug problem, then the heat would be concentrated there instead.
```

---
## \#4 Posted by: Steven1 Posted at: 2018-10-01T22:45:01.539Z Reads: 103

```
 I checked again and the BMS also gets hot when the positive discharge cable is connected so I'm guessing it's just normal and I was overly cautious. Unfortunately, I still can't get the board to turn on. Here is another pic. Anyone tell me where I might have gone wrong? 

![IMG_20181002_002540|666x500](upload://q1aJEt2WSji6ga3YDn5lVNdKpyz.jpeg) ![IMG_20181002_002628|666x500](upload://ahFqg3cMPcVYxdbWAtvTxGUUm3z.jpeg) ![IMG_20181002_003039|666x500](upload://kMpNjdC42eIybS8nciRlP0T3eBy.jpeg) ![IMG_20181002_003028|666x500](upload://nEPn2TTPDtC73pCUkfGSquGCIxU.jpeg)
```

---
## \#5 Posted by: psychotiller Posted at: 2018-10-01T23:10:37.331Z Reads: 95

```
If the bms is getting too hot to touch,  there's definitely a big chance your cells are different voltages. Did you check all of them before you welded them together to make sure they were the same? 

Also I'd triple check that your balance wires are in proper order.
```

---
## \#6 Posted by: Steven1 Posted at: 2018-10-01T23:37:16.697Z Reads: 91

```
I checked the cells before welding they were all 3.4x. I'll check the balance leads tomorrow again as well. Hope I get this thing to work :)
```

---
## \#7 Posted by: b264 Posted at: 2018-10-01T23:47:23.352Z Reads: 91

```
[quote="psychotiller, post:5, topic:69779"]
Also I’d triple check that your balance wires are in proper order.
[/quote]

&lrm;&lrm;This
```

---
## \#8 Posted by: psychotiller Posted at: 2018-10-02T01:10:00.538Z Reads: 90

```
Can you confirm that the 1st wire on your balance lead (The wire before number 1) is going to your number one group? should basically be connected to your neg terminal.
```

---
## \#9 Posted by: Steven1 Posted at: 2018-10-02T06:59:27.480Z Reads: 79

```
Yep, the BO wire is basically soldered right on the bigger B- wire on the negative terminal of group 1. Thanks for the suggestions, I'm checking everything again after work.
```

---
## \#10 Posted by: Steven1 Posted at: 2018-10-02T21:58:22.316Z Reads: 74

```
So I checked the bms wiring and one wire as loose and I replaced it. Unfortunately, the BMS still gets hot afterwards, so Im just gonna redo all the wiring in the weekend, no rush. Thanks for the advice!
```

---
## \#11 Posted by: dg798 Posted at: 2018-10-03T02:47:43.483Z Reads: 68

```
Make sure all the balance wires are in order and when you are done soldering then check the voltages from the balance lead cable itself just in case.
```

---
## \#12 Posted by: psychotiller Posted at: 2018-10-03T02:51:23.463Z Reads: 66

```
If all of those wire turn out to be in order, My on;y other sugestion is shorten all of the wires. They seem really long.
```

---
## \#13 Posted by: dg798 Posted at: 2018-10-03T02:54:28.149Z Reads: 60

```
Also make sure that if ur balance wires have an extra wire attach it to ground.
```

---
## \#14 Posted by: Steven1 Posted at: 2018-10-08T20:13:59.210Z Reads: 56

```
Can you elaborate, I'm not sure what you mean.

So I checked the balance leads and they read fine, thing is when I check the voltage at the
bms 11 pin plug, I can't get a clear reading half the time. Urgh gotta say the start was fun but this last part of building a battery is an exercise in frustration
```

---
## \#15 Posted by: dg798 Posted at: 2018-10-08T22:38:03.350Z Reads: 54

```
Is the 11 pin 0v
```

---
## \#16 Posted by: Steven1 Posted at: 2018-10-10T10:19:08.102Z Reads: 54

```
I redid the balance wiring yesterday. New wires and soldering. Before that I checked all the battery group voltages - they are all 3.45 or 3.46. After soldering the balance wires to the groups, I checked the balance leads to make sure that each balance lead was 3.4x  higher than the balance lead of the previous group. Then I attached the balance wires to the plug and measured the voltages inside the plug - all good. Except when I insert the plug in the BMS it immediately starts getting hot again. Will upload new pics tonight. Hope to get this sorted.
```

---
## \#17 Posted by: Steven1 Posted at: 2018-10-10T16:17:41.558Z Reads: 52

```
@darkkevind I know you did tons of these upgrades, do you see anything wrong in the pics? Or have any suggestions to get it working. Any help is much appreciated. 
 ![IMG_20181010_181357|666x500](upload://tvknuzr72hw2eckdgkawGUysuNg.jpeg) ![IMG_20181010_181329|666x500](upload://C5Yvor21cwAPfNXmO9y3F4ARaN.jpeg) ![IMG_20181010_181315|666x500](upload://gVcoG9sbvYTpPFIFuxcoCVbLEKE.jpeg) ![IMG_20181010_181412|375x500](upload://ff8jeB5zNqEMH7Lkl9NWPrPQ0if.jpeg)
```

---
## \#18 Posted by: Fiori Posted at: 2018-10-10T16:41:12.133Z Reads: 49

```
Sounds like one of your balance wires is in the wrong spot. I forget how the balance order goes on these, but I think the right most wire on the balance connector is the negative, and it goes 0-10s starting with that lead. Let us know the voltage of each wire on the balance connector.
```

---
## \#19 Posted by: Steven1 Posted at: 2018-10-10T19:14:19.166Z Reads: 53

```
I tested the wires, from left to right it's B0-0v, B1-3.43, B2-6.86, B3-10.31, B4-13.75, B5-17.2, B6-20.6, B7-24, B8-27.5, B9-31, B10-34.3 red wire is B10
![IMG_20181010_210334|375x500](upload://s7Ojrv4hWzpTNGQIJXpOfkNLg7R.jpeg)
```

---
## \#20 Posted by: b264 Posted at: 2018-10-10T19:30:30.618Z Reads: 51

```
[quote="Steven1, post:16, topic:69779, full:true"]
I redid the balance wiring yesterday. New wires and soldering. Before that I checked all the battery group voltages - they are all 3.45 or 3.46. After soldering the balance wires to the groups, I checked the balance leads to make sure that each balance lead was 3.4x higher than the balance lead of the previous group. Then I attached the balance wires to the plug and measured the voltages inside the plug - all good. Except when I insert the plug in the BMS it immediately starts getting hot again. Will upload new pics tonight. Hope to get this sorted.
[/quote]

[quote="Steven1, post:19, topic:69779"]
I tested the wires, from left to right it’s B0-0v, B1-3.43, B2-6.86, B3-10.31, B4-13.75, B5-17.2, B6-20.6, B7-24, B8-27.5, B9-31, B10-34.3 red wire is B10
[/quote]

This isn't looking good.

Also you should manually charge that a little bit (connect charger to B0 and B10 while monitoring) so they're around 3.65V each.  That's a bit low for comfort.  If it sits around too long, it will creep down as well.
```

---
## \#21 Posted by: Steven1 Posted at: 2018-10-10T20:53:05.104Z Reads: 45

```
I only have the evolve charger do I need to buy extra tools to charge manually and monitor or do I just bypass BMS and monitor voltage every once in a while with voltmeter?
```

---
## \#22 Posted by: b264 Posted at: 2018-10-10T22:07:36.437Z Reads: 44

```
Yes just charge B0 and B10 and monitor the whole time.  Storage charge on li-ion is about 3.6V to 3.7V --  3.45V is basically dead.  It's not super-important though.  Just don't let it get lower.
```

---
## \#23 Posted by: Steven1 Posted at: 2018-10-12T07:55:28.229Z Reads: 44

```
Thanks for all the help and suggestions. I charged the battery, bypassing the bms, to 3.63. I hoped this might fix the issues but unfortunately when connecting the plug to the VESC or when connecting the balance cable plug, the BMS still gets way too hot. I dont think it's a balance cable issue because the pic below shows in green that the balance resistors are fine but the red-marked area is burned. Anyone know why this might be?

![IMG_20181012_084457%20II|375x500](upload://b3siWioeZDOvrc9KkpvaT4QTuHS.jpeg) 
![MVIMG_20181012_084508|666x500](upload://cz5cNByNxNBIDShTJY5AmvfR4mQ.jpeg)
```

---
## \#24 Posted by: b264 Posted at: 2018-10-12T08:37:10.160Z Reads: 43

```
It's a capacitor, but do you have a higher-resolution photo?
```

---
## \#25 Posted by: Steven1 Posted at: 2018-10-12T08:39:35.490Z Reads: 44

```
I'll take one as soon as I get home from work.
```

---
## \#26 Posted by: Steven1 Posted at: 2018-10-12T15:03:58.895Z Reads: 44

```
New foto's incoming.
![IMG_20181012_165913|666x500](upload://kTZh2NH4OVK6wr8dpBlxwrrJFGg.jpeg) ![MVIMG_20181012_170000_1|666x500](upload://6KYQYlTmRiiqYZZMndnlXHfQ5x2.jpeg) ![MVIMG_20181012_170000|666x500](upload://dBxWjgf4wdSH2e855vtk3ZDVbUo.jpeg) ![MVIMG_20181012_165952|374x500](upload://lzMBozIT1aIHpKMI1WIteVAdQg4.jpeg)
```

---
## \#27 Posted by: b264 Posted at: 2018-10-12T18:47:32.561Z Reads: 45

```
That capacitor's insides have blown out.  Remove it and replace it with another 100V electrolytic capacitor, 4.7μF
```

---
## \#28 Posted by: Goonman Posted at: 2018-11-04T06:58:07.132Z Reads: 40

```
Did you ever get the bottom of this?
 I put a pack together using Lipo cells and the BMS MOSFETs get hot to touch. Charger is putting out 42v but it's not getting to the pack. Cells were balanced first. Then I tried charging via the evolve charging system. Despite all cells @3.8v the charger went light green within half an hour. Got 4/5km out of it. Battery indicator dropped consistently over that distance and won't recharge. Cell voltages are all over the place.
Remote indicates battery is flat. 
Yes cell order on balance plug checked wiring ok. No shit stains on PCB
Cells weren't new. But were all serviceable. Salvaged Multistars from my own packs. I know they were performing well.
Bought second hand. Previous owner complained about battery sag. I experienced the same symptoms. One cell in the original pack was a lot lower than the rest. So that's why I went ahead and DIYed a replacement.
```

---
## \#29 Posted by: Steven1 Posted at: 2018-11-04T15:05:12.122Z Reads: 33

```
Unfortunately no, I didn't. I gave up ordered a new BMS, vesc and remote.
```

---
## \#30 Posted by: asuras Posted at: 2019-04-16T08:52:54.540Z Reads: 21

```
Having the exact same issue, if anybody has any updates, post em!
```

---
