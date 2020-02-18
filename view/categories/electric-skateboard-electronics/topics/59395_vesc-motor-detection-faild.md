# Vesc motor detection faild

### Replies: 3 Views: 177

## \#1 Posted by: kataklysm Posted at: 2018-06-19T17:57:38.631Z Reads: 47

```
Hi i have big problem, my vesc dont detecting my motor. My setup is:

Sk3 6364 190KV
2x Turnigy lipo batteries 6s and 4s multistar 10c
Vesc 4.12 turnigy Sk8-ESC FW:3.38

My vesc was have old FW and before first connect i was update my FW to 3.38
After this i connected the battery (serial connect to 10s) and my motor.
Vesc tool connect ok.
i chose motor setup wizard 
i chose BLDC
In motor max i set 50A in min -40A
Battery i set to  max 30A and -10A
and i chose sensorless type

And i try to detect my motor in wizard. Unfortunetly red lights on vesc blink 
a few time and program say detect fault

after this i enter to terminal and write "faults", this is my output:

The following faults were registered since start:

Fault            : FAULT_CODE_DRV
Current          : 0.2
Current filtered : 0.2
Voltage          : 41.82
Duty             : 0.008
RPM              : 0.2
Tacho            : 5
Cycles running   : 1
TIM duty         : 423
TIM val samp     : 211
TIM current samp : 25604
TIM top          : 50785
Comm step        : 1
Temperature      : 30.25
 
Fault            : FAULT_CODE_DRV
Current          : -0.6
Current filtered : -0.2
Voltage          : 41.85
Duty             : 0.009
RPM              : 6.4
Tacho            : 8
Cycles running   : 2
TIM duty         : 446
TIM val samp     : 223
TIM current samp : 25470
TIM top          : 50495
Comm step        : 4
Temperature      : 30.33
 
Fault            : FAULT_CODE_DRV
Current          : 0.4
Current filtered : 0.2
Voltage          : 41.83
Duty             : 0.008
RPM              : 3.6
Tacho            : 11
Cycles running   : 1
TIM duty         : 415
TIM val samp     : 207
TIM current samp : 25646
TIM top          : 50878
Comm step        : 1
Temperature      : 30.39
 

Please help. mosfets on vesc looking good
```

---
## \#2 Posted by: Brontech Posted at: 2018-06-19T18:42:14.460Z Reads: 31

```
From what you said, you first updated your firmware before testing if the VESC had a defect from the factory. The DRV may have a defect from the manufacture or you didn't update your VESC properly.
I cant really tell you an exact fix or reason for the error, because I'm not quite sharp in this category.
Good luck! :slight_smile:
```

---
## \#3 Posted by: kataklysm Posted at: 2018-06-19T19:07:19.301Z Reads: 29

```
Yes, i updated vesc before use because vesc tool dont working with old fw.
```

---
