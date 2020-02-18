# Connecting the VESCS?

### Replies: 5 Views: 731

## \#1 Posted by: Raf Posted at: 2016-09-13T12:22:08.725Z Reads: 75

```
Hey guys,

so i have been reading the vesc tutorial on here but i am still confused on how to connect dual vescs? I know you connect them through CANBUS. but do i connect one vesc to a motor and power and configure settings then repeat to the other motor, or do i only do it to one vesc? how do the settings affect both vescs to run both motors?

Also i am using my lipo battery to power them, should i charge the battery before doing this so its full or should i leave it at the 3.7v?
```

---
## \#2 Posted by: Jinra Posted at: 2016-09-13T12:35:27.511Z Reads: 69

```
Treat each VESC as if you were going to run them solo. Each VESC gets configured for the motor it's driving and needs is own power source (which can be shared from 1 per source).

The VESC can be programmed from 3-12s, so as long as your voltage lies within that we should be fine. Make sure to read up on the thread that describes how to connect the CAN bus, as you have to set the master to have *multiple ESCs over CAN* and enabled, and the slave to have *send status over CAN* enabled.
```

---
## \#3 Posted by: Raf Posted at: 2016-09-13T12:38:10.715Z Reads: 70

```
ahh okay this makes sense, thank you. As for the battery. what i meant is i have a x2 5s LIPO and i haven't charged them so they are at the storage volt (3.7). i will be using on 5s lipo to power the vesc. Should i charge this battery before so its full or doesn't it matter?
```

---
## \#4 Posted by: Raf Posted at: 2016-09-13T12:48:00.836Z Reads: 60

```
also do i set up the receiver on both or just one?
```

---
## \#5 Posted by: Jinra Posted at: 2016-09-13T12:50:37.436Z Reads: 60

```
[quote="Raf, post:3, topic:9518"]
Should i charge this battery before so its full or doesn't it matter?
[/quote]

doesn't matter. Only set up the receiver on the master VESC, leave the slave app configuration disabled.
```

---
