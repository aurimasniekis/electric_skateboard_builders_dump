# Overheated VESC Replaced a new DRV8302

### Replies: 11 Views: 970

## \#1 Posted by: Deakbannok Posted at: 2017-10-21T12:36:23.810Z Reads: 158

```
Hi. A few weeks ago I have bought a new motors to upgrade a dual drive build.
One of the motor shorted both of my VESC on a test hall sensored detection in FOC. Because one of the mounting bolt touching the motor coil.
It causes both of my VESC heated up rapidly on DRV8302.
Now I have replaced both of the DRV8302. (It was a tricky for first time)
But the problem is still persisting, powered on connected USB; DRV8302 started to heat up and get fault code on one of the VESC is OVER VOLTAGE
other VESC, is older version will not show fault codes.

What could it be?
Thank you
```

---
## \#2 Posted by: Deakbannok Posted at: 2017-10-21T12:38:29.504Z Reads: 157

```
<img src="/uploads/db1493/original/3X/9/b/9b159ed923bbfc6fc4f224764ea0266ac1fabe81.jpg" width="281" height="500">
```

---
## \#3 Posted by: JohnnyMeduse Posted at: 2017-10-21T17:53:34.426Z Reads: 142

```
Check the Mosfet, They are most likely to blow before the DRV.. And check all the resistor around the DRV and the mosfet specially R48 to R51... 


https://www.youtube.com/watch?v=SQxAmLe63Fs
```

---
## \#4 Posted by: Deakbannok Posted at: 2017-10-21T20:06:32.379Z Reads: 120

```
Thank you Johny. I was wondering where can i find these mosfets to replace?
```

---
## \#5 Posted by: JdogAwesome Posted at: 2017-10-21T21:06:11.576Z Reads: 118

```
I forgot what type of MOSFET the FOCBOX uses but it should say right on the top of it. Once you have the the name of it just look it up on either Mouser, Digikey, Arrow or whatever trusted seller you normally use. Personally I love Arrow way cheaper than mouser or Digi and free shipping.
```

---
## \#6 Posted by: Deakbannok Posted at: 2017-10-22T10:38:45.705Z Reads: 101

```
this is what I have found
https://octopart.com/irf7749l2tr1pbf-international+rectifier-12634961

not sure is the right one or not.
```

---
## \#7 Posted by: Deakbannok Posted at: 2017-10-22T11:27:38.597Z Reads: 92

```
<img src="/uploads/db1493/original/3X/f/e/fe56b717c09ba9337940510dbcaf31bb848cf5e9.jpg" width="690" height="333">

Mosfets are good. I did replace them.
it still giving me a fault code.

Fault_code_over_voltage
```

---
## \#8 Posted by: Deakbannok Posted at: 2017-10-22T12:39:13.974Z Reads: 82

```
The highlight in red marker is where the hot areas beside DRV8302
<img src="/uploads/db1493/original/3X/2/d/2db48f37f998a6289829eb61edb91e631de56305.jpg">


Blue marker are the ones I have replaced.
<img src="/uploads/db1493/original/3X/f/9/f9eab6766708185510be3a0ad0b92ea38622dc06.jpg" width="361" height="500">
```

---
## \#9 Posted by: JohnnyMeduse Posted at: 2017-10-22T13:55:19.780Z Reads: 72

```
These mosfet need to be solder dead center or they might short. 

<img src="/uploads/db1493/original/3X/e/3/e34ea1a7a036aed65c86a7025e9f86d503344ccb.png" width="361" height="500">

Also, Make sure that you have 5V on the 5V leg (C33) if not the Drv is badly solder and the TVS diode is most likely to be blown.
```

---
## \#10 Posted by: Deakbannok Posted at: 2017-10-22T16:14:52.432Z Reads: 70

```
@JohnnyMeduse  Are you talking about these 2?  C33 and D5.
If I am not wrong these two are the diode. and they supposed to be oneway check valve.
When I checked with multimeter, I get a both beep reading on both A+ and C-. So these 2 are shorted most likely?
<img src="/uploads/db1493/original/3X/7/3/73a8681ede81222f716f9ac165b772d46ca7beca.jpg" width="589" height="500">
 
This one is reading out normal
<img src="/uploads/db1493/original/3X/e/1/e1130af65a617ecb7284b5f5eaa8f3588d72a864.jpg" width="635" height="500">
```

---
## \#11 Posted by: Deakbannok Posted at: 2017-10-24T10:53:56.806Z Reads: 54

```
Can anyone direct me please. What are these part number for D5 and C33 on Mouser.
D5 is TVS diode 5v and C33 is 100u.

Thank you
```

---
