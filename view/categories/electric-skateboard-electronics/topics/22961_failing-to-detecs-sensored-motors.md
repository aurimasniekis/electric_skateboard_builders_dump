# Failing to detecs sensored motors

### Replies: 6 Views: 613

## \#1 Posted by: Mike_Lemon Posted at: 2017-05-13T16:06:17.198Z Reads: 61

```
Hello I've been tring to detect some sensorless motors with the BLDC tool on windows now previously I've had luck with that on the same setup but now it doesn't seem to work all I've done since then is removing the CAN BUS IC on both vescs sins it was shorting the VREG and communicated with the vescs over uart to control their duty. so other than the sensor detection the VESCS do work.

What should I do?

BTW this is the motor:
diy-electric-skateboard-kits-parts/electric-skateboard-motor-5055-190kv/
```

---
## \#2 Posted by: JohnnyMeduse Posted at: 2017-05-13T18:06:35.465Z Reads: 46

```
Do you have any picture of your connection ?

Also have you try to contact @torqueboards.
```

---
## \#3 Posted by: Mike_Lemon Posted at: 2017-05-13T21:37:08.045Z Reads: 37

```
The connection is good it worked before but now it suddenly doesn't.
```

---
## \#4 Posted by: JohnnyMeduse Posted at: 2017-05-13T21:52:55.360Z Reads: 37

```
Did your setup had work with sensor before or only sensorless, and is it still working sensorless ?
```

---
## \#5 Posted by: Mike_Lemon Posted at: 2017-05-13T21:59:58.580Z Reads: 35

```
It does work sensorless and did work sensored. didn't even get to ride it sensored tough it was still in proto stage.
```

---
## \#6 Posted by: JohnnyMeduse Posted at: 2017-05-13T22:10:44.433Z Reads: 31

```
Can you just swap to phase (so the motor will run the other) and try it, because sometime when sensor are misplace inside a motor they tend to only work in one direction.
```

---
