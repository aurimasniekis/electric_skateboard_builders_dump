# Vesc chider over current spike after revive attempt and a replaced DRV

### Replies: 1 Views: 71

## \#1 Posted by: Mike_Lemon Posted at: 2018-09-10T21:45:09.813Z Reads: 19

```
Hello there, 

I'm trying to repair a broken VESC that got damaged probably because of a small short while riding (eventought there were 2 idenical oned connected to the same line and only one of them made it) I just had to replace two mosfets that were connected to one of the phases and replaced the DVR and boom it works after once of twice of just cleaning the DRV pins now the problem comes when trying to actually drive the motor the motor makes a single step and then kinda gets into fault mode with these results after trying to run a motor detection: 

The following faults were registered since start:

    Fault            : FAULT_CODE_ABS_OVER_CURRENT
    Current          : 147.2
    Current filtered : 145.1
    Voltage          : 31.18
    Duty             : 0.643
    RPM              : 181.5
    Tacho            : 7
    Cycles running   : 2528
    TIM duty         : 4031
    TIM val samp     : 2015
    TIM current samp : 5149
    TIM top          : 6267
    Comm step        : 3
    Temperature      : 43.77
     
    Fault            : FAULT_CODE_ABS_OVER_CURRENT
    Current          : 143.5
    Current filtered : 144.7
    Voltage          : 31.15
    Duty             : 0.651
    RPM              : 52.8
    Tacho            : 13
    Cycles running   : 5824
    TIM duty         : 4037
    TIM val samp     : 2018
    TIM current samp : 5121
    TIM top          : 6205
    Comm step        : 3
    Temperature      : 44.22
     
    Fault            : FAULT_CODE_ABS_OVER_CURRENT
    Current          : 145.1
    Current filtered : 145.3
    Voltage          : 31.06
    Duty             : 0.680
    RPM              : 157.5
    Tacho            : 23
    Cycles running   : 5817
    TIM duty         : 4056
    TIM val samp     : 2028
    TIM current samp : 5012
    TIM top          : 5968
    Comm step        : 3
    Temperature      : 41.11
     
    Fault            : FAULT_CODE_ABS_OVER_CURRENT
    Current          : 146.5
    Current filtered : 144.6
    Voltage          : 31.32
    Duty             : 0.685
    RPM              : 52.9
    Tacho            : 29
    Cycles running   : 5613
    TIM duty         : 4059
    TIM val samp     : 2029
    TIM current samp : 4994
    TIM top          : 5929
    Comm step        : 3
    Temperature      : 44.12
 

any clue to what could cause that?
something to replace?

Thanks for helping!
```

---
