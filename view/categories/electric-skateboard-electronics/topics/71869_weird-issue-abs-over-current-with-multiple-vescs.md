# Weird issue: abs over current with multiple VESCS

### Replies: 3 Views: 156

## \#1 Posted by: multiplexor Posted at: 2018-10-21T05:07:12.115Z Reads: 51

```
Hey guys, have you encountered an issue when you're using multiple vescx(focbox)'s where the master is controlling the slave, but the master throws over current when at high rpm. AND only when traction control is enabled. 

Only way to resolve it is by disabling traction control. At lower RPM it's not too much of an issue. However once over 25k erpm, you start seeing small spikes. Eventually at even higher rpm, the master will just shutdown leaving the slave spinning.
```

---
## \#2 Posted by: Trdolan03 Posted at: 2018-10-21T05:10:29.313Z Reads: 48

```
Try checking your capacitors and make sure they are not shorted or blown on the master.
```

---
## \#3 Posted by: multiplexor Posted at: 2018-10-22T03:46:15.390Z Reads: 34

```
So I decided to try updating my VESC-X firmware to one of the newer ones... then switched from BLDC tool to the VESC app and now it's running 1000000% better. smooth acceleration, smooth braking. No more issues with traction control, and one motor over spinning. night and day difference.
```

---
