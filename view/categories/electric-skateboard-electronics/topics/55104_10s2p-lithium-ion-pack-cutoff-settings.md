# 10s2p lithium ion pack cutoff settings

### Replies: 9 Views: 513

## \#1 Posted by: Michaelj1 Posted at: 2018-05-11T13:32:11.067Z Reads: 106

```
I recently switched to the new vesc tool and I noticed that it automatically sets the cutoff end for my batteries at 3.1v. The guy who sold me the battery said to set it to 3.3v, but what should my cutoff start be set to? I don’t want to damage my battery and I read from some people that 3.1v is dangerously low because of voltage sag
```

---
## \#2 Posted by: E1Allen Posted at: 2018-05-11T13:47:35.932Z Reads: 101

```
I've set my end to 3.0v per cell and my start to 3.1v per cell.  I use 30q.  I'm not sure what battery you have but the higher cutoff he recommended would be to prolong battery life.  In the vesc when you request more than the battery can deliver it reduces it's output to maintain a constant battery voltage.  So under heavy loads with a mostly depleted battery it should maintain the constant voltage so to not kill your battery.  Nothing wrong with adjusting to the recommended cutoffs from your battery supplier. As far as cutoff start.  If you're setting your end to 33v then start should be a volt or two higher. 34/35.  It's you telling the vesc when to start reducing output.
```

---
## \#3 Posted by: Michaelj1 Posted at: 2018-05-11T14:09:05.473Z Reads: 97

```
Yeah my pack uses Samsung 30q cells too, and I’m running in FOC mode. Have you had any problems with voltage sag? It hasn’t affected me at all but my battery indicator goes down like 20% when I accelerate quickly or when I’m going up a hill. Not sure how accurate the thing is tho it says my battery is dead when the vesc says it’s reading like 33 volts lol
```

---
## \#4 Posted by: Michaelj1 Posted at: 2018-05-11T14:32:54.432Z Reads: 91

```
I don’t know a whole lot about lithium ion batteries, my first board used lipo so this is new to me. Are there any differences I need to know about?
```

---
## \#5 Posted by: E1Allen Posted at: 2018-05-11T17:28:03.063Z Reads: 72

```
So the percent gauge dropping going up hills, that's voltage sag.  It's normal.  Battery cutoff for liion is lower than lipo.  If you have a multimeter check the actual voltage of the pack to the vesc reading.  They should be pretty close
```

---
## \#6 Posted by: Michaelj1 Posted at: 2018-05-11T17:44:24.336Z Reads: 74

```
Yeah I ran it with the vesc plugged in, but that was with no load so it’s probably not a good test, it stayed at a consistent 33v. Will voltage sag cause the board to shut down early? Or shut down at random near the cutoff end?
```

---
## \#7 Posted by: Michaelj1 Posted at: 2018-05-11T17:46:25.114Z Reads: 74

```
By the way it was at 33v because I need to charge it soon lol
```

---
## \#8 Posted by: E1Allen Posted at: 2018-05-11T17:51:38.210Z Reads: 67

```
It should not shut down.  It just limits the current output to keep voltage at the minimum level you determine in the settings.  So your board will get slower and acceleration will be less when you're out of battery.
```

---
## \#9 Posted by: Michaelj1 Posted at: 2018-05-11T17:53:50.436Z Reads: 63

```
Got it. Sounds good! Thanks!
```

---
