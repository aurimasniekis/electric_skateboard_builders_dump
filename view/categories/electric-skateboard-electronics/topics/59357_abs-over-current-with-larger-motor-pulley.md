# ABS over current with larger motor pulley

### Replies: 2 Views: 168

## \#1 Posted by: bloke900 Posted at: 2018-06-19T08:44:28.411Z Reads: 61

```
My board and initial set up:
10s LIPO, FOCBOX, SK8 6374 192kv, 15t:36t on 97mm wheels. (single motor)

Initially, I had VESC settings at:
Max Motor: 70a
Max Batt: 40a
ABS Max: 130a. 

Things were good - but I wanted to run a larger motor pulley to get some extra speed and less belt slippage. 

Now, all settings remain the same, but I changed the gearing to 20t:36t. almost no belt slippage - its great.  However, I am getting ABS_OVER_CURRENT errors when applying too much throttle. I am pretty big guy (250lbs), and the gearing feels much less torque focused...  Just wondering, am I expecting too much from my single drive board?  Am I pushing my FOCBOX too hard, or should it be able to handle this kind of abuse?   Before I start digging in to find a problem, I just want to know if there is a problem to find... 

Cheers!
```

---
## \#2 Posted by: Benjamin899 Posted at: 2018-06-19T09:11:48.013Z Reads: 51

```
well you did increase the motor pulley from 15 to 20, as a result you get more top speed but less torque, for a single drive and a heavy guy that is not an ideal idea, i am way lighter than you and if go up a steep hill from almost a standstill i will get ABS Overcurrent too. I would recommend a dual drive or if you don't want to spend that much go for a better ratio and a 15mm belt maybe 20mm.
```

---
