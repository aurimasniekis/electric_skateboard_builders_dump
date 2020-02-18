# VESC &#124; pins only drops to 2.7 v when off

### Replies: 2 Views: 426

## \#1 Posted by: chibby Posted at: 2016-05-13T21:12:49.400Z Reads: 46

```
I have configured the hall-pins to act as output pins (PAL_MODE_OUTPUT_PUSHPULL). When I call pallClearPad it only drops down to 2.7 v from 3.3 v. Shouldn't it drop to 0?
```

---
## \#2 Posted by: chibby Posted at: 2016-05-14T07:55:45.744Z Reads: 22

```
Had to do with the resistors near the pins, Removed the 2k and now it's showing 0 v when low. I guess I also need to change the 10k to zero-ohm link to avoid voltage drop ([the circuit](http://i.imgur.com/hJzqvml.png)).
```

---
