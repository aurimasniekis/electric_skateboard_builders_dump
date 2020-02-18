# 7s1p wiring diagram help

### Replies: 17 Views: 788

## \#1 Posted by: banksta Posted at: 2018-07-21T05:01:23.773Z Reads: 80

```
Hi all, noob here, upgrading and building a new 7s1p battery for my ebay pennyboard as a first simple little DIY project to get my feet wet. Please let me know if my diagram looks correct, don't want to blow anything. Will be using sanyo 20700b cells, upgraded from 22p. Also, will switching from 10A cells (22P) to 15A cells (20700B) affect my BMS/ESC? Thank you, really appreciate all the advice.

![New%20Doc%202018-07-20_1|594x500](upload://lhCuRcQfFGwhLxU3lDwS0XkhabH.jpg)
```

---
## \#2 Posted by: LittleSheepz Posted at: 2018-07-21T11:08:27.024Z Reads: 64

```
Hello!

1) You diagram is wrong. The BMS balance Lead should have 8 connections for 7S. If you BMS have only 7 connections, it may probably means its for 6S.

2)You would need to check your BMS rated Discharge limits. I would reconmend having the dischage limit higher than what the battery can provide. Tho you can also use the BMS soley for charging purpose and bypass the BMS for the ESC connection.

3) Again, it depends on what type of ESC you are using. I highly guess it's not VESC based since it's from ebay.. Nonetheless, for example, your esc consume a max of 10A only, upgrading your batteries to 15A is pretty pointless except for increased range. Though 15A still seems pretty low to me...

Why not try the Samsung 30Q or 25R?
```

---
## \#3 Posted by: e.board_solutions Posted at: 2018-07-21T13:15:28.827Z Reads: 57

```
Every bms is different, it's possible having 7s bms with with 8 connections, the B- is the 8th connection ;)


grtz
```

---
## \#4 Posted by: rojitor Posted at: 2018-07-21T16:37:21.442Z Reads: 47

```
I do not get the idea of your charging wires.
C- is for charge negative and positive goes on main positive. Maybe you mean that but your drawing does not show poles.
Also 1p is suicidal and inefficient.
Using 2p you will have an almost decent battery and 3p is probably good enough.
```

---
## \#5 Posted by: banksta Posted at: 2018-07-21T16:55:25.838Z Reads: 47

```
Well the negative comes from the C- of the BMS and the positive from the main positive, I just labeled CH as charging, if you do see my drawing, it is coming from the main positive, I should have written c- instead of ch on the bms.

Putting aside what is better than others, my board currently does 5 miles at 13mph, which is surprisingly good for a 7s1p. I don't understand why you are saying that battery is suicidal, could you please explain?
```

---
## \#6 Posted by: rojitor Posted at: 2018-07-21T17:02:51.251Z Reads: 48

```
1p forces the cells to work at full power. They are Hot all the time. You can't expect a normal lifespan from that pack. Will be dead in a few months.
```

---
## \#7 Posted by: banksta Posted at: 2018-07-21T17:03:05.151Z Reads: 43

```
Hmm I believe that the 8th connection is the negative leading to the b- of the BMS, as @e.board_solutions stated, which I believe is correct. Also the BMS will be used only for charging.

The two main points of upgrading this little battery is 1. for me to get experience building a simple battery pack, 2. increased range on my pennyboard. For this board, I'm happy with acceleration and top speed, it already feels fast and unsafe at 13mph on that little 26 inch deck, I'm just trying to squeeze a bit more than the 5 miles I get from it, and by using Sanyo 20700B 4000mah cells, I'll almost double my range, this is more for the fun of DIY and to learn by doing something. Later down the road I'll be building a 10s3p using 30Q cells. Thanks again everyone, all the advice is much appreciated.
```

---
## \#8 Posted by: banksta Posted at: 2018-07-21T17:11:49.427Z Reads: 41

```
Hmm that is a good point, however based off the graph below, I'm gambling that the 20700B cells will perform better than expected. 

![tesla-cell-2|523x340](upload://qNecqdmKOEaoBOtAcfveQbJzuD0.png)
What's really impressive about those tesla cells is the 85% capacity after 3000 cycles, based off my research they seem to be pretty damn robust, but I haven't found enough real world evidence to know for sure. Anyways you might be right but I'm willing to take the gamble, and it's still a pretty cheap one at that
```

---
## \#9 Posted by: Hummie Posted at: 2018-07-21T17:23:12.194Z Reads: 37

```
you'll have to limit the cells' discharge with so few cells in parallel.  the graph you posts shows them being used within they discharge limits but if you go over the discharge limits they will die quickly if not worse.   with those cells and only one in parallel you have a max of 15amps you can use.  that's not much.

if you want to do so few cells they need to have a very high discharge rate.   headway lithium iron red cells, or lipos with a high c rate.
```

---
## \#10 Posted by: banksta Posted at: 2018-07-21T17:46:41.977Z Reads: 30

```
Those headway red cells look amazing, however they are way too big and would have to replace my enclosure, in which case I would just do a 7s2p or 3p using 30q, however a 1p is the parameter I'm stubbornly trying to work with.

Forgive me for my ignorance as I'm still doing my best in researching, but by discharge, you mean capacity right? As in example limiting the cells to be discharged max 80%, either through BMS or  stop riding the board when it starts hitting lower battery voltage? 

Also the board is currently running on 22p cells which are only 10 amps, same 7s1p configuration, I was under the impression that running 15 amps could only be an improvement? Thanks for your input @Hummie
```

---
## \#11 Posted by: Hummie Posted at: 2018-07-21T17:59:57.387Z Reads: 29

```
capacity and discharge ability are different.  there are lots of li-ion cells in computers for example that will have a larger capacity but low discharge ability and they can only put out a little current/amps/juice at a single moment otherwise they will get hot, not last long, have voltage sag...maybe catch on fire even.
charging  and discharging with 80% of the stated capacity is a good thing to do but somehting else.

look at the c rating on lipo or the discharge rating on other cells and every cell you put in parallel will double it.   so youre just doing 7s1p so only one cell in parallel...   you could even take those same cells and put them all in parallel instead of series and you would then be able to put out comfortably 7x 15 amps.  but then your voltage would be so low at like 4 volts.  

if you want to use as little space as possible lipo is the easy way to get the super high discharge ability....the "c" rating.   they exaggerate maybe double the reality but if you had 7 lipo cells with 5amphour of energy and lets say 40c....that would be 40 time 5....and 80 amps can be continuously pulled from the cell (stated)...but youre better off doing half that...so 40amps.   And that's a decent board.  i will pull 50 and so will many others and then you have real power.  

i guess youre not using the vesc?  worth doing.for many reasons.  another esc will maybe be drawing way more current from the cells and you probably cant set the limits.  if that's the case youve likely been killing your other cells quickly and you would likely feel extreme voltage sag with a hard draw.    cheap and easy is vesc and lipo. plug and play

going from the 10 amp ability cell to the 15 is an improvement and where you need it but still not close to a nice 50amps.  with lithium ion cells this is a problem and one of the reasons people will do  likely 4p and many more cells.
```

---
## \#12 Posted by: Fiori Posted at: 2018-07-21T18:26:51.065Z Reads: 26

```
You have to understand that a Tesla(or any modern electric car) has so many cells in parallel that they aren't pushing the cells near as hard as we do in esk8.

We tend to push the limits of these cells, and because of this they will not hold their capacity for near as many recharge cycles.
```

---
## \#13 Posted by: Erniechan Posted at: 2018-07-21T20:21:09.334Z Reads: 24

```
1p??
That pack is dead or in flames in under 3 months.
I would use A123 lifepo4 for 1p
```

---
## \#14 Posted by: Hummie Posted at: 2018-07-21T20:25:59.922Z Reads: 25

```
wow here's 50 amps in one can.  bit bigger can at 26mm.  and a lower voltage being lifepo but still.  and a good deal
http://www.batteryspace.com/a123-lifepo4-26650-rechargeable-cell-3-3v-2500-mah-50a-rate-8-25wh-anr26650m1b---un38-3-passed-and-iec-listed.aspx?gclid=EAIaIQobChMIve2Sn4Ox3AIVh7fsCh33PwH-EAYYAiABEgJ9R_D_BwE

if you dont know lifepo theyre much safer and have like 3x the lifecycles of li-ion.  so your graph above wouldnt be as good as these
```

---
## \#15 Posted by: banksta Posted at: 2018-07-21T21:29:47.272Z Reads: 22

```
[quote="Hummie, post:11, topic:62421, full:true"]
capacity and discharge ability are different. there are lots of li-ion cells in computers for example that will have a larger capacity but low discharge ability and they can only put out a little current/amps/juice at a single moment otherwise they will get hot, not last long, have voltage sag…maybe catch on fire even.
charging and discharging with 80% of the stated capacity is a good thing to do but somehting else.

look at the c rating on lipo or the discharge rating on other cells and every cell you put in parallel will double it. so youre just doing 7s1p so only one cell in parallel… you could even take those same cells and put them all in parallel instead of series and you would then be able to put out comfortably 7x 15 amps. but then your voltage would be so low at like 4 volts.

if you want to use as little space as possible lipo is the easy way to get the super high discharge ability…the “c” rating. they exaggerate maybe double the reality but if you had 7 lipo cells with 5amphour of energy and lets say 40c…that would be 40 time 5…and 80 amps can be continuously pulled from the cell (stated)…but youre better off doing half that…so 40amps. And that’s a decent board. i will pull 50 and so will many others and then you have real power.

i guess youre not using the vesc? worth doing.for many reasons. another esc will maybe be drawing way more current from the cells and you probably cant set the limits. if that’s the case youve likely been killing your other cells quickly and you would likely feel extreme voltage sag with a hard draw. cheap and easy is vesc and lipo. plug and play

going from the 10 amp ability cell to the 15 is an improvement and where you need it but still not close to a nice 50amps. with lithium ion cells this is a problem and one of the reasons people will do likely 4p and many more cells.
[/quote]

Ah I see, so just to verify my understanding, (c-rating) x (Ah) = Amps, so 20c battery with 2000mAh would provide me with 40A. And if I were to wire two of those in series, I would get 4000mAh, or 4Ah, still at 40A. 

Also if my board has currently been running on a 10A battery (7s1p samsung 22p), you are saying that, even if my board esc is limited to 10A, it's much safer to run a battery that has higher max discharge ability, like the 40A lipo example. I'm realizing what you and everyone else, including @Fiori, are saying is that my board, by design of 1p, will inevitably die soon, even if I haven't seen any signs of that yet, and unless I change to 2p at least or different battery, I'll be stuck in the same loop by replacing with another 1p even with tesla cells.

Also I'm saving my vesc for my jet spud build, which I'll be using a 10s3p 30Q cells for, if I'm correct 45A. I'm trying to keep the same esc that this crap board is currently using. 

[quote="Hummie, post:14, topic:62421"]
wow here’s 50 amps in one can. bit bigger can at 26mm. and a lower voltage being lifepo but still. and a good deal

[BatterySpace.com/AA Portable Power Corp. Tel: 510-525-2328](http://www.batteryspace.com/a123-lifepo4-26650-rechargeable-cell-3-3v-2500-mah-50a-rate-8-25wh-anr26650m1b---un38-3-passed-and-iec-listed.aspx?gclid=EAIaIQobChMIve2Sn4Ox3AIVh7fsCh33PwH-EAYYAiABEgJ9R_D_BwE)

![|35x60](http://www.batteryspace.com/productimages/lifepo/6610t.jpg)

### [A123 LiFePO4 26650 Rechargeable Cell: 3.3V 2500 mAh, 50A Rate, 8.25Wh,...](http://www.batteryspace.com/a123-lifepo4-26650-rechargeable-cell-3-3v-2500-mah-50a-rate-8-25wh-anr26650m1b---un38-3-passed-and-iec-listed.aspx?gclid=EAIaIQobChMIve2Sn4Ox3AIVh7fsCh33PwH-EAYYAiABEgJ9R_D_BwE)

6610

if you dont know lifepo theyre much safer and have like 3x the lifecycles of li-ion. so your graph above wouldnt be as good as these
[/quote]

These look great and may just barely fit in the enclosure. So, I don't think the esc is reprogrammable for the change in voltage to 3.3v in the a123, down from 3.7v, and what I'm confused about is if it will hurt the esc, my battery or motors to run lower voltage battery than designed. Same argument for the lipos, I found some good thin ones with a c rating that will work but only 7.4v, so running three in series would still only give me 22.2v. I know in either case i'd have to get a new charger for sure, either a balance charger or BMS/charger. I think I'm suffering from information overload, I'm forgetting things I just read, let me go have a coffee, and do more research on batteries and running different voltages. 

Anyhow, this little project isn't worth buying a new vesc for either way. Still looking into the feasibility of other options, maybe build a 7s2p with 30Q glued in diagonal to save space, shave a layer of wood under deck between enclosure and it would fit, this way I could keep most of the same charging equipment. Still not 40A or 50A, but much better at 30A max discharge. I grew up modifying cars and building PC rigs, but this is whole new world, and let me tell you, I love it.
```

---
## \#16 Posted by: Hummie Posted at: 2018-07-21T21:38:57.657Z Reads: 22

```
[quote="banksta, post:15, topic:62421"]
Ah I see, so just to verify my understanding, (c-rating) x (Ah) = Amps, so 20c battery with 2000mAh would provide me with 40A. And if I were to wire two of those in series, I would get 4000mAh, or 4Ah, still at 40A._if you wire the battery in series it increases the voltage but mah stays the same.  with a 4ah battery at 20c that battery would be specd to do 80amps._

Also if my board has currently been running on a 10A battery (7s1p samsung 22p), you are saying that, even if my board esc is limited to 10A, it’s much safer to run a battery that has higher max discharge ability, like the 40A lipo example. I’m realizing what you and everyone else, including @Fiori, are saying is that my board, by design of 1p, will inevitably die soon, even if I haven’t seen any signs of that yet, and unless I change to 2p at least or different battery, I’ll be stuck in the same loop by replacing with another 1p even with tesla cells.
_I dont know what your esc is pulling from the cells but surely more than ten amps.  if it were set to 10 amp max you would not be moving much.  if it were 1p with the 123 cells above youd be good to 50amps and could set the vesc to that for battery amp limit
in testing 30Q show to be good even to 20amps continuous._

Also I’m saving my vesc for my jet spud build, which I’ll be using a 10s3p 30Q cells for, if I’m correct 45A. I’m trying to keep the same esc that this crap board is currently using.

you could run a lower voltage very likely with your esc but not good for performance.  
7s2p with 30Q...wouldnt be too bad.  but you need to make sure your esc is not sucking more from them.  the vesc you can control that.  some of those rc escs are rated for very high current and because they use low voltage they need it.  rough on a ion cell unless many in parallel.

![|20x20](https://www.electric-skateboard.builders/user_avatar/www.electric-skateboard.builders/hummie/40/31081_1.png) Hummie:

> wow here’s 50 amps in one can. bit bigger can at 26mm. and a lower voltage being lifepo but still. and a good deal
>
>
>
> [BatterySpace.com/AA Portable Power Corp. Tel: 510-525-2328](http://www.batteryspace.com/a123-lifepo4-26650-rechargeable-cell-3-3v-2500-mah-50a-rate-8-25wh-anr26650m1b---un38-3-passed-and-iec-listed.aspx?gclid=EAIaIQobChMIve2Sn4Ox3AIVh7fsCh33PwH-EAYYAiABEgJ9R_D_BwE)
>
>
>
> ![|35x60](http://www.batteryspace.com/productimages/lifepo/6610t.jpg)
>
>
>
> ### [A123 LiFePO4 26650 Rechargeable Cell: 3.3V 2500 mAh, 50A Rate, 8.25Wh,…](http://www.batteryspace.com/a123-lifepo4-26650-rechargeable-cell-3-3v-2500-mah-50a-rate-8-25wh-anr26650m1b---un38-3-passed-and-iec-listed.aspx?gclid=EAIaIQobChMIve2Sn4Ox3AIVh7fsCh33PwH-EAYYAiABEgJ9R_D_BwE)
>
>
>
> 6610
>
>
>
> if you dont know lifepo theyre much safer and have like 3x the lifecycles of li-ion. so your graph above wouldnt be as good as these

These look great and may just barely fit in the enclosure. So, I don’t think the esc is reprogrammable for the change in voltage to 3.3v in the a123, down from 3.7v, and what I’m confused about is if it will hurt the esc, my battery or motors to run lower voltage battery than designed. Same argument for the lipos, I found some good thin ones with a c rating that will work but only 7.4v, so running three in series would still only give me 22.2v. I know in either case i’d have to get a new charger for sure, either a balance charger or BMS/charger. I think I’m suffering from information overload, I’m forgetting things I just read, let me go have a coffee, and do more research on batteries and running different voltages.

Anyhow, this little project isn’t worth buying a new vesc for either way. Still looking into the feasibility of other options, maybe build a 7s2p with 30Q glued in diagonal to save space, shave a layer of wood under deck between enclosure and it would fit, this way I could keep most of the same charging equipment. Still not 40A or 50A, but much better at 30A max discharge. I grew up modifying cars and building PC rigs, but this is whole new world, and let me tell you, I love it.
[/quote]

emphasized text

but if the battery can do the amps, based on the math above, then it's good and you dont have to worry and no reason to set for less amps from vesc unless youre trying to make your battery last forever or something
```

---
## \#17 Posted by: banksta Posted at: 2018-07-23T02:26:51.812Z Reads: 16

```
The more I research, the more confusing things get, but I think I’m a bit closer to understanding how things connect, I don’t think I was looking at it right to begin with. So a few things that helped;
wiring in series = increases voltage
wiring in parallel = increases mah
voltage x Ah = Wh (to guesstimate range)
Amp x Voltage = Watts
C-rating x Ah = Amps

So, my board has a single advertised 350w motor (most likely less, but we’ll say 350w), let’s also guesstimate that 36V is the healthiest voltage rating for the motor. 
With the current 22p 2200mah 10A cells in the 7s1p in the board, 10A x 25.2v (nominal) only gives 252W, not only underpowering the motor but also damaging the battery because of max 10A constantly being drawn. Also only giving 55.4 Wh (still gets me almost 5 miles)

With the a123 cells, at 7s1p, 22.4v, a total (50Ax(7x3.2)) = 1,120 watts is provided, which is much better especially with 50A rating. However, despite having a much, much more robust battery, Wh rating stays nearly the same at 56Wh, more range is the primary goal is this project, while keeping the battery small for enclosure. 

With a lipo battery that is 8000mAh, 11.1v with 30C rating, that’s 2,664 watts at 240A max rating! A bit better range with 88.8Wh. 

So, here’s where I’m getting confused as I’m not sure where my concerns should be:

1.	In the example of the lipo, pushing the higher 2,664 watts to the 350w motor won’t damage or affect anything? Is it safe to assume that it’s because the motor will only be drawing the 350w max?

2.	The only thing I should be worried for, in anything here, is if my power source is pushing a way higher voltage to the motor AND/OR esc than they are designed for, right? 
Stupid question but for example, 48V 12s battery to my current esc/motors, I’d have to make sure that all my BMS (if using li-ion) should be rated for 48V, esc set at 48V(??) and motors rated to take 48V, right? 

3.	By this assumption, the 11.1v 30C 8000mah lipo battery won’t fry my esc right? The only issue is if my esc has a low voltage cutoff, which would prevent it from working, right? And the 11.1v will only mainly affect my acceleration, not top speed, right?

The only thing getting fried here is my brain, I feel like I’m getting a masters in electrical engineering. Meanwhile I’ll keep researching.
```

---
