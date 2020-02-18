# Vesc-x not taking power

### Replies: 11 Views: 340

## \#1 Posted by: Mathias03 Posted at: 2018-04-24T15:12:52.649Z Reads: 85

```
I have a problem with my vesc-x. I just got the drv8302 chip replaced after a failure but now the vesc wont connect to the bldc tool and it does not take power. The lights on the vesc does not turn on either. 

Is the whole vesc shorted?

would love to get som answers
```

---
## \#2 Posted by: banjaxxed Posted at: 2018-04-25T04:32:13.530Z Reads: 75

```
Sounds like a bad repair tbh
```

---
## \#3 Posted by: MysticalDork Posted at: 2018-04-25T05:27:20.898Z Reads: 61

```
Sounds like either the DRV wasn't replaced properly, or something else is fried, maybe the 3.3v regulator. Double-triple-check all your work, under a magnifying glass and strong light, etc.

Look for burn marks or blistering on or around any components. 

Look for solder bridges between pins, and make sure the DRV chip is perfectly aligned with the pads.
```

---
## \#4 Posted by: Mathias03 Posted at: 2018-04-26T13:30:50.897Z Reads: 48

```
doesnt look like anything is fried. but if the drv was porly replaced could this cause the issue?
```

---
## \#5 Posted by: TarzanHBK Posted at: 2018-04-26T13:47:49.423Z Reads: 42

```
could be.
Just contact the person who repaired it, i´m sure he helps you out.
```

---
## \#6 Posted by: SOICDIP Posted at: 2018-04-26T15:29:11.748Z Reads: 37

```
If you have a multimeter, check the voltages on the 3.3V LDO. If you have no 5V input to the LDO, the DRV was soldered poorly, and if there is, there may be a short somewhere else that is pulling the 3.3V down and hence no blue LED. Try to see if anything is heating up, even barely.
```

---
## \#7 Posted by: Mathias03 Posted at: 2018-04-26T15:42:29.376Z Reads: 36

```
Ran into a little bit of a problem here... the drv fell of... what do i do now?
```

---
## \#8 Posted by: RedEagle Posted at: 2018-04-26T16:25:59.902Z Reads: 36

```
Contact the guy who repaired it. Tell him to do a good job this time.
```

---
## \#9 Posted by: SOICDIP Posted at: 2018-04-26T22:13:16.249Z Reads: 32

```
[quote="Mathias03, post:7, topic:53348, full:true"]
Ran into a little bit of a problem here… the drv fell of… what do i do now?
[/quote]

Yeah, the blue LED may not light up in that case. :thinking:
```

---
## \#10 Posted by: MysticalDork Posted at: 2018-04-27T01:24:27.344Z Reads: 26

```
Yeah, if the DRV isn't properly soldered and falls off, you may have problems getting all the functions of your vesc to work correctly.
```

---
## \#11 Posted by: b264 Posted at: 2018-04-27T02:07:13.074Z Reads: 24

```
[quote="Mathias03, post:7, topic:53348"]
the drv fell of
[/quote]

Means the solder paste didn't get hot enough to melt and weld the leads to the pads.  It was essentially stuck to the board with bubble gum.
```

---
