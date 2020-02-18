# VESC can&rsquo;t control motor anymore

### Replies: 8 Views: 920

## \#1 Posted by: Alan_Smithee Posted at: 2017-05-03T17:53:56.118Z Reads: 60

```
After only about 15km on this VESC (egreenmotion) it stopped working and when I pull the trigger on the remote a red LED flashes 3 times, stops and flashes another 3 times. BLDC tool can connect fine but also cannot controll the motor. Detection fails, LED response is the same.
```

---
## \#2 Posted by: mmaner Posted at: 2017-05-03T17:54:40.901Z Reads: 60

```
are you getting any faults?
```

---
## \#3 Posted by: Jinra Posted at: 2017-05-03T17:54:52.363Z Reads: 58

```
type "faults" in terminal and post results. If it's a DRV failure, you're gonna need a new one.
```

---
## \#4 Posted by: Alan_Smithee Posted at: 2017-05-03T18:03:27.550Z Reads: 57

```
returns: `FAULT_CODE_DRV8302`

The following faults were registered since start:

    Fault            : FAULT_CODE_DRV8302
    Current          : 0.1
    Current filtered : -0.2
    Voltage          : 40.49
    Duty             : 0.02
    RPM              : 10.1
    Tacho            : 4
    Cycles running   : 4
    TIM duty         : 889
    TIM val samp     : 456
    TIM current samp : 22970
    TIM top          : 45028
    Comm step        : 4
    Temperature      : 30.70

    Fault            : FAULT_CODE_DRV8302
    Current          : 0.2
    Current filtered : -0.2
    Voltage          : 40.49
    Duty             : 0.03
    RPM              : 2.0
    Tacho            : 5
    Cycles running   : 4
    TIM duty         : 1160
    TIM val samp     : 609
    TIM current samp : 21453
    TIM top          : 41687
    Comm step        : 5
    Temperature      : 30.70

    Fault            : FAULT_CODE_DRV8302
    Current          : -1.7
    Current filtered : -0.3
    Voltage          : 40.49
    Duty             : 0.03
    RPM              : 1.9
    Tacho            : 6
    Cycles running   : 4
    TIM duty         : 1160
    TIM val samp     : 609
    TIM current samp : 21453
    TIM top          : 41687
    Comm step        : 6
    Temperature      : 30.73
```

---
## \#5 Posted by: mmaner Posted at: 2017-05-03T18:04:06.666Z Reads: 49

```
You will have to get it repaired or replaced .  If you dont have warranty talk to @JohnnyMeduse .
```

---
## \#6 Posted by: Namasaki Posted at: 2017-05-03T18:10:56.471Z Reads: 47

```
What is the KV of your motor and what voltage are you running?
```

---
## \#7 Posted by: Alan_Smithee Posted at: 2017-05-03T18:24:03.350Z Reads: 54

```
sk3 192kv @10s6p

<img src="/uploads/db1493/original/3X/8/2/82a4dc0d449b3957210bcaf326e1852d0610cb1b.PNG" width="690" height="380">
<img src="/uploads/db1493/original/3X/c/5/c542ae4f1cd86764081f626ac42530fcd3ab2c3d.PNG" width="690" height="381">
<img src="/uploads/db1493/original/3X/3/2/32e0361745cfb3dff9b7f324b3eec9104808a581.PNG" width="690" height="382">
<img src="/uploads/db1493/original/3X/e/5/e5de436a950cdbcfe5226f947594041b889c7166.PNG" width="690" height="379">
<img src="/uploads/db1493/original/3X/a/2/a28014add81379c821e1377f11d9ede62c7204d1.PNG" width="689" height="387">

for some reason when I connected to the vesc after it stopped worrking "Sensorless - Communication Mode" under Motor Configuration > BLDC was set to "delay" instead of "intergrated". I don't recall doing that.

[and here is a video of the issue](https://www.youtube.com/watch?v=AGvVVSpLuNo)
```

---
## \#8 Posted by: Jinra Posted at: 2017-05-03T18:26:54.209Z Reads: 48

```
You have buggy firmware, as shown by the 50.00 max current ramp step. In addition to replacing the DRV8302 chip you need to update your f/w to get rid of the bug.

Bug details:
https://www.electric-skateboard.builders/t/psa-remember-to-reset-your-max-current-ramp-step-when-programming-your-vesc/6262
```

---
