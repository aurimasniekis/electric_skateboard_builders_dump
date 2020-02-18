# Help me troubleshoot weird losses of power

### Replies: 10 Views: 471

## \#1 Posted by: karosass1 Posted at: 2017-10-06T07:04:26.005Z Reads: 78

```
First of all, I shorted my charging port yesterday, probably is the problem, but here're full details of what happened today:

I was going to university, climbing hill and near the top where it gets steeper, my motor didn't have enough power to finish the climb (Which is ok, because it barely would climb it over before), but after it just turned off on a flat, with low-average speed and starting turning off whenever I would put more than 10~20% throttle, using full brakes doesn't cause the shutdown. I put my board on the side and whenever I would put more than same amount of throttle without any load, the board would completely shut off, if I turn it off and on again, it turns on but same happens.

BUT WAIT THERE'S MORE!

With this problem I decided to go home instead of university, hoping I could get home without pushing with super low speed. It worked.. Then midway I tried giving a little bit more power. IT WORKED... Finally on final 500 meters I started doing full stop -> max throttle short sprints. **IT WORKED**. WTF?!!

10s3p 30Q, mono 6374, focbox, 70A besttech BMS, 40A antispark switch
```

---
## \#2 Posted by: ARetardedPillow Posted at: 2017-10-06T07:09:36.288Z Reads: 72

```
Similar thing happened to me, see if you can recreate the problem again and check for faults, and your bms might be fried
```

---
## \#3 Posted by: Jebe Posted at: 2017-10-06T07:16:27.764Z Reads: 65

```
whats your vesc low voltage cut off settings ?
```

---
## \#4 Posted by: karosass1 Posted at: 2017-10-06T07:29:12.213Z Reads: 59

```
cutoff end is 30V

By any chance could the antispark switch somehow be the culprit? Because atm it started not working at all, I turn it on, but vesc doesn't turn on, if I bypass it, and connect discharge plug from bms+battery straight to Vesc - it turns on

Checked the battery, it's at 37.9V, I don't think even with sag it should hit the cutoff
```

---
## \#5 Posted by: karosass1 Posted at: 2017-10-06T07:38:38.431Z Reads: 54

```
Another hint that explains probably why I ran out power when climbing the hill -> Somehow my vesc settings got reset, either I accidentally wrote default ones when I had it connected few days ago or perhaps somehow it got affected and reset when I shorted the charging port?
```

---
## \#6 Posted by: Jebe Posted at: 2017-10-06T07:57:58.806Z Reads: 56

```
sounds like the anti spark is done. I don't use them anymore - mine failed on me first week, replaced the fets and it went again. Loop key is more reliable. Voltage settings sound good.
```

---
## \#7 Posted by: karosass1 Posted at: 2017-10-06T08:37:00.072Z Reads: 53

```
Probably I fried my bms or some weird shit is happening, tried reproducing the problem (without antispark) which was fun, since i dont have bluetooth module and had to ride with laptop in between my legs. At first everything seemed fine, was doing again full stop -> full throttle sprints, after a few i try to do one more, and like 1 seconds after i start accelerating - vesc shut off, bldc tool managed to record the error code just before which was Under_Voltage
https://i.imgur.com/1wr3S1U.png
My guess is that bms is kind of half fried and has random discharge problems?

When standstill battery had 37.2V, last recorded is 6.1V...
```

---
## \#8 Posted by: ARetardedPillow Posted at: 2017-10-06T14:40:40.171Z Reads: 40

```
Yea your antispark is gone, use a loop key for now and check for any loose wires and bad connections that are hot, they drop voltage
```

---
## \#9 Posted by: Jebe Posted at: 2017-10-07T00:35:24.489Z Reads: 35

```
Could be a loose battery cell connection to the BMS dropping it out.
```

---
## \#10 Posted by: karosass1 Posted at: 2017-10-07T12:44:20.598Z Reads: 24

```
I was about to ask if loose balance cables could be the problem, because I just noticed that the plug was barely holding on the port. And as much as I'm testing it now, I can't reproduce it anymore
```

---
