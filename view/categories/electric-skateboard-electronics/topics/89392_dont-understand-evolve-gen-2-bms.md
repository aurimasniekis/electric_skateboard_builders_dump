# Dont understand Evolve Gen 2 bms

### Replies: 20 Views: 347

## \#1 Posted by: AdamE3399 Posted at: 2019-04-04T22:43:28.120Z Reads: 106

```
![20190405_073651|281x500](upload://d3bmsWUqptcMLHfXEFUm9hfoQAV.jpeg) 
Anyone know what the white wires are for?
```

---
## \#2 Posted by: b264 Posted at: 2019-04-04T22:44:08.483Z Reads: 100

```
I don't have one of those, but I'll toss a guess out there, that they are for a temperature sensor.  One that would be inside the battery somewhere.
```

---
## \#3 Posted by: AdamE3399 Posted at: 2019-04-04T23:09:22.770Z Reads: 93

```
If this was the case would it be essential i wire it?
```

---
## \#4 Posted by: AdamE3399 Posted at: 2019-04-05T03:58:21.678Z Reads: 86

```
Would i have to add the sensor in order for this to work or would it work without being wired?
```

---
## \#5 Posted by: AlexBE Posted at: 2019-04-05T04:09:20.022Z Reads: 78

```
Maybe for a deleted power switch? On mine, those wires are not present. The pads are still there though.
```

---
## \#6 Posted by: AdamE3399 Posted at: 2019-04-05T04:21:36.363Z Reads: 76

```
Did it work fine without using them?
```

---
## \#7 Posted by: AlexBE Posted at: 2019-04-05T07:23:20.602Z Reads: 67

```
Well yes, because those wires don't exist on mine. It might be for a battery temperature sensor that was deleted from the product. Only one way to find out if it works without them.......
```

---
## \#8 Posted by: AdamE3399 Posted at: 2019-04-05T11:05:47.116Z Reads: 58

```
So i ended wiring up the new battery with the bms, battery negative, power negative, charge port negative, charge port positive and the balance leads and the esc works and the board charges but the bms gets extremley hot and stopa charging after 30 zeconds, anyone know why?
```

---
## \#9 Posted by: olestra Posted at: 2019-04-05T15:24:39.505Z Reads: 46

```
cells are out of balance, and the BMS needs a heat sink?
```

---
## \#10 Posted by: AdamE3399 Posted at: 2019-04-05T21:32:33.655Z Reads: 40

```
Brand new batt so all cells are balanced and it originally didnt have a heatsink and didnt get hot so i have no idea whats causing this
```

---
## \#11 Posted by: AdamE3399 Posted at: 2019-04-05T21:42:06.193Z Reads: 40

```
I opened up the old battery and found that it was a temp sensore, could this not being plugged in cause the bms to overheat?
```

---
## \#12 Posted by: AlexBE Posted at: 2019-04-08T04:24:59.501Z Reads: 29

```
I doubt it. Maybe post a wiring diagram, detailed photos and try to determine exactly which part is getting hot. Then I might be able to diagnose it for you.
```

---
## \#13 Posted by: AdamE3399 Posted at: 2019-04-08T07:11:40.958Z Reads: 26

```
So i have outlined the part of the bms that gets real hot, my c- is charge port negative, positive charge port is positive battery, b- is battery negative and my balance leads are sequential and correct and so i have no idea why its getting so hot and shutting down
```

---
## \#15 Posted by: AdamE3399 Posted at: 2019-04-08T07:14:37.919Z Reads: 26

```
![20190408_171401|281x500](upload://o7mSvqrOghDx2H2j95tjlcTxq0z.jpeg)
```

---
## \#16 Posted by: AlexBE Posted at: 2019-04-08T08:19:23.094Z Reads: 23

```
Is the thick red wire you have connected to B- your negative battery lead? You really need to take proper photos and draw diagrams, its impossible to help when you don't show where the leads go. Ie you say you have B- connected to battery negative, but it's better to just show that. These problems are 95% of the time due to silly mistakes and other people can spot that for you.

edit: having another look at your photo, pretty sure you have battery -ve connected in the wrong place, but its impossible to tell.
edit2: by the way, the bottom left of the board with the three large resistors, that is B-. The label might be on the other side of the board.
```

---
## \#17 Posted by: AdamE3399 Posted at: 2019-04-09T05:14:14.633Z Reads: 19

```
Sorry about that i have tried to include a more detailed diagram and yes that is b-, it is red wire cause that all i had.![diagram|484x500](upload://1Zjxs7PFYJ67CYCljPosofyGMbN.jpeg)
```

---
## \#18 Posted by: AlexBE Posted at: 2019-04-09T08:32:13.895Z Reads: 16

```
Do you have a multimeter? If so, measure the voltage between the CH- and B- while you are charging.
```

---
## \#19 Posted by: AdamE3399 Posted at: 2019-04-09T10:03:33.317Z Reads: 14

```
I actually ended up changing out the bms for another 10s bms i had laying around and it is now working though i am bypassimg discharge and am wondering whether the esc in the gen 2 will cut off the battery at 3.2v or not, do you happen to know? If not i will have to discharge through
```

---
## \#20 Posted by: AlexBE Posted at: 2019-04-10T01:18:10.756Z Reads: 12

```
No sorry I don't know what the ESC does regarding cutoff. If it does cutoff, it does it at a lower voltage than the BMS, which is a huge design flaw, definitely want to bypass discharge. I swapped all my evolve electronics out because I don't believe they are safe.
```

---
## \#21 Posted by: AdamE3399 Posted at: 2019-04-10T05:17:00.935Z Reads: 13

```
Thats all good, i ended up discharging througb the new bms and all is working fine so im happy
```

---
