# Batteries out of balance \[Solved\] (fake cells)

### Replies: 41 Views: 786

## \#1 Posted by: J95hicks Posted at: 2018-11-29T22:44:55.020Z Reads: 200

```
So i finally put together my pack and was able to take it for a ride... i have a 12s8p pack and i experienced either voltage sag or a low battery...doesnt matter. Took apart my pack and the cells are off.. 1st series group 3.793, 2nd 3.736, 3rd 3.733, 4th 3.751, 5th 3.452, 6th 3.606, 7th 3.754, 8th 3.754, 9th 3.75, 10th 3.746, 11th 3.756, 12th 3.755.. i have a bms for charge and discharge but ime worried about that 5th series group.. should i be or is that okay?
```

---
## \#2 Posted by: Erniechan Posted at: 2018-11-29T22:47:03.880Z Reads: 196

```
The bms will not balance them under 4.10v
```

---
## \#3 Posted by: J95hicks Posted at: 2018-11-29T23:07:43.024Z Reads: 181

```
Could you eleborate or explain that a lil further... i thought that was the whole point of the bms. To manage each series.... each series being below 4.1 V
```

---
## \#4 Posted by: thisguyhere Posted at: 2018-11-29T23:24:11.415Z Reads: 176

```
0.3v drift is a lot.

some bms won't balance if the difference between series is too high.

try charging up your pack all the way 4.2v (50.4v) so bms goes into float charge and leave it plugged in for HOURS and see if the drift goes away.

your bms will get hot though since it'll have to drain essentially 11 P groups down from 4.25 to 4.2 repeatedly until your 5th cell comes up to 4.2v.

my guess is you have a dead cell in the 5th group.  not sure if possible but try measuring each cell's voltage in that group and see if anything obvious is happening there.
```

---
## \#5 Posted by: J95hicks Posted at: 2018-11-29T23:32:26.032Z Reads: 162

```
I have nese modules so yes, i can check each cell in a parallel group. All 8 read 3.448, no dead cell. I will try plugging it in for a few hours to see if it bring that group up
```

---
## \#6 Posted by: thisguyhere Posted at: 2018-11-30T00:53:51.645Z Reads: 148

```
That makes it easy then, just bring the 5th group up to the same voltage, good to go.
```

---
## \#7 Posted by: b264 Posted at: 2018-11-30T01:04:18.693Z Reads: 141

```
After the charger turns green, leave it plugged-in for a LONG time, maybe even days.  This is when the balancing happens.  Also check that it is being corrected... it might not be since it's so far off as @thisguyhere said 

You catching this now likely saved your battery from the junk pile
```

---
## \#8 Posted by: J95hicks Posted at: 2018-11-30T03:52:44.335Z Reads: 129

```
Sweet, i think i did save it... been charging it since last post and the voltage drift is only .08 now.... ill let it charge longer though...but its looking hopeful......also my charger only does 48.1v.. will this be an issue later or not... i couldnt find a 50.4v charger??
```

---
## \#9 Posted by: b264 Posted at: 2018-11-30T03:53:49.148Z Reads: 128

```
What charger are you using?  It must be a lithium-ion charger and the correct voltage
```

---
## \#10 Posted by: J95hicks Posted at: 2018-11-30T03:56:05.909Z Reads: 129

```
![1543550067748159659642|375x500](upload://mU47Bkfw5jLpKgkbRxhZWQnfBZ8.jpeg) i was lead to this by someone on this forum. They said they used this for there liion pack with no problems
```

---
## \#11 Posted by: b264 Posted at: 2018-11-30T03:59:13.023Z Reads: 125

```
I don't think that will balance the battery if it never approaches 50.4V.  Some LED power supplies can work for lithium chargers, but only certain ones.  I would not use that to charge a 12S lithium-ion battery
```

---
## \#12 Posted by: J95hicks Posted at: 2018-11-30T04:03:39.758Z Reads: 123

```
Okay, i just unplugged it and the lowest voltage was 3.91 and highest being 4.04. I think thats good enough for now to ease my worries or a bricked batt pack. I just ordered a 50.4 v charger from some foreign place, so itll take like a month to get so at least i wont worry about my pack being ruined.
```

---
## \#13 Posted by: thisguyhere Posted at: 2018-11-30T04:46:34.030Z Reads: 118

```
U have to get 50.4v for float charge to kick in. 

Whoever led u to that led driver did u a disservice
```

---
## \#14 Posted by: J95hicks Posted at: 2018-11-30T04:51:29.819Z Reads: 114

```
Damn, well i just looked up 50.4v chargers and saw your post about the charger you use.. so i got that one lol thx for everyones help.
```

---
## \#15 Posted by: thisguyhere Posted at: 2018-11-30T04:59:26.435Z Reads: 114

```
The one i use is slow af, for your 12s8p it'll take forever fyi
```

---
## \#16 Posted by: Eboosted Posted at: 2018-11-30T05:26:05.244Z Reads: 111

```
How are your p-groups connected? Are you using only nickel strips?
```

---
## \#17 Posted by: J95hicks Posted at: 2018-11-30T06:06:58.706Z Reads: 108

```
Im using 3/8in pure copper tabs/bars with nese modules
```

---
## \#18 Posted by: J95hicks Posted at: 2018-11-30T06:07:55.230Z Reads: 107

```
Well shucks, oh well. I dont ride that much. Mostly for fun, so itll have time to charge....that and i hope i never run down this battery lol
```

---
## \#19 Posted by: PXSS Posted at: 2018-11-30T09:45:00.134Z Reads: 101

```
I'll take the meanwell off your hands if you don't know how to use it :P

That's one of the best chargers you can get...
```

---
## \#20 Posted by: deucesdown Posted at: 2018-11-30T13:29:28.667Z Reads: 95

```
HLG series 240w PSU, 48"A"djustable. I have the same unit on my desk, set to 52.5v.

This unit is actually perfect for the task at hand, being a psu and not a charger (no termination), and both voltage and max current being adjustable. And not dodgy cheap no name stuff.

2nd dibs if selling :)
```

---
## \#21 Posted by: Acido Posted at: 2018-11-30T14:27:27.589Z Reads: 82

```
that all depends on the bms
theres isnt an universal answer you can give about this topic you need to know the exact bms model

some balance all the time some not, some only when charging etc
```

---
## \#22 Posted by: deucesdown Posted at: 2018-11-30T14:50:15.882Z Reads: 82

```
[quote="thisguyhere, post:4, topic:76556"]
drain essentially 11 P groups down from 4.25 to 4.2 repeatedly
[/quote]

[quote="b264, post:7, topic:76556"]
leave it plugged-in for a LONG time, maybe even days
[/quote]

This part bugs me. lithium ion doesn't like being left at full state. 4.25v is slight overcharge. Days. It feels like trading convenience for pack life. Sigh.

Wouldn't it be nice if there was a balancing device that worked by charging the low groups instead of discharging the high groups? It'd be hella slow but surely faster than the typical 50-100ma bleed current too.
```

---
## \#23 Posted by: b264 Posted at: 2018-11-30T15:17:37.738Z Reads: 84

```
It'd be hella nice.  It'd also be more complex with more parts to fail. :expressionless:   There's always a tradeoff. 

Most of the time I only charge to  4.15V / cell and every 5 charges or so to the full 4.20V / cell
```

---
## \#24 Posted by: sk8l8r Posted at: 2018-11-30T15:37:37.167Z Reads: 80

```
[quote="deucesdown, post:22, topic:76556"]
balancing device that worked by charging the low groups instead of discharging the high groups
[/quote]

I use a usb powered 1p charger to bring low groups in line - loads quicker than waiting for BMS to do it I would imagine?
```

---
## \#25 Posted by: LEE Posted at: 2018-11-30T15:56:15.853Z Reads: 77

```
![0|666x500](upload://ncs5yNoli0ksCqyj1kq2H1VFzzv.jpeg) 

There was a balancing collapse of 0.4V at the maximum between P.
I used this to make the cell balun uniform.
But it was not good.
It was balanced to a certain extent. Even if I connected the 42V charger afterwards it was not fully charged.
Is it possible to balance by keeping the charger connected for a few days?
```

---
## \#26 Posted by: thisguyhere Posted at: 2018-11-30T16:07:01.036Z Reads: 75

```
[quote="deucesdown, post:22, topic:76556"]
lithium ion doesn’t like being left at full state. 4.25v is slight overcharge
[/quote]

agreed.  i actually asked bestech if we can modify the module so the float charge occurs at a lower voltage - answer was no.

[quote="deucesdown, post:22, topic:76556"]
Wouldn’t it be nice if there was a balancing device that worked by charging the low groups instead of discharging the high groups?
[/quote]

definitely!  if i was better with an arduino, i think it'd be relatively simple to put together a prototype that charges each P group until it comes up to a specific voltage (ie 4.1v).  essentially a bottom-up charge scheme as opposed to top-bottom charging.

i think an opportunity was missed here when [this bms was put together](https://www.electric-skateboard.builders/t/diy-6s-to-12s-bms-with-can-diebiems/2639).  it's just like a fancy bms with a bunch of features i don't really care about.
```

---
## \#27 Posted by: deucesdown Posted at: 2018-11-30T16:13:36.512Z Reads: 72

```
The problem I think is, for each charge circuit, the ground needs to be floating. Perhaps if the charger charged a single p group at a time... Like, bulk charge until 1 group hits the defined max, then charge individual groups one at a time. It would take FOREVER with the CV stage, but might still be preferable to the way it's done now.

DieBieMS uses an off-the-rack battery management chip. So it would be a nontrivial change.
```

---
## \#28 Posted by: thisguyhere Posted at: 2018-11-30T16:16:05.476Z Reads: 71

```
[quote="deucesdown, post:27, topic:76556"]
charger charged a single p group at a time
[/quote]

yup, this is what i had in mind.

shoulda gone into electrical engineering instead of software....
```

---
## \#29 Posted by: b264 Posted at: 2018-11-30T16:44:45.198Z Reads: 65

```
[quote="thisguyhere, post:28, topic:76556"]
shoulda gone into electrical engineering instead of software…
[/quote]

The difference between the two is narrowing...
```

---
## \#30 Posted by: J95hicks Posted at: 2018-11-30T18:13:18.887Z Reads: 63

```
Wow, i literally remember buying this bc its adjustable lol. Just bought my parts so long ago, i finally have a board lol. I see the adjustment "screw"  just plugged it in and its charging at 49.4v and rising. Thx man....sorry not selling nowXD but what is the other adjustment screw for??
```

---
## \#31 Posted by: deucesdown Posted at: 2018-11-30T18:28:03.041Z Reads: 66

```
[quote="J95hicks, post:30, topic:76556"]
but what is the other adjustment screw for??
[/quote]

max current ("I" is the symbol for current)
```

---
## \#32 Posted by: J95hicks Posted at: 2018-11-30T18:32:27.549Z Reads: 67

```
Okay, i thought so. Just making sureXD.... so for everyone else who gave me input too.... should i get it to 50.4 and hold it there and bring it down to the 1.2 amp charge and like let it "drip" charge(sorta) the whole pack to balance it out, bc lower amps is healthier for the battery so to speak..correct?..... i also ordered a 4.2 v charger for that P group if the issue continues.
```

---
## \#33 Posted by: J95hicks Posted at: 2018-12-05T17:14:48.079Z Reads: 59

```
Made another thread here  https://www.electric-skateboard.builders/t/12s8p-30q-cells-experiencing-voltage-sag-solved-fake-cells/76843 
Title is the reason, and we determined they were fake cells. So yeah... i have however determine a 2 P groups 1 higher and 1 lower than the rests v. I will try mixing the 2 P groups cells to reach the mean i guess.
```

---
## \#34 Posted by: Andy87 Posted at: 2018-12-05T17:46:18.166Z Reads: 53

```
[quote="deucesdown, post:22, topic:76556"]
lithium ion doesn’t like being left at full state.
[/quote]

But how than all the one way cells work?
They sit for years on 4.2v till they sold and used.
🤔
Not saying that it’s no like that, just wondering.
Is there a study to it? I mean I read here everywhere that it’s not good to let LiIon and lipos left at full charge, but I couldn’t find any evidence to it yet.
If somebody has something about it I would be happy to read through it.
Especially with lipos it would be interesting for me. 
At the moment lipos are my main power source and i can’t just charge them an hour before I go for a ride. So if I think I will go the next day I charge them up. If I can’t ride the next day I already have a bad feeling that it’s not good for the packs. But is it really like this? I also couldn’t find any recommendation how long I could let the lipo packs with a full charge. Just: not longer than needed...
```

---
## \#35 Posted by: J95hicks Posted at: 2018-12-05T17:57:48.271Z Reads: 47

```
Actually, i know part of the problem was fake cells.. but tbh, that 1P charger is getting every P group pretty lined up. I think ill be with .003 V soon. Partial solution cedit should go here too, thx
```

---
## \#36 Posted by: thisguyhere Posted at: 2018-12-05T18:03:47.159Z Reads: 47

```
[quote="Andy87, post:34, topic:76556"]
They sit for years on 4.2v till they sold and used.
[/quote]

nope, they sit at around 3.5v for long term storage.

lithium batteries build dendrites as their cycled and the higher voltage accelerates this buildup.

look up "lithium ion dendrites"
```

---
## \#37 Posted by: b264 Posted at: 2018-12-05T18:11:12.614Z Reads: 47

```
[quote="J95hicks, post:35, topic:76556"]
part of the problem was fake cells
[/quote]

Just to reiterate, the seller of the fake, fraudulent 30Q cells was

***bought from dhgate website***

https://www.electric-skateboard.builders/t/12s8p-30q-cells-experiencing-voltage-sag-solved-fake-cells/76843/16?u=b264

So anyone who finds this, never buy cells or anything else from there
```

---
## \#38 Posted by: sk8l8r Posted at: 2018-12-05T18:54:52.712Z Reads: 43

```
glad to help 

and if you accidentally over charge I used something like this, did the jobs pretty well without too much heat

https://www.amazon.co.uk/Witmoving-Headlamps-Flashlight-Headlight-Camping/dp/B074VVP4QT/
```

---
## \#39 Posted by: Andy87 Posted at: 2018-12-05T19:57:27.314Z Reads: 41

```
I never bought one way cells which where charged only to 70%
```

---
## \#40 Posted by: thisguyhere Posted at: 2018-12-05T20:13:35.819Z Reads: 38

```
lipo or liion?

samsung liion cells come out of the factor at 3.5v.
```

---
## \#41 Posted by: Andy87 Posted at: 2018-12-05T20:29:05.016Z Reads: 35

```
I was speaking about one way cells but I realized that this is not comparable...
I looked up what you said and I understood some things now better. Thx for this!
For lipos it seems that the graphens really are a great cycle life extender 😅
For lipos I read that a reduction of the max voltage at about 0.1V can double the cycle life....that’s a huge benefit.
If to calculate about 300 cycles up to 4.2v this would be 600 cycles with only 4.1v ... time that I get my smart bms and I can set my balance voltage to 4.1v per cell 😅
```

---
