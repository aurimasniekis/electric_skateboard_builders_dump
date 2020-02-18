# What numbers do I punch in on vesc tool for 6374 190kv 3200w motors?

### Replies: 7 Views: 193

## \#1 Posted by: Taliesin Posted at: 2018-08-23T20:29:34.649Z Reads: 69

```
I’m searching, haven’t found the answer yet.

6374 190kv 3200w dual motors
12s4p

Not sure what to put here

![image|666x500](upload://8Z4PvYmPsk2NwaBpClxmOAzNUdh.jpeg)
```

---
## \#2 Posted by: danielz Posted at: 2018-08-23T21:15:31.845Z Reads: 56

```
I have same motors, and use 12s my settings are

60a  (max continuous of each of my vescs)
-40a (keep changing this until happy with brake strength, max -60)
100a (I use lipo, max 200a, split equally between vescs, so 100a)
-5a (Set this to maximum charge rate of battery, -5 each for me(Arguably you can go higher)

All braking is done via charging of the battery, but motor amps is different to battery amps. That why changing motor current max brake effects brake strength even when max regen amps is low. At some point it wont brake any harder unless you increase max regen, to this you can either have more batteries in parallel or higher charge rate batteries.
```

---
## \#3 Posted by: Taliesin Posted at: 2018-08-23T21:33:19.288Z Reads: 50

```
@danielz 

You mind helping me with a walkthrough since we have similar setup?

I have lion so I went 80 instead of 100

Next

![image|666x500](upload://q957JCcU0BNvT4MJzmtsh9pqRIx.jpeg)
```

---
## \#4 Posted by: danielz Posted at: 2018-08-23T21:34:58.274Z Reads: 45

```
click apply to set the two limits its suggested.
```

---
## \#5 Posted by: danielz Posted at: 2018-08-23T21:36:04.057Z Reads: 44

```
Remember to go into motor settings after the wizard and change erpms to +60,000 and -60,000 The stock numbers are 100k.
```

---
## \#6 Posted by: Taliesin Posted at: 2018-08-23T21:49:29.825Z Reads: 42

```
Copy that.

Ok next?

![image|666x500](upload://tjSDxm6uZhmyC1tOl0pLNRTs2cY.jpeg)
```

---
## \#7 Posted by: Taliesin Posted at: 2018-08-23T21:58:19.144Z Reads: 39

```
So I’m doing the RL button, it works, then the teepee button, it spins the motor and I get all green but it’s only doing 1 motor.
How do I get the other motor to spin with it?

Edit: do I need to go back and reprogram the other esc from scratch as well?
```

---
