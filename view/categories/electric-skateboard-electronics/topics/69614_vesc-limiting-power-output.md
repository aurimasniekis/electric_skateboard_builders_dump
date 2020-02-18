# VESC limiting power output?

### Replies: 6 Views: 142

## \#1 Posted by: Spyro Posted at: 2018-09-30T10:47:09.332Z Reads: 47

```
I've build an e-scooter that runs on 6S, a VESC 4.12 and a 6374 motor.
It accelerates very hard and reaches rly high speeds.
However, sometimes the motor seems sluggish as if it only has like 30% power or something. Then when I go slow for abit, the full torque comes back on. 
What could this be due to?
Isit my voltage soft cut off at 3.7V too low? 
Anyone experienced the same issue?
```

---
## \#2 Posted by: FredrikHems Posted at: 2018-09-30T10:56:27.936Z Reads: 45

```
I am pretty sure you are hitting temperatur cutoff, which means you either need to go lower on the power output of the vesc or cool the vesc more effective.
```

---
## \#3 Posted by: Benjamin899 Posted at: 2018-09-30T11:13:47.306Z Reads: 38

```
3.7 soft cut off? think about what that means.
```

---
## \#4 Posted by: Vanarian Posted at: 2018-09-30T11:18:25.032Z Reads: 36

```
Your low voltage cut-off is too high and you're most probably triggering overheat protection too, just like @FredrikHems said :thinking:
```

---
## \#5 Posted by: FredrikHems Posted at: 2018-09-30T11:19:16.565Z Reads: 33

```
He is probably using lipo guys. I use 3.7 soft and 3.6 hard for lipo too
```

---
## \#6 Posted by: ElectricCoast Posted at: 2018-09-30T11:20:07.423Z Reads: 31

```
This could also be voltage sag causing the problem.  What type of battery are you using?  Lion or Lipo?  How many parallel groups are you running?
```

---
