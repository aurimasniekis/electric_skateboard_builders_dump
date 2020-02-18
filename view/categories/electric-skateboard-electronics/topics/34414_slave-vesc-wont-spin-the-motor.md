# Slave VESC won&rsquo;t spin the motor

### Replies: 30 Views: 1004

## \#1 Posted by: Colson003 Posted at: 2017-09-30T21:23:43.308Z Reads: 116

```
I've had my board as a single motor and just got the second motor and VESC today. I'm using canbus and followed what @skslingo21 said and now my new VESC won't spin the motor. Just three red flashes in series, the older VESC still works and spins. Any ideas??
```

---
## \#2 Posted by: aigenic Posted at: 2017-09-30T21:39:21.872Z Reads: 112

```
Maybe DRV fault? Check out real time data in BLDC programm if there is some kind of error...
```

---
## \#3 Posted by: ElskerShadow Posted at: 2017-09-30T21:42:02.376Z Reads: 106

```
Have you done properly motor detection ? And applied the Can fwrd ?
```

---
## \#4 Posted by: Colson003 Posted at: 2017-09-30T23:11:27.687Z Reads: 95

```
@aigenic fault code: NONE
```

---
## \#5 Posted by: Colson003 Posted at: 2017-09-30T23:12:47.689Z Reads: 86

```
@ElskerShadow yeah I did the motor detection and chose Id 1 and Ticked CAN Fwd on the master with the CAN connected
```

---
## \#6 Posted by: Colson003 Posted at: 2017-09-30T23:14:15.100Z Reads: 83

```
<img src="/uploads/db1493/original/3X/5/6/56870c5f574514957d00056f826d6efe1d1b5664.jpg" width="666" height="500">
```

---
## \#7 Posted by: Colson003 Posted at: 2017-09-30T23:21:22.954Z Reads: 79

```
I typed can_devs into the terminal and the master detects the slave.
```

---
## \#8 Posted by: faithfulpuppy Posted at: 2017-09-30T23:38:10.919Z Reads: 78

```
Check that the slave works on its own
```

---
## \#9 Posted by: Colson003 Posted at: 2017-09-30T23:41:06.516Z Reads: 76

```
ok. Give me a few minutes.
```

---
## \#10 Posted by: Colson003 Posted at: 2017-09-30T23:44:48.593Z Reads: 79

```
@faithfulpuppy it does not. Series of three flashing lights.
And no fault codes in realtime data.

EDIT: I applied throttle and it gave DRV8302, didn't realize I had to do that for the code to show up.
```

---
## \#11 Posted by: faithfulpuppy Posted at: 2017-10-01T00:10:29.882Z Reads: 73

```
Welp, guess that solves it. Sorry bro.
```

---
## \#12 Posted by: Namasaki Posted at: 2017-10-01T00:26:01.816Z Reads: 74

```
What do you think broke the DRV chip? 
Setting up canbus incorrectly?
```

---
## \#13 Posted by: Colson003 Posted at: 2017-10-01T02:02:05.638Z Reads: 72

```
I'm not sure what caused it. I'm pretty sure I followed the instructions correctly, but I may have connected it before setting up the id's.
```

---
## \#14 Posted by: Namasaki Posted at: 2017-10-01T02:21:40.704Z Reads: 68

```
My advice to anyone is to forget Canbus and just run dual masters with split ppm with just signal wire from one of the vescs. And all 3 wires for the other Vesc.
It's the simplest and safest setup for Vesc 4
oops, here we go again....
```

---
## \#15 Posted by: Colson003 Posted at: 2017-10-01T02:27:06.056Z Reads: 69

```
Yeah I've read lots about that argument and wanted to try the traction control. I have an extra ppm cable. Which single wire do I keep?
```

---
## \#16 Posted by: Namasaki Posted at: 2017-10-01T02:31:27.907Z Reads: 70

```
It doesn't matter as long as you only feed 5v from one vesc to the receiver.
If you try to feed 5v from both Vesc, it will damage them.

This rule was the same when we where using dual car esc's
```

---
## \#17 Posted by: Colson003 Posted at: 2017-10-01T02:39:15.629Z Reads: 72

```
I was just thinking, one VESC was running hybrid and the other was sensorless (couldn't get the other to spin properly while in hybrid) could that have messed it up too? The master was the hybrid.
```

---
## \#18 Posted by: Namasaki Posted at: 2017-10-01T02:41:32.550Z Reads: 67

```
One was sensored and the other was not sensored?
I dont know, maybe someone else can answer that.
```

---
## \#19 Posted by: Colson003 Posted at: 2017-10-01T02:45:31.389Z Reads: 63

```
Correct.
10 characters.
```

---
## \#20 Posted by: Namasaki Posted at: 2017-10-01T02:47:53.737Z Reads: 67

```
I would think that it is not possible to run like that with Canbus.
Just dont know if it would blow the drv
```

---
## \#21 Posted by: cwazy1 Posted at: 2017-10-01T03:17:42.179Z Reads: 62

```
and another one bites the dust from canbus.
```

---
## \#22 Posted by: ElskerShadow Posted at: 2017-10-01T08:14:37.335Z Reads: 58

```
It might be the problem. 2 differents modes maybe the can tried to applied that to the slave and fried it. Donyou know someone that can replace your drv chip ?
```

---
## \#23 Posted by: Colson003 Posted at: 2017-10-01T16:14:32.870Z Reads: 53

```
@ElskerShadow yeah I've already sent an email to the DRVwizard. $45 is worth it.
```

---
## \#24 Posted by: karma Posted at: 2017-10-01T19:01:38.305Z Reads: 51

```
How did you connect the can bus cable? After setting up settings for each VESC, master and slave, did you disconnect the power cables from both VESCs, plug in the CANBUS cable, then plug in the power leads from the battery at the same time with a parallel connector? I set up my build with canbus last night and it worked out fine after some fiddeling around.
```

---
## \#25 Posted by: Colson003 Posted at: 2017-10-01T19:16:56.989Z Reads: 51

```
Yes, but I don't think that I had the id set correctly when I did.
```

---
## \#26 Posted by: karma Posted at: 2017-10-01T19:25:19.540Z Reads: 51

```
I have a hard time thinking the id would cause the DRV to blow up.
```

---
## \#27 Posted by: taroko Posted at: 2017-10-01T19:26:17.163Z Reads: 51

```
Is Canbus not robust once you get it working? Are there common failures that can occur by using it?

I have mine working. It has been reliable, but I've only used it for about 30km so far.
```

---
## \#28 Posted by: Namasaki Posted at: 2017-10-01T19:44:23.772Z Reads: 50

```
The only reliability issue that I know of is the canbus wire falling out of the socket with vibration and causing damage.
Other than that, there is just too many ways that you can damage the Vesc with canbus by not getting the settings right or by not powering both vescs at the same time. 
It seems a bit complicated and one misstep and your toast.
I just always went with split ppm or dual receiver because of the simplicity and redundancy.
```

---
## \#29 Posted by: Texknocreeper Posted at: 2019-04-30T05:14:25.187Z Reads: 20

```
Currently two issues
1.) any setting a try to apply to VESC will not stay it just goes back to default.
2.)slave motor will not spin while using reciver but it works when checking for motor spin direction in software 
Info 
Dual 6374 with 2 VESC from 
Have can bus connector and it’s powered on
Using latest version of tool and software for VESC
```

---
## \#30 Posted by: Andy87 Posted at: 2019-04-30T07:26:11.199Z Reads: 18

```
are you sure you connected to the vesc?

do you power on both vescs in the same moment?

did you go through all wizards and it still don´t take the settings?

if you didn´t save the motor detection results to your vesc you can´t spin your motors via remote.

maybe upload a video how the situation is. might help us to find your problem.
```

---
