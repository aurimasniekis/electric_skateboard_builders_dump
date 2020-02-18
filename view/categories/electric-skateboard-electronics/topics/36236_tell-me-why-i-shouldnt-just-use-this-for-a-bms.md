# Tell me why I shouldn&rsquo;t just use this for a bms?

### Replies: 21 Views: 1007

## \#1 Posted by: Hummie Posted at: 2017-10-23T02:37:39.301Z Reads: 183

```
https://m.ebay.com/itm/3S-13S-Lithium-Battery-Balanced-Function-Board-For-18650-Polymer-Battery/332160632043?varId=541192613484&_trksid=p2057872.m2749.l2649&_mwBanner=1

@Fatos showed this and is planning to use it.  Anyone done it?
It's seems half a bms in that it works on charging only.  So ud have to rely on the vesc low voltage cut off for discharge as this device doesn't work there.   
I'm trying to imagine how a battery failure would go w this.  With a rare check w a multimeter of the cell voltages at full discharge this things seems a god send
```

---
## \#2 Posted by: Jinra Posted at: 2017-10-23T02:43:00.137Z Reads: 179

```
> 2.This balanced board has no function of charging or discharging,and it cannot replace the protection board.When the battery is in the end of full charged,it will discharge by resistor to first fully charged battery,namely shunt and balance function 

No specs, horrible english, who knows wtf you're buying!
```

---
## \#3 Posted by: Hummie Posted at: 2017-10-23T02:51:07.518Z Reads: 169

```
I'm pretty sure its a cheap china version of the "dumb shunt" which is generally much bigger and more expensive. Discharging through a resistor the highest cells
```

---
## \#4 Posted by: b264 Posted at: 2017-10-23T02:51:49.400Z Reads: 153

```
It's definitely not a battery management system, looks more like a voltage divider
```

---
## \#5 Posted by: Hummie Posted at: 2017-10-23T03:03:53.433Z Reads: 140

```
my only fear is it would be too slow discharging with the resistor compared to the power going in while charging.  it says 66ma
```

---
## \#6 Posted by: b264 Posted at: 2017-10-23T03:53:02.255Z Reads: 119

```
My fear is if you don't unplug the charger at the exact correct moment, you will destroy your battery by overcharging it
```

---
## \#7 Posted by: Hummie Posted at: 2017-10-23T04:14:24.420Z Reads: 108

```
this thing, if it can discharge at the rate it's being charged I think, would have cells hold at 4.2 till all are there.   so you have a bulk power supply charging everything in series and these would turn that energy to heat as soon as it hits 4.2.  There'd be the danger of going higher if you're putting in more than they will burn off .  waiting for someone who knows better but it looks like the simple "dumb shunt" design on endless sphere and elsewhere and think that's how it works.  maybe could add a bigger resistor for higher power charging
I bought 6 so will see   and they shipped within an hour.
```

---
## \#8 Posted by: b264 Posted at: 2017-10-23T04:43:14.982Z Reads: 88

```
Please let us know how it turns out :slight_smile:
```

---
## \#9 Posted by: scepterr Posted at: 2017-10-23T05:09:41.921Z Reads: 81

```
This is just the passive balancing function separated from a bms with passive balancing. 

It will burn off energy till each cell is at 4.2V
If you upgrade the resistors you can increase balancing current, meaning it can maintain a higher energy burn off charging the lower cells quicker, a heatsink would be suggested

I used these for an early PowerWall build modded with chunky ceramic resistors to balance 40P 18650 packs
```

---
## \#10 Posted by: Hummie Posted at: 2017-10-23T05:46:58.295Z Reads: 78

```
 if the charger were putting out 5 amps, would the math be that's divided by the 12 cells so .416 amps into each cell, and this device can only discharge 68ma, so it would still be charging the cells regardless of them being 4.12, they'd just get less of a charge.  Even at one amp charging that would be .08amps to a cell and even then the cell would be charging after it had hit 4.2? 
how big a resisitor would I need to never allow a cell over 4.2 and charge at 5 or ten amps?  could I put it on this board?
```

---
## \#11 Posted by: scepterr Posted at: 2017-10-23T05:54:44.497Z Reads: 68

```
It won't go over 4.2 unless/until it heats up enough for something to fail/burn. The idea being you're never so out of balance that it needs to run long enough to burn up... that is why I stopped using it, it can't handle balancing large variations for long. 
New, matched 18650s won't drift apart more than 50-100ma or .005-.02v over hundreds of cycles, assuming all the connections are proper and of equal resistance
```

---
## \#12 Posted by: scepterr Posted at: 2017-10-23T05:57:17.744Z Reads: 65

```
The board kicks in when 1 cell is at 4.2, so you can charge at high amps, problem is how long itll need to balance
Also capacity will determine how quickly the current will drop when charging hits CV stage

It's a lot of balls to keep in the air at once for the whole thing not to go up in flames 😐
```

---
## \#13 Posted by: scepterr Posted at: 2017-10-23T06:03:31.574Z Reads: 61

```
The thru-hole boards are easier to modify if you want to http://batterybms.com/balanceboard/
Ultimately these are relatively simple devices, you could always make a high current PCB that meets your needs
```

---
## \#15 Posted by: Fatos Posted at: 2017-10-23T06:19:13.313Z Reads: 60

```
As written it will '' kind off '' replace one function of BMS. 
In my opinion if this one is not being able to balance your battery cells than you should check your pack. Same Li-ion cells(what I guess most of us has) should not drift so much from each other. Unless something is wrong, or you have a pack of different manufacturers and capacity cell.
Remember that Li-ion batterys have a somewhat flat resistance curve until they are almost fully charged or discharged. It means that while  charging, or discharging the pack you might see some drift wich should minimise itself when you approach 4.2v.
```

---
## \#16 Posted by: Hummie Posted at: 2017-10-23T06:31:34.590Z Reads: 55

```
with the ones I posted here what is meant by operating current?
```

---
## \#17 Posted by: scepterr Posted at: 2017-10-23T06:39:31.495Z Reads: 49

```
http://liionbms.com/php/wp_balance_current.php
```

---
## \#18 Posted by: JdogAwesome Posted at: 2017-10-23T07:39:46.409Z Reads: 46

```
You usually don't need to worry about over charging your cells as long as your PSU is set to the correct max voltage and your cells are balanced, once the cells charge to the same voltage as the PSU they stop drawing current because there at the same voltage difference. If you plan on bypassing the charge and discharge protection of a BMS then yeah just use this it will be smaller and cheaper and work just as well, plus you could add a second one to double balance current if you don't want to swap resistors.
```

---
## \#19 Posted by: PXSS Posted at: 2017-10-23T08:57:26.847Z Reads: 39

```
[quote="Hummie, post:10, topic:36236"]
if the charger were putting out 5 amps, would the math be that's divided by the 12 cells so .416 amps into each cell, and this device can only discharge 68ma, so it
[/quote]

Wrong. That's not how physics works. 

[quote="Hummie"]
Tell me why I shouldn’t just use this for a bms?
[/quote]
Because it is not a BMS. 
A balance board discharges a small amount of energy though a resistor in parallel with the battery. Which means it'll charge slightly slower than the rest. 

A BMS does so much more than that.
```

---
## \#20 Posted by: Fatos Posted at: 2017-10-23T10:11:41.148Z Reads: 35

```
@Hummie @PXSS
If you charge a 12s1p with 5 amps at 50.4V. Ideally, every cell is charged up to 50.4V/12cells=**4.2V each cell**.   
But each of them is still getting charged at a rate of 5Amps(which is a bit too fast for Li-ion) good cells will tolerate that but will degrade faster. 
But I'm guessing you have a  **12s4p** pack and therefor   5A/4cell=**1.25 Amps per each cell**.This is totally accepted and should give you much better life-expectancy of your pack.

This card has one function:
Balancing the pack.And it does it the same way as most BMS do.

BMS will/can (not all of the have all the extra functions ):
Basic:
Overdischarge protection.(Both for whole pack and individual cells)
Overcharge protection.(Both for whole pack and individual cells)
Charge rate protection.(A set MAX of amps).
Discharge rate protection.(A set of MAX amps).
Short circuit protection.
Extra features:
Balancing.
Temperature protection.
Anti-spark switch.
Communincation(bluetoth,I2C and other)

Hope this clears things a bit. As stated before for quality cells of same producer, same type and same age the internal resistance will vary so little that most likely balancing is not a problem. And by that as long as you have a cut off voltage on vesc and a reliable/accurate charger you should be fine with this balancing card. I wold use a fuse in addition to protecting the pack from short circuits. Remember to use a fuse that does allow for those peak amp draws. And an antispark switch or AS-XT90 wold be a good idea also.

@PXSS 
Please correct me if I'm wrong on something.
```

---
## \#21 Posted by: Okami Posted at: 2017-10-23T11:03:23.197Z Reads: 31

```
I was also looking at these modules. Nice that someone also found them and brought this in the forum.

Didnt order anything myself, but report back if you get good results.

And yes, if you got somewhat decent charger, it should go in CV phase and just lower the current at the end of charge cycle, so I assume that should help with balancing and not overstraining anything.
```

---
## \#22 Posted by: lowGuido Posted at: 2017-10-23T12:55:15.231Z Reads: 23

```
This looks like a BMS just like every other BMS except without the FET switching. I see no reason why you wouldn't want to use this.

Its basically the same as buying a low amp BMS and using it for charge only. Except you arent paying for bits you arent using.
```

---
