# Something is wrong. Please help

### Replies: 4 Views: 422

## \#1 Posted by: Shahar9320 Posted at: 2017-09-21T08:30:39.115Z Reads: 119

```
Hey guys, so the other day I rode into a little puddle of water by mistake , and since then the board just don't work and I have no idea what is wrong.
At first I thought it was the motor because everything seemed to work - the battery turns on , so is the vesc and the receiver and remote (all are in an enclosure) but I took the motor to a technician that said the motor is fine and now I have no idea what could be wrong . Did this happen to anyone ?? Please help!
```

---
## \#2 Posted by: Der6FingerJo Posted at: 2017-09-21T09:07:03.127Z Reads: 112

```
So in theory RC Brushless Motors are at least splashproof so that's probably not the cause. If the battery still shows voltage on the outputs, everything should at least turn on. 
Next step would be checking in on the VESC using BLDC/VESC Tool and trying to see whether there's a signal from the remote or not. You can also try to spin up the motor using the tool. If nothing responds you could check the error codes in the real-time data tab and if nothing connects at all the whole ESC is gone. 
Just be careful when doing this in case there's a short somewhere and something in the PCB blows up.
```

---
## \#3 Posted by: Martinsp Posted at: 2017-09-21T15:47:55.779Z Reads: 86

```
My guess would be that the water that got in the motor might have shorted the phase wires/output of the VESC together and blow the FET/s maybe even a DRV. But if you dont get any faults in BLDC-tool you might have blown FETs only. Just a guess because there is not enough evidence (pictures etc)
```

---
## \#4 Posted by: Shahar9320 Posted at: 2017-09-21T20:08:23.500Z Reads: 59

```
thanks for the reply. just checked the bldc tool and the drv is gone. im considering buying a focbox now..
```

---
