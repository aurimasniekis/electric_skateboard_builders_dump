# VESC X, SK3 6374 configuration problems

### Replies: 16 Views: 1237

## \#1 Posted by: Concept Posted at: 2017-02-07T08:13:58.796Z Reads: 168

```
Hello All

Attempting new setup: VESC X v1.3 (firm 2.18) - SK3 6374 - 9S - BLDC compatible with 2.17 & 2.18

The motor detection in FOC sometimes fails and on the odd attempt where it says it has worked I still cannot control the motor with the arrow keys as it either hums/stalls or it is very jittery. I have also tried BLDC but that constantly gets bad detection results. 

Voltage settings are Min 6V, Max 42V, Batt cutt start 32V, Batt cut end 29V. All other motor config default.

let me know what other info will help.
```

---
## \#2 Posted by: Ackmaniac Posted at: 2017-02-07T08:29:48.292Z Reads: 165

```
Just set the max Voltage to 57 V and give that a try.
```

---
## \#3 Posted by: Concept Posted at: 2017-02-07T10:56:44.378Z Reads: 157

```
Hi, gave the 57 volts setting a try but same result. Motor has intermittent problems detecting and when I do get a clear run through the Measure R and L, Measure (Req: R) etc I have a humming motor which will not spin.

To note I have gotten the motor to spin previously just seem to get varied results.
```

---
## \#4 Posted by: onloop Posted at: 2017-02-07T11:02:47.758Z Reads: 149

```
please show a picture of your motor connections and soldering.
```

---
## \#5 Posted by: Concept Posted at: 2017-02-07T11:33:52.008Z Reads: 149

```
Apologies as I do not have great lighting tonight. Photo shows wiring and then I have removed some heat shrink to show a couple of the joints. 
Also I get some red lights flashing on the vesc during detection but when I view Fault in the Terminal tab I get FAULT_CODE_NONE
<img src="/uploads/db1493/original/3X/9/e/9e861320d88def44dd9acca2d2c4379ec149847e.jpg" width="281" height="500"><img src="/uploads/db1493/original/3X/3/6/36cc9bede56c89ad54df42df446be67c62b275a4.jpg" width="281" height="500">
```

---
## \#6 Posted by: Ackmaniac Posted at: 2017-02-07T11:49:31.636Z Reads: 139

```
Please post screenshots of the Motor General, BLDC, FOC and Advanced Tab. And also the Applications General and PPM Tab.
And please check the voltage in the Realtime Data Tab when you enable "Activate Sampling"
```

---
## \#7 Posted by: Concept Posted at: 2017-02-07T12:01:22.017Z Reads: 139

```
<img src="/uploads/db1493/original/3X/1/9/19fddab0d3e87f0dbb2b5e2f31a4722665cf1ece.png" width="690" height="360">
<img src="/uploads/db1493/original/3X/0/c/0cea940d68b894433b2d5a89643dc7ee37854e5b.png" width="690" height="359"><img src="/uploads/db1493/original/3X/b/7/b73c876c0961f8cf5a24b5958904813cdb278d77.png" width="690" height="359">
<img src="/uploads/db1493/original/3X/4/7/47b08eb01f5ba9624436760bcc506795f8ea21a5.png" width="690" height="356">
```

---
## \#8 Posted by: Concept Posted at: 2017-02-07T12:12:37.461Z Reads: 134

```
To confirm testing battery voltage on the XT60 which connects to the VESC I am getting 37.6 volts but battery voltage on Realtime is 6.8 volts?

<img src="/uploads/db1493/original/3X/0/2/0224f5238a0ebfb395269bdfb6bec69c673ac922.png" width="690" height="358">
<img src="/uploads/db1493/original/3X/8/6/869478b41f50b5446eb5a436c00bbb3ab4b917c0.png" width="690" height="357"><img src="/uploads/db1493/original/3X/7/5/752b94baf63f752ece34492af443f034b00166f2.png" width="690" height="361">
```

---
## \#9 Posted by: Ackmaniac Posted at: 2017-02-07T12:22:50.394Z Reads: 128

```
OK there we go. The battery voltage is absolutely wrong. 6.8V is not even close to a charged battery. So please check the battery with a voltage meter. Could it be that the battery is damaged. Normally with a LiPo it shouldn't go below 3.3V a cell (29.7V in your case for a 9S)
And for a 9S Battery (i guess a Lipo) the cutoff start should be 32.4V (3.6V a cell) and end 30.6V (3.4V a cell).
Also the FOC detected values can't be correct. They are too low. 
So first your battery issue needs to be solved and then you can do the FOC motor detection again.
Don't run the motor with those settings because you will damage the VESC with these FOC values.
```

---
## \#10 Posted by: Concept Posted at: 2017-02-07T20:51:30.646Z Reads: 115

```
Thanks for the assistance.
I will have to wait until after work to do anything further. I assume I will have to open up the VESC to determine where the 37.6 volts drops down to 6.8 volts?
```

---
## \#11 Posted by: Ackmaniac Posted at: 2017-02-07T21:54:24.891Z Reads: 107

```
No need to open the VESC. Check you battery first with a multimeter if it really has that voltage.
```

---
## \#12 Posted by: Concept Posted at: 2017-02-08T00:28:38.644Z Reads: 109

```
Yes I have checked the battery several times and have gotten between 37.8 and 37.5 volts each time. I have not tested while connected as everything is insulated. I will just have to cut some away some spots along the wiring harness so I can test it whilst powered up/under load. 

I will separately test the batteries individually under load just to try and eliminate everything I can.
```

---
## \#13 Posted by: Concept Posted at: 2017-02-08T09:14:40.439Z Reads: 98

```
Ok so I have checked the voltage whilst powered up and it is currently sitting at 37.4 volts. I have checked the power on the connections to the VESC and it is also sitting at 37.4 volts. At the same time I have run the Realtime data and Battery voltage is saying around 6.4 volts. This does not make sense does it? So am I correct in saying there is something wrong with the VESC?

Still getting FAULT_CODE_NONE in the Terminal tab.
```

---
## \#14 Posted by: Concept Posted at: 2017-02-09T02:14:11.738Z Reads: 81

```
Update:
Enertion support are arranging a replacement of the VESC X. Thanks to Ackmaniac for the fault finding assistance and Enertion for monitoring the posts and offering the replacement before being approached about it.
```

---
## \#15 Posted by: Tampaesk8er Posted at: 2017-02-11T12:55:48.056Z Reads: 75

```
Try using different USB cables, I had an issue with my vesc where it wasnt connecting properly and tried 4 different USB cables and finally one of them made the vesc work correctly.
```

---
## \#16 Posted by: Concept Posted at: 2017-02-15T03:12:42.586Z Reads: 64

```
Hi Tampaesk8er, I can try this next time but I have already sent back the VESC for a replacement. Thanks for the tip.
```

---
