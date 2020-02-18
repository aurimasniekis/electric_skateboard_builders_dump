# Motor detection with dual motors

### Replies: 4 Views: 484

## \#1 Posted by: Strawbs Posted at: 2016-08-11T14:28:35.290Z Reads: 93

```
Should both motors spin up when running a motor detection with a dual motor config?  I can spin each individually by connecting the mini USB port to their respective VESCs, but they don't spin together.
```

---
## \#2 Posted by: chaka Posted at: 2016-08-11T14:39:49.351Z Reads: 93

```
No, only the vesc that is connected via usb should spin during detection.
```

---
## \#3 Posted by: Jinra Posted at: 2016-08-11T16:02:14.201Z Reads: 81

```
Do motor detection for each motor individually, then turn on multiple escs over CAN on the primary VESC and send status over can on the slave VESC to enable dual motors.
```

---
## \#4 Posted by: evoheyax Posted at: 2016-08-11T16:14:32.747Z Reads: 77

```
that's how it works, you connect to them individually and do motor detection one at a time. Then after connecting them over can, use the controller, and both should spin.
```

---
