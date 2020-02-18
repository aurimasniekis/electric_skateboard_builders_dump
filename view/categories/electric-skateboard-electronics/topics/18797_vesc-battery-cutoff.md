# VESC battery cutoff

### Replies: 7 Views: 1615

## \#1 Posted by: faaailix Posted at: 2017-03-09T10:26:26.329Z Reads: 253

```
Hi,
I just finished my first diy skateboard build. I run a single mounted 270KV motor with an 8S LiPo (2x4S in series), and I use VESC in BLDC mode. I tested it and I'm happy with it so far. However, there is one thing I don't quite understand. To protect my battery, I set battery cutoff start to 8*3.5V=28V, and battery cutoff end to 8*3.3V=26.4V using the BLDC tool. I wrote configuration to the VESC and to guarantee it's written, I reconnected the VESC and read configuration, showing that the correct values have been written. So far so good. However, just as a test I connected a 4S LiPo to the build and pressed the throttle - and the motor was spinning. I expected it to not work sine the supplied voltage is far below the set battery cutoff voltage. Does someone share this experience or can explain why this happens?
Best and thanks in advance.
```

---
## \#2 Posted by: benwong Posted at: 2017-03-09T14:18:20.348Z Reads: 237

```
means the cut off feature not working? 
i also curious that.
```

---
## \#3 Posted by: faaailix Posted at: 2017-03-09T14:23:06.574Z Reads: 233

```
It seems like. But maybe I just don't understand exactly how the cutoff is working. Maybe someone here has a good explanation why I can use a 4S LiPO to power my board, even though I set the voltage cutoff end to 26.4 V.
```

---
## \#4 Posted by: Ackmaniac Posted at: 2017-03-09T18:19:55.817Z Reads: 218

```
Can you please check again to really make sure that the actual settings are at 26.4V. If that is really the case then I will try to find the reason in the firmware. And please also check in the Realtime tab what the actual voltage is.
```

---
## \#5 Posted by: faaailix Posted at: 2017-03-09T19:31:20.668Z Reads: 194

```
I just checked again. Everything is correctly written to VESC (battery cutoff at 26.4). However, I think I misunderstood something: I tried again with 4S (as before), with the board laying with wheels upside down. The wheels spin when I press the throttle. But when I put the board back on the ground the torque is by far to weak to move the board even without me standing on the board. So I guess everything works fine. I thought the battery cutoff wouldn't allow any current, but it seems like there is a very little current supplied to the motor that is large enough to spin the motor without load. @Ackmaniac, would you say that's a correct interpretation?
```

---
## \#6 Posted by: faaailix Posted at: 2017-03-23T10:41:25.457Z Reads: 158

```
I finally got my first ride (hell yeah) and the battery cutoff worked perfectly fine.
```

---
## \#7 Posted by: Ackmaniac Posted at: 2017-03-23T11:21:06.494Z Reads: 147

```
thx for the update
```

---
