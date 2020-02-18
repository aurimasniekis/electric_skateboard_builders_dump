# Is this the typical DRV failure?

### Replies: 4 Views: 431

## \#1 Posted by: Silverline Posted at: 2018-03-22T13:52:38.794Z Reads: 85

```
I have a problem with a board with a 4.12 vesc from esk8.de
With newest vesc tool, motor detection fails..... I got this from the terminal

Is my DRV dead ?? The voltage reading seems to be right (6s board)


FAULT_CODE_NONE

The following faults were registered since start:

Fault            : FAULT_CODE_DRV
Current          : -0.2
Current filtered : -0.6
Voltage          : 24.69
Duty             : 0.008
RPM              : 0.1
Tacho            : 4
Cycles running   : 2
TIM duty         : 412
TIM val samp     : 206
TIM current samp : 25668
TIM top          : 50924
Comm step        : 4
Temperature      : 28.91
 
Fault            : FAULT_CODE_DRV
Current          : 1.1
Current filtered : 0.2
Voltage          : 24.69
Duty             : 0.008
RPM              : 3.5
Tacho            : 7
Cycles running   : 2
TIM duty         : 412
TIM val samp     : 206
TIM current samp : 25668
TIM top          : 50924
Comm step        : 1
Temperature      : 28.94
 
Fault            : FAULT_CODE_DRV
Current          : -1.2
Current filtered : -0.4
Voltage          : 24.72
Duty             : 0.008
RPM              : 3.6
Tacho            : 10
Cycles running   : 1
TIM duty         : 412
TIM val samp     : 206
TIM current samp : 25668
TIM top          : 50924
Comm step        : 4
Temperature      : 28.97
 
Fault            : FAULT_CODE_DRV
Current          : 0.3
Current filtered : -0.1
Voltage          : 24.72
Duty             : 0.008
RPM              : 0.1
Tacho            : 13
Cycles running   : 1
TIM duty         : 412
TIM val samp     : 206
TIM current samp : 25668
TIM top          : 50924
Comm step        : 1
Temperature      : 29.02
 
Fault            : FAULT_CODE_DRV
Current          : 0.0
Current filtered : -0.2
Voltage          : 24.70
Duty             : 0.008
RPM              : 4.3
Tacho            : 16
Cycles running   : 2
TIM duty         : 412
TIM val samp     : 206
TIM current samp : 25668
TIM top          : 50924
Comm step        : 4
Temperature      : 28.86
 
Fault            : FAULT_CODE_DRV
Current          : 1.1
Current filtered : 0.5
Voltage          : 24.70
Duty             : 0.008
RPM              : 3.5
Tacho            : 16
Cycles running   : 1
TIM duty         : 412
TIM val samp     : 206
TIM current samp : 25668
TIM top          : 50924
Comm step        : 6
Temperature      : 29.04
```

---
## \#2 Posted by: Bjork3n Posted at: 2018-03-22T15:07:44.506Z Reads: 61

```
Im afraid so, you need to replace the vesc or the DRV chip
```

---
## \#3 Posted by: Acidfie Posted at: 2018-03-22T15:54:56.169Z Reads: 53

```
maybe telling us what you have done with it could led to some informations.
```

---
## \#4 Posted by: Silverline Posted at: 2018-03-22T16:20:22.744Z Reads: 45

```
The vesc is just blinking when i push the throttle.... and motor detection fails
```

---
