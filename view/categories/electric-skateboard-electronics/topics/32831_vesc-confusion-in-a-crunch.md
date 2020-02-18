# Vesc Confusion! In a crunch

### Replies: 10 Views: 391

## \#1 Posted by: Nix Posted at: 2017-09-11T00:48:47.970Z Reads: 71

```
So the vesc 4.12 can take 50amps continuous. The battery max should be lower than this like at 50 amps. But the motor max doesn't have to follow under 50 amps right? It's the max of the motor amps? 

If this is the case, then I have another one (hold on please) I have a 6s and a 2000 watt motor. (2000/25 = 88) 88 amps, but the motor can only take 80 amps? So which one do I set the settings to?
```

---
## \#2 Posted by: Jinra Posted at: 2017-09-11T00:53:58.545Z Reads: 67

```
If you want to be safe don't set your limits above their rated currents. So 80A motor max (at the highest), though I'd start with 60A and see how you feel. 50A battery max assuming your battery can output it.
```

---
## \#3 Posted by: Nix Posted at: 2017-09-11T00:55:14.688Z Reads: 65

```
@jinra what does the motor max control exactly? Like speed?
```

---
## \#4 Posted by: Jinra Posted at: 2017-09-11T00:56:13.297Z Reads: 60

```
In current control mode (most usable and popular mode) it controls how much current your suppplying the motor based on your throttle. 0 throttle = 0 amps, 100% throttle = 100% if the amps you specified.
```

---
## \#5 Posted by: Nix Posted at: 2017-09-11T01:10:15.270Z Reads: 53

```
Oh, so at %100 it's 80 amps but what does that do to the volts? It will be a little less than the Mac right?
```

---
## \#6 Posted by: Jinra Posted at: 2017-09-11T01:23:05.767Z Reads: 47

```
voltage is regulated by duty cycle
```

---
## \#7 Posted by: Nix Posted at: 2017-09-11T01:29:57.232Z Reads: 44

```
Oh thanks. 10 characters
```

---
## \#8 Posted by: Nix Posted at: 2017-09-11T01:45:10.720Z Reads: 38

```
@jinra also, so if I change my battery to 9s, to make sure my drv chip not to blow here are some calculations... (8571/[9*4.2]= 226) so I should be good with 220kv motor and to blow the chip it's 38.9 volts. So should I be good not to blow the chip with that 1 v difference in blowing and not blowing itm
```

---
## \#9 Posted by: Jinra Posted at: 2017-09-11T01:48:34.628Z Reads: 35

```
you'll be fine, there are a bunch of other factors that will prevent you from hitting 60k erpm. I run 10s with 230kv motors just fine.
```

---
## \#10 Posted by: Nix Posted at: 2017-09-11T02:02:59.964Z Reads: 35

```
Wow thanks
```

---
