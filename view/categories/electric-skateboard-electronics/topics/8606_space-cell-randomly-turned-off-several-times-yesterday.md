# Space Cell Randomly turned off several times yesterday?

### Replies: 6 Views: 494

## \#1 Posted by: michaelcpg Posted at: 2016-08-29T22:21:44.245Z Reads: 78

```
Hey guys,
I was riding home from work yesterday and found my older space cell which I've since upgraded to a 4P pack (the version with 50A BMS) completely shut off several times. Each time it occurred while I was mildly accelerating and low speeds (ie. not much faster than walking speed). 

In total, it happened 4 times within a matter of ~10 minutes, each time while I was riding on the flat. After this I managed to continue riding the rest of the way home without any more issues which is about 5km with several large uphill sections, one of which is over 1km long.

I'm assuming it's an issue with the battery/BMS and not my VESC because I completely lost power and the LCD battery meter turned off until I flicked the power switch off and on again which would solve the issue.

From memory these are my VESc settings:
Motor Max: 60A
Motor Min: -60A
Batt Max: 40A
Batt Min: -15A
Absolute Max: 130A

Min Input Voltage: 8V
Max Input Voltage: 50V
Battery Cutoff Start: 33V
Battery Cutoff End: 28V


From memory, these are the only settings I've changed other than for setting up my remote.
At the time, my battery was on around 60% - 70% so I don't expect it would be a result of the low voltage cutoff kicking in.

Here's my board main specs:
Enertion 6374 Motor
10S4P Space Cell
Ollin VESC
GT2B

Hopefully somebody has an idea as to what might be going on, let me know if you need any more info.
Cheers
```

---
## \#2 Posted by: JohnnyMeduse Posted at: 2016-08-30T01:12:27.497Z Reads: 62

```
That really sound like low voltage cutoff... You probably have a broken cell... Or a unbalance one (yep, cell balancing are optional on some BMS).

OR this could just be a cold solder joint on one of the cell lead.
```

---
## \#3 Posted by: michaelcpg Posted at: 2016-08-30T01:17:30.986Z Reads: 61

```
That's something I forgot to mention actually. When I got home I checked the battery cells and noticed that one of the fuse wires on one of my cells had broken, likely just from vibration as the cells aren't secured as well as I like atm (current waiting on parts so I can better secure the cells). 

So you reckon a single cell disconnecting from one of the parallel packs could have that effect?
I remember when testing cell voltage when I got home that all of my cells were at 3.69V apart from the disconnected one which was at 3.8V.
```

---
## \#4 Posted by: JohnnyMeduse Posted at: 2016-08-30T01:18:57.499Z Reads: 58

```
yes, in fact it is the bms getting in UnderVoltage state.

And it should stop the power to the output... so your BMS is working good.
```

---
## \#5 Posted by: onloop Posted at: 2016-08-30T01:48:35.692Z Reads: 55

```
[quote="michaelcpg, post:3, topic:8606"]
So you reckon a single cell disconnecting from one of the parallel packs could have that effect?
[/quote]

YES, this is definitely a reason for it to cut out. Is your deck flexy? flexion is a big battery killer....

you should be able to fix this with some wire & solder.
```

---
## \#6 Posted by: michaelcpg Posted at: 2016-08-30T01:55:33.872Z Reads: 52

```
Thanks for the replies guys. I'm surprised that the voltage could drop so much just from a single cell being disconnected.
It's all fixed now. 

My deck is rigid, I believe it's more general vibrations on rougher roads that cause the fuse wires to break. Currently my cells are just hot glued together so if they become unstuck, they become able to move ever so slightly which obviously isn't great for fuse wires.

I'm looking to use cell holders that @chaka has designed to properly secure my cells so hopefully this wont be an issue for much longer :)
```

---
