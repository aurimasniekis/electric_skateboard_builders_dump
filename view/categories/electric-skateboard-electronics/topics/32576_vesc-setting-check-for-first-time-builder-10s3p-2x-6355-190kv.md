# VESC Setting Check for first time builder - 10s3p - 2x 6355 190kv

### Replies: 2 Views: 689

## \#1 Posted by: cody00 Posted at: 2017-09-08T01:54:25.910Z Reads: 115

```
Hi All, I recently built a board after spending weeks of reading here in the forums.  Everything went well and board is working amazing.  I just want to confirm that I didn't make any gross mistakes that is going to burn up my VESC or Batteries.  I realize these are fairly agressive settings, but does anyone spot any dangers or big mistakes here?

I didn't have any heat issues after some riding today.  The only hiccup i had was when braking regen on a full battery today through the BMS and it spiked past 57V cutting out the VESC.  After riding for about 30 seconds it drained the battery enough where it worked as normal.

10s3p with LG HG2
2x Torque ESC VESC with Canbus & Sensor in Hybrid
2x Torque 6355 190kv
Charge and Discharge through BMS 42V 60A

<img src="/uploads/db1493/original/3X/8/c/8c01f6adcd8bd903d5f0d8e6e4ef2d95aae94d5a.png" width="690" height="431">
```

---
## \#2 Posted by: cody00 Posted at: 2017-09-15T01:14:49.080Z Reads: 82

```
Maybe more specific questions

I understand Motor Max, Motor Min but having issues with Batt Max/Matt Min.  Is Batt Max the limit of AMPS that the VESC will pass through to the Motor?  With dual vesc, 10s, and BMS current protection of 60A, should it never be higher than a combined 60A?  So I should set each VESC to 30A Batt Max?

In a similar fashion, if someone is using a 40A fuse, should you limit the max to 20A for each VESC if dual?

I am also discharging through BMS with the following SPECS.
> Over-discharged threshold: 2.90 ± 0.05 V
> Over-discharged delay: 5mS
> Over-current Protecton: 60 A
> Max Continuing discharge Current : 60A
> Max Charge Current : 30A

Can someone let me know where my thought process is flawed?
```

---
