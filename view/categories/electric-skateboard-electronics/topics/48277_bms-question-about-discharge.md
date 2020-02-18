# BMS question about discharge

### Replies: 16 Views: 2233

## \#1 Posted by: Strykerpm Posted at: 2018-03-06T04:41:24.467Z Reads: 196

```
So Im trying to round out my parts list for my first build one thing im not clear on is what is the advantage of having a BMS that can discharge the battery? In my mind riding the board does that? Is there a reason for cleaning your battery pack other than by riding it? 

BTW I was origionally planing on running a 10s2p or 12s2p but it seems most people feel that that would not be quite enough for a 6374 190kv motor? this would be a secondary question that any input is welcome.
```

---
## \#2 Posted by: Ishayc Posted at: 2018-03-06T05:57:54.487Z Reads: 189

```
Never heard of a bms that discharges the battery completely. 
When you charge the battery to full the bms discharges some of the cells to get them balanced.
You can discharge through a bms to protect your battery from overdischarge but your esc should be able to do that as well.
```

---
## \#3 Posted by: Acido Posted at: 2018-03-06T06:01:07.048Z Reads: 182

```
You can also go super low with liion like 2.6v
```

---
## \#4 Posted by: Deckoz Posted at: 2018-03-06T07:02:50.753Z Reads: 176

```
Not recommended. Amps fall off and heat increases below 3.35 on most cells we use...
```

---
## \#5 Posted by: Frank Posted at: 2018-03-06T07:46:12.895Z Reads: 168

```
not exactly true. Your ESC can only "see" your pack voltage. That works fine when your pack is in balance yes but when it is unbalanced you can damage your pack.

for example, 1 cell is 3.2v(let say empty) and one is 4.2v(a little extreme but you get the point). Your ESC will "think" your pack is 3.7v per cell. Not empty at all but in fact, one cell is empty(3.2v) and will be damaged when you discharge it more. A BMS will notice that one cell is empty and will therefore take action(by shutting down).

i know this is a little extreme and you already have a problem when you pack is this unbalanced.
```

---
## \#6 Posted by: Ishayc Posted at: 2018-03-06T08:25:52.713Z Reads: 158

```
Yup, it’s extreme.
The bms will not balance your cells during the charge in that situation.
I always discharge my batteries through the bms but I pay more to get a high discharge current bms.
```

---
## \#7 Posted by: Namasaki Posted at: 2018-03-06T16:12:51.497Z Reads: 149

```
Although what @Frank  said may sound extreme it is actually very possible. 
If welds within a parallel group break loose because of vibration caused by rough road conditions or by flexing with a deck that isn’t quite stiff enough. 
That parallel group will have only partial capacity and discharge current capability and will discharge much faster than the rest of the pack. 
All the while fooling the Vesc low voltage protection until it’s too late and the cells are damaged or worse. 
This type of failure is no myth, it has happened and in some cases the results where catastrophic.

Since a bms will monitor each group individually, it will catch such a situation before it goes too far.
```

---
## \#8 Posted by: Ishayc Posted at: 2018-03-06T18:44:49.761Z Reads: 144

```
Well that’s why I discharge through the bms.
Actually a soldering joint in my old board broke and disconnected a whole cell. The bms cut me off so I figured the problem in no time.
```

---
## \#9 Posted by: Strykerpm Posted at: 2018-03-08T06:20:44.616Z Reads: 127

```
So humor me a little.  Normal riding you plug in your charger and the BMS charges your pack. I think I understand that if there is a faulty cell the bms will cut off the power? But what about normal operation? I.e. charge ride then what? How do you have the BMS discharge?  Do you do this every cycle?
```

---
## \#10 Posted by: ZackoryCramer Posted at: 2018-03-08T06:28:05.414Z Reads: 120

```
BMS when used for discharge and charge acts as an intermediary that protects the cells and balance them. They will cut output/input when one cells is out of norms(under or over voltage) or if the whole pack is using more than the rated amp output/input. Other than that they consume a small amount of power for the circuit.
```

---
## \#11 Posted by: Strykerpm Posted at: 2018-03-09T05:18:31.312Z Reads: 108

```
So passive interaction.  But ones that don't discharge won't level/equal out a battery pack.
```

---
## \#12 Posted by: ZackoryCramer Posted at: 2018-03-09T05:21:26.505Z Reads: 108

```
Even if they don't discharge I am pretty sure they will still balance. :grinning:
```

---
## \#13 Posted by: Strykerpm Posted at: 2018-03-09T05:24:03.183Z Reads: 106

```
Lol so back to my original question why do I see some bms saying charge only?  And if I get one that does both what is the benifit?
```

---
## \#14 Posted by: Strykerpm Posted at: 2018-03-09T05:24:58.220Z Reads: 101

```
Honesty just trying to understand this segment more.
```

---
## \#15 Posted by: ZackoryCramer Posted at: 2018-03-09T05:26:45.255Z Reads: 104

```
They really just have a discharge rate too low to be practical for esk8 purposes.

Pro of discharge/charge BMS:
-low cell voltage cut
-individual cell voltage detection

Pro of charge-only BMS:
-no needs to pay twice the price for high discharge rate
-no over-charge cut to leave you break-less down a hill when fully charged
-can use vesc settings to protect low voltage
```

---
## \#16 Posted by: Mrpow124 Posted at: 2018-10-21T03:51:15.065Z Reads: 77

```
Not that I know a lot but I'm learning.  I'm thinking the best cheap/reliable  option is a bms for charging only and some cheap 8s rc cell voltage monitor alarms.
I think that for long term battery life. Active cell balancing from the bms on discharge with no current limit cuts sounds ideal. Then just a cell alarm if it all goes majorly out of balance. 
I'M thinking I would rather break a cell or 2 then lose power or brakes. Just my 10pence worth alarms are £2 on eBay.
```

---
