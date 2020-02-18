# Is regenerative breaking bad for battery?

### Replies: 76 Views: 1650

## \#1 Posted by: nikoli280 Posted at: 2018-02-18T18:20:55.232Z Reads: 352

```
Hi i have a 18650 pack made from 50x LG HE4 cells. Each cell has a max charge current of "fast charge" 4A.
 
My question is what is my max regenerative charging power in the BLDC tool.

is it 

4A * 10 = 40A

or is it

4.2V * 4A = 16.8W * 50 = 840W / 42V = 20A ?
```

---
## \#2 Posted by: Hummie Posted at: 2018-02-18T18:26:23.691Z Reads: 336

```
I think on paper it would be 20a with 5 cells in parallel with each of them stated as good for 4 amp charge rate, but is that charge rate similar to discharge and we could consider a peak or continuous?  I bet, and think it's probably all related to how much heat is produced in the cells.   I think a graphing of regen current at different amounts and time periods would show a similar curve as the discharge graph
```

---
## \#3 Posted by: E1Allen Posted at: 2018-02-18T18:26:36.910Z Reads: 324

```
10s5p?

10char
```

---
## \#4 Posted by: nikoli280 Posted at: 2018-02-18T18:29:35.863Z Reads: 313

```
Yes 10S5p battery
```

---
## \#5 Posted by: nikoli280 Posted at: 2018-02-18T18:30:16.133Z Reads: 305

```
I talked to Hobbyking support and they said that 40A should be fine for charging. Im going to ask them about the formula since im a bit confused .
```

---
## \#6 Posted by: E1Allen Posted at: 2018-02-18T18:30:58.823Z Reads: 295

```
What is the mAh capacity of each cell?
```

---
## \#7 Posted by: nikoli280 Posted at: 2018-02-18T18:33:12.781Z Reads: 296

```
2500 mah pr cell. and 12.500mah when packed
```

---
## \#8 Posted by: Hummie Posted at: 2018-02-18T18:33:54.303Z Reads: 284

```
surprised they would give out info so casually that could be so dangerous.  I bet for short periods it would be fine at 40amps regen.  how bout you get a temp sensor and hook it up to the vesc and your batteries and tell us what happens!!
```

---
## \#9 Posted by: Acido Posted at: 2018-02-18T18:34:11.341Z Reads: 274

```
Open up the specs sheet of your battery and see whats the max charge current and add like 5 10amps more since you will not be breaking full power all the time
```

---
## \#10 Posted by: nikoli280 Posted at: 2018-02-18T18:35:27.274Z Reads: 264

```
The max charge current is 4A pr cell. But as i write in the top its a homemade 10S5P battery of 50Cells
```

---
## \#11 Posted by: Acido Posted at: 2018-02-18T18:36:35.738Z Reads: 256

```
So 5x4=20a
I have set mine to 20a and im pretty sure never reached that much amperes  if 20is low for you increase it id say to around 30
```

---
## \#12 Posted by: SOICDIP Posted at: 2018-02-18T18:41:02.745Z Reads: 242

```
[quote="Acido, post:9, topic:46766, full:true"]
Open up the specs sheet of your battery and see whats the max charge current and add like 5 10amps more since you will not be breaking full power all the time
[/quote]

Yup, momentarily exceeding max charging current is fine.
```

---
## \#13 Posted by: Fiori Posted at: 2018-02-18T19:03:12.935Z Reads: 228

```
I would not set it to 40 amps regen..... If max charge current is 4 amps, I would suggest not exceeding 20 amps regen. 

If you are running dual motors it should be even lower, at 10 amps per vesc.
```

---
## \#14 Posted by: ZackoryCramer Posted at: 2018-02-18T19:08:25.064Z Reads: 228

```
Hope this isn't off topic but how exactly does the VESC figure out what voltage to regenerate? Is there a step-up converter managing the recharging battery? Does the VESC turn excess power into heat since there is a battery regen limit?
```

---
## \#15 Posted by: PXSS Posted at: 2018-02-18T19:14:15.771Z Reads: 222

```
[quote="ZackoryCramer, post:14, topic:46766"]
how exactly does the VESC figure out what voltage to regenerate?
[/quote]
It regens to whatever the voltage of the battery is. 

[quote="ZackoryCramer, post:14, topic:46766"]
Is there a step-up converter managing the recharging battery
[/quote]
No. 

[quote="ZackoryCramer, post:14, topic:46766"]
Does the VESC turn excess power into heat since there is a battery regen limit?
[/quote]
Up to a certain point yes, then to protect itself, decrease the brake power.
```

---
## \#16 Posted by: Hummie Posted at: 2018-02-18T19:33:46.480Z Reads: 195

```
the bldc tool has two variables for the brakes and I hear theyre similar to the amp output and have a "motor max" and "battery max"...I'm guessing the motor regen can be adjusted with the same limits as the motor max and depending on the vesc model it will likely have a 120 amp override limiting it, but you can adjust this to your heart's content and its the battery regen which is the what is actually true regen and going back to the battery?
```

---
## \#17 Posted by: nikoli280 Posted at: 2018-02-18T19:35:48.540Z Reads: 188

```
I got this formula for calculating max current charge from Hobbyking.

each parrallel packs of 5 cells can charge the current of 1cell but at higher voltage. So its 4A pr pack. 

So with 10 packs its 4*10 = 40A max. Doesnt that seem right
```

---
## \#19 Posted by: Sebike Posted at: 2018-02-18T20:06:02.964Z Reads: 177

```
To me this sounds funny.. 

Charging current will be distributed between parallel cells, so that a charger providing 5a to your pack will roughly give each cell 1a charging current 

(exact current draw somewhat depending on how parallels are connected).

💫
```

---
## \#20 Posted by: PXSS Posted at: 2018-02-18T22:07:59.939Z Reads: 164

```
That is absolutely wrong. Please read the posts above
```

---
## \#21 Posted by: nikoli280 Posted at: 2018-02-19T12:10:23.868Z Reads: 144

```
which one?
```

---
## \#22 Posted by: nikoli280 Posted at: 2018-02-19T13:48:54.068Z Reads: 136

```
This time i think i cracked the formula. please correct me if it is not true.

12.500 mah / 1000 = 12.5Ah * 1.6 (4000mah / 2500mah) = 20A?

12.500 = battery pack capacity
4000mah = max charge current pr cell
2500mah = capacity of one cell
```

---
## \#23 Posted by: bevilacqua Posted at: 2018-02-19T14:01:16.451Z Reads: 137

```
The capacity of a single cell or pack does NOT matter when charging. 
As stated above the Parallel stack number 10S5P -> 5 in this case dictates the max. (continuous) charging current. So: 

4A (Per Cell in Series!) * 5 (Stacks in Prallel!) = 20A 

As braking is not cont. (Maybe 5-25s) you can increase it a bit: Up to 25-30A
```

---
## \#24 Posted by: bevilacqua Posted at: 2018-02-19T14:06:57.172Z Reads: 139

```
As this thread is called “Is regen charging bad for the battery” it think I should wirte something down: 

-Regen Charging is good for the Battery! 

There are a few published Papers and Studyes on electric cars which studied this topic. They wanted to know if the increased charge cycles had a negative effect on the battery life. It turned out there was no negative effect, and even a “healthier” longer lasting effect.
```

---
## \#25 Posted by: Sebike Posted at: 2018-02-19T15:02:33.678Z Reads: 138

```
Charge current is in amps. Capacity is in Ah. Power Capability is usually stated as C for lipos and for liions they usually state how many amps they can put out continously.

Imagine your batteries being pigs.

Either you have a small pig that can eat only 1 pound of corn til its full. The larger pig can eat 30 pounds. How much corn the pig can eat is equal to its capacity. Thats the amount of energy it can utilize when digging in the dirt. So lets say 30 pounds of corn gives the pig a full day of gentle digging until its out of energy and collapses or overheats, or it can do super intensive digging for 1 hour, but not many pigs have done that without ending up in ICU, so thats only in theory. So lets call the capacity of the larger pig 30 pounds of corn in 1 hour as it's the absolute maximum in theory. The smaller pig has a capacity of 1 lbs corn in 1h, so in comparison it's a piglet. 

Then there is something we call C or power capability, and in the pigs world this is digging capability. A high C means the pig is comfortable digging at a rate that is so intense that it burns a lot of that corn it previously digested. The smaller pig is in super good shape and it digs holes at a rate that would make it end up in China before sunset (if it would only have had a bigger belly to store that corn). If you try to push the pig to dig any faster, in time it will most likely overheat and eventually die. So at the maximum rate, it will burn lets say 10 lbs of corn / hour, so we decide to say it can output a continous digging "energy" of 10 lbs of corn. 
The larger pig is a lot slower though and if you pushed it to dig at the same rate as the small pig it would probably end up with hyperthermia and a heart attack.

How fast can you feed the pigs then to make them go dig again? Well for that you'll have to ask their moms and dads, cause they usually know best. For batteries this is found in the specs for the specific cell. This is much dependent on how large the pigs mouth is. It likes to eat slowly, but it's capable of eating faster as well, although its inner organs will probably take a beating if you feed it too fast too often. 

What if you feed four equally large pigs at a time then? If they stand next to each other and you throw the corn on the ground, they share the food equally, cause every single pig will get to just as much corn as the one next to it. Every pig gets a 1/4 of the corn.

What if the pigs are standing in line while you're feeding the first line of pigs? The first pig will be happy and eat all the food that was meant for all four, but after a while, what goes in must come out, and that's where the second pig gets happy, cause even though he will have to eat shit, he is a dirty pig, so he will happily eat up all that processed corn,,,and so will the third and the fourth.

So there's your batteries for dummies! 

:pig: :pig: :pig: :pig:
```

---
## \#26 Posted by: SkateYS Posted at: 2019-01-29T04:10:37.081Z Reads: 85

```
Regenerative breaking is good, but not for everyone! If you are using a battery without a BMS (Or bypassing the BMS for discharge), regenerative breaking will unbalance your cells. That's why your new battery is fully charged at 42.3V the first time, 42v the second time and 41.8 V next, so on and so forth. I really need a good way to disable it but when I set regen at 0, I don't have no brake anymore 🤷‍♂️ Honestly why would I wanna charge my battery this way? (3 seconds every 30 seconds)😂
```

---
## \#27 Posted by: Andy87 Posted at: 2019-01-29T04:18:15.287Z Reads: 86

```
I don’t think that your cells get out of balance by this little tinny bit you charge back.
You use a bms for charge only what means even if your cells get out of balance by reg breaking at the next charge the bms will bring them up on the same level.
If you still worry than just use a bms for charge and discharge
```

---
## \#28 Posted by: Winfly Posted at: 2019-01-29T04:19:39.762Z Reads: 88

```
I wondering if you can set battery min to 0 and then turn on reverse to brake. Problem with 0A regen is that you with have no control of your brake. It can only short 3 phase together or not break at all.
```

---
## \#29 Posted by: SkateYS Posted at: 2019-01-29T15:01:53.400Z Reads: 79

```
Most people think that BMS balance charge you battery! But in fact, that is just what it is suppose to do. Only good quality BMSs (expensive ones and industrial ones) do that. The ones we all end up buying for e-bike and e-sk8te don't balance charge. They just cut off the current flow from the charger when one cell reaches 4.2V (some 4.15 or even less).Same for $50 and less lipo balance chargers. It is important to know that, they won't bring your cells back to the same voltage if they were off, but they will keep the same gap between cells until fully charged. That s why you have to charge equally your cells before building your pack. A regular bms can't stop charging one cell and keep charging the others.
```

---
## \#30 Posted by: Andy87 Posted at: 2019-01-29T15:05:43.986Z Reads: 80

```
That’s not correct.
You can get a bms for charge only at 25$ or less like the d140 from bestech which will balance your cells out.
There also smart bms options on the market with which you even can watch how the voltage from every pack get paired up to the others.
```

---
## \#31 Posted by: SkateYS Posted at: 2019-01-29T15:06:04.317Z Reads: 78

```
Yeah, just tried! It's very unsafe. Braking becomes very jerky and I think this gives hard time to the VESC. Might work on different setup tho!
```

---
## \#32 Posted by: Andy87 Posted at: 2019-01-29T15:11:17.019Z Reads: 78

```
[quote="SkateYS, post:29, topic:46766"]
.Same for $50 and less lipo balance chargers
[/quote]

Also not right.
I have a i max b6 charger for my lipos.
It’s like 35€ balance charger.
With it i definitely balance out every cell of my pack. I can even discharge the lipo pack to storage voltage.


One thing I need to add on the comment I made before,
If you have a 2p 3p or how ever pack for sure the bms will not balance every single cell, only the p pack, but this will every bms even the most expensive one.
```

---
## \#33 Posted by: Andy87 Posted at: 2019-01-29T15:17:22.222Z Reads: 76

```
And one more thing... the data sheet from the d140. As you can see it’s written the balance current and also how the bms will balance your cells.
![image|365x500](upload://b9lyUvbR1KLP4o4NsfeEuh0jb3C.jpeg)
```

---
## \#34 Posted by: SkateYS Posted at: 2019-01-29T15:19:18.259Z Reads: 73

```
I used to setup BMS both for charge and discharge. But you can't use the full potential of your battery if you do so. That's not really bad if you re using a decent amp tolerance BMS and a less power hangry setup. Furthermore, BMSs can also die during agressive rides and it's painful. For the regenerative braking, you don't really need to actually charge it for it to unbalance cells. I tried charging off BMS on a power supply (set charging current at .2 amps) at that point with a 10s6p, it's not really charging but still, cells go unbalanced after a longtime. Pretty slow but effective. Now imagine the amount of juice your vesc tries to push to your battery trying to give you the max for your couple of seconds braking
```

---
## \#35 Posted by: Andy87 Posted at: 2019-01-29T15:30:16.322Z Reads: 69

```
[quote="SkateYS, post:34, topic:46766"]
But you can’t use the full potential of your battery if you do so
[/quote]

That depends on your pack and your bms.
If you buy the right bms this is not an issue.

[quote="SkateYS, post:34, topic:46766"]
BMSs can also die during agressive rides and it’s painful
[/quote]
That’s right. That’s why people go with charge only bms. But again, if you choose the right bms this will also not happen.

[quote="SkateYS, post:34, topic:46766"]
Now imagine the amount of juice your vesc tries to push to your battery trying to give you the max for your couple of seconds braking
[/quote]
If you want to know that, than I can recommend you to get a Bluetooth module and track it. It’s not that much a current you think 😉
```

---
## \#36 Posted by: Benjamin899 Posted at: 2019-01-29T15:46:38.154Z Reads: 61

```
agree. i was also surprised by the litlle amount it pushed back
```

---
## \#37 Posted by: SkateYS Posted at: 2019-01-29T15:50:35.326Z Reads: 63

```
"2p 3p or how ever pack for sure the bms will not balance every single cell, only the p pack"
This is not making sense. It does not matter how many cell you have in parallel (those cells in parallel are always balanced since they act like a single cell, they charge each other and drain at the same rate if they are similar). Cells in series need to be balanced (not P), your battery pack, you bought it, that means same voltage on each cell already. I build them, I test many of those lipo chargers (also got that i max b6). What I'm saying is simple and you can rely on it. If your lipo (3s) has 
Cell 1: 3V
Cell 2: 3.5v
Cell 3: 4v
If you put it to charge with your imax, charging will stop when cell 3 is 4.20v, and will not care about 1 and 2 (they will not be 4.20v 😂).
Use a small dc motor and drain one single cell from your pack (through your balance leads), put back the pack in charge until full and you will tell me "now I see what you are saying"
```

---
## \#38 Posted by: SkateYS Posted at: 2019-01-29T15:52:45.649Z Reads: 57

```
This data sheet is full of what an Original balance charger or advanced BMS should have (even cheap balance chargers come with it lol). I don't even look at advertisement! I test for myself.
```

---
## \#39 Posted by: SkateYS Posted at: 2019-01-29T15:54:04.544Z Reads: 58

```
[quote="Andy87, post:35, topic:46766"]
your
[/quote]

You re just repeating what I said
```

---
## \#40 Posted by: SkateYS Posted at: 2019-01-29T15:55:21.053Z Reads: 57

```
[quote="Andy87, post:35, topic:46766"]
That’s right. That’s why people go with charge only bms. But again, if you choose the right bms this will also not happen.
[/quote]

The right BMS, you have a link for it?
```

---
## \#41 Posted by: SkateYS Posted at: 2019-01-29T15:57:14.681Z Reads: 58

```
[quote="Andy87, post:35, topic:46766"]
If you want to know that, than I can recommend you to get a Bluetooth module and track it. It’s not that much a current you think
[/quote]

Not that much current, I hope you re not thinking it can be less than the .2 amps from my power supply
```

---
## \#42 Posted by: pjotr47 Posted at: 2019-01-29T16:04:58.312Z Reads: 60

```
[quote="SkateYS, post:26, topic:46766"]
Regenerative breaking is good, but not for everyone! If you are using a battery without a BMS (Or bypassing the BMS for discharge), regenerative breaking will unbalance your cells.
[/quote]

Wrong! If so, then you also can't charge your battery. Each battery can take regenerative braking, the only thing that is important is that each parallel group must be equals to each other (same capacity). That is also the reason why using older and newer cells together is not good.

[quote="SkateYS, post:26, topic:46766"]
That’s why your new battery is fully charged at 42.3V the first time, 42v the second time and 41.8 V next, so on and so forth
[/quote]
Lol, if you have a new 10s pack, you must charge it max to 42v volts. It is not that each time you charge it the voltage will be lower. The capacity will lower each charge time but the voltage stays the same.

[quote="SkateYS, post:29, topic:46766"]
Most people think that BMS balance charge you battery! But in fact, that is just what it is suppose to do. Only high quality BMSs (expensive ones and industrial ones) do that. The ones we all end up buying for e-bike and e-sk8te don’t balance charge.
[/quote]

This depends much on the BMS itself, normally each BMS that has a balance function will balance your cells out at the end. But this can only be done when the voltage difference is not much between each parallel group. That is also a reason why you must use cells with the same capacity and lifetime.

[quote="SkateYS, post:37, topic:46766"]
I build them, I test many of those lipo chargers (also got that i max b6). What I’m saying is simple and you can rely on it. If your lipo (3s) has
Cell 1: 3V
Cell 2: 3.5v
Cell 3: 4v
If you put it to charge with your imax, charging will stop when cell 3 is 4.20v, and will not care about 1 and 2 (they will not be 4.20v :joy:).
[/quote]
If your pack looks like that it is game over for a good working pack. While riding cell 1 & 2 would have much more sag then the 4v. Also like you said charging would be a problem, but there is a normally a balance program on such a charger.
```

---
## \#43 Posted by: SkateYS Posted at: 2019-01-29T16:22:12.221Z Reads: 56

```
[quote="pjotr47, post:42, topic:46766"]
Lol, if you have a new 10s pack, you must charge it max to 42v volts. It is not that each time you charge it the voltage will be lower. The capacity will lower each charge time but the voltage stays the same.
[/quote]

You literally did not understand what I said and said something I believe too!
```

---
## \#44 Posted by: pjotr47 Posted at: 2019-01-29T16:31:56.022Z Reads: 58

```
[quote="SkateYS, post:26, topic:46766"]
Regenerative breaking is good, but not for everyone! If you are using a battery without a BMS (Or bypassing the BMS for discharge), regenerative breaking will unbalance your cells. That’s why your new battery is fully charged at 42.3V the first time, 42v the second time and 41.8 V next, so on and so forth.
[/quote]
What are you saying here?  what is your understanding of this?
```

---
## \#45 Posted by: GrecoMan Posted at: 2019-01-29T16:33:10.637Z Reads: 59

```
Huh? My $15 Chinese bms balances cells every time I charge
```

---
## \#46 Posted by: Mich21050 Posted at: 2019-01-29T16:33:52.838Z Reads: 60

```
[quote="SkateYS, post:26, topic:46766"]
BMS for discharge), regenerative breaking will unbalance your cells
[/quote]
Sorry, but you got no idea what you are talking about.. Please do some more research and listen to guys like @pjotr47 who know their stuff... 
How will a bms which is bypassed for DISCHARGE unbalance your cells when you CHARGE it...
```

---
## \#47 Posted by: GrecoMan Posted at: 2019-01-29T16:40:57.343Z Reads: 59

```
Yea I just read the rest of the thread and your wrong on pretty much everything...

If you set the vesc to 0a regent he only option it has to break is to short the motor phase wires, meaning the brakes are all or nothing

And unless you’re braking downhill for a mile or more the amount that’s charged thru regent shouldn’t be enough to cause any cell imbalance 

The primary function of a bms is to charge and balance all cells. That’s literally the entire point

When one cell in a pack hits full charge voltage the BMS won’t stop charging, but it’ll trickle charge all the other cells. Trickle charging takes forever cuz it’s super low amperage charging. It’s really only meant for cell imbalances of less than .1v but if you leave it for a day or two it’ll balance the cells depending on how far apart they are
```

---
## \#48 Posted by: pjotr47 Posted at: 2019-01-29T16:51:40.058Z Reads: 58

```
@GrecoMan  A 10/10 for your explanation

[quote="GrecoMan, post:47, topic:46766"]
When one cell in a pack hits full charge voltage the BMS won’t stop charging, but it’ll trickle charge all the other cells. Trickle charging takes forever cuz it’s super low amperage charging. It’s really only meant for cell imbalances of less than .1v but if you leave it for a day or two it’ll balance the cells depending on how far apart they are
[/quote]
As you told, this current is low. A cheap bms is most of the time around 60mah, High discharge is around 100-150mah.

Also some charge adapters cut off the current when the current is that low
```

---
## \#49 Posted by: Benjamin899 Posted at: 2019-01-29T17:00:28.807Z Reads: 56

```
yeah my charger only has 41.4v, which sucks balls.
```

---
## \#50 Posted by: Andy87 Posted at: 2019-01-29T17:13:24.337Z Reads: 55

```
Seems you have a lot of real life experience, so it will not make a big sense to argue further.
But to give you some credit, you right there are bms which will only cut off over and under voltage.
But those are without balance board and yes I know you don’t like to read data sheets, but you could find that out by reading those.
No any bms will ever balance all cells in your pack. Maybe that was a bit confusing how I wrote it, but a bms can just balance every single p group. So if you have 12 parallel groups in series  your bms will measure the average voltage in each pack and bring it up or down to 4.2v (or any other voltage which your bms is set to).
If it’s a 5p pack it’s the average voltage over all the 5cells in this pack. The 5cells in each pack should balance each other by there own, but if one cell is fucked that will not really happen. The defective cell can only lower the average voltage so much that your bms will recognize it an stop charging this pack.

One last thing to mention which is more related to your vesc than the battery, if you set your battery min for example to -6A and run dual drive than you will never push more than 12A regenerative back to your battery.
So it’s totally up to you and your knowledge about your pack to set this values right.
```

---
## \#51 Posted by: SkateYS Posted at: 2019-01-29T17:55:03.794Z Reads: 53

```
Yeah, totally agree! I did not try to mislead anybody! Except if there is something wrong on every single BMS and balance charger I bought, one should get the same results as me. When it comes to the VESC, it can have different results depending on the motor, VESC version, battery and currents setup.
```

---
## \#52 Posted by: GrecoMan Posted at: 2019-01-29T18:33:07.442Z Reads: 49

```
What can have different results?
```

---
## \#53 Posted by: SkateYS Posted at: 2019-01-29T18:54:18.947Z Reads: 49

```
By that I mean if your discharge wires are connected directly to you battery (not through the bms P lead), your vesc will recharge your battery straight off bms. Which is not safe and can lead to unbalanced cells or even overcharging. Can you respond? I wanna make sure I'm not mistaken because thats what happens in my case
```

---
## \#54 Posted by: Sn4pz Posted at: 2019-01-29T18:59:29.275Z Reads: 49

```
You should really be doing all of this messing around *outside*

You dont know what youre doing, please verify your problems and then find solutions that are clearly outlined.
```

---
## \#55 Posted by: linsus Posted at: 2019-01-29T19:18:28.758Z Reads: 48

```
Can vouch that 3/3 of my BMSes from Supower balances my pack(Like they're suposed to). My cells berly drift 10mV after 100+ charging cycles. Which i find acceptable.
```

---
## \#56 Posted by: pjotr47 Posted at: 2019-01-29T20:25:44.897Z Reads: 47

```
It is safe to bypass. Ok it is not a good idea for charge your battery to 100% and go downhill. But I you have charged your battery full. After 1km you have 10wh less. If I do a ride of 10km I have max 15wh regen

But your part about unbalanced cells is wrong... it can’t be that such a small amount of wh can unbalance your cells. Trust me: You can’t have unbalanced cells due regen. The amount of regen is to small for that. The only thing about unbalanced cells can be due a bad parallel group or broken cell in such a group. Then whould that group be faster empty then the others. The unbalance is only possible with discharge
```

---
## \#57 Posted by: SkateYS Posted at: 2019-01-30T03:54:11.374Z Reads: 41

```
You literally did not understand what I said, because I also agree will all you said! You say it's not true and then you say if the BMS has balance function! How about if it doesn't? I just shared something I experimented myself, nobody told me, I figured it out throughout years of building. Not happening on most builds but worth knowing.
```

---
## \#58 Posted by: SkateYS Posted at: 2019-01-30T04:01:48.506Z Reads: 41

```
Yeah, if your battery pack has always been balanced since you bought it, even them Aliexpress $4.5 BMSs will keep it balanced! Now if your BMS can bring back a non balanced pack (example:a 3S pack where cell 1=3.5v, cell 2= 4v and cell 3= 3.2v) back to a fully charged pack where all cells are 4.2V, Then I would love to have that BMS. Can you past a link?
```

---
## \#59 Posted by: SkateYS Posted at: 2019-01-30T04:10:26.887Z Reads: 40

```
Are you asking me how can a battery pack cells go unbalanced if charged without a BMS??? Read carefully what I said and do some research. Nobody told me! I tested myself (might be different in your case if you are doing it right, like using a good quality bms so it can fix the regenerative braking mess while charging with the real charger). Bypass BMS for discharge is basically ran discharge wires straight from the battery to the VESC. That means, VESC regen is going back to your Battery without protection (BMS still there but gets in action only when charging current is coming from C-)
```

---
## \#60 Posted by: Andy87 Posted at: 2019-01-30T04:11:33.017Z Reads: 41

```
If you have such a big drift between cells no bms will balance that out. The limit is at 0.1-0.2V difference what an usual bms can balance out.
If to think a bit more about that it also make sense as with such a big drift (0.5V or bigger) it’s very likely that the cell or pack is faulty and should be replaced anyhow. As a bms also protect your pack that would be an indirekte result in it.
```

---
## \#61 Posted by: SkateYS Posted at: 2019-01-30T04:14:52.587Z Reads: 40

```
A higher quality BMS (The ones with that balance thing) LOL
```

---
## \#62 Posted by: SkateYS Posted at: 2019-01-30T04:18:32.512Z Reads: 41

```
I know exactly what I'm doing! I'm using Cheap BMSs just for charging! I just shared that not all BMSs will Bring back your Unbalanced cells to a fully balanced pack, and everybody went against me 😂
```

---
## \#63 Posted by: Andy87 Posted at: 2019-01-30T04:21:34.061Z Reads: 40

```
Just to clear that up (sorry if you already said so, I just did undetstood it different) unbalance cells comming from different things, the regenerative break is the last which will affect it.
Maybe if you live in a very hilly area and you go a lot downhill it could have a minimal effect, but if you live for example in New York it's just super less you charge back.
And even than, if you build your pack right and use quality cells the effects is very very low.
Unbalanced comes through different internal resistance of the cells and how you weld/solder them together and which materials you use for it.
If you use nickle for your serial connections instead of copper wire that could be a reason.
```

---
## \#64 Posted by: Andy87 Posted at: 2019-01-30T04:25:30.684Z Reads: 39

```
Unfortunately you said this 

[quote="SkateYS, post:29, topic:46766"]
Only good quality BMSs (expensive ones and industrial ones) do that. The ones we all end up buying for e-bike and e-sk8te don’t balance charge
[/quote]

Maybe your words lead us to don’t understand it right.
There are bms which don’t balance, that’s totally right, but even the cheap ones we use from bestech like the d140 have a balance function.
So it’s not correct to say that all the bms WE use in our packs don’t balance.
If you would say, all the cheap bms YOU used in your packs didn’t balance that would be a different story 😜
```

---
## \#65 Posted by: SkateYS Posted at: 2019-01-30T04:32:18.338Z Reads: 36

```
[quote="Andy87, post:64, topic:46766"]
So it’s not correct to say that all the bms WE use in our packs don’t balance.
[/quote]

Never said that! what s a good quality BMS to you? The ones that work as expected
```

---
## \#66 Posted by: Andy87 Posted at: 2019-01-30T04:39:51.805Z Reads: 36

```
Read the words I linked in my last comment, you literally said WE 😅
Good quality bms you can find here
http://www.bestechpower.com/11s12s13spcmbmspcbforli-ionli-polymerbatterypack/
```

---
## \#67 Posted by: SkateYS Posted at: 2019-01-30T04:43:43.837Z Reads: 41

```
🤔Looking good
```

---
## \#68 Posted by: TowerCrisis Posted at: 2019-01-30T07:46:03.213Z Reads: 42

```
I'm PRETTY sure I get what @SkateYS is trying to say here about balance charging.

The vast majority of BMS's I've seen here do not balance cells throughout the complete charge and discharge cycle. They will only burn off some charge once the cells reach their max voltage. If the cells ever become unbalanced, they will be balanced once the pack reaches a near full charge again.



Our BMS's DO:
-protect the pack from overdischarge
-protect the pack from overcharge
-balance cells once they reach 4.15V (varies between brand / model)
-protect from getting too hot (only applies to temp sensor models)

Our BMS's do NOT:
-equalize cells when charging or discharging between 0% and 95% capacity

The more advanced models that he is talking about have an actual IC that will constantly monitor cell voltages and CONTINUOUSLY keep the cells balanced, even when the pack is disconnected. I know the diebms monitors cell voltage, but I'm unsure if it uses a traditional analog balance board to balance cells. These models are much safer than traditional BMS's, as they prevent user error.

The user error I'm talking about is referring to this scenario. If you want to extend your cell cycle lifetime, you can keep your cells between 30% and 80%. Doing this with vesc settings via minimum voltage cutoff, and with a lower voltage charger is a BAD idea. Your BMS will NOT balance your cells unless you have a BMS that is configured to charge cells to a LOWER voltage than 4.2V.

That's why these more advanced BMS's are safer. But I haven't seen one in a typical hobbyist use. I plan on using one for my next build.

If I got anything wrong lmk.
```

---
## \#69 Posted by: Andy87 Posted at: 2019-01-30T08:38:46.273Z Reads: 43

```
I think the upcoming smart bms are the future.
You can set your balance voltage and monitor the individual cell/p pack voltage when ever it is needed.
```

---
## \#70 Posted by: lrdesigns Posted at: 2019-01-31T00:49:30.197Z Reads: 33

```
My thoughts on topic. 

1c is a full charge from empty in 1 hour. 2c is 30min etc. What we are doing is high amp pulse charge for a few seconds. Its a completely different scenario so you can't use the 1c amp rating and apply it to a pulse rating. 

As far as I'm aware there is no scientific research on this use case and it’s effect on battery life. If there is please share?

It’s logical that a battery can take a much higher pulse then it’s rated 1C charge in amps. How that affects it’s life we don’t really know.

Most people will choose shorter battery life over a high speed crash though.
```

---
## \#71 Posted by: SkateYS Posted at: 2019-01-31T02:16:57.597Z Reads: 28

```
Anyone knows why my e-sk8 (Just finished building) goes full throttle when I turn off the remote? rocking a dual FOCbox, split PPM
```

---
## \#72 Posted by: Andy87 Posted at: 2019-01-31T03:23:20.428Z Reads: 26

```
Your fail safe is not adjusted.
```

---
## \#73 Posted by: dareno Posted at: 2019-01-31T03:32:28.442Z Reads: 27

```
[quote="SkateYS, post:71, topic:46766, full:true"]
Anyone knows why my e-sk8 (Just finished building) goes full throttle when I turn off the remote? rocking a dual FOCbox, split PPM
[/quote]

[quote="SkateYS, post:57, topic:46766"]
I figured it out throughout years of building.
[/quote]

:thinking::face_with_raised_eyebrow:
https://www.electric-skateboard.builders/search
Figure this one out with 5 minutes of reading.  :sunglasses:
```

---
## \#74 Posted by: SkateYS Posted at: 2019-01-31T04:30:32.797Z Reads: 24

```
Seriously? 😂
```

---
## \#75 Posted by: dareno Posted at: 2019-01-31T04:33:57.526Z Reads: 24

```
Couldn't help myself my friend.  Good luck!
```

---
## \#76 Posted by: SkateYS Posted at: 2019-01-31T04:37:19.320Z Reads: 23

```
No matter what we think, we are always wrong, and most of time it doesn't take a second to realize it. That's the world we live in. nice post!
```

---
## \#77 Posted by: dareno Posted at: 2019-01-31T04:40:11.089Z Reads: 25

```
Mate we are all noobs.  This is a brand new industry.  We are just varying degrees of noobs.  There is always something to learn.  Thats what makes it so exciting!
```

---
