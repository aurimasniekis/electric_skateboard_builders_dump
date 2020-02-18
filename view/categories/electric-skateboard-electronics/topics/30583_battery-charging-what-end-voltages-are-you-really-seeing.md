# Battery Charging. What End Voltages are you Really Seeing?

### Replies: 11 Views: 619

## \#1 Posted by: pshaw Posted at: 2017-08-14T14:18:54.646Z Reads: 105

```
My setup is a 12s4p using samsung 30q. The charger I have is in the link below. Fully charged would be 50.4 volts but I can't get it charged past 49.3v which equates to 4.1 per cell instead of 4.2 per cell. I'm using a 12S BMS as well that is supposed to balance to 4.20v per cell. The end of the charge plug is showing 50.6v with the multimeter. What gives?

http://www.batterysupports.com/432v-44v-504v-4a-lithium-ion-lipo-battery-charger-12s-12x-36v-p-167.html
```

---
## \#2 Posted by: Jinra Posted at: 2017-08-14T14:35:58.206Z Reads: 102

```
Check every cell group's voltage. Likely one of them hit max voltage and the bms cut off charging to protect the group
```

---
## \#3 Posted by: pshaw Posted at: 2017-08-14T14:37:53.063Z Reads: 100

```
@Jinra  They are all the same within .01 of each other. Do you have a 12S rig? If so what is your final voltage typically?
```

---
## \#4 Posted by: Jinra Posted at: 2017-08-14T14:51:45.885Z Reads: 90

```
I have 10s, but have experienced the same problem as you. However mine were because of two various reasons.

1. It was as i suggested and 1 group was at 4.22v compared to 4.05 of the rest.

2. The second time it happened was because i didn't plug in the main battery negative (because i was not discharging through the bms). Apparently this was important for balancing as well.
```

---
## \#5 Posted by: pshaw Posted at: 2017-08-14T14:57:14.563Z Reads: 84

```
What did you do to fix the issue the first time? 

Right now I think I two wires coming off BMS (not including balance leads). One goes to negative main side the other goes to positive main side. Is this what you are referring to being the correct way to have it wired?
```

---
## \#6 Posted by: Jinra Posted at: 2017-08-14T15:05:59.434Z Reads: 79

```
The first issue was one of the cells in the parallel group wasn't connect so it charged/discharged faster than the rest. Solution was to reattach the cell, discharge to below the overcharge release voltage, then charge up again.

I think the SUPower BMS's are different. My Bestech BMS had a B- for the balance lead **and** a B- main on the PCB. For this reason I thought I only needed to plug int he B- on the balance header for balancing. However, I don't think Supower has a B- on the balance header so you need to plug B- on the PCB anyway.. Sorry I can't be more helpful.
```

---
## \#7 Posted by: treenutter Posted at: 2017-08-14T15:15:35.597Z Reads: 73

```
[quote="pshaw, post:1, topic:30583"]
I can't get it charged past 49.3v which equates to 4.1 per cell instead of 4.2 per cell
[/quote]


@pshaw While it's perplexing that it is happening, many folks prefer to limit max charge to 4.1V to increase cell longevity and to give some overhead for when battery regen kicks in. So maybe this a feature instead of a problem? 

Doesn't seem like you get much between 4.2V and 4.1V in terms of riding time, look at the discharge curve:

http://budgetlightforum.com/node/42075
```

---
## \#8 Posted by: Jinra Posted at: 2017-08-14T15:21:08.470Z Reads: 68

```
There's something that can happen where all cell groups are reading the same voltage, but the overcharge detection kicked in anyway. For me, this was due to to a loose cell in a group, but wasn't loose enough to be completely disconnected. The 3 other cells charged to max triggering OC detection, but then slowly charged the loose cell as it wasn't completely disconnected.

This may be difficult to visualize, but TL;DR check the connects of all your cells.
```

---
## \#9 Posted by: pshaw Posted at: 2017-08-14T16:27:19.231Z Reads: 60

```
Thanks for all the help guys. The chart was a really good visualization. Looks like from 4.1 to 4.2 you lose maybe 50mah. So about 1-2% of your range if I'm reading it correctly hah
```

---
## \#10 Posted by: Randyc1 Posted at: 2017-08-14T18:23:22.915Z Reads: 55

```
Check Voltage directly at charger's Plug ?
```

---
## \#11 Posted by: pshaw Posted at: 2017-08-15T04:13:14.552Z Reads: 39

```
50.6v at plug
```

---
