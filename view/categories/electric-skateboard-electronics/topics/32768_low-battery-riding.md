# Low battery riding

### Replies: 34 Views: 1255

## \#1 Posted by: Vampiresquid64 Posted at: 2017-09-10T04:29:09.869Z Reads: 164

```
so when my batteries get really low, of course my board slows down a bunch. I'm talking like 10 or 15 percent here. If I ride it til its at zero I know normally this will damage my battery but with the vesc I have set a cutoff. so is that 10 percent battery that I see on my phone 10 percent til the cuttoff or 10 percent till the battery is actually dead and by using the battery in those last 10 percent I'm damaging it.
```

---
## \#2 Posted by: treenutter Posted at: 2017-09-10T04:47:57.716Z Reads: 163

```
We'd need to know some additional information. What app are you using to get your info from VESC? What are your battery cutoff settings? What voltage is your battery?

My guess is that your app is reporting percentage of total voltage and disregarding battery capacity.
```

---
## \#3 Posted by: Vampiresquid64 Posted at: 2017-09-10T05:05:42.032Z Reads: 157

```
@treenutter I'm using the vesc monitor app. On bldc my start cuttoff is 3.5 and end is 3.2 or 3.3 I forget which. My battery is a 10s lipo
```

---
## \#4 Posted by: dotruongq Posted at: 2017-09-10T06:37:48.203Z Reads: 145

```
I think with you should base on your vesc cut off and that would be safe. 10% reading on your phone  is just a  number based on how you set each % to a certain voltage. ( since battery discharge is not linear line ). you shoudn't be worry if you set you cutoff right in VESC.
```

---
## \#5 Posted by: jmasta Posted at: 2017-09-10T07:23:12.821Z Reads: 131

```
With lipos you never really know. Sure the VESC protects if the overall pack voltage gets low. But it does not protect each cell like a BMS does

Running to 3.2V nominal on lipos is really low. Might work for a while but eventually your cells will degrade. Some could actually be at 2.9V or below
```

---
## \#6 Posted by: Nordle Posted at: 2017-09-10T07:42:08.593Z Reads: 121

```
Hope you don't burn up your house
```

---
## \#7 Posted by: onepunchboard Posted at: 2017-09-10T14:23:47.719Z Reads: 97

```
for lipo 3.0 is absolute 0. 3.7 is about 30 percent. from my experience 3.3 is like 5 percent
```

---
## \#9 Posted by: Vampiresquid64 Posted at: 2017-09-10T14:52:11.036Z Reads: 85

```
Ok so like 3.5 is a good in between maybe? Or could I go 3.4
```

---
## \#10 Posted by: Vampiresquid64 Posted at: 2017-09-10T14:54:36.618Z Reads: 93

```
Well I mean as long as I don't run it past zero percent I should be fine right? Or would u say even 5 percent is too low and Will damage the batteries
```

---
## \#11 Posted by: Deckoz Posted at: 2017-09-10T15:06:43.703Z Reads: 94

```
Lithium packs are best when only taking 80% out of them

Lipo voltage range of 3.75-4.20v, Taking lipos any lower with load will degrade the packs. And typically begin to sag quite a bit once they go past storage voltage(3.75v). Full discharge on LiPO is considered to be 3.6, however if you are breaking in packs, a low static discharge of .5 amps, down to 3.0v/c will yeild the mAH rating of the pack. Lipo's are the most volatile when it comes to balance runaway, if you discharge past 3.65v under load you will have very very quick balance runaway. which is not good

Li-ions working range - depending on the cell is 3.35-4.20. While most li-ions can discharge to 2.5v the current curve falls off around 3.35v/c

Life working voltage is 2.9-3.4v, any lower then 2.9v and the current curve falls off and begins to have voltage sag. Most life can discharge to 2.0v, but again any lower then 2.9v and your have voltage sag

for a 10s setup

lipo - max input  48v, min input 35v, cut off start 38v, cut off end 37v
liion - max input 48v, min input 30v, cut off start 35v, cut off end 33.5v
life - max input 46v, min input 28v, cut off start 30v, cut off end 29v

The above should leave you with about 20% charge on each of these configs, Discharging more then 80% under load from lithium cells is just abuse.
```

---
## \#12 Posted by: onepunchboard Posted at: 2017-09-10T15:17:11.635Z Reads: 85

```
I set it really low cuz i dont care that much of life span. i put cut off at 3.2. typically cycle is abaout 800 but if u salvage it. cutt off at 3.5 u can increas to about 1000 to 1200. 3.7 is really good but it wont really go beyond. it will get voltage sag and lower mah. quality lipo dont get sag under load anywys
```

---
## \#13 Posted by: Deckoz Posted at: 2017-09-10T15:23:08.037Z Reads: 85

```
Thats an incorrect statement, ALL batteries have voltage sag under load. Taking Lipos below 3.6 under load is asking for them to puff/swell and will destroy the IR of the pack, continual abuse will only make the IR higher, as the IR gets higher, the pack gives off less and less ampers with increased voltage sag. Eventually it will reach the point where either the pack ignites, or the pack will be fully charged but sag so much  that you hit Low voltage cut off right after you start riding. Internal Resistance is a key player in all lithium battery's health and amper capability. 

Take care of your packs.

Also your statement about quality lipos

Quality lipos typically have an IR of 1.5-3.0milliohms, while lower quality packs will have around 3.0-11milliohms IR.

JUST ONE TIME on an abusive discharge can increase the IR to that of a lower quality pack. On lithium polymers they pretty much become useless at around 15-18milliohms/cell and have so much sag that all they do is generate heat because of their IR. Once they get upto 25-40milliohms IR you have ticking time bombs any time you discharge, and each discharge is damaging the cell further because the majority of the layers have already been comprimised. 

WIth your methodology of discharge you could ruin a pack in as little as 10-25 cycles. lol...If your not actively watching your IR over time, you really have no clue about a packs health.
```

---
## \#14 Posted by: Vampiresquid64 Posted at: 2017-09-10T23:49:39.023Z Reads: 66

```
Ok thanks for the info and recommendations@deckoz Super useful. back to my original question, after I feel the board start to slow down, is it okay to keep riding it? Does slowing down mean it has reached the upper cuttoff limit or the lower one.
```

---
## \#15 Posted by: Deckoz Posted at: 2017-09-11T00:18:29.900Z Reads: 57

```
When it starts to slow down its OK to keep riding. Just know you have limited range left. Eventually it will cut off.
```

---
## \#16 Posted by: Vampiresquid64 Posted at: 2017-09-11T00:20:17.988Z Reads: 56

```
Ok thanks so I can basically ride it till it stops and not have to worry about killing my lipos
```

---
## \#17 Posted by: Deckoz Posted at: 2017-09-11T00:20:48.813Z Reads: 52

```
Yup as long as your params are set right.
```

---
## \#18 Posted by: Vampiresquid64 Posted at: 2017-09-11T22:49:34.204Z Reads: 45

```
ok @Deckoz so I changed it, and now I seem to be getting significantly less range than before. like I only got about 6 miles, whereas before it seemed like I was getting a lot more. also before, it would be at full power until the very end when it would dip but now it seems like that period of lower power lasts longer.
```

---
## \#19 Posted by: Deckoz Posted at: 2017-09-11T23:11:57.192Z Reads: 44

```
you can change the threshold of when the cuttoff starts - but i would keep the cutt off end where they are supposed to be.
```

---
## \#20 Posted by: Vampiresquid64 Posted at: 2017-09-11T23:24:16.058Z Reads: 42

```
Hmm 3.7 seems super high. Idk seen other people run it at like 3.5 but if u say it has to be at 3.7 then I guess I'll keep it there. Will it really damage the battery that much if it's a tad lower? I just have some cheap hobby King batteries btw. Nothing fancy
```

---
## \#21 Posted by: Vampiresquid64 Posted at: 2017-09-11T23:29:43.924Z Reads: 40

```
I've heard people say to set it to 3.3 as well. seems all over the place
```

---
## \#22 Posted by: scepterr Posted at: 2017-09-11T23:35:50.376Z Reads: 40

```
It depends what cells they are, their sag characteristics under load
```

---
## \#23 Posted by: Vampiresquid64 Posted at: 2017-09-11T23:36:32.316Z Reads: 38

```
like what quality of cells or just the chemistry
```

---
## \#24 Posted by: scepterr Posted at: 2017-09-11T23:37:24.134Z Reads: 37

```
I would look at the datasheet for your cells, it should tell you exactly what cutoffs should be
```

---
## \#25 Posted by: Vampiresquid64 Posted at: 2017-09-11T23:41:23.433Z Reads: 38

```
hmm cant seem to find one for my hobbyking cells
```

---
## \#26 Posted by: Deckoz Posted at: 2017-09-11T23:42:18.383Z Reads: 38

```
if you read my description above, you will see the different cell limits by cell type...divide my above example numbers by 10

but to answer your question, no, there is no lithium polymer designed to be discharged to 3.3v/cell.
```

---
## \#27 Posted by: Vampiresquid64 Posted at: 2017-09-11T23:51:41.366Z Reads: 36

```
yeah done that already. idk 3.7 just seems high for a cutoff. maybe I should just deal tho and just buy more batteries
```

---
## \#28 Posted by: Deckoz Posted at: 2017-09-12T00:01:49.290Z Reads: 36

```
Hey, they're your lipos man...  I've got boxes upon boxes of lipos that have been abused from discharging below 3.7 under load and cells have dropped out due to the increased internal resistance from the abuse. I rebuild them when I have time(take good cells and toss the bad). 

<img src="/uploads/db1493/original/3X/2/7/271ec6da036f9c6ef8e702c7e5b7d42f93568572.jpg" width="375" height="500">
```

---
## \#29 Posted by: Vampiresquid64 Posted at: 2017-09-12T00:03:03.272Z Reads: 32

```
damn thats hella batteries. why havent you switched to 18650s yet tho?
```

---
## \#30 Posted by: Deckoz Posted at: 2017-09-12T00:03:49.684Z Reads: 33

```
I run 18650s on my esk8, those are from my quads. But lipo is lipo no matter the size all the same chemistry

The other hobby that uses lipos because the wh/gram is better on lipos and every gram matters on quads..
https://youtu.be/v5E-2cfXTeM
```

---
## \#31 Posted by: onepunchboard Posted at: 2017-09-12T00:18:57.562Z Reads: 35

```
lipo is more less disposable batt. i even drained them to 3.1and 3.0 on load when i was doing rcs. use 500 cycle and toss it. if u really want to go forever batt, liion is only option. it's also heavy have to build it bms ans so on. both has pro and con but u know what? at the end of the day u will use that lipo for more than a yr if u ride every single day. 3.7 is very conservative. if u worry that much I rather ride a motor bike
```

---
## \#32 Posted by: Vampiresquid64 Posted at: 2017-09-12T00:23:02.486Z Reads: 32

```
hmm yeah good point. my lipos are pretty cheap, like 50 bucks each so even if i dont get a ton of charge cycles it may be worth my while.
```

---
## \#33 Posted by: Deckoz Posted at: 2017-09-12T00:24:50.816Z Reads: 33

```
Sure just watch them...and check IR and puffyness every couple charges. I dont wanna see a "my board caught on fire like a hoverboard" post :laughing:
```

---
## \#34 Posted by: Vampiresquid64 Posted at: 2017-09-12T00:37:29.855Z Reads: 30

```
haha yeah. I've never had that happen to me luckily. with all my rc stuff I just let the esc handle low voltage and its never been an issue.
```

---
## \#35 Posted by: onepunchboard Posted at: 2017-09-12T00:53:01.664Z Reads: 27

```
have u pierced a lipo? i have. it smoked a lot but fire? at low voltage u dont get one. u get hardly at even 4.0v. hoverboard used liion. u know what caused it? bs BMS. it over charged.
```

---
