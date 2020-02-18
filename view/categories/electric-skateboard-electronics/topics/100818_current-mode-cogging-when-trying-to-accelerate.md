# Current mode cogging when trying to accelerate

### Replies: 3 Views: 93

## \#1 Posted by: Xadiant Posted at: 2019-08-25T01:08:26.831Z Reads: 33

```
Hello,

I am building a custom board, but am having trouble tuning.

When I control the board using duty cycle, I get strong reliable acceleration, but when I try to switch to current mode the motors will start jerking around and lose torque when I push the throttle very high.  I have to be very conservative to get a smooth ride.... like it will take about a thousand feet to get up to top speed, where duty cycle mode will get there nearly immediately.

The cogging seems as if the vesc is losing the position of the motor (like if you have the motor leads plugged in in the wrong order).  I guess it could possibly be a limit in the settings, but when reading other forum posts it seems like that should feel more like the motors cutting out, not continuously pulsing.  As soon as I pull the throttle back it will resume normal smooth operation.

Any ideas?
```

---
## \#2 Posted by: Xadiant Posted at: 2019-08-25T01:09:38.824Z Reads: 32

```
Oh, this also does not happen without a load, I have to actually be riding the board.
```

---
## \#3 Posted by: Soflo Posted at: 2019-08-25T16:21:05.690Z Reads: 18

```
Following,  I've got a build doing the same thing but it's regular duty cycle mode.
```

---
