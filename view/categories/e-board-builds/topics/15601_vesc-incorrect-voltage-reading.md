# VESC incorrect voltage reading

### Replies: 4 Views: 566

## \#1 Posted by: oripaamoni Posted at: 2017-01-03T19:27:45.008Z Reads: 61

```
on my dual vesc build my primary vesc read ~0.8V low, but my slave VESC is spot on. I had to set my primary vesc voltage setting so that the cut offs and over volt behave the same on both motors but now that i am reading voltage with an app i would love to get this more accurate.  Is there anyway to adjust this?
```

---
## \#2 Posted by: JohnnyMeduse Posted at: 2017-01-03T19:31:52.225Z Reads: 60

```
You can change the resistor R3 and R4 for the same value as they are, but use some resistor with less error coefficient. Or it might be a bad reading from the MCU, so tou need to change it.
```

---
## \#3 Posted by: oripaamoni Posted at: 2017-01-03T19:58:27.814Z Reads: 50

```
thanks for the suggestion, I will check the resistance of r3 and r4 and see how the resistance compares to the resistors on my slave vesc. On my custom drones the flight controllers use a voltage divider to read up to 6s but they also give you an adjustment in the GUI
```

---
## \#4 Posted by: JohnnyMeduse Posted at: 2017-01-03T20:01:13.860Z Reads: 44

```
They are probably the same... since the 0.8v difference is easely within the tolerance of the resistor (and is not really abnormal)
```

---
