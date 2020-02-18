# Power draw of Anti Spark when off \[Update: Battery losing charge on its own\]

### Replies: 19 Views: 860

## \#1 Posted by: jimbosays Posted at: 2017-04-24T20:10:23.994Z Reads: 132

```
Hi All, I recently changed switches from a circuit breaker to Vlad's anti-spark switch. It works great, but I noticed that even when the switch is off, the anti-spark draws 1.3 Amps. When I turn the switch on, I get the same load at ~1.3 Amps on my voltmeter. Since I didn't have an issue with power leakage with the circuit breaker switch, my question is how do I get the Anti-spark to stop drawing power when the system isn't on. Currently it seems like it would unnecessarily put more cycles on my battery pack from idle discharging unless I physically disconnected the anti-spark from the pack every time. Thanks!
```

---
## \#2 Posted by: goldenHusky Posted at: 2017-04-24T21:29:34.383Z Reads: 118

```
Could you please link his topic or provide some pictures/ schematics etc.? 
I don't know his switch but it sounds like the Gates of the Mosfets do not get pulled down properly.
```

---
## \#3 Posted by: TarzanHBK Posted at: 2017-04-24T21:57:44.047Z Reads: 114

```
I do have the same problem with my BMS E-switch. 2,5V when it´s off, everything else seems cool..
```

---
## \#4 Posted by: sl33py Posted at: 2017-04-24T22:22:30.061Z Reads: 108

```
Sounds like a failed Mosfet to me.  Typically they seem to fail "open" which can pass current.  I'll see if i can measure my on and off voltage on one i have to compare.
```

---
## \#5 Posted by: laurnts Posted at: 2017-04-24T22:43:23.863Z Reads: 96

```
I believe an antispark switch its self is a load. It's just a relay and a relay requires energy to operate at time they are triggered. But it should take a very low amount of energy and not constantly drawing power for more than an amp (which is strange).
```

---
## \#6 Posted by: jimbosays Posted at: 2017-04-24T22:44:03.071Z Reads: 93

```
So I disconnected my pack and it turns out that load is not from the e-switch entirely. On just the pack alone, the voltmeter shows a 1.3 A draw. Didn't think I had this issue on my pack before, but I recently had to rewire the BMS. The BMS works fine, but not sure why there would be that draw when disconnected. Or is this this draw just the result of the voltmeter measuring the internal resistance of the pack? 

I'll leave my pack alone for a day or two and see if the voltage drops on its own. The A123 cells have a flatter discharge curve than 18650's so it might be awhile to notice a difference if there is one (when connected to the e-switch; pack voltage would drop overnight from 42V to ~41.7V)
```

---
## \#7 Posted by: laurnts Posted at: 2017-04-24T22:53:37.421Z Reads: 88

```
Remember that amp measurement can only be taken if the circuit is closed with a load. You can't measure amp draw the way you measure voltage.
```

---
## \#8 Posted by: Namasaki Posted at: 2017-04-25T00:25:59.227Z Reads: 80

```
[quote="TarzanHBK, post:3, topic:21703, full:true"]
I do have the same problem with my BMS E-switch. 2,5V when it´s off, everything else seems cool..
[/quote]

I have also noticed this on the Bestech BMS's. 2.5v when it's off. The current draw is extremely  low so it hasn't been an issue for me.
I think if you where going to store your board for a long time, you probably should disconnect the battery from the system.
But for everyday use, its fine.

<img src="/uploads/db1493/original/3X/2/d/2d5f41da47bf88ec13bd5dc5ca94aae0ca5e32ff.png" width="547" height="109">

It's lower than I thought, only 20 microamps
```

---
## \#9 Posted by: whitepony Posted at: 2017-04-25T00:53:45.406Z Reads: 78

```
[quote="jimbosays, post:6, topic:21703"]
when connected to the e-switch; pack voltage would drop overnight from 42V to ~41.7V
[/quote]

im with @sl33py - think the switch is broken and your whole setup is always on as default setting for broken switches. its how I nearly killed a battery and its when I decided I like simple loop keys a lot more!
```

---
## \#10 Posted by: jimbosays Posted at: 2017-04-25T00:56:30.891Z Reads: 70

```
So it might be the switch, but in the last 2-3 hours, my pack went from 42.1V to 41.8V while not being connected to anything other than the BMS. Is this normal? I have a 12S 26650 A123 LiFePo4 pack with a charger that stops at 42.1V
```

---
## \#11 Posted by: whitepony Posted at: 2017-04-25T00:59:06.920Z Reads: 67

```
oh, thought it was connected. no, thats not normal :grimacing: my batteries didnt even drop 0.1V during the whole 5month winter sleep. wonder what the bms could be doing? :thinking:
```

---
## \#12 Posted by: jimbosays Posted at: 2017-04-25T00:59:51.529Z Reads: 65

```
this BMS is hooked up to the pack: 

http://www.ebay.com/itm/12s-15A-Battery-Protection-BMS-PCB-Board-for-12-Packs-36V-LiFePO4-Cell-w-Balance-/331884003288?hash=item4d45d3ffd8:g:AOgAAOSwjXRXY85t
```

---
## \#13 Posted by: jimbosays Posted at: 2017-04-25T01:02:36.963Z Reads: 58

```
I thought at first that it was the e-switch that caused the problem, but I've managed to isolate the issue past the e-switch and to the pack itself.
```

---
## \#14 Posted by: Namasaki Posted at: 2017-04-25T05:08:12.745Z Reads: 55

```
This sounds like another good reason to not use cheap generic bms's from eBay.
```

---
## \#15 Posted by: Namasaki Posted at: 2017-04-25T05:12:21.221Z Reads: 54

```
Disconnect the bms then check the pack voltage after a few hours to verify but I think the bms is draining your battery.
```

---
## \#16 Posted by: jimbosays Posted at: 2017-04-25T05:47:15.313Z Reads: 54

```
haha i ordered an Supower BMS that is on its way. I had this pack built and this is the BMS it came with
```

---
## \#17 Posted by: jimbosays Posted at: 2017-04-26T00:39:27.536Z Reads: 45

```
So it turns out to be worse than i expected. After measuring the voltages of individual cells (between b2 and b3 for example), all my cells are at ~3.4. However, measuring between the two b1's i get 3.9v. This is also the measurement that fluctuates the most when the pack is left at idle. Does that mean the first series is i) overcharged and ii) the bms is broken and only seems to charge the first cell to achieve the target voltage of 42V? @laurnts I'd appreciate your input as you seem to know a lot about electronics :)

<img src="/uploads/db1493/original/3X/3/2/32d454a66974f826d9c7291db0a914862b8b613d.jpg" width="375" height="500">
```

---
## \#18 Posted by: laurnts Posted at: 2017-04-26T16:55:18.353Z Reads: 40

```
The way bms works is by overcharging (CMIIW). The bms cant measure per cell voltage (only the first cell group), the rest is measured by accumulative voltage. So incase of 10s, first is 3.6, second is 7.2, third is 10.8 and so on...

When the bms detect 3.6 for the first cell, it start to switch filling the other ones until the ideal voltage of each s is achieved.

It's kinda hard to tell which cell groups didnt work or if the bms is faulty. You kinda have to take them apart and test separately.
```

---
## \#19 Posted by: mccloed Posted at: 2017-04-26T17:03:17.310Z Reads: 37

```
Hey @jimbosays, I used that same BMS and had two cells die on my 10s battery. I removed that BMS and changed the cells and now have zero issues. I would suggest a different BMS.
```

---
