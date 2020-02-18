# Motor detection bldc or foc

### Replies: 5 Views: 481

## \#1 Posted by: KidProzac Posted at: 2017-08-04T01:04:00.471Z Reads: 100

```
Do I do a motor detection in bldc then foc?  Or is it one or the other? #newbie
```

---
## \#2 Posted by: nart Posted at: 2017-08-04T05:19:32.368Z Reads: 94

```
you mean sensorless application?
```

---
## \#3 Posted by: JLabs Posted at: 2017-08-04T05:23:08.236Z Reads: 92

```
You either run a BLDC motor detection or FOC detection. You can run both at the same time.
```

---
## \#4 Posted by: KidProzac Posted at: 2017-08-04T10:54:25.975Z Reads: 72

```
I have 6374 190kv motor with hall sensor from torque boards. I fried one vesc already.  So is this considered a sensor motor. Also it's rated for 80amps.  Do I put that in motor max amps.  Should I run motor detection in bldc mode or FOC. Thank you!!
```

---
## \#5 Posted by: rich Posted at: 2017-08-04T14:43:12.331Z Reads: 53

```
I would do BLDC detection only if you want to stay on the safe side. Go FOC later. You can set 80A max like the rating of your motor. But better start reading all the nice information on this forum first and then I would ask your remaining/advanced questions later :wink:
```

---
