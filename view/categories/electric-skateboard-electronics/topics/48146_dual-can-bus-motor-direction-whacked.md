# Dual CAN bus motor direction whacked

### Replies: 7 Views: 496

## \#1 Posted by: Bataleon Posted at: 2018-03-04T19:37:52.702Z Reads: 138

```
I'm in the process of configuring a dual motor setup over CAN bus.

When running the motor detection for each motor, each spins in the correct direction. However when pulling the trigger on my mini remote (after following @skslingo21's guide [here](http://www.electric-skateboard.builders/t/y-piece-or-canbus/26461/188)), they spin in opposite directions.

Is it safe to simply swap two phase wires of the motor spinning in the wrong direction? Or should this be avoided because I'm running a dual setup over CAN bus, potentially resulting in VESC damage?

VESC HW is 4.12 and firmware 2.18.

Thanks
```

---
## \#2 Posted by: ElskerShadow Posted at: 2018-03-04T19:51:39.614Z Reads: 136

```
Just don’t bother and swap cables
```

---
## \#3 Posted by: krloz Posted at: 2018-03-05T10:16:23.059Z Reads: 96

```
Sensored or sensorless?
```

---
## \#4 Posted by: Bataleon Posted at: 2018-03-05T11:39:00.190Z Reads: 83

```
Running unsensored.
```

---
## \#5 Posted by: JTAG Posted at: 2018-03-05T12:33:14.304Z Reads: 77

```
With the old firmware your only choice if to swap two phase wires indeed.
```

---
## \#6 Posted by: Nordle Posted at: 2018-03-05T12:39:21.891Z Reads: 78

```
Bataleon snowboards?
```

---
## \#7 Posted by: krloz Posted at: 2018-03-05T21:34:02.499Z Reads: 49

```
well then. swap two wires and forget
```

---
