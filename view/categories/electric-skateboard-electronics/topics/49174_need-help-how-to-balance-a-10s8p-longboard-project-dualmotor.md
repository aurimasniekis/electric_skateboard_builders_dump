# NEED HELP: How to Balance a 10S8P (Longboard Project Dualmotor)

### Replies: 18 Views: 720

## \#1 Posted by: Kallewarrio Posted at: 2018-03-15T12:10:52.558Z Reads: 111

```
Hey guys
i need your help

i need to balance a 10S8P pack
i played with the idea of a BMS 
but the problem is the 120A discharge current. (180 peak)

Parts i use:
- (2x) Turnigy Aerodrive SK3 - 6354-260KV Brushless Outrunner Motor (2,35 KW each)
- (1x) Alien 120A 2-12S V4 Factory ESC HV Twin
- INR 1850 Cells (100pcs) 3000mAh 20-30A discharge 

if i missed some information, just tell me xD

thx for your help guys :slight_smile:

.
.
.
**_DOCUMENTATION of the board started, follow if u like to_** :sunny: **:**
https://www.electric-skateboard.builders/t/build-and-planning-longrange-cruiser-dualmotor/49262?u=kallewarrio
```

---
## \#2 Posted by: dg798 Posted at: 2018-03-15T13:14:07.331Z Reads: 98

```
You could bypass the discharge on BMS due to your vet high current and just use it for charging. @thisguyhere I think is selling bestech charge only BmS for like $30. Ask him
```

---
## \#3 Posted by: dg798 Posted at: 2018-03-15T13:15:10.752Z Reads: 94

```
I mean unless you want to spend a ton of money on a 10s balance Charger. I wouldn’t do that though. A bms is much cleaner and cheaper. Just takes some research and some time to wire everything up.
```

---
## \#4 Posted by: dg798 Posted at: 2018-03-15T13:19:23.383Z Reads: 91

```
Also if I’m not mistaken you only need 90 cells for a 10s8p battery:
10 cells in series, 8 parallel sets, 90 cells I think. Someone correct me if I’m wrong.
```

---
## \#5 Posted by: Kallewarrio Posted at: 2018-03-15T13:24:21.266Z Reads: 87

```
thx for ur reply,
i think that the way of using it only to charge is the way to go.

ps acually 10 times 8 is 80 cells, so the drive system is powered by 80 cells
     there are 20 additional cells (10S2P) for other systems on the board like light and gps systems (just for fun)
     btw this could also be used as backup
```

---
## \#6 Posted by: DeathCookies Posted at: 2018-03-15T15:10:54.099Z Reads: 79

```
[quote="Kallewarrio, post:5, topic:49174"]
there are 20 additional cells (10S2P) for other systems on the board like light and gps systems (just for fun)

btw this could also be used as backup
[/quote]

When you use 20 cells for different stuff do not make a 10s2p. you would have to use buck converters which lowers the Efficiency. imo i would Analyse what voltage i use for my different stuff and make a pack that compares to it
```

---
## \#7 Posted by: dg798 Posted at: 2018-03-15T16:57:40.821Z Reads: 72

```
Yeah u got to check all of the specs for whatever ur hooking ur batteries up to to make sure u don’t put took much voltage into them
```

---
## \#8 Posted by: BoostedBuilder Posted at: 2018-03-15T17:10:10.179Z Reads: 64

```
Or you could use this [BMS](https://ru.aliexpress.com/item/12S-120A-version-S-LiFePO4-BMS-PCM-PCB-battery-protection-board-for-12-Packs-18650-LiFePO4/32767760750.html) from Aliexpress, I think @bimmer got a few and was willing to let 1 go!
```

---
## \#9 Posted by: b264 Posted at: 2018-03-15T17:14:22.853Z Reads: 64

```
[quote="dg798, post:4, topic:49174, full:true"]
Also if I’m not mistaken you only need 90 cells for a 10s8p battery:

10 cells in series, 8 parallel sets, 90 cells I think. Someone correct me if I’m wrong.
[/quote]

That's not correct.  eight times ten is eighty
```

---
## \#10 Posted by: b264 Posted at: 2018-03-15T17:15:34.063Z Reads: 60

```
[quote="Kallewarrio, post:5, topic:49174"]
there are 20 additional cells (10S2P) for other systems on the board like light and gps systems (just for fun)

btw this could also be used as backup
[/quote]

Use a 3S1P for those systems with a cell like the Samsung 35E

How many watts will the other systems be using?
```

---
## \#11 Posted by: dg798 Posted at: 2018-03-15T17:23:42.325Z Reads: 56

```
I thought it’s 10 cells series plus another 80 cells for parallel. 😬
```

---
## \#12 Posted by: Kallewarrio Posted at: 2018-03-15T21:17:42.922Z Reads: 45

```
[quote="BoostedBuilder, post:8, topic:49174, full:true"]
Or you could use this BMS from Aliexpress, I think @bimmer got a few and was willing to let 1 go!
[/quote]

Hmm, i looked at this.
To me it seems to be a bit under powered.
it can "handle" a discharge of 120A ...  
but running this at maximum capacity .. mmmh 
actually i think if i only charge with bms and use additional safety features .. this could work as good as this method for less money ..
what do you guys think ?
```

---
## \#13 Posted by: Kallewarrio Posted at: 2018-03-15T21:20:27.880Z Reads: 41

```
[quote="b264, post:10, topic:49174"]
Use a 3S1P for those systems with a cell like the Samsung 35E

How many watts will the other systems be using?
[/quote]

there are 100W +/- 20 for light systems and 50W for other things

the point is, that i could use the 10S2P pack as backup if i run out of juice on a long ride (calc about 60KM / 37 Miles)
```

---
## \#14 Posted by: bimmer Posted at: 2018-03-15T21:57:08.728Z Reads: 38

```
Jep actually I've hurt myself and will let both go.
```

---
## \#15 Posted by: BoostedBuilder Posted at: 2018-03-15T21:59:57.345Z Reads: 37

```
sorry about that! hope it's not too bad!. How is hurting yourself related to no longer needing the BMS?
```

---
## \#16 Posted by: bimmer Posted at: 2018-03-15T22:01:24.342Z Reads: 37

```
I can't fall on my Ass for a while. If I do my build I wont be able to not ride it.
```

---
## \#17 Posted by: bimmer Posted at: 2018-03-16T00:28:38.719Z Reads: 27

```
![20180315_172508|281x500](upload://d3X3vRM6NdCEPpHxotimP8vxtlN.jpg) Monster and little monster for scale... lets just say I absolutely believe these can do 120A cont. :smile:
```

---
## \#18 Posted by: krloz Posted at: 2018-03-16T00:49:22.561Z Reads: 25

```
[quote="dg798, post:11, topic:49174"]
thought it’s 10 cells series plus another 80 cells for parallel. :grimacing:
[/quote]

Nothing like that. When we talk of xSyP battery configurations look at it as if it were a table with columns and rows.  So 10 rows of 8 columns
```

---
