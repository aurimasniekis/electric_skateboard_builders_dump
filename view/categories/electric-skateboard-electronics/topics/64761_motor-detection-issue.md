# Motor Detection Issue

### Replies: 4 Views: 144

## \#1 Posted by: TamShay777 Posted at: 2018-08-13T17:41:07.366Z Reads: 50

```
This is my first ever build, and I can't seem to get it to work...
I'm using the free vesc project tool.  After the battery is fully charged, I connect my vesc to my pc and do the motor set up wizard with the following parameters:

BLDC 
motor max: 80a
motor min: -35a

battery max: 15a
battery min: -12a

battery cutoff start: 31V
battery cutoff end: 28V

here are the parts I'm working with:

DIY electric Vesc 4.12 with FW 3.4 HW 410
TB 6355/190kv motor
samsung 6.0 Battery: https://www.ownboard.net/products/ownboard-electric-skateboard-battery?variant=6940852715562

when I click motor detection, the motor spins for like 1-2 seconds, then the vesc flashes red 3x.  I get a failed motor detection result.

I went to vesc terminal and typed in "faults" and got this result.
The following faults were registered since start:

Fault            : FAULT_CODE_DRV
Current          : -0.2
Current filtered : 0.0
Voltage          : 41.29
Duty             : 0.009
RPM              : 0.3
Tacho            : 6
Cycles running   : 1
TIM duty         : 435
TIM val samp     : 217
TIM current samp : 25533
TIM top          : 50632
Comm step        : 4
Temperature      : 26.51
 
Fault            : FAULT_CODE_DRV
Current          : -0.2
Current filtered : -0.1
Voltage          : 41.28
Duty             : 0.009
RPM              : 5.5
Tacho            : 10
Cycles running   : 1
TIM duty         : 438
TIM val samp     : 219
TIM current samp : 25520
TIM top          : 50602
Comm step        : 2
Temperature      : 26.49
 
Fault            : FAULT_CODE_DRV
Current          : -0.5
Current filtered : -0.1
Voltage          : 41.32
Duty             : 0.009
RPM              : 3.3
Tacho            : 12
Cycles running   : 1
TIM duty         : 446
TIM val samp     : 223
TIM current samp : 25478
TIM top          : 50511
Comm step        : 4
Temperature      : 26.64
 
Fault            : FAULT_CODE_DRV
Current          : 0.2
Current filtered : 0.2
Voltage          : 41.32
Duty             : 0.008
RPM              : 0.5
Tacho            : 15
Cycles running   : 1
TIM duty         : 425
TIM val samp     : 212
TIM current samp : 25590
TIM top          : 50755
Comm step        : 1
Temperature      : 26.90
 
Fault            : FAULT_CODE_DRV
Current          : 0.7
Current filtered : 0.3
Voltage          : 41.28
Duty             : 0.008
RPM              : 2.7
Tacho            : 17
Cycles running   : 2
TIM duty         : 407
TIM val samp     : 203
TIM current samp : 25696
TIM top          : 50986
Comm step        : 3
Temperature      : 26.79
 
Fault            : FAULT_CODE_DRV
Current          : 0.3
Current filtered : 0.0
Voltage          : 41.32
Duty             : 0.008
RPM              : 2.9
Tacho            : 18
Cycles running   : 1
TIM duty         : 420
TIM val samp     : 210
TIM current samp : 25626
TIM top          : 50832
Comm step        : 4
Temperature      : 26.92
 
What am I doing wrong?  Please help!
```

---
## \#2 Posted by: Bjork3n Posted at: 2018-08-13T20:44:12.877Z Reads: 31

```
It's a diyelectricskateboard vesc, they are prone to fail out of the blue. Mine did too during detection. 
You need a new vesc, that one is fried i'm afraid. 
I can highly recommend focbox, been using mine for 1600km with no issues .
```

---
## \#3 Posted by: TamShay777 Posted at: 2018-08-13T21:01:19.269Z Reads: 27

```
Looking into FocBox now!...  were you able to get any sort of refund?  I'm sending them an email now, but I'm not to optimistic.
```

---
## \#4 Posted by: Bjork3n Posted at: 2018-08-13T21:32:47.083Z Reads: 22

```
Nope, no refund.
```

---
