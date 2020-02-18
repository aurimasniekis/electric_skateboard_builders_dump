# VESC 4.12 12S cuts out during hard acceleration

### Replies: 1 Views: 369

## \#1 Posted by: flyingox Posted at: 2017-10-31T21:33:36.196Z Reads: 74

```
Hope you can help me find the solution. 

here's my setup: mountain board with E-Toxx dual Direct drive, Dual VESC 4.12, 12S 100Amp Lithium battery, 75Kg rider   Config and fault code below.  Under hard acceleration power cuts then resumes as I reset the throttle.  Using 10s with higher Max motor amps works fine.  I wanted to keep the high motor amps setting for maximum torque.

   <img src="/uploads/db1493/original/3X/b/1/b144d88b46e26b87e4258cd8c7756ac1fbaeb6db.jpg" width="690" height="387">

The following faults were registered since start:

Fault            : FAULT_CODE_DRV8302
Current          : 56.0
Current filtered : 45.1
Voltage          : 48.04
Duty             : 0.48
RPM              : 24167.4
Tacho            : 74572
Cycles running   : 51041
TIM duty         : 3880
TIM val samp     : 1936
TIM current samp : 6001
TIM top          : 8130
Comm step        : 3
Temperature      : 20.77

Fault            : FAULT_CODE_DRV8302
Current          : 57.8
Current filtered : 49.6
Voltage          : 48.34
Duty             : 0.28
RPM              : 12681.9
Tacho            : 199450
Cycles running   : 25293
TIM duty         : 3513
TIM val samp     : 1754
TIM current samp : 8089
TIM top          : 12670
Comm step        : 3
Temperature      : 23.33

Fault            : FAULT_CODE_DRV8302
Current          : 55.0
Current filtered : 47.3
Voltage          : 48.08
Duty             : 0.35
RPM              : 15783.9
Tacho            : 203444
Cycles running   : 30775
TIM duty         : 3691
TIM val samp     : 1844
TIM current samp : 7079
TIM top          : 10470
Comm step        : 3
Temperature      : 25.27

The following faults were registered since start:

Fault            : FAULT_CODE_DRV8302
Current          : 56.0
Current filtered : 45.1
Voltage          : 48.04
Duty             : 0.48
RPM              : 24167.4
Tacho            : 74572
Cycles running   : 51041
TIM duty         : 3880
TIM val samp     : 1936
TIM current samp : 6001
TIM top          : 8130
Comm step        : 3
Temperature      : 20.77

Fault            : FAULT_CODE_DRV8302
Current          : 57.8
Current filtered : 49.6
Voltage          : 48.34
Duty             : 0.28
RPM              : 12681.9
Tacho            : 199450
Cycles running   : 25293
TIM duty         : 3513
TIM val samp     : 1754
TIM current samp : 8089
TIM top          : 12670
Comm step        : 3
Temperature      : 23.33

Fault            : FAULT_CODE_DRV8302
Current          : 55.0
Current filtered : 47.3
Voltage          : 48.08
Duty             : 0.35
RPM              : 15783.9
Tacho            : 203444
Cycles running   : 30775
TIM duty         : 3691
TIM val samp     : 1844
TIM current samp : 7079
TIM top          : 10470
Comm step        : 3
Temperature      : 25.27
```

---
