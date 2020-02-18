# vESC output **Help** New build Rayne DualRear Enertion kit mechanical, motor, electrical, nunchuk

### Replies: 7 Views: 1709

## \#1 Posted by: davinzz Posted at: 2015-12-23T20:37:33.423Z Reads: 129

```
Hi Builders,

Just start building a eSkate on a Rayne.
It gonna be great but:
- I'm stuck having the motors spin (detection failed).
- Nunchuck display in bldc

So the config:
1 Rayne Deck
1 Enertion SPACE cell
2 vESCs via CAN
2 Enertion motors
1 Nunchuk via the built-in vESC App

I can access both vESCs v2.5 (read/write/upgrade) via BLDC mac. Led is ON on each vESC.
vESCs are connected via CAN, CAN is working, I can see realtime data from the slave vESC when usb-connected to the master vESC using BLDC (mac) with 'CAN Fwd' enabled.

Nunchuck and its dongle are in sync (led blinks when nunchuck is not connected, led is on when nunchuck is connected, 1 blink when pressing the button Z or C.
Dongle is connected to the master vESC, wire mapping is as per FAQ (Rx green pin1, Tx blue pin2, GND black pin4, 3,3v red Pin5 on a JST 6pin male connector plug into a 7pin female (ADC2 pin is shifted). 

FAQs are not helping me anymore. Basically:
Nothing OUT of the vESCs to the motor
Seems that nothing IN from the Nunchuk

I'm stuck!  ;) Any ideas?
Thanks
```

---
## \#2 Posted by: NIK Posted at: 2015-12-23T21:23:18.520Z Reads: 118

```
Hi @davinzz

Do you get any fault code in the realtime data? Like DRV8302 or MOSFET. Bottom left box in your bloc tool.
```

---
## \#4 Posted by: psychotiller Posted at: 2015-12-24T00:03:40.433Z Reads: 112

```
Just went through this myself! After you changed your setting to Nunchuck did you reboot? Once I did that things started to come to life.
```

---
## \#5 Posted by: davinzz Posted at: 2015-12-24T08:58:19.322Z Reads: 107

```
Hi,
Thanks for your advices, here is screenshot of Real Time Data for both vESCs.
Esc1: Fault code: Over_temp_fet
Esc2: Fault code: None

I reboot after each configuration changes.

<img src="/uploads/db1493/original/2X/b/b65058370c5070e94d1d64cec4866bc2efc8654d.jpg" width="690" height="434"><img src="/uploads/db1493/original/2X/f/fa8090f44c3629692b7b5644cbca5ef327f74546.jpg" width="690" height="434">
```

---
## \#6 Posted by: davinzz Posted at: 2015-12-24T09:18:25.341Z Reads: 98

```
here is some other BLDC screenshots:
<img src="/uploads/db1493/original/2X/c/c85db05fedd9637e7a2f0d0d98e9a2b64a0fa3a0.jpg" width="690" height="434"><img src="/uploads/db1493/original/2X/8/8d3a34cfcb64906821cfe29f6f8d38d28e631bb0.jpg" width="690" height="434"><img src="/uploads/db1493/original/2X/f/f6f1dc1432a062cdd93a77078fa88d6eb2d285ed.jpg" width="690" height="434"><img src="/uploads/db1493/original/2X/c/c0fc35bc13682a12954f05858879323da84979e5.jpg" width="690" height="434"><img src="/uploads/db1493/original/2X/e/ea7c05d8d9c6540d55c629dd908bd04ec7e9f148.jpg" width="690" height="434"><img src="/uploads/db1493/original/2X/e/e69a4be555083070e8455e2c649386e87ddb7f90.jpg" width="690" height="434"><img src="/uploads/db1493/original/2X/8/8861e7910487b8dafaa233957d497e88e577e17a.jpg" width="690" height="434">
```

---
## \#7 Posted by: davinzz Posted at: 2015-12-24T09:25:00.910Z Reads: 88

```
Temp on ESC 1 from 0 to 23sec, ESC 2 from 23sec and up
<img src="/uploads/db1493/original/2X/f/fa469f9c43bd7f7473ebb7de3fdfa588e2b4d39c.jpg" width="690" height="434">
```

---
## \#8 Posted by: davinzz Posted at: 2015-12-24T09:32:46.797Z Reads: 90

```
the beast sleeping ;)
<img src="/uploads/db1493/original/2X/4/41b9071398f3a6316a33e04c89024634b033f9c1.jpg" width="281" height="500">
```

---
