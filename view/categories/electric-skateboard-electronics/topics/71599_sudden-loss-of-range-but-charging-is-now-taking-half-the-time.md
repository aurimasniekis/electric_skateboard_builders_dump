# Sudden loss of range, but charging is now taking half the time

### Replies: 13 Views: 266

## \#1 Posted by: itsmikeholland Posted at: 2018-10-18T01:20:02.279Z Reads: 135

```
Hi guys! I have a 4.12 @chaka vesc from almost 3 years ago, running a 14 month old 10s4p 30q and usually get 20+ miles out of my board, but now after a week of not riding Im suddenly barely getting 5 miles with the same 32v cutoff, but my 2a charger is shutting off after 45ish minutes vs the usual 1.5 hour charge. 

I changed the cutoff to 30v before the ride im on now and have noticed it hasnt gone into its low-performance mode when it did yesterday and earlier today, im charging it at a mall now to ensure I can get home tonight so no full range test at the new cutoff..

Any ideas? Is this something a new DRV would fix? Id chalk it up to old batteries but the shorter charging time makes me think that something else is up..

Thanks team! Looking forward to the discussion!
```

---
## \#2 Posted by: mmaner Posted at: 2018-10-18T01:29:52.935Z Reads: 128

```
I would check the negative legs between your P groups.
```

---
## \#3 Posted by: ElectricCoast Posted at: 2018-10-18T01:37:24.019Z Reads: 125

```
yeah i'd agree with mmaner on this one.  Pretty sure you have lost a p group.
```

---
## \#4 Posted by: itsmikeholland Posted at: 2018-10-18T01:46:12.961Z Reads: 119

```
I think that might be a little out of my skill level, is it going to be dangerous charging the battery in the meantime if I'm missing a Parallel Group?

I'm eventually going to learn how to build a battery pack but right now I just don't have the equipment to put it back together if I did in fact lose a group
```

---
## \#5 Posted by: mmaner Posted at: 2018-10-18T01:47:56.833Z Reads: 109

```
It ain't good 😀.

Is your voltage correct at full charge and cutoff?  Can you see the different groups through the heat shrink?
```

---
## \#6 Posted by: Goonman Posted at: 2018-10-18T01:51:54.711Z Reads: 101

```
I'd say you lost a series group as well. Crack it open and have look. Discharge it and be ginger careful.
```

---
## \#7 Posted by: b264 Posted at: 2018-10-18T01:54:11.292Z Reads: 93

```
[quote="Goonman, post:6, topic:71599"]
Discharge it
[/quote]

Monitor the individual P-packs while slowly discharging.  If one is moving faster, investigate that one more.  Are all the cells at the same voltage in the P-pack?
```

---
## \#8 Posted by: torqueboards Posted at: 2018-10-18T02:25:10.677Z Reads: 92

```
Yeah, most likely you have one P group that has a lower overall voltage to your other P groups. So your voltage drops quickly.
```

---
## \#9 Posted by: ARetardedPillow Posted at: 2018-10-18T05:41:10.892Z Reads: 73

```
Check the output voltage of the charger
```

---
## \#10 Posted by: Eboosted Posted at: 2018-10-18T06:02:51.959Z Reads: 67

```
Stop charging your board immediately, open the battery pack and meassure the voltage of each P-Group. Report back
```

---
## \#11 Posted by: Sebike Posted at: 2018-10-18T06:53:52.482Z Reads: 54

```
If he lost a series group battery would read zero voltage...

Sounds like cells are lost in parallel (bad/lost connection /bad cell) and I would neither run or charge this board until I had located and fixed whatever is faulty.

Also, I'd check the individual parallel packs to see if they are out of balance.
```

---
## \#12 Posted by: dareno Posted at: 2018-10-18T10:57:24.626Z Reads: 47

```
Sounds to me like batteries are above your skill level and thats fine.  I would suggest starting a new thread to find someone local that can assess the issue and repair it for you.  In the mean time do as you've been advised and do not use/charge it further.  Good luck with it man.
```

---
## \#13 Posted by: itsmikeholland Posted at: 2018-10-18T16:21:38.587Z Reads: 37

```
Thank you! I'll start a new thread
```

---
