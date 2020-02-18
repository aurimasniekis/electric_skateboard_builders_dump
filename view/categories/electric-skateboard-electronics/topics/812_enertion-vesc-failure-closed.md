# Enertion VESC Failure - \[closed\]

### Replies: 12 Views: 3674

## \#1 Posted by: trbt555 Posted at: 2015-12-26T17:33:09.429Z Reads: 143

```
I've been finalizing my build in [this thread][1] and today I attempted to spin up the motors and only one VESC appears to be working correctly.
Connection with Nunchuck was OK.
CANbus communication was OK.

VESC HW version: 4.10 from Enertion's recent batch.
FW version : 2.5
BLDC version : 2.5

When I spin up the motors, only the slave VESC spins up as it should, the other one doesn't budge.
I switched motor/VESC connection to verify motors are OK and I can conclude that the slave VESC and both motors are OK, there is a problem with the master VESC.

When I try to spin up the motor gently, it jitters: [VIDEO][2]

Realtime data:
<img src="/uploads/db1493/original/2X/3/33bc500f3e0b1c4004089ae1f14de602873d6ac0.jpg" width="690" height="364">

When I try to spin up the motor abruptly, it jolts, I get red LED and the VESC loses connection with the BLDC tool: [VIDEO][3] 

Realtime data:
<img src="/uploads/db1493/original/2X/e/e24e5c85d09f528e595949ced353ef80b70b6b87.jpg" width="690" height="364">

I've reproduced this problem with two dfferent power supplies as well as my 12S pack.
I've briefly seen a variety of errors in the realtime data window: DRV_8302, UNDER_VOLTAGE and ABS_OVER_CURRENT, but generally there is no fault reported.

When I try to run motor detection get an error code saying "bad detection data received" or something along those lines. Detection obviously fails.

I've tried reflashing the firmware and reloading the R-SPEC 6355 default XML file, which doesn't change anything.

I've inspected the VESC under a loupe and cannot find any obvious bridging.
Here are the high-res pictures if you want to pixel-peep:
<img src="/uploads/db1493/original/2X/6/6212a0a2915b3817058302c5e8fda24418089828.jpg" width="666" height="500">
<img src="/uploads/db1493/original/2X/d/d33a93188b1ecc6cf0fe9653b4d9a4e6d039a2a7.jpg" width="666" height="500">

I'm afraid I may have received a bad VESC from Enertion.

Can anyone come up with additional troubleshooting tips ?

Thanks,

Tom









 


  [1]: http://www.electric-skateboard.builders/t/loaded-dervish-dual-r-spec-6355-dual-vesc-nunchuck-paris-195-90mm-flywheels/524
  [2]: https://youtu.be/1_83jwSyuJs
  [3]: https://youtu.be/VlW7P_rJx08
```

---
## \#2 Posted by: chaka Posted at: 2015-12-26T21:20:13.278Z Reads: 126

```
Remove those metal nuts near the motor wires and use nylon spacers or nuts to fasten instead.
```

---
## \#3 Posted by: trbt555 Posted at: 2015-12-26T21:55:41.183Z Reads: 129

```
I measured those, they're not connected to anything so thay can't be causing the problem.
I also had heat shrink on the nuts but took it off when I removed the VESC.
But you're right, a nylon nut would be better. On my todo list.
```

---
## \#4 Posted by: chaka Posted at: 2015-12-26T22:07:06.553Z Reads: 128

```
The symptoms you are having are indicative of a bridged gate pin on your mosfets. Be sure this nut is not bridging this area here.
<img src="/uploads/db1493/original/2X/4/487ad7cc71a1e1c9d363d3da59f2d8f1ae14b76b.jpg" width="666" height="500">

It also looks like you may have a solder bridge on the stm chip but it is hard to tell from here.
```

---
## \#5 Posted by: chaka Posted at: 2015-12-26T22:13:38.719Z Reads: 124

```
Check this area too. It looks like a bad short just waiting to happen.

<img src="/uploads/db1493/original/2X/f/f53a8279aa6b0d480cf95b69f35967375088e375.jpg" width="666" height="500">
```

---
## \#6 Posted by: trbt555 Posted at: 2015-12-27T10:48:48.795Z Reads: 121

```
I removed all nuts and rechecked the mosfets for bridging, nothing.

Which is the STM chip ?

I inspected the power leads coming onto the PCB and was appalled by what I saw..
Strands of copper just waiting to touch something.
<img src="/uploads/db1493/original/2X/1/1e5af05a1ecddc7657780b640d31a1067eb12d36.jpg" width="666" height="500"><img src="/uploads/db1493/original/2X/b/bd6ca1fd96efb2751e5d0b87af9d3384617415ac.jpg" width="666" height="500">

But for tthe time being, these don't seem to be touching anything, so they cannot be the source of the problem.
```

---
## \#7 Posted by: chaka Posted at: 2015-12-27T15:46:49.466Z Reads: 115

```
These two spots look suspect But it is hard to tell from a photo. It could be something else.
<img src="/uploads/db1493/original/2X/b/b7a81dff76aba5e1f3705645e51224f8f465377e.jpg" width="666" height="500">

I agree that those wires are probably not causing anything at the moment but it is just a matter of time.  If you are good with an iron I would suggest replacing all the cheap car audio cable with high strand-count silicon cable if you can get that VESC working.
```

---
## \#8 Posted by: Jeff Posted at: 2015-12-27T17:52:41.189Z Reads: 110

```
I will echo @chaka's advice. The wire that comes on the enertion VESC is very cheap and can break while riding which can be very dangerous (happened to me).

Switch it out with high strand count cables ASAP.
```

---
## \#9 Posted by: trbt555 Posted at: 2015-12-27T19:02:12.001Z Reads: 111

```
@chaka there are absolutely no bridges on the processor. Besides, wouldn't bridges on the processor make flashing new firmware a problem ?

Anyway, I don't think I'm going to modify anything further on this VESC, it's clearly a dud. I'm contacting Enertion and claiming warranty. We'll see how that goes.
```

---
## \#10 Posted by: onloop Posted at: 2015-12-27T23:07:00.852Z Reads: 109

```
Those cables are unacceptable. That should of been resolved before shipping but obviously got missed. I appologise for that. Next time I won't rush to ship to ensure everything is checked.

Please submit an RA via our website.
```

---
## \#11 Posted by: trbt555 Posted at: 2015-12-29T09:43:29.176Z Reads: 106

```
RA submitted, waiting for authorization to return + return address.
```

---
## \#12 Posted by: trbt555 Posted at: 2016-01-22T07:21:32.319Z Reads: 91

```
Just to close this thread, I received a store-credit refund from Enertion for this defective VESC.
Too bad I now need to re-pay shipping, local VAT and import duties on anything I get from Enertion to replace an item that should have worked from day one.
Ah well, lessons learned...
```

---
