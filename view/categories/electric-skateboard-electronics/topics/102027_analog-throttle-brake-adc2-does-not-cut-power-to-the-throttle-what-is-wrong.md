# Analog Throttle/Brake &ndash; ADC2 does NOT cut power to the throttle? What is wrong?

### Replies: 1 Views: 61

## \#1 Posted by: 010203040506070809 Posted at: 2019-09-20T17:29:57.058Z Reads: 10

```
Hi everyone,

 

I'm using an Analog Throttle/Brake for an electric scooter that I am using VESC on. The problem is that -- ADC2 does NOT cut power to the throttle (ADC1 is hooked up to the signal wire of the throttle, ADC 2 is hooked up to the signal wire of the brake). If I hold BOTH the throttle and the brake, the motor still runs at full speed. What am I doing wrong? I did the calibration and have ADC1 voltage set to min 0.83v, max 3.3v, center voltage 2v. and ADC2 is set at 0.85v, 3.30v max.

The brake signal is definitely working as I have a brake light attached to it that turns on when i hold the analog brake. Why won't ADC2 cut the throttle from ADC1?

I'm using the control setting Current No Reverse Brake ADC2
```

---
