# How do I know BMS is working?

### Replies: 17 Views: 737

## \#1 Posted by: Bart_Dood Posted at: 2019-05-08T17:23:20.024Z Reads: 123

```
So I've wired up my BMS to the battery pack and my PSU is an off the shelf one that feeds into a DC-DC converter that outputs the correct voltage that I want to charge my 18650 cells at which is about 4.05 volts each cell as I want to get a good cycle life out of them.

How can I tell the BMS is working? so far when I plug it all in and I check with a volt meter I can't see that the cells are charging at all (they are at 3.58/3.6 volts so should increase as they charge).

How can I tell the BMS is working? during charge or discharge?
```

---
## \#2 Posted by: ZachTetra Posted at: 2019-05-08T17:24:32.139Z Reads: 122

```
Show us a pic of your setup and your wire diagrams if you have it, if you can measure the amps going from the DC source to the BMS
```

---
## \#3 Posted by: Bart_Dood Posted at: 2019-05-08T17:26:32.285Z Reads: 119

```
Thanks, I don't have that here but checking the amps is a good test. Does the PSU have to be anything special or can it just be a constant voltage source?
```

---
## \#4 Posted by: ZachTetra Posted at: 2019-05-08T17:28:14.374Z Reads: 110

```
Do you have your bms set for bypass or discharge?

Either way you should have a constant DC source going into the charge port of the BMS at a constant voltage equal to 4.2V times the series count (6, 7, 10, or 12)
```

---
## \#5 Posted by: Bart_Dood Posted at: 2019-05-08T17:30:50.814Z Reads: 106

```
I used one of those little BMS boards which doesn't seem configurable, yes I have a constant voltage equal to 4.05v X the number of cells.

Maybe I should discharge a bit down to 3.4 volts per cell and then see if it charges up again
```

---
## \#6 Posted by: ZachTetra Posted at: 2019-05-08T17:31:18.068Z Reads: 98

```
Whats your series count?
```

---
## \#7 Posted by: Bart_Dood Posted at: 2019-05-08T17:32:30.841Z Reads: 95

```
Its 4S for this part
```

---
## \#8 Posted by: ZachTetra Posted at: 2019-05-08T17:33:13.571Z Reads: 89

```
4s?  What kinda tiny pocket board is this?

Anyways give the BMS constant 16.8V and let it charge up, the cells wont balance unless they are full charge.  Next time you charge you can pull the plug once a cell gets to 4.05V, make sure it gets balanced every few cycles
```

---
## \#9 Posted by: LiquidSkater Posted at: 2019-05-08T17:41:18.406Z Reads: 89

```
Hey, I have a problem with my battery pack... I just went for a long ride and drained my battery to 30.6V. Now, when I plug in the charger nothing happens. When i opened the board the battery pack was a a bit warm in ONE place (the middle on the right row) now its not charging... what should I do?
I checked the charging port connectors and everything goes smoothly into BMS but nothing is charging, the charger light doesn't change to red when plugged in ![1557337143640279613301608802735|375x500](upload://88sgji5Iaua9oSf8FeHV4fiYd6s.jpeg) ![15573371806923218806124129208418|375x500](upload://50b5orOawVwaMpYtzSRwVUKAaTF.jpeg)
```

---
## \#10 Posted by: Bart_Dood Posted at: 2019-05-08T17:55:03.768Z Reads: 82

```
Can you use a volt meter and measure each cell? you should find the warm cells are higher voltages than the cold cells. Which probably means the BMS has problems.

From what I can gather a lot of these cheap chinese direct BMS PCB are really junk quality..
```

---
## \#11 Posted by: LiquidSkater Posted at: 2019-05-08T18:28:16.367Z Reads: 78

```
I have charged the pack a couple of times and now this happened, I can't check the batteries with multimeter cause then it would ruin the shrink whap and it was pain in the ass to put together...
```

---
## \#12 Posted by: Bart_Dood Posted at: 2019-05-08T18:34:47.756Z Reads: 72

```
Can't you read the cell voltages through the white BMS connector on the BMS? no need to open the pack
```

---
## \#13 Posted by: AlanZhou Posted at: 2019-05-08T19:00:01.603Z Reads: 66

```
those are chilly joints and you didnt tin the wires..., a little bit of vibration and they will pop off

i recommend getting some flux and a better iron
```

---
## \#14 Posted by: thisguyhere Posted at: 2019-05-08T19:17:48.319Z Reads: 64

```
https://medium.com/@esk8life.orders/checking-and-correcting-voltage-drift-in-a-battery-pack-616e139d2e3b
```

---
## \#15 Posted by: Bart_Dood Posted at: 2019-05-14T20:29:23.891Z Reads: 36

```
Hi All,

I thought I'd write back with the solution to this. I figured out what was wrong.

I tried multiple boards with the same result which was frustrating. I then swapped power supplies, I had been using a stock 24volt supply and I hooked it up to a DC-DC board to dial it back to the 16.8v for the 4S BMS.

Well instead I tried a benchtop supply and just set it to 16.8v with a current limit of 1 amp.

When i plugged it in, the voltage dropped to match the battery and it slowly went up as the battery charged. As the voltage reached the setpoint the current load dropped.

So it seems it was a PSU problem. Now I need to figure out what kind of PSU I need for this thing, I don't want to have to charge with my benchtop supply. Any ideas?
```

---
## \#16 Posted by: McErono Posted at: 2019-05-14T20:41:00.840Z Reads: 34

```
I count 40 cells. You are running a 4s10p battery?!
```

---
## \#17 Posted by: LiquidSkater Posted at: 2019-06-07T13:23:07.057Z Reads: 24

```
Yep indeed I am
```

---
