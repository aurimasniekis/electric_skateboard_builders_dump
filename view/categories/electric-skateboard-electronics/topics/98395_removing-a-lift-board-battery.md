# Removing a Lift Board battery

### Replies: 18 Views: 606

## \#1 Posted by: b-rad Posted at: 2019-07-13T19:00:42.061Z Reads: 60

```
Hello I recently stumbled upon a Lift Board and i was trying to salvage the battery for another build but i was having a hard time actually getting to the battery. I removed all the screws but still it seems the battery is stuck in the tube of the aluminum enclosure of the board. I have pictures attached. Does anyone know how i should go about removing the battery from the enclosure?

I was thinking i could just cut the motor wires and then unscrew the charging\power button and then slide the battery out. 

Anyone got any ideas?

![image|374x500](upload://bT3CCmiI2wviDUZWuHtm17mlHJT.jpeg) ![image|374x500](upload://qYqaoZkUR7Y828nQZcnXwljr7sJ.jpeg) ![image|374x500](upload://7jPnAtfcf4qOkCTLAiioOYE9GyY.jpeg) ![image|374x500](upload://seu6RIUB1oLUPI6JxT1Vopdf2Jo.jpeg) [Uploading: 8F60FC88-0A81-43A4-81B0-2C2508865F4F.jpeg...]() [Uploading: F03AEFE2-D8AB-45D9-AF75-0525E640B047.jpeg...]() [Uploading: A78ADEFB-732E-44CC-947A-17F6E3BE305F.jpeg...]()
```

---
## \#2 Posted by: KaramQ Posted at: 2019-07-13T19:22:22.040Z Reads: 52

```
You have to remove the charging port and power button
```

---
## \#3 Posted by: b-rad Posted at: 2019-07-13T19:25:48.804Z Reads: 52

```
What about the motor wires? Should i just cut them
![image|375x500](upload://fbzWWV6bhoPAErEf0BuF81tDxTn.jpeg)
```

---
## \#4 Posted by: KaramQ Posted at: 2019-07-13T19:33:21.309Z Reads: 48

```
You probably have to
```

---
## \#5 Posted by: legend27 Posted at: 2019-07-13T21:07:49.760Z Reads: 47

```
JUST MAKE SURE THERE IS NO POWER GOING THRU WHEN CUTTING :sweat_smile:
```

---
## \#6 Posted by: b-rad Posted at: 2019-07-13T22:25:59.954Z Reads: 44

```
I was able to slide the battery out of the aluminum enclosure. I have the battery as shown in the attached images. There is a main battery wire (xt-60) and on the other side the two red wires are just a fuse.

i was wondering if i can just use a regular lipo/liion 6s charger to charge the battery on the xt60 wires? (With the correct settings of course) 

It seems as the bms is already hooked up to the battery so i wouldent need to hook up balance wires. Im not sure what the other two wires coming out of the battery are though (thin black and red wires).

![image|374x500](upload://k3uZtpCGrsrdKwoi7cyIfj366s6.jpeg) ![image|374x500](upload://Aq7STF833vczIoRXTP6OhfaFRSW.jpeg)
```

---
## \#7 Posted by: Skunk Posted at: 2019-07-13T22:31:45.259Z Reads: 42

```
[quote="b-rad, post:6, topic:98395"]
Im not sure what the other two wires coming out of the battery are though (thin black and red wires).
[/quote]

For Charge port?
```

---
## \#8 Posted by: b-rad Posted at: 2019-07-13T22:34:18.281Z Reads: 40

```
Is there a way to check? 

Because im wondering if it could be the power switch?
```

---
## \#9 Posted by: Skunk Posted at: 2019-07-13T22:44:25.935Z Reads: 43

```
:man_shrugging:
Probably but i wouldn't know.

Didn't you take it apart?
```

---
## \#10 Posted by: b-rad Posted at: 2019-07-13T22:47:26.759Z Reads: 42

```
When i was able to slide the battery out of the aluminum enclosure, the esc is still stuck in the aluminum enclosure. The xt60 and 2 thin wires was the only thing that came off when i was able to slide the battery out. Everything else is still stuck to the ESC which is still stuck in the enclosure...
```

---
## \#11 Posted by: Skunk Posted at: 2019-07-13T22:49:52.429Z Reads: 40

```
I would think the power switch is attached to the esc. So that really should be the wires for charge port.
```

---
## \#12 Posted by: b-rad Posted at: 2019-07-13T23:09:14.958Z Reads: 36

```
Does any one else have any idea about this?
```

---
## \#13 Posted by: Jumpman Posted at: 2019-07-13T23:21:45.734Z Reads: 33

```
Got to agree with @Skunk.  Seems like the thin black wire is attached to C- which is usually the charge port connection.
```

---
## \#15 Posted by: iespoba Posted at: 2019-07-14T05:21:04.753Z Reads: 32

```
i think there maybe an extra screw in the middle holding the esc, i smashed the hell out one trying to get the esc out, i found that there was one more screw in the middle under the foam, pull up all the foam and see if there’s a sneaky lil screw holding out, there were 3 in a row
```

---
## \#16 Posted by: yelnats8j Posted at: 2019-07-14T13:43:51.372Z Reads: 23

```
What are the cells in this board?

My friend has one right now and I wass know if its worth trying to salvage.
```

---
## \#17 Posted by: legend27 Posted at: 2019-07-14T13:52:44.706Z Reads: 22

```
Seems like charge port. Pretty sure “C-“ on he bms is Usually used for charge port. Maybe you can find a schematic of the BMS?
```

---
## \#18 Posted by: b-rad Posted at: 2019-07-14T14:36:57.662Z Reads: 21

```
So as I have read the liftboard has a 21.9V 8.8Ah (LG-HD2-18650-3.65V-2000mAh-6S4P). The supposed range of this battery is 16 miles but after i mod this board i plan to use a Vesc and a 6355 260kv (1500W) motor i am going to be drawing alot more power than the original motor (900W) so i would theoretically say this battery is good for about 8-10 miles after modding the setup. 

After further investigation i can see that the two thin wires (black and red) attached to the battery are in fact the charging port wires as they are coming out of the C- port on the BMS.
```

---
## \#20 Posted by: b-rad Posted at: 2019-07-22T21:23:11.967Z Reads: 9

```
So I recently had the time to play around with this battery and i came to find out that when i plug it into my 6s ESC the connectors get extremely hot ( i replaced the existing xt-60 with an xt-90).

The original wire gauge on the bms was 16 gauge so i thought it would be a good idea to swap out the existing wiring and change it to 10 gauge wire. 

i plugged the battery in and still when i press the throttle for a regular period of time the battery to ESC connectors get extremely hot to touch. is this normal?
```

---
