# 5S VESC configuration

### Replies: 11 Views: 140

## \#1 Posted by: PeterMcKane Posted at: 2019-02-22T05:36:51.443Z Reads: 56

```
Hey guys, so one of my 5S batteries just died but I still need my board for the next couple days. Are there any 5S battery VESC configurations possible?

I have a turnigy 6364 213kv motor with 5000 mAh 5S battery.
```

---
## \#2 Posted by: Friskies Posted at: 2019-02-22T05:42:20.140Z Reads: 54

```
Adjust vesc settings for max amps etc and just ride it. Should work just fine - I think the vesc minimum voltage is 8v or so.

In saying that I can't imagine you will be going very quickly or going up any decent sized hill.....
```

---
## \#3 Posted by: Andy87 Posted at: 2019-02-22T05:43:10.462Z Reads: 54

```
8V is the vesc lowest voltage limit, so 5S will work without issues.
You just will have less top speed than before if nothing else changes in your setup
```

---
## \#4 Posted by: PeterMcKane Posted at: 2019-02-22T16:46:13.560Z Reads: 27

```
@Friskies @Andy87 so what would i put as the motor in and out parameters?
```

---
## \#5 Posted by: Andy87 Posted at: 2019-02-22T16:55:51.953Z Reads: 22

```
You don’t need to change anything there.
Just the cut off voltage is the thing you need to  change as your pack becomes smaller in S count.
```

---
## \#6 Posted by: PeterMcKane Posted at: 2019-02-22T16:57:04.282Z Reads: 21

```
oh so I dont need to change the amount of current being outputted from my battery?
```

---
## \#7 Posted by: PeterMcKane Posted at: 2019-02-22T16:58:01.897Z Reads: 22

```
and also im trying to configure on the new 2019 vesc tool and doesnt seem like it wants to connect after i update the firmware. when i replug the usb, it says firmware too old again
```

---
## \#8 Posted by: Andy87 Posted at: 2019-02-22T17:00:14.395Z Reads: 21

```
Yes the amps stay the same as you took away a series pack and not a parallel parallel pack.
Your single pack is still capable to output the same amount of amps than before. Just now it’s half of the voltage.
```

---
## \#9 Posted by: PeterMcKane Posted at: 2019-02-22T17:03:17.857Z Reads: 20

```
okay i am configuring my vesc rn and i ran the detection but the software seems to have froze. my motor never ran but the loading bar for detecting the motor is still going.
```

---
## \#10 Posted by: Friskies Posted at: 2019-02-22T17:19:25.527Z Reads: 19

```
I would lower the battery amps a bit anyway as I have a feeling the vesc may draw more at a lower voltage to get the motor moving(5s is quite low for Esk8). I could be wrong but I prefer operating on the safe side. And as above adjust the voltage limits of the pack.

Your motor might not be spinning because the 5s voltage limit has not been applied. Basically you are probably still on the 10s cutoff which would should be above 5s even at full charge.
```

---
## \#11 Posted by: Andy87 Posted at: 2019-02-22T17:21:26.514Z Reads: 19

```
What ☝️ @Friskies said
```

---
