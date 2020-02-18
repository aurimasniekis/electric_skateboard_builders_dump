# Arduino controlled modes

### Replies: 13 Views: 549

## \#1 Posted by: freerice Posted at: 2017-07-17T15:06:50.563Z Reads: 76

```
Sorry if this has been posted before, but, would it be possible to use an arduino to have modes on a dual motor skateboard? What I mean is to have one motor always active, and the arduino could keep the other motor off, for extra range, and you could enable the other when you wanted extra power?
```

---
## \#2 Posted by: Sander Posted at: 2017-07-17T16:00:50.459Z Reads: 68

```
Yeah, just use a Mosfet to turn it off and on, so you can turn off the ESC with shutting off the mosfet so one of the motor is disabled.
```

---
## \#3 Posted by: pennyboard Posted at: 2017-07-17T16:44:56.501Z Reads: 54

```
I don't know that you would get any extra range from doing that. 

The reason is that to move at a certain speed the boards motors have to overcome a certain force (rolling resistance, wind resistance, gravity up a hill, etc.). The overcome the forces and propel that board forward at any moment you need a set amount of power, which is dependent on amps and volts through the motor.

So if you use only one motor, you'd have to put all the amps through that motor, as opposed to using 2 motors and putting half the required amps through each motor. So I think the overall amp draw would be the same whether you use 1 or 2 motors.

Also, the second motor being shut off would provide a lot of resistance that the first motor would have to overcome, meaning you might actually get worse range by shutting off one motor. It would be really interesting to try in the real world and see what the results are though.
```

---
## \#4 Posted by: wafflejock Posted at: 2017-07-17T16:50:51.478Z Reads: 44

```
Sounds mostly right to me, you might actually get better range with the 2 motors since you are reducing the amperage through each side and power loss is a square relation with amperage so I^2*R.  So say we have 10Amps through 1 VESC and motor it's 100A*R (with a set R) if we have two motors and two VESCs each getting 5Amps it's 25A*R+25A*R = 50A*R so assuming both paths through the motors and ESCs has the same resistance you get more electrical power loss with just 1 motor.

The idea is interesting I've heard of V8 engines that can shut off some of the pistons when they don't need the extra horsepower to save some fuel I'm just not sure that will translate to our electrical drives.
```

---
## \#5 Posted by: freerice Posted at: 2017-07-17T16:52:40.248Z Reads: 41

```
Yes, definitely. Although, oddly, I seem to recall someone saying that a single motor will always be more efficient than dual motors.....
```

---
## \#6 Posted by: chinzw Posted at: 2017-07-17T16:53:21.517Z Reads: 36

```
Also, if you're going to blow up your VESC if you're using one, because when its switched off the mosfets will take all that charging current.
```

---
## \#7 Posted by: freerice Posted at: 2017-07-17T16:54:27.375Z Reads: 35

```
Couldn't you just "reenable" the vesc when charging?
```

---
## \#8 Posted by: chinzw Posted at: 2017-07-17T16:55:37.751Z Reads: 37

```
No, not when charging, if one of the motors is turning, then the other will be regenerating. That current is cut of from the battery since the vesc is off, so it will dissipate in the mosfets until they blow up
```

---
## \#9 Posted by: freerice Posted at: 2017-07-17T16:56:57.813Z Reads: 32

```
Oh, for some reason I thought you were planning to charge the board through the motors.... :blush: stupid me
```

---
## \#10 Posted by: pennyboard Posted at: 2017-07-17T16:58:12.626Z Reads: 31

```
If you really wanted to do this, the thing to do would be to use a split servo cable and then hook up a transistor to the signal wire of the servo cable going to the second vesc (the one to be shut off) and then control that transistor with an arduino. 

That way, the vesc would still be on and could regenerate the batteries from the back emf its getting, but the motor wouldn't turn/get power because the signal from the remote would be cut off
```

---
## \#11 Posted by: Vanarian Posted at: 2017-07-17T17:19:13.595Z Reads: 32

```
Hi, you can try this experiment if you "burn" the Regen from the inactive motor (this or you double shunt the ESC - battery and motor sides). So it both turns ON and OFF totally. But that's a shitload of work to make it work safely when you ride. You know your ESC has a moment of timing to initialize on start? You need to manage this too. Or keep the ESC active and only shut the motor?
```

---
## \#12 Posted by: freerice Posted at: 2017-07-17T18:26:34.973Z Reads: 23

```
Sorry to change the topic all of a sudden, but about a welded 18650 pack, what happens if a cell goes dead? Do you remake the entire pack? Or can you fix the single cell? Are there any good threads to read about this?
```

---
## \#13 Posted by: wafflejock Posted at: 2017-07-17T18:42:49.160Z Reads: 21

```
If it hasn't caused the other cells in the pack to get below the low voltage for the cells then they should be okay.  The only problem with replacing a single cell is it won't have the same wear level as the rest of the pack so if the rest of the cells were used for say 100 cycles and then you change out one of the cells that one cell is always going to have slightly more capacity than the rest of the pack so when the pack is fully drained that one cell is going to artificially inflate the average for all the cells connected/measured together (ones in parallel with it, so you run the risk of low voltage on one of those other cells).  Basically if they are the same chemistry and have the same discharge cycles approximately then in theory it should be fine.  With my own packs when I let a cell go too low I just removed it from the pack (was just a temporary measure while I ordered some new batteries, and using LiPos so wasn't terribly hard to remove).

If you're replacing a single cell would just make sure it has the same charge as the rest of the pack while doing the replacement so you don't end up dumping a bunch of charge in either direction to/from the new cell (can probably use the same limits as when parallel charging LiPo batteries believe +/- .05V but don't quote me on this).
```

---
