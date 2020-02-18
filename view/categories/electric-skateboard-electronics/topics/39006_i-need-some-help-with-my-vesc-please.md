# I need some help with my VESC, please

### Replies: 9 Views: 733

## \#1 Posted by: erikkondo Posted at: 2017-11-22T17:38:48.188Z Reads: 94

```
I have read multiple VESC related posts here and watched several videos, but I still have some problems,  I would appreciate some help.

Here is my setup:

DUAL SETUP

CONTROLLER
(2) VESC from DIY Skateboards Firmware 2.18

MOTORS
(2) Electric Skateboard Motor 6355 190KV

BATTERIES
(2) LIFE Zippy 4200 4S in series for a total of 8S.

BLDC Tool supports 2.17 & 2.18

TRANSMITTER
Flyski FS-GT2B

PROBLEM #1. 

When I setup my Master VESC, I can use the Transmitter to control and spin the motor, but the motor has minimal force. I can hold it with my hand and stop it from turning.
NOTE: I have been unable to get the BLDC to detect the motor successfully.

PROBLEM #2.
When the Master VESC motors turns (weakly), the Slave VESC blinks Red, but it's motor doesn't turn.


I used the following instructions from DIY, to program the dual setup.

Please advise. I am over my head on this.


INSTRUCTIONS FROM DIY
Simply, just turn on power to both VESCs with XT90 Parallel and CAN
bus connectors connected.
Start with Master VESC first and plug in the mini usb cable and
connect to it through the VESC BLDC Tool.
Program the master VESC based off the settings below and repeat the
same process for the slave VESC.
App Configuration > General
Controller ID
For master VESC = 0
For slave VESC = 1
Send status over CAN
For master VESC = Uncheck
For slave VESC = Checked
You want to transfer the data to master VESC over CAN
App to use = PPM
For master VESC = Select PPM
For slave VESC = Select No app
App Configuration > PPM
Control Mode
For master VESC = Current no reverse with brake
For slave VESC = Disabled
Multiple ESCs over CAN = Uncheck
For master VESC = Select both - Multiple ESCs over CAN + Enable
Traction Control (current mode only)
For slave VESC = Select both - Multiple ESCs over CAN + Enable
Traction Control (current mode only)
```

---
## \#2 Posted by: Hummie Posted at: 2017-11-22T17:42:41.122Z Reads: 70

```
things are different when riding than on the bench.  but if you cant get it to pass the test that's a problem somewhere which I don't think settings will solve.  please tell us how it goes with your vescs, I wonder how they perform from different sellers.
```

---
## \#3 Posted by: Martinsp Posted at: 2017-11-22T17:43:24.488Z Reads: 74

```
I would first suggest you to try to fix the detection problem because that is the basic setting necessary for your estate... You could ditch the can bus in worst case scenario but you have to get successful motor detection first. 
Please tell us more about the detection failure

Make sure you have no app selected when doing detection.
```

---
## \#4 Posted by: erikkondo Posted at: 2017-11-22T17:48:22.356Z Reads: 70

```
I have selected No App.

When I try to detect the motor, the motor spins fairly fast. But I get "No detection".
<img src="/uploads/db1493/original/3X/c/b/cb280b4eebb87149518079ac4a7636c23b955e46.PNG" width="690" height="359"><img src="/uploads/db1493/original/3X/a/d/adf80c64e43ff0d38a539c5967603641e09413fe.PNG" width="690" height="361">
```

---
## \#5 Posted by: erikkondo Posted at: 2017-11-22T17:57:13.335Z Reads: 54

```
The Arrows work to spin the motor.
The motor is also free from the wheel,  but the motor is weak, I can stop it with my hand.
```

---
## \#6 Posted by: Martinsp Posted at: 2017-11-22T18:40:35.174Z Reads: 48

```
Does the motor stutter at any point of detection? Maybe upload a video of the detection to YouTube and share a link so we can see and judge better
```

---
## \#7 Posted by: erikkondo Posted at: 2017-11-22T21:06:03.174Z Reads: 49

```
I uploaded a brief video showing what happens when I try to detect the motor with the BLDC tool.

[https://www.youtube.com/watch?v=sA4K7QRPHF8&feature=youtu.be](https://www.youtube.com/watch?v=sA4K7QRPHF8&feature=youtu.be)
```

---
## \#8 Posted by: JohnnyMeduse Posted at: 2017-11-22T22:12:48.087Z Reads: 45

```
Are your battery fully charge?

 Because most of the issue you have are usually cause by weak battery... just make sure you charge them up to 100% before trying to setup anything 😉
```

---
## \#9 Posted by: wafflejock Posted at: 2017-11-22T22:48:44.822Z Reads: 38

```
Check the battery voltage with a voltmeter (vs your start and end cut off) can also try going over to the realtime tab and see if it's showing any faults (or in the terminal tab type faults) or if any of the values look out of wack voltage or amperage wise (typically shouldn't be anything more than an amp or two when just spinning the motor freely but adding friction to it should cause increased amperage to keep it turning).  Believe KB control has a limit in the box as well make sure that is something reasonably high enough.

---

Just watched the end of the vid too agree with others would just focus on the voltage to make sure that's right and make sure there's nothing obstructing the motor or adding friction while doing the detection, doesn't visually appear to do anything too weird to me.  I would do detection with the VESCs individually (1 motor 1 VESC 1 receiver) to keep it simple at first.
```

---
