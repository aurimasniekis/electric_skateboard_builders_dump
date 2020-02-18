# Are my cells unbalanced?

### Replies: 16 Views: 1395

## \#1 Posted by: Eboosted Posted at: 2017-02-05T06:56:53.896Z Reads: 116

```
I installed a Battery Supports 10S 60A BMS on a 10S4P with Samsung 25R, I opened the enclosure today just to check the voltage on each pack after some riding,  I found there were differences of until 0.2V of difference between the packs 

Does this range of 0.2v mean the battery is being correctly balanced?
```

---
## \#2 Posted by: Alextech Posted at: 2017-02-05T07:05:08.336Z Reads: 114

```
My cheap multi reader is inconsistent, what kind are you using? The cheaper the more inconsistent.
```

---
## \#3 Posted by: barajabali Posted at: 2017-02-05T08:14:12.647Z Reads: 107

```
Did you charge it yet
```

---
## \#4 Posted by: Eboosted Posted at: 2017-02-05T15:37:38.910Z Reads: 91

```
I measured the voltage of each pack several times and the voltage for each cell was very consistent everytime, I took the measure after a full charge. I wonder if my BMS is good. 

Pack 1: 4.21v
Pack 2: 4.20v
Pack 3: 4.21v
Pack 4: 4.25v
Pack 5: 4.15v
Pack 6: 4.05v
Pack 7: 4.19v
Pack 8: 4.21v
Pack 9: 4.20
Pack 10: 4.20v
```

---
## \#5 Posted by: barajabali Posted at: 2017-02-05T22:53:51.692Z Reads: 75

```
Only one to be slightly worried about is 6

Try bottom balancing vs top balancing
```

---
## \#6 Posted by: Eboosted Posted at: 2017-02-05T23:38:59.918Z Reads: 72

```
What you mean by bottom or top balancing? I'm lost here. 

I thought the pack was bad so I swapped it for a new one and it's still has low voltage even on the new pack, maybe one of the BMS mosfets is bad, is the anyway to test the BMS or the mosfets?
```

---
## \#7 Posted by: Alextech Posted at: 2017-02-05T23:57:59.198Z Reads: 71

```
Bms does typically mosfets, is uses a series of Resistors to limit voltage to 4.2v but don't have Balancing. 

Now i have seen that if my cells are to unbalanced from each other the BMS will just not charge them. Try to charge up your 4.05v up to 4.2v using a lipo charger, then ride and cahrger and check for balancing :slight_smile:
```

---
## \#8 Posted by: barajabali Posted at: 2017-02-06T00:19:03.089Z Reads: 69

```
Discharge the pack all the way to the lowest safest voltage then recharge. Simple way to bottom balance
```

---
## \#9 Posted by: JohnnyMeduse Posted at: 2017-02-06T00:19:55.642Z Reads: 70

```
[quote="Alextech, post:7, topic:17235"]
Bms does not use mosfets
[/quote]

What the hell.... BMS can use mosfet to be more efficient at balancing cell... BUT first you need a bms that actualy balance, because most of the bms sold in the market aren't balancing cell they are monitoring them.. Wich is normal since they are Battery MONITORING System. You actually need a balacing charger (or also call smart chager) to do the job of balancing cell while charging... 😉
```

---
## \#10 Posted by: Alextech Posted at: 2017-02-06T00:28:40.062Z Reads: 67

```
[quote="JohnnyMeduse, post:9, topic:17235"]
BMS can use mosfet to be more efficient at balancing cell... BUT first you need a bms that actualy balance
[/quote]

Since most don't balance shouldn't we make the assumption that is is a monitoring bms than a Balancing bms?   I'll edit my post to reflect that they infact can , but most dont.
```

---
## \#11 Posted by: Eboosted Posted at: 2017-02-06T00:45:53.359Z Reads: 62

```
Wow!, Hold on, this information is kind of a break through, I though BMSs function was to balance the cells or packs, not just monitor them, so what would a BMS function be in the case of a Battery Support?, just check/verify if there is a significative difference between pack voltages and shut the circuit off in case they aren't ballanced?
```

---
## \#12 Posted by: Eboosted Posted at: 2017-02-06T00:51:21.177Z Reads: 60

```
What would you suggest could be a safe method to discharge each (4-pack) to per say 3.2V? fortunately I can remove all packs individually as I used XT60 to connect them in series.
```

---
## \#13 Posted by: barajabali Posted at: 2017-02-06T00:53:08.943Z Reads: 59

```
Just put lid on the pack. You can only discharge the pack as a whole. Don't discharge each cel alone. Same goes with charging you can only charge as a whole don't charge each cell alone. 

Just drop the entire pack to nearly dead. The voltage of each pack should leave out once nearly dead
```

---
## \#14 Posted by: Eboosted Posted at: 2017-02-06T00:54:44.657Z Reads: 57

```
I'm guessing you wanted to say LED instead of LID
```

---
## \#15 Posted by: JohnnyMeduse Posted at: 2017-02-06T00:58:45.198Z Reads: 55

```
If you have this model... http://www.batterysupports.com/36v-37v-42v-10s-60a-10x-36v-lithium-ion-lipolymer-battery-bms-p-267.html

You should be alright since the balance fontion is clearly stated

@Alextech if you look at the picture you can clearly see some 60ma mosfet use for balancing the cell
```

---
## \#16 Posted by: Eboosted Posted at: 2017-02-06T01:00:46.893Z Reads: 55

```
Yes that's the one I'm talking about, ok great. So back on the track, any idea on why the pack #6 is charging less voltage that the rest? Does a 42V charger need several charger cycles to be able to balance all packs?
```

---
