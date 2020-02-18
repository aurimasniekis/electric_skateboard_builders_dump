# Dual VESCs won&rsquo;t communicate after CAN Chip repair

### Replies: 6 Views: 175

## \#1 Posted by: SaveMe Posted at: 2018-08-15T22:23:11.606Z Reads: 62

```
Hi everyone, 

Recently I blew both my CAN Chips on my FOCBOXs by having one powered on and the other turned off while they were still connected via canbus wire.  Since then, they would not blink when starting with the blue LEDs but I could tell they were still putting out power because when I would connect my receiver to it it would power on.  After some research I found that one solution would be to replace the CAN chip, SN65HVD232DR, on the FOCBOXs.  I ordered them and as soon as they arrived my friend and I got to work and replaced them yesterday.  Once the repairs were done we tested each one separately and they were working as normal.  The problem comes when they are connected through canbus and one is the master while the other is a slave; they simply don't want to communicate and only the master works.This goes both ways, we tested both as the master role and slave role so they both work fine but still refuse to communicate in either setup.  Is there another part that possibly needs to be replaced?a
```

---
## \#2 Posted by: JTAG Posted at: 2018-08-15T23:11:13.790Z Reads: 57

```
Is the termination resistor still on the board? Does it have the right impedance? About 250Ohms or less should be measured between canh and canl when the vesc is not connected to another vesc.
```

---
## \#3 Posted by: SaveMe Posted at: 2018-08-15T23:30:02.615Z Reads: 51

```
I am only getting one reading from my FOCBOXs which is 660 ohms for one of them and the other is not sending a signal/reading

Edit: I got around 220 ohms for both of them when they were powered off and not connected to each other.  My last readings were when they weren't connected to one another but they WERE turned powered on.  Doesnt that sound/look strange to you?
```

---
## \#4 Posted by: JTAG Posted at: 2018-08-15T23:57:57.677Z Reads: 46

```
No that does not sound strange. The higher impedance that you measure is actually the impedance measurement of the multimeter being disrupted by the vesc putting a voltage on the can bus because it tries to communicate. 
 
So in that sense it sounds good that you measure higher, that meens that that one works ( at least a little bit). 

They should measure however both the same ( only of they are configured the same!). 

Please note that you are on the parasitic / great side of measuring / evaluation with this, evaluating like this is not the intended way and will differ from multi meter to multi meter. The best way would be visualizing the can signals with an oscilloscope, then you will immediately see the problem.
```

---
## \#5 Posted by: SaveMe Posted at: 2018-08-16T00:03:54.441Z Reads: 44

```
So should both measure the same when powered on, and if so what might be causing this issue? As for measuring this properly what would be the proper way to go about this.  I was using a Fluke multi meter for the impedance measurement but if I need an oscilloscope I can head over to my university and use one there.  What would I be measuring and how would the connections look like for getting the readings? Thank you for your help!
```

---
## \#6 Posted by: JTAG Posted at: 2018-08-16T13:40:09.528Z Reads: 26

```
Oscilloscope would be ideal, ill make some reference screen shots for you. I hope tonight.
```

---
