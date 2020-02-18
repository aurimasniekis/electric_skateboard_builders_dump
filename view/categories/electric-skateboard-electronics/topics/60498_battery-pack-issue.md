# Battery Pack Issue

### Replies: 4 Views: 241

## \#1 Posted by: Kit Posted at: 2018-06-30T08:06:07.255Z Reads: 95

```
I made a couple of batt. packs for my CGT, both of which read on a multi-meter at 36V(#1) & 33V(#2) at the power connectors (I am able to power up the ESC just fine here), but they then read at 40V(#1) & 34V(#2) at the charging connectors. Is the latter connector wired wrong? 

Plus, the first batteries charging connector does not seem to actually charge - when I plugged it into the 2A Evolve charger, there is no red charging LED, despite having the multi-meter read at 40V on the charging connector. Would anyone happen to have an idea as to why this wouldn't charge?

@Fiori would you happen to have any insight by any chance?


This current pic I have up is my #2 pack, which I haven't tested charging on due to some concerns about the multi-meter readout I made. It has the 34V readout on the charging connector.
![20180630_012721|666x500](upload://7mrfbQLWhApdsAAFnFUAkZMg3E0.jpg)
```

---
## \#2 Posted by: ARetardedPillow Posted at: 2018-06-30T08:32:03.171Z Reads: 84

```
Maybe your BMS has some problems, howd you wire your charge port?
```

---
## \#3 Posted by: Kit Posted at: 2018-06-30T08:41:26.187Z Reads: 83

```
TBH I'd have to rip open the pack to double-check...it's 1:33am atm so I'll do it after some shut eye methinks. But IIRC, for pack #1, the positive (red 22awg) wire is connected to the same cell/positive terminal as the positive (red 14awg) wire; the last cell. The negative (black 22awg) wire is connected to the BMS. However, if the BMS is the issue, wouldn't that possibly prevent the ESC from powering up?

Also I am comparing #2 to @Fiori's battery build and honestly I may have wired it everything else wrong (shows me for not labeling terminals on the sides..and for working on this at like 1AM...):

![20170929_000020|666x500](upload://eMVTgUXeqQukwbmcJ8ZIBM9hZJZ.jpg)
```

---
## \#4 Posted by: Fiori Posted at: 2018-06-30T14:27:21.556Z Reads: 48

```
Are you still using the evolve BMS and ESC? EDIT: looks like you are. 

The bms may be cutting power to/from the charger if you have the order of the BMS leads wrong.

Pull out the connector for your balance leads and check the voltage at each pin. Leave your negative multimeter lead on the black wire and probe each other wire individually and tell us the values.
```

---
