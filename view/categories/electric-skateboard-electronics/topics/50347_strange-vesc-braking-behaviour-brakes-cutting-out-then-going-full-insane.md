# Strange VESC braking behaviour / Brakes cutting out then going full insane

### Replies: 20 Views: 1075

## \#1 Posted by: Acidfie Posted at: 2018-03-27T18:09:59.618Z Reads: 148

```
So i finished my second built and i have a strange behaviour while braking.

i am using 2 vescs connected via can-bus. 2 ST 6355 190kV motors and i have 10S3P VTC5 battery pack. 

Accelerating works fine without problems but when it comes to braking i have a strange behaviour - if i pull the lever back to start braking it all works very good, just the braking force feels very low. then theres a point that i reach - the brakes cut completely out and after 0.5 - 1 second the go full insane mode, at higher speed throwing one off the board. since the last build did not had this behaviour, i think its a vesc setting i am not aware of.

also, are these settings correct for this setup? never had a dual at all.

![10|690x442](upload://jmqO9CtZ7tKAowB4TtyETlPIfbI.png)![59|690x400](upload://mcG67miY07Lq0Lvl9XVFTr2nT4v.png)
![04|690x445](upload://hMtpuPByOf2BEqK1Q1JINDStfcr.png)![12|690x472](upload://itP9RXSYDm1FsC6YT5nsjvZm6uC.png)
```

---
## \#2 Posted by: Ishayc Posted at: 2018-03-27T19:08:11.759Z Reads: 121

```
What is the vescs brand and what is the drive ratio?
```

---
## \#3 Posted by: theviith Posted at: 2018-03-27T19:08:39.883Z Reads: 125

```
I would uncheck "enable traction control" under "multiple ESC over CAN"
Not sure if that is the primary issue but that's my setting and has been working great for me
```

---
## \#4 Posted by: Acidfie Posted at: 2018-03-27T19:36:47.145Z Reads: 117

```
ESK8 VESC 1.1

drive ratio is i think 35:15

@theviith i think this is no traction control problem
```

---
## \#5 Posted by: Der6FingerJo Posted at: 2018-03-27T19:45:33.449Z Reads: 115

```
Do you have unusually long power wires to the VESC? Or some kind of coil in the wiring? Maybe there are voltage spikes due to induction that trigger maximum voltage and that's why it won't brake anymore.
```

---
## \#6 Posted by: Acidfie Posted at: 2018-03-27T19:55:28.274Z Reads: 110

```
the GND is about 40cm long since its from the battery pack end, is this unusually?

also no coils or else, straight and then splitted up to both esc

NOTE: The problem occurs even with low voltage/empty battery
```

---
## \#7 Posted by: Sebike Posted at: 2018-03-27T20:00:38.545Z Reads: 109

```
Drawing 90 amps from that battery sounds a lot. 

Don't beleive you should draw more than 75 continously from that pack, so lowering Batt max to ~37A not to overheat the cells ?
```

---
## \#8 Posted by: Ishayc Posted at: 2018-03-27T20:00:51.722Z Reads: 107

```
Don’t turn off your vesc and connect it to a pc after this happens and see what error you get in the terminal
```

---
## \#9 Posted by: Acidfie Posted at: 2018-03-27T20:13:53.523Z Reads: 104

```
the VTC5 are rated at 30 amps cont. so i think this should be fine

@Ishayc this happens every time i brake.

could it be from the pulswidth of the recevier? sometime i heard about this..
```

---
## \#10 Posted by: Sebike Posted at: 2018-03-27T20:19:17.804Z Reads: 103

```
according to the mooch's tests he rated these 25A cont cells. if you say 30 is fine, 30 is fine :slight_smile:
```

---
## \#11 Posted by: Ishayc Posted at: 2018-03-27T20:34:21.524Z Reads: 94

```
Connect it to a pc and check the terminal. I bet it can shed some light.
```

---
## \#12 Posted by: Acidfie Posted at: 2018-03-27T21:05:39.031Z Reads: 85

```
i will try it, how long is the error saved?
```

---
## \#13 Posted by: Ishayc Posted at: 2018-03-27T21:16:30.121Z Reads: 83

```
Until you turn your vesc off
```

---
## \#14 Posted by: banjaxxed Posted at: 2018-03-28T09:38:20.967Z Reads: 78

```
Try another remote?
```

---
## \#15 Posted by: Acidfie Posted at: 2018-03-28T09:42:54.542Z Reads: 77

```
i just have this one.. need to get a good one imho. i have this kickz or what it is called idk. looks a bit like the womanizer vibrator.
```

---
## \#16 Posted by: banjaxxed Posted at: 2018-03-28T09:48:03.132Z Reads: 74

```
A mini remote as a baseline may be helpful, sounds weird
```

---
## \#17 Posted by: Acidfie Posted at: 2018-03-28T10:00:38.971Z Reads: 72

```
found it

![MTSKR1512-6X3|600x300](upload://crDH3OblodzueGpvcrCPxM3HxnJ.jpg)
```

---
## \#18 Posted by: Acidfie Posted at: 2018-03-28T15:51:15.270Z Reads: 57

```
no fault codes displayed.
```

---
## \#19 Posted by: Ishayc Posted at: 2018-03-28T15:54:36.029Z Reads: 56

```
Then it might be the remote as @banjaxxed said.
```

---
## \#20 Posted by: Acidfie Posted at: 2018-03-28T15:56:35.302Z Reads: 56

```
i lowered the pulsewidth, i will give it a try but it rains here..
```

---
