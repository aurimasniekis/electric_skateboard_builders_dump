# When does the Bestech 80A BMS do its final balancing?

### Replies: 26 Views: 384

## \#1 Posted by: Toughook Posted at: 2019-05-09T22:08:29.143Z Reads: 132

```
As the title suggests, could someone clear this up for me please.

My problem is that after charging to 100% and getting the green light on the brick charger the board will run OK for about 2 miles and them suffer compete shutdowns. Board needs to be turned off/on to power up again and then might be ok for a minute or two before shutting down again. This gets progressively worse until you can't apply any throttle without it shutting down. By 85% it's unusable.

Battery is 10s5p.

The thoughts are that a p group is unbalanced due to the battery being stored over winter for 5 months. The unbalanced group causing the BMS to shut down ?

 I've charged to 100% and left on 'green' for 20 mins. Should this be longer to allow BMS to do its thing? 

Does the charger need to be connected and board be ON for the BMS to balance ? Or does the BMS balance whilst OFF ?

Can't find a definitive answer in the search function, or by googling. Has anyone else suffered this?

Thanks, Tony
```

---
## \#2 Posted by: goldrabe Posted at: 2019-05-09T23:47:20.347Z Reads: 121

```
You need to check how much the P groups drifted apart. To my knowledge BMS's can only balance differences in the 0.05V range.\
For me it sounds more like you have dead cells. My smart BMS starts balancing before the light turns green. I don't know how your BMS is doing this.
```

---
## \#3 Posted by: Toughook Posted at: 2019-05-10T05:59:51.371Z Reads: 110

```
thanks, how do you go about checking the P Groups exactly ? Is it from the balance lead JST plug (for +ve) and placing the -ve probe of multimeter one a ground terminal on BMS ? 

As the battery is well used, if I have dead cells what's the prognosis ? I've read that you shouldn't mix old and new cells, so therefore can't simply replace a dead cell with a new one ? Also since I'm not a battery builder, having never done any spot welding in my life to date, I don't think I could safely fix my pack even if this were possible.

Could my whole pack be screwed then ?
```

---
## \#4 Posted by: mynamesmatt Posted at: 2019-05-10T06:05:17.192Z Reads: 96

```
![e6d3821d1e8c5beff61e44fb1fff1895808a4d4e_2_708x1000|354x500](upload://aG6Io2bNulVnmyqFkCX2Lntzrff.jpeg)

I've literally watched each of my cells charging with a cell tester with that exact bms. once one cell hits 4.00v, it sorta stays there and the rest catch up slowly and end up at 4.18v each when full. also o don't remember where but i believe it was that it begins balancing at 4v/cell.

take your balance leads out and measure from 1-2, 2-3, 3-4, 4-5 etc along the pack. if there is a large discrepancy between cell voltage then you've got a dead cell on that p group
```

---
## \#5 Posted by: Toughook Posted at: 2019-05-10T06:10:21.745Z Reads: 91

```
thanks for the info ! Can I ask where excatly you are placing the multimeter probes to get the readings please. Is it from the JST plug (+ve probe) with the -ve probe placed where ?
```

---
## \#6 Posted by: mynamesmatt Posted at: 2019-05-10T06:24:53.474Z Reads: 88

```
[quote="mynamesmatt, post:4, topic:93341"]
take your balance leads out and measure from 1-2, 2-3, 3-4, 4-5 etc along the pack
[/quote]

there on the balance leads
```

---
## \#7 Posted by: mynamesmatt Posted at: 2019-05-10T06:26:29.233Z Reads: 90

```
![Screenshot_20190510-162556_Chrome|243x500](upload://ubY0pzUn5qte5j7PF0pUhegD5e1.jpeg)
```

---
## \#8 Posted by: Toughook Posted at: 2019-05-10T06:30:32.790Z Reads: 85

```
Thanks, that's helpful ! Since I couldn't get my multimeter probes into this plug (probes too big) I propose to use this : 
![p|140x140](upload://m4MfpW4l4wSy8y64GFLAxxDSPiR.jpeg) 
to make it easier to get the readings.

This is my exact BMS:
![BMS%2080A|546x500](upload://5krxdHaGOQsD6if5IzJIZEouM0S.jpeg)
```

---
## \#9 Posted by: Andy87 Posted at: 2019-05-10T06:36:05.576Z Reads: 81

```
That would work, but I wouldn’t recommend it as it’s super easy to short something when the probes touch each other accidentally. You could make an extension tip for your probes out of thin solid wire and take off the Isolation only on the ends a bit.
```

---
## \#10 Posted by: dareno Posted at: 2019-05-10T06:51:11.457Z Reads: 81

```
As you probably have a bad p group I would be stripping off the shrink and taking a look.  Those bms's are a good unit.  What battery is it?
```

---
## \#11 Posted by: mynamesmatt Posted at: 2019-05-10T07:29:01.121Z Reads: 80

```
yeah they're almost the exact same pcb
```

---
## \#12 Posted by: Toughook Posted at: 2019-05-10T08:00:06.428Z Reads: 78

```
@Andy87 yeah I had planned on soldering different length wires onto this header plug so that it's impossible to get a short when testing. Something I could then keep for use again in the future if I need to test the p groups.

@dareno I've got the shrink off and can see where I need to get to. Just what are my options if I do find a group that is bad ? Is the whole pack toast then ?
```

---
## \#13 Posted by: Andy87 Posted at: 2019-05-10T08:08:43.559Z Reads: 75

```
I made an adapter for my lipos with this connector. It’s super easy to measure than on the terminals of that clamp.

![image|690x466](upload://5B3LGwBRUBkKFluGm7ISh39qC4t.jpeg)
```

---
## \#14 Posted by: Toughook Posted at: 2019-05-10T08:12:20.280Z Reads: 73

```
can't beleive I didn't think of this ! Of course it's far easier to buy a 11pin jst plug with the wires attached already and then do what you've done with the big plastic wire connector ! 

Sometimes I can't believe how thick I am :blush: haha !
```

---
## \#15 Posted by: Andy87 Posted at: 2019-05-10T08:13:33.341Z Reads: 74

```
Exactly what I did. Just for 7pin jst. Easy peasy 😂
```

---
## \#16 Posted by: hyperIon1 Posted at: 2019-05-10T09:04:48.511Z Reads: 70

```
[quote="dareno, post:10, topic:93341"]
As you probably have a bad p group
[/quote]

Yes, this is a big possibility and if so you are charging the rest of the p groups to overcharge, but that would force the balance function to engage and bleed the excess off. Are you discharging through the bms? 
If so, and your escs are drawing more than 80a it will cause cutouts.
```

---
## \#17 Posted by: hyperIon1 Posted at: 2019-05-10T09:13:55.647Z Reads: 71

```
[quote="Toughook, post:12, topic:93341"]
Just what are my options if I do find a group that is bad ? Is the whole pack toast then ?
[/quote]

If you find the group or in some cases the one cell it can be replaced, but you have to prime the replacement to do so. If the rest of the cells or groups are 3.8v then you must match this voltage to add it and keep balance. 

Examine every group and test each cell, look for the lowest volt group. once you test each group by the count up method you should find something out of place.

an easy way to test each group without all the extra wiring would be to attach your negative probe from meter to negative (small jumper spring loaded) and use the positive probe with a point to probe the JST connector, You have to be careful to probe strieght up and down to avoid contact with two. It works well and you only need to do some math to find if a group or groups are out of balance or low voltage.
```

---
## \#18 Posted by: Toughook Posted at: 2019-05-10T09:25:42.382Z Reads: 63

```
I am discharging through the BMS but he Unity was set to the default 50A Max Min. I tried to lowering this but the cut outs continued. The thing worked perfectly fine for about 2 or 3 miles, scary fast as it happened, but buy 90% charge the cut outs started, and got more fequent (close together). By 85% the cut outs were immediate and therefore required a walk home !

The thing is, even if I find a bad group or cell(s) I just don't have any experience in fixing li-ion batteries. Never done spot welding, and also don't have equipment for charging single cells. Looks like I have a steep learning curve ahead of me............!
```

---
## \#19 Posted by: hyperIon1 Posted at: 2019-05-10T09:32:30.034Z Reads: 62

```
Well, if It can be a few things, have you updated the FW on the unity and adjusted the thermal throttling? Look for a loose solder joint in a connector T60 or T90. if all that checks out then I would consider the bad cell/group or bms, that tank may be the cause of the problem. 

if all else fails you can send it to us for repairs
```

---
## \#20 Posted by: Toughook Posted at: 2019-05-10T09:53:09.139Z Reads: 61

```
thanks, that's loads of info and hopefully useful pointers for me to investigate tonight on the bench. I did update the FW on unity before anything, but not considered the thermal throttling. It wasn't the unity that was cutting out though, it was the BMS. That required a turn OFF/ON to reset. I have checked all connections first and they seem fine, but will go through them again tonight to be sure.

Whilst it was working there was no hint of poor performance at all. In fact it felt as fast and powerful as ever. I'm hoping that it's the BMS, and can just replace that with a charge only version, discharging direct into Unity. That would be the ideal solution, but need to check the P groups are fine first of course.
```

---
## \#21 Posted by: goldrabe Posted at: 2019-05-10T11:00:58.158Z Reads: 59

```
I made a 10S4P pack out of the 10S5P with a bad P group. Because I was at the same point as you  regarding Spotwelding etc. I bought Nese modules to not waste the leftover good cells.\
It's not recommended to mix old and new cells because of the difference in internal resistance. The new cells are getting discharged unproportionally and could be damaged. But that's only read knowledge not my first hand experience.
```

---
## \#22 Posted by: Toughook Posted at: 2019-05-10T19:37:22.469Z Reads: 53

```
Ok i think i have found the issue.... 

Took readings from the jst balance plug and found this:
![20190510_202908|281x500](upload://48cSGg2L5tX51s7cX46cwDIW2dE.jpeg) 

B6 has no voltage to read, indicating a broken connection I'm assuming. This would cause the p group not to balance, correct ?

I haven't stripped the shrink wrap off yet to check, but does this sound like the root of the problem to you?

Would explain why the pack worked OK when 100% and started playing up by 90% as group balance would be more of an issue ?
```

---
## \#23 Posted by: Jumpman Posted at: 2019-05-10T20:04:48.278Z Reads: 47

```
Could just be a loose/broken balance connection, but I guess you’ll have to remove the shrink wrap to see.
```

---
## \#24 Posted by: rich Posted at: 2019-05-10T21:09:45.074Z Reads: 44

```
[quote="Jumpman, post:23, topic:93341"]
loose/broken balance connection
[/quote]

This :point_up_2:

Looks good because between B5 and B7 the voltage increases about 8V. With a dead p group it would be 4V only. Open the shrink wrap and find the loose balance connection at group 6. But check first if it's not the connector itself, who knows.

Good Luck!
```

---
## \#25 Posted by: Toughook Posted at: 2019-05-11T10:11:29.996Z Reads: 29

```
Here's the broken balance lead connection !

![20190511_110056|690x388](upload://tf7T1pRB0Q44Rfg1O7K1wh7yu38.jpeg) ![20190511_110118|690x388](upload://5Lsk9EFzgEET2ekfOgNh9aoGXNT.jpeg) 

Hoping that a little solder job followed by a decent balance charge will save the pack and stop the BMS cut outs.

Anything i should be ultra careful of when reconnecting this balance lead?

I don't want a 🔥

Thanks for any help !
```

---
## \#26 Posted by: spei Posted at: 2019-05-11T11:36:10.143Z Reads: 26

```
Just disconnect balance plug from bms and you should be golden
```

---
