# Weird braking: force is reduced just before stopping and motor amps spike

### Replies: 1 Views: 248

## \#1 Posted by: egzplicit Posted at: 2017-10-18T09:23:14.975Z Reads: 59

```
Hi guys,

Need your help. I've almost finished my 1st build (build thread will soon be posted) but I found some weird behaviour when it comes to braking. Applying the brakes works fine until just before you come to a stop. At that point it feels the braking force is reduced by 80-90%, the motor stops whining and according to @rpasichnyk metr app, the motor amps spikes.

If you have a look here (values are for a single motor):

[https://metr.at/r/z1ctA?zoom_start=646&zoom_end=684](https://metr.at/r/z1ctA?zoom_start=646&zoom_end=684)

you can see at 5:37:29 PM that I have **-18.1A on the motor and -2.4A on the battery**. Then just before the board stops, the **battery amp is 0A but the motor amps are spiking to 32A (at 5:37:30 PM)**. This is without releasing the brakes on the remote. You can see this behaviour happened before, at 05:35:07 PM.

This happens every time I'm almost at a dead stop. Braking hard from any speed (tested at 20mph for example) works just fine, but again, when it reaches a very low speed (about 2-3mph) the vesc stops most of the braking (there's still some left but only 10-20% at most) and the board coasts to a stop. When this kicks in you can tell because the motors stop whining and you can feel the board not wanting to stop as hard as before that point. It happens regardless of the speed when you start braking... as soon as it's almost stopped, it does it. Every time.

My hardware:

* Dual 5065 140kv sensored motors
* 10s4p 30q 18650 battery with bypassed BMS
* Antispark Switch with fuse
* FOCBOXes connected via can bus
* Nano X remote
* BT module

Software and settings (per vesc):

* Battery max: 20A
* Battery min: -20A
* Motor max: 35A
* Motor min: -35A
* BLDC mode
* 2.18 standard firmware

Nano x was calibrated and PPM signal was correctly set on the master vesc.

Any thoughts? How is it possible for motor amp to spike like that while battery amps are at 0... and most importantly, why are the brakes reduced at that point?

Thanks!
```

---
