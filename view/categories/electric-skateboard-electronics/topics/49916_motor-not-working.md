# Motor not working

### Replies: 9 Views: 348

## \#1 Posted by: danyCRO Posted at: 2018-03-23T11:51:21.330Z Reads: 72

```
Hi,
I am not sure is the mistake in motor or speed controler. Can I test motor with 3 wires to one smaller baterry which have only (-) and (+)?
```

---
## \#2 Posted by: Jumpman Posted at: 2018-03-23T12:01:49.932Z Reads: 70

```
No, not a good idea.
```

---
## \#3 Posted by: pat.speed Posted at: 2018-03-23T12:06:25.708Z Reads: 68

```
What motor? What esc? How are you connecting them?
```

---
## \#4 Posted by: Acidfie Posted at: 2018-03-23T12:15:26.594Z Reads: 62

```
never do that
```

---
## \#5 Posted by: danyCRO Posted at: 2018-03-23T12:21:17.533Z Reads: 56

```
Motor 170KV C6374 and SC from [Here .](https://m.ebay.com/itm/single-motor-electric-longboard-skateboard-controller-ESC-Substitute-/322688416729?varId=511729897872&txnId=1873705098011)
```

---
## \#6 Posted by: Acido Posted at: 2018-03-23T14:28:27.493Z Reads: 45

```
connect 2 phases to a battery for a short time if it stutters it should work
it will throw a spark tho
```

---
## \#7 Posted by: danyCRO Posted at: 2018-03-23T16:54:47.044Z Reads: 32

```
I test on 6V and it moves a few milimeters, several times. That means that motor is alive :slight_smile:
Thank you.
```

---
## \#8 Posted by: b264 Posted at: 2018-03-23T17:02:13.526Z Reads: 32

```
Let's call the phase wires "A", "B", and "C"

To test it:
1) Verify the motor spins free with A,B,C unconnected
2) Verify connecting A to B causes pulsing brake
3) Verify connecting B to C causes pulsing brake
4) Verify connecting A to C causes pulsing brake
5) Verify connecting A to B to C causes smooth, strong brake
6) Never connect the motor leads to DC power or anything except a BLDC controller

Also 2, 3, and 4 should feel identical if the motor doesn't have any issues.  Any differences here indicate a defect.
```

---
## \#9 Posted by: danyCRO Posted at: 2018-03-23T17:06:41.893Z Reads: 30

```
I test it with speed controller and working fine. Thanks guys.
```

---
