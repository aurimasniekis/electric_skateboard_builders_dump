# Over voltage fault. Stuttering

### Replies: 10 Views: 729

## \#1 Posted by: pshaw Posted at: 2017-09-26T01:37:05.399Z Reads: 82

```
So I have been getting over voltage faults and my limit is set at 57v (12s). Every time it happens i have no power or brakes for 3 seconds then I have power again. 

When I accelerate I get under voltage faults and the same thing happens... no power or brakes for 3 seconds. Sometimes it happens under hard accel and other times it is just when cruising and not pushing the board at all.

Any suggestions? I took a look at the battery and all the inidiviual cells are within .01 voltage of each other so they are discharging evenly. 

Help :/
```

---
## \#2 Posted by: scepterr Posted at: 2017-09-26T01:37:58.088Z Reads: 80

```
Post all your details , battery, motor, bldc screenshots
```

---
## \#3 Posted by: pshaw Posted at: 2017-09-26T01:41:07.703Z Reads: 78

```
battery 12s4p 30q. motor dual 6374 190kv. vesc 4.12. working on screenshots.

I will tell you when I check the imetr app and look at the logs when the over voltage fault happens it is nowhere near 57v... usually under 50v actually. Now i do realize maybe an instantaneous spike might trigger the esc to cut to protect itself however not actually show up in the log.
```

---
## \#4 Posted by: SORRENTINO Posted at: 2017-09-26T01:52:22.060Z Reads: 75

```
You mean over voltage not over current?
```

---
## \#5 Posted by: pshaw Posted at: 2017-09-26T02:02:50.733Z Reads: 72

```
thx i corrected it
```

---
## \#6 Posted by: scepterr Posted at: 2017-09-26T02:20:07.176Z Reads: 72

```
What vesc do you have ?
```

---
## \#7 Posted by: Jinra Posted at: 2017-09-26T02:41:56.635Z Reads: 73

```
You say you corrected it, but I still see you saying "over voltage" in the OP and "over current" in your first reply.

Post screenshots of the fault!
```

---
## \#8 Posted by: Deckoz Posted at: 2017-09-26T03:14:44.998Z Reads: 72

```
Basically, 

-we checked all the wiring & solder joints
-vescs are fine 
-BMS is bypassed for discharge so not bms
-loop key was replaced
-12s4p is perfectly balanced within .01~

The board rides fine when I'm on it (I'm 127lbs), where when pshaw rides it,(180lbs~) it undervolts and overvolts. I'm thinking that there is a weak series connection in the battery. The board has never acted like this before. I think @pshaw is gonna check the series connections when he can open it up again. But I'm also suggesting we test with another battery to confirm its either the power system or the battery to isolate the issue further, if nothing is discovered from a reinspection of the series connections on the board.
```

---
## \#9 Posted by: Jinra Posted at: 2017-09-26T03:44:25.568Z Reads: 73

```
yea, perhaps one of the series is connection is worn out due to the board flex and the segmented parallel groups. I wouldn't be surprised if the wire connecting it is frayed and is intermittently connecting.
```

---
## \#11 Posted by: Deckoz Posted at: 2017-09-26T17:48:11.875Z Reads: 63

```
Hahaha I think we found the issue :joy:

<img src="/uploads/db1493/original/3X/d/3/d3dd2a680a4611f47f96e1dc6c47838f456f2f73.jpeg" width="281" height="500">
```

---
