# Adding cells in series to older battery? 12S9P

### Replies: 13 Views: 347

## \#1 Posted by: michaelcpg Posted at: 2019-01-22T21:41:24.563Z Reads: 113

```
Hey all,

I'm currently using a 10S9P pack made of Panasonic NCR18650GA cells on my Trampa board. I've been using the pack for about 8 months now but since upgrading from 170KV to 200KV motors, I've had a lot of issues with my FOCBoxes overheating during large hill climbs (several KM+ long) even after mounting them on an aluminium block to act as a heatsink. 

I'm looking at upgrading the pack to 12S in order to reduce my current draw and hopefully increase my efficiency overall. 

In my case, the battery has never been discharged below 3V/cell and rarely above 4V and has never been fully charged to 4.2V. I've also never balanced the pack but all cells are still within less than 10mV of each other so the pack has been reasonably well looked after.

I'm just wondering if anyone has had any experience with upgrading the series count of packs that've already been in use for a while?
```

---
## \#2 Posted by: Indiangummy Posted at: 2019-01-22T22:18:35.878Z Reads: 99

```
As long as they are in balance you should not have any problems with it. Although you will have to remove the old welds and make new welds which might damage the cells. But if your carful you should have no problem making it into a 12s 7p or 8p
```

---
## \#3 Posted by: michaelcpg Posted at: 2019-01-22T23:08:12.332Z Reads: 87

```
Adding the extra 18 cells to change it from 10S9P to 12S9P won't be be an issue because the battery is built as 10 separate 1S9P packs that are connected in series via 6mm bullet connectors so it'll just be a matter of plugging in another two 1S9P packs in series.
Photo for reference:

![20180913_193031|690x388](upload://breMDAC6kmXFZsaXHlp9OyRqy69.jpeg) 

I'm more wondering if anyone has done this in the past as I'm curious to see if they've having had any issues with the new cells going out of balance over time with the older cells after having all been balanced during initial installation of the extra cells.
```

---
## \#4 Posted by: accrobrandon Posted at: 2019-01-22T23:21:49.905Z Reads: 76

```
[quote="michaelcpg, post:3, topic:81758"]
I’m more wondering if anyone has done this in the past as I’m curious to see if they’ve having had any issues with the new cells going out of balance over time with the older cells after having all been balanced during initial installation of the extra cells.
[/quote]

I think this is going to be the common comment to NOT do it... If it's been 8mo use who knows truly how many cycle counts it has and where the cell capacity is at... It could be fine...could be not...

With that being said I'm about to do the same. I built a 10s4p a while back but didnt cycle it very much at all.so.its basically New... Now I'm going to bump it to 12s.. And only becuase I know it has super low mileage use
```

---
## \#5 Posted by: dareno Posted at: 2019-01-22T23:23:28.320Z Reads: 70

```
[quote="michaelcpg, post:1, topic:81758"]
I’ve also never balanced the pack but all cells are still within less than 10mV of each other so the pack has been reasonably well looked after.
[/quote]

Does this mean you don't have a bms on the pack?  Just curious is all.
```

---
## \#6 Posted by: will_manners Posted at: 2019-01-22T23:39:27.991Z Reads: 66

```
Bad idea. Adding 2 new 9P packs in series will most likely go out of balance without a BMS. Cells increase in resistance over time and lose capacity, thus the older cells are likely to drain quicker than the new packs that you would put in. In your case the capacity loss would be lower since you've only charged them to a conservative voltage, however that doesn't mean the capacity loss and increase in resistance compared to the new cells would be negligible.

However your solution alone doesn't really address the initial problem which is your ESC's overheating. Remember, just increasing voltage won't result in higher efficiency and lower current draw. You need to change your gearing to a lower top speed whilst increasing voltage in order to see any heat management benefits.
```

---
## \#7 Posted by: michaelcpg Posted at: 2019-01-23T00:03:24.595Z Reads: 55

```
That's correct, no BMS on the pack. The 1S9P packs are easy to separate partly for this so that I could balance each pack separately if need be but it turns out they haven't needed to be balanced at all yet
```

---
## \#8 Posted by: michaelcpg Posted at: 2019-01-23T00:14:35.920Z Reads: 56

```
Yea I'm fully expecting to get some drift between new and old cell voltages over time. I'm not too concerned about that due to easily being able to balance the cells when needed as well as never fully charging/discharging the pack. 

I'm more just interested in getting an idea as to exactly how far I could expect the cells to drift based on other people's experience, although I understand it varies greatly depending on cell chemistry and how the cells have been treated so far. 

Unfortunately changing gearing is not an option. I'm using an E-Toxx 5:1 gear drive with 8" wheels so I can't really changing the gears themselves and anything smaller than 8" tires won't give me enough ground clearance.

While my thinking with upping pack voltage is it should help to reduce current draw and voltage sag to some extent, because I ride near max speed (~40km/h) a lot of the time, particularly when hill climbing, giving me a higher top speed should mean that I'll be riding close to the max speed of the board a lot less of the time and my understanding is that electric motors tend to loose some of their efficiency near the top end of their RPM range.

It'll also give me the option of going back to 170Kv motors without loosing any of my current top speed which would be another option as I never had any issues with hill climbing on 170Kv motors. The board was just too slow at 10S with 170Kv motors was all :p
```

---
## \#9 Posted by: AlexBE Posted at: 2019-01-23T07:12:14.737Z Reads: 42

```
Increasing to 12s will do nothing for your FOCBOX heat issues. Heat in the FOCBOX is cause by motor current, not battery current. Changing to 12s and going the same speed up the same hill will cause a decrease in battery current, but the motor current will stay exactly the same. (Unless you are also changing your gearing)
```

---
## \#10 Posted by: Marsen Posted at: 2019-01-23T08:02:38.971Z Reads: 35

```
The problem is the 200kV motors. The 200kV requires less voltage for the same speed, so going up the hill at the same speed as before means you require less voltage. However you still require the same amount of power to get up the hill so as power is volts x amps then you have caused an increase in current by changing to 200kV motors. Hence the over heating. Changing to a 12S battery will make no difference just increase the amount of voltage available.
```

---
## \#11 Posted by: Marsen Posted at: 2019-01-23T08:16:00.564Z Reads: 35

```
Adding dissimilar batteries together in parallel will work as batteries in parallel have the same voltage irregardless of capacity. Adding dissimilar cells in series however will cause a big problem even with a BMS attached. They will go out of balance really quickly. BMS's only have 20-80mA balancing circuits. You can get high amp balancing circuits but they are big and expensive. The only way you could do it would be to find the capacity of the P cells as well as the internal resistance and then build a P group that matches those parameters.
```

---
## \#12 Posted by: Marsen Posted at: 2019-01-23T08:17:55.332Z Reads: 31

```
Doesn't look like you have any more room in that case either.
```

---
## \#13 Posted by: FullMetal_Machinist Posted at: 2019-01-23T21:20:44.142Z Reads: 22

```
Good solution would be to take 2 cells form each pack (20 total) and make additional 2 pack of 7 from them, having 6 cell lefrover. Then you add 2 new cell per pack, total of 24 cells.
This way you buy 6 more new cells and have 6 leftover old cells (use them for flashlight or e-cigarette) but you 100% wont have balancing issues.
However it wont solve overheating issues, just as Marsen described. Fix for that would be to get smaller motor pulley, with 2 teeth less. This way after increasing voltage and decreasing pulley size top speed would remain the same, torque would increase (more kick for acceleration) and heat issue will be solved.
```

---
