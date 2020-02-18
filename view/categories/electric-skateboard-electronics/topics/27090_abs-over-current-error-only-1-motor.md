# ABS_OVER_CURRENT error. Only 1 motor

### Replies: 4 Views: 353

## \#1 Posted by: slerm Posted at: 2017-07-08T20:54:43.402Z Reads: 65

```
I just set up a new build and did afew quick runs with no issues. Went out today after I finished up the enclosure, and mounting everything. I was accelerating hard and power just cut out. I ran a fault and got the below:

Fault            : FAULT_CODE_ABS_OVER_CURRENT
Current          : 156.0
Current filtered : 137.4
Voltage          : 28.09
Duty             : 0.63
RPM              : 56832.2
Tacho            : 3856
Cycles running   : 605
TIM duty         : 4025
TIM val samp     : 1937
TIM current samp : 5109
TIM top          : 6344
Comm step        : 3
Temperature      : 33.84

Fault            : FAULT_CODE_ABS_OVER_CURRENT
Current          : 133.0
Current filtered : 130.5
Voltage          : 35.28
Duty             : 0.76
RPM              : 368.7
Tacho            : 4875
Cycles running   : 808
TIM duty         : 4100
TIM val samp     : 2009
TIM current samp : 4724
TIM top          : 5429
Comm step        : 2
Temperature      : 34.42

If I try running motor detection it keeps failing with blinking red lights. 

Set Up is:

TorqueBoards Dual Hubs
10s3P Li-IOn, Samsung 25R
Dual VESC-x
Mini RC Remote

Any ideas? It's only one motor/vesc that's having the issue (slave)

BLDC Settings:
http://imgur.com/5LlW7Fg
http://imgur.com/PDzkT4Y
```

---
## \#2 Posted by: slerm Posted at: 2017-07-08T23:01:33.404Z Reads: 54

```
<img src="/uploads/db1493/original/3X/3/c/3c6aa88da82768583e19edfcd76957cd2c790d16.jpg" width="690" height="338"><img src="/uploads/db1493/original/3X/d/c/dce52e90424580f262a128c5780a8c74d423c56b.jpg" width="690" height="329">
```

---
## \#3 Posted by: Ackmaniac Posted at: 2017-07-08T23:06:12.498Z Reads: 53

```
Just connect the motor to the other VESC which is OK and try it there. if you get the errors again it is the motor. If not it is the VESC.
```

---
## \#4 Posted by: slerm Posted at: 2017-07-09T18:07:10.856Z Reads: 41

```
Turns out the problem is that I'm just an idiot. When I cut the heat shrink off to switch vescs the bullet connector fell off the one vesc lead. Resoldered that and all is good....
```

---
