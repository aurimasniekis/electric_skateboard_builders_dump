# Dual VESC, Canbus and 2 receivers paired to the same remote. Possible?

### Replies: 4 Views: 210

## \#1 Posted by: gmurad Posted at: 2018-07-22T16:18:27.360Z Reads: 67

```
It doesn't seem to be possible but just want to make sure.

I want to use CANBus so I get telemetry via bluetooth from both VESCs but I also already have 2 receivers that I could pair to the same remote.

Is there a way to setup the VESC in Master/Slave via CANBus but make each of them independent in terms of receiving input from the remote (each VESC with it's own receiver) for extra redundancy? Or something that would achieve the same.
```

---
## \#2 Posted by: dareno Posted at: 2018-07-23T04:08:06.176Z Reads: 49

```
Why would you want to do this?  What would it achieve?
```

---
## \#3 Posted by: Pedrodemio Posted at: 2018-07-23T04:15:12.880Z Reads: 45

```
Yeah, you can do that, just disable multiple VESC’s on whatever control mode you are using,  just remember to chance the CAN Id, on one of the VESCS
```

---
## \#4 Posted by: gmurad Posted at: 2018-08-01T22:45:26.674Z Reads: 23

```
The idea is to get redundancy, if one receiver fails during a period you want to break the other would still work, but I also want to get some benefits of canbus like both VESCs sharing the same bluetooth module
```

---
