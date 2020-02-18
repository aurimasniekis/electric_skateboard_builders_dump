# Motor is pulling 2A and is HOT

### Replies: 13 Views: 1327

## \#1 Posted by: Hillso Posted at: 2016-11-04T11:54:16.833Z Reads: 178

```
Last time I rode the key fell, so I inserted loctite in the small slit between the key and the shaft, and left the motor vertical... the loctite got to the motor. 
the motor now spins with friction.
I haven't succeeded removing the pulley / key. 
any idea what can I do? Thanks.
next time I will use loctite 648 without any key or screw (and put the motor horizontally), it seems like the easiest way

the motor now uses 4 amps no load without the belt.

<img src="/uploads/db1493/original/3X/4/b/4b5a96a4c0bd737c3e4f1577ffa27bab6c7b7fc1.jpg" width="666" height="500">
```

---
## \#2 Posted by: mmaner Posted at: 2016-11-04T12:08:07.138Z Reads: 179

```
Use heat to remove the pulley.
```

---
## \#3 Posted by: onloop Posted at: 2016-11-04T12:13:55.111Z Reads: 179

```
Best bet is to cut (dremmel / grinder) the pulley off completely and start again.

Maybe you will disassemble the motor after you removed the pulley & Make sure the bearings aren't thread locked. Or just remove and replace them.

It is possible to install the pulley onto a motor shaft using the key as a wedge. Similar to how axe heads are installed onto handles.

You can also use a ground down, normal bearing spacer (remove 3mm). Place it on the motor shaft before pulley to ensure the pulley stays in correct position when you hammer the key in.
```

---
## \#4 Posted by: TheImmortalJew Posted at: 2016-11-04T13:10:28.187Z Reads: 166

```
Heat is the only way to get loctite loose. If you want more localized heat, use a soldering iron.
```

---
## \#5 Posted by: TarzanHBK Posted at: 2016-11-04T13:12:08.693Z Reads: 160

```
also be carefull with heat, don´t let the motor heat up too much. It will loosen the magnets
```

---
## \#6 Posted by: elkick Posted at: 2016-11-04T13:19:15.616Z Reads: 156

```
You could try it like this: http://www.esk8.de/tutorials-d-e-f/motor-pulley-removal/
```

---
## \#7 Posted by: Nowind Posted at: 2016-11-05T09:25:03.525Z Reads: 130

```
Have had a similar problem once i glued my Pulleys to the Shaft, and let it dry with the Pulley higher then the Motor...runs into motor.... motor turns really hard now
I took the brutal way : let the motor run for a while, it melted the Loctide and all was good. You can smell when the Loctide has gone. 
Do on own risk (-;
```

---
## \#8 Posted by: Jebe Posted at: 2016-11-05T10:24:55.039Z Reads: 129

```
Heat it. Butane torch will do it. Bearing puller helps.
```

---
## \#9 Posted by: Hillso Posted at: 2016-11-05T10:41:57.506Z Reads: 122

```
The key is stuck mechanically and prevents pulleying out the pulley.

EDIT: I have test ridden the board and it looks like the loctite wore out. I was probably too paranoidic. Thanks guys for the help.
```

---
## \#10 Posted by: Hillso Posted at: 2016-11-06T13:47:24.734Z Reads: 95

```
My setup is 245kv 8s 5Ah.
After the ride, the mosfets were cool, and the motor was hot to touch. 
Is it normal, or does it means that the friction is too high, or something else?
```

---
## \#11 Posted by: Hillso Posted at: 2016-11-07T11:58:52.145Z Reads: 79

```
I successfully removed the pulley by removing the bolts that hold the motor to the mount so that the mount is between the pulley and the motor, and then rotating the board so that the motor hangs by the pulley, and then hammering the axle with a chisel. little by little the pulley came out.

then I cleaned all the parts that looked not clean outside the motor, and then I disassembled the motor and cleaned it inside.

the motor now takes 2.5 amps at max duty cycle on current control (50k erpm, no pulley), and the front stator plate still gets too hot to touch for more than 1.5 seconds after 1-2 minutes of max duty cycle (no load). VESC is 35-40 celsius. stator front plate and windings feel like 80 celsius.

bearings feel good. I don't know what to do, and want to ride so bad after I rode it for the first time :sob:

<img src="/uploads/db1493/original/3X/5/a/5a334f5fcdc74195e2882bdba6d4af604853c06e.PNG" width="690" height="389">

<img src="/uploads/db1493/original/3X/d/9/d9ed6d1cc1170ac635265bbe557a08a06ad44c5f.PNG" width="690" height="460">
```

---
## \#12 Posted by: Hummie Posted at: 2016-11-07T16:02:02.286Z Reads: 64

```
Maybe the bearings feel good but not. Oil them. To get that hot that quickly without many amps I think there must be friction somewhere
Or maybe u have the ramping bug?  Someone would know better than me where to find it
```

---
## \#13 Posted by: Hillso Posted at: 2016-11-07T18:00:50.400Z Reads: 55

```
max current ramp step configured ok
<img src="/uploads/db1493/original/3X/8/0/80f162bb4be4c04f1463c6806b39d901fe4f3be2.PNG" width="690" height="346">
VESC version is 4.12, firmware 2.18


EDIT:  maybe the motor timing settings are causing this?
[quote="Daniel92104, post:4, topic:548, full:true"]
Also the higher the motor timing is the hotter the motor casing can get. Not good if you want the motor to last. These motors were made to run at 8 degrees but that was if it was only turning a propeller. Not the case here with all this weight holding the motor back from turning hence you end up with motor cogging at start and must push start the board . At 0 degrees a push start is not needed if on a flat Street.
[/quote]

Where can I see and change the timing angle? thanks.
```

---
