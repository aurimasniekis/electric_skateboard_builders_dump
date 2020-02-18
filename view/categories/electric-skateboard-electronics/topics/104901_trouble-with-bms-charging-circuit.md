# Trouble with BMS charging circuit

### Replies: 3 Views: 86

## \#1 Posted by: Ashwc Posted at: 2019-12-23T09:54:01.140Z Reads: 20

```
![bms%20thing2|666x500](upload://tAbn3EjnoMZlMZGOqclY4R68Z3A.jpeg) 

I've tried to hook up the charging circuit on my first build, but I think I may have screwed something up. I'm going off this image for the wiring-  ![image|670x500](upload://7Se2Jd9X4Qm7WZy4Q6euzHWUzri.jpeg)   I've got the battery's negative to B-, and I should be able to power things and charge off P- and the battery's positive side, but when I tried to solder on a step-down converter the battery shorted and i got a bunch of sparks. whats going on here? I'm getting 49ish volts between the battery's positive and the positive side of my step-down converter. (or p-) is this normal and should I continue with soldering on a charge port and more loads like the wiring diagram says, or is something wrong? thanks
```

---
## \#2 Posted by: Tinp123 Posted at: 2019-12-23T11:38:56.565Z Reads: 17

```
please don't take offense, but you have so many exposed wires and pcb that this looks like bomb, please do not close your enclosure and ride like that before isolating everything. you will most certain get fire. 

![cf56219f2d41f4d85a605c36beb0282a7dd05252|666x500](upload://mgLyB47lVivtpHRPNLu7iJp29oP.jpeg) 

if you wired everything like on diagram, did you check voltages between P- from bms and battery main positive first? you should do that before soldering any step down or anything else. if your voltage there is right, you can proceed. step down can be soldered parallel with charging port and with load. 

what is discharge rate of your bms? looking at wires, they look thin and I know Daly never saves on wire thickness.
```

---
## \#3 Posted by: Ashwc Posted at: 2019-12-23T20:38:25.561Z Reads: 11

```
Thanks! I'll definitely isolate everything before riding. The voltage between p- and the battery's positive was like 49v I think, but is was also 49v from the positive side of the step down to p-.
I'm going to try to bypass the bms for discharge like in this thread- https://www.electric-skateboard.builders/t/solved-wiring-bms-bypass-discharge-10s-anti-spark-help-please/27876
So this bms is very low amperage. I think it's like 15a, and I'm just using it for a little USB charging circuit and lights
```

---
