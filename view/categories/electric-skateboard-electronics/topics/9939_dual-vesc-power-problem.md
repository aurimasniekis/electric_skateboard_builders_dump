# Dual VESC - Power Problem

### Replies: 7 Views: 768

## \#1 Posted by: ryan4321 Posted at: 2016-09-21T12:50:03.718Z Reads: 106

```
I have a 'Bisek' board from China. The electronics were faulty (common for their boards).

So I have replaced with the VESC. However I have it all connected (although not gone into the BLDC tool yet) but when pressing the power button on the board with both Vesc's plugged into the boards power, the blue light on the boards switch fires up then fades along with the light on 1 of the Vesc's. 

If I take the power off 1 of the Vecs's then the Vesc with power is fine and the board stays on. Same thing with the other Vesc.

I'm only guessing, but is there some issue powering 2 Vesc's with the 1 power supply that have not been 'fiddled' with yet in the BLDC tool? If so, what setting do I have to change.

* Note: The motors wires are not yet connected to the Vesc's but I assume this wouldn't be an issue.

<img src="/uploads/db1493/original/3X/5/3/539a1b9f6cac307558de1506dc8d9d174cce910f.jpg" width="690" height="388">
```

---
## \#2 Posted by: michaeld33 Posted at: 2016-09-21T13:13:20.580Z Reads: 94

```
Very strange. I usually associate a dimming light with a failing component, but it works with just one so that's weird. It wouldn't make any sense if it was the battery since the VESC unplugged from the motor should only draw a few amps... Hmm.
```

---
## \#3 Posted by: Blasto Posted at: 2016-09-21T13:45:41.107Z Reads: 84

```
Your motor leads seem to be touching, try again with those leads taped up temporarily.
```

---
## \#4 Posted by: ryan4321 Posted at: 2016-09-21T13:54:51.284Z Reads: 80

```
Good point - I just made sure they were all not touching and no change.

If I start up with just the 1 connected, then hot plug the 2nd vesc with the power switch on, I get a spark when connecting but the light stays on and both vesc's stay on as well. So maybe a switch change? Do switches have current limitations or built in 'brains' / fuse?
```

---
## \#5 Posted by: DeathCookies Posted at: 2016-09-21T14:17:26.487Z Reads: 73

```
Can you measure both voltages going to each VESC?

Maybe you should just connect it to BLDC-Tool and check the faults
```

---
## \#6 Posted by: ryan4321 Posted at: 2016-09-21T14:26:52.801Z Reads: 73

```
Will do - thank you..

Does anyone know how much each vesc pulls in Amps (without the motors connected) and also what Amps does the switch have to cope with... The switch I have seems the same as below which is only 2A. Maybe this is the problem and I need a higher Amp Switch.

http://www.ebay.com.au/itm/LED-Ring-36V-12mm-Car-ON-OFF-Stainless-Metal-WaterProof-Flat-Push-Button-Switch-/131512524301
```

---
## \#7 Posted by: Blasto Posted at: 2016-09-21T14:30:41.839Z Reads: 70

```
That type of switch should be switching a higher power stage like a mosfet for example. If you are passing the entire current of the vesc through that switch it will blow.

You might need get a anti-spark switch with a mosfet drive.
```

---
