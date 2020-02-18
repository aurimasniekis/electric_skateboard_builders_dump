# VESC Will Occasionaly Timeout When Even A Little Throttle Is Applied

### Replies: 9 Views: 764

## \#1 Posted by: deverewb Posted at: 2017-07-07T00:15:25.802Z Reads: 51

```
Hey esk8 builders,

I recently built an electric long board. And it's great! It works perfectly, hits 30, but there's just one problem.

If I apply any amount of throttle from a stopped position, the VESC seems to have a 1 in 5 chance of timing out. When this happens it will start blinking red for about 3 seconds before going back to normal. I have no clue what causes this, and to my knowledge, it seems to happen at random. Doesn't matter how gradually I apply the throttle and it's pretty annoying. 

The VESC comes from diyelectricskateboard. This one: diy-electric-skateboard-kits-parts/vesc-the-best-electric-skateboard-esc/

I'm sorry if I messed up with the tags, it's my first time posting here, plus I have no idea if the problem could possibly be the motor, the VESC, or how I programmed it.

Thanks in advance!
```

---
## \#2 Posted by: Jinra Posted at: 2017-07-07T00:42:00.913Z Reads: 50

```
get it to happen again but this time don't turn off your vesc. plug it into bldc tool and go to terminal and type faults. let us know the output
```

---
## \#3 Posted by: deverewb Posted at: 2017-07-07T01:05:43.231Z Reads: 48

```
Fault            : FAULT_CODE_DRV8302
Current          : -0.0
Current filtered : 0.3
Voltage          : 37.55
Duty             : 0.02
RPM              : 429.5
Tacho            : 475
Cycles running   : 14
TIM duty         : 718
TIM val samp     : 383
TIM current samp : 23958
TIM top          : 47151
Comm step        : 2
Temperature      : 29.02

EDIT:
Ran it a few more times

Fault            : FAULT_CODE_DRV8302
Current          : -0.0
Current filtered : 0.3
Voltage          : 37.55
Duty             : 0.02
RPM              : 429.5
Tacho            : 475
Cycles running   : 14
TIM duty         : 718
TIM val samp     : 383
TIM current samp : 23958
TIM top          : 47151
Comm step        : 2
Temperature      : 29.02

Fault            : FAULT_CODE_DRV8302
Current          : -1.7
Current filtered : 0.1
Voltage          : 37.58
Duty             : 0.01
RPM              : 2.5
Tacho            : 483
Cycles running   : 1
TIM duty         : 554
TIM val samp     : 297
TIM current samp : 24879
TIM top          : 49165
Comm step        : 4
Temperature      : 30.07

Fault            : FAULT_CODE_DRV8302
Current          : 0.7
Current filtered : -0.3
Voltage          : 37.58
Duty             : 0.00
RPM              : 4.6
Tacho            : 486
Cycles running   : 1
TIM duty         : 263
TIM val samp     : 10
TIM current samp : 26384
TIM top          : 52747
Comm step        : 1
Temperature      : 30.04

Fault            : FAULT_CODE_DRV8302
Current          : 0.2
Current filtered : 0.0
Voltage          : 37.58
Duty             : 0.01
RPM              : 7.6
Tacho            : 487
Cycles running   : 1
TIM duty         : 554
TIM val samp     : 297
TIM current samp : 24879
TIM top          : 49165
Comm step        : 6
Temperature      : 30.15

Fault            : FAULT_CODE_DRV8302
Current          : 0.3
Current filtered : -0.1
Voltage          : 37.53
Duty             : 0.01
RPM              : 12.4
Tacho            : 20672
Cycles running   : 2
TIM duty         : 594
TIM val samp     : 10
TIM current samp : 26384
TIM top          : 52747
Comm step        : 1
Temperature      : 30.76
```

---
## \#4 Posted by: rpn314 Posted at: 2017-07-07T01:17:52.226Z Reads: 40

```
Yeah, I'm pretty confident in saying you have a faulty DRV chip :frowning:
```

---
## \#5 Posted by: deverewb Posted at: 2017-07-07T01:36:46.741Z Reads: 41

```
Aw crap, is that my fault? What could have caused this? For future reference.
```

---
## \#6 Posted by: rpn314 Posted at: 2017-07-07T02:49:43.804Z Reads: 37

```
Could be DOA or settings. Can you post screenshots of your settings in BLDC-Tool?
```

---
## \#7 Posted by: deverewb Posted at: 2017-07-07T04:23:51.883Z Reads: 35

```
Yea, they told me the VESC was pre-programmed for my setup and I'd be fine, plus for a week or so I couldn't even program the VESC itself because they sent me a busted cable that I had to replace.

This is how it was set up:
<img src="/uploads/db1493/original/3X/5/b/5ba7b351c381c576ed381c3c95292536975a625e.PNG" width="690" height="388"><img src="/uploads/db1493/original/3X/a/a/aa6b682261fd7ba151dcf88c0597093f6e687f7b.PNG" width="690" height="388"><img src="/uploads/db1493/original/3X/c/2/c25cbf29594f9ac0aa247a7e58d84ab52c4b075c.PNG" width="690" height="388"><img src="/uploads/db1493/original/3X/f/c/fc3066c43a1bd8667de1551a988c36ac690a1da8.PNG" width="690" height="388">
```

---
## \#8 Posted by: Jinra Posted at: 2017-07-07T05:27:14.067Z Reads: 33

```
Oof yea, that's outdated firmware. You got the max current ramp step bug. The VESC or DRV will have to be replaced and you should load updated f/w on it.

See here:
http://www.electric-skateboard.builders/t/psa-remember-to-reset-your-max-current-ramp-step-when-programming-your-vesc/6262
```

---
## \#9 Posted by: rpn314 Posted at: 2017-07-07T14:19:25.805Z Reads: 24

```
Yep. @Jinra caught it; that's at least part of your problem. If your VESC arrived with that firmware (ie you didn't flash the firmware at all yourself) then I'd contact them for a replacement. That bug happened about a year ago, but has been lingering ever since. Either way, you'll need a DRV replacement.
```

---
