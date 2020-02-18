# VESC problem, help!

### Replies: 19 Views: 417

## \#1 Posted by: Davo Posted at: 2018-08-31T12:25:08.506Z Reads: 58

```
hey there, I just received my new flipsky dual vesc V4, but I keep running in the same problem.
When in the VESC tool I'm running the motor wizard setup of the master I have a bad detection problem. I've tried to switch in FOC, and when I run the detection and measurement of resistace and inductance the motor isn't spinning at all and there are just a few noises and a message after a while is shown![vsc%202|690x436](upload://1vrizSSheNo5eBC4d36E79brtZm.png)![vesc%20sc|690x433](upload://mx4STj3BoUktGZdMOzfpmSKMSwg.png)
I'm running a 10s5p and two 1600 Watt motors
edit, I forgot to include, when I use the remote and I accelerate there is no spinning at all, just a small noise kinda the motor tries to power up and then the red light from the master start blinking, but the slave even in the motor setup can work fine
```

---
## \#2 Posted by: Andy87 Posted at: 2018-08-31T12:27:15.050Z Reads: 50

```
did you check you sensor cables.
maybe one cable or the plug became lose.
```

---
## \#3 Posted by: Kug3lis Posted at: 2018-08-31T12:28:50.830Z Reads: 50

```
Either phase leads wrong or something is wrong with power stage, because measure motor R normally never fails...

EDIT: open terminal and write faults after red blinks
```

---
## \#4 Posted by: Davo Posted at: 2018-08-31T12:29:01.858Z Reads: 45

```
yep I did, it was the first thing I did, but nope, everithing is fine
```

---
## \#5 Posted by: Andy87 Posted at: 2018-08-31T12:31:08.903Z Reads: 42

```
did you swap the motors?
to find out if it´s problem of the motor or the VESC itself. It runs fine on the slave, or you didn´t tried it there?
```

---
## \#6 Posted by: Davo Posted at: 2018-08-31T12:44:31.648Z Reads: 38

```
ok, just did, I copy the text it's giving me cos I can't upload the screenshot

The following faults were registered since start:

Fault            : FAULT_CODE_DRV
Current          : -5.5
Current filtered : -18.9
Voltage          : 37.86
Duty             : 0.440
RPM              : 90.4
Tacho            : 1
Cycles running   : 7
TIM duty         : 3697
TIM val samp     : 2
TIM current samp : 4200
TIM top          : 8400
Comm step        : 5
Temperature      : 31.26
 
Fault            : FAULT_CODE_ABS_OVER_CURRENT
Current          : 151.1
Current filtered : 144.0
Voltage          : 38.62
Duty             : 0.001
RPM              : 40173.9
Tacho            : 2
Cycles running   : 0
TIM duty         : 2
TIM val samp     : 1050
TIM current samp : 3150
TIM top          : 4200
Comm step        : 6
Temperature      : 30.97
```

---
## \#7 Posted by: Davo Posted at: 2018-08-31T12:45:11.543Z Reads: 36

```
yeah, I did it to make sure and the motors are fine
```

---
## \#8 Posted by: Kug3lis Posted at: 2018-08-31T12:47:24.712Z Reads: 38

```
Looks like DRV is fcked, plus at positive duty negative current something is bad with esc itself.
```

---
## \#9 Posted by: Davo Posted at: 2018-08-31T12:50:20.975Z Reads: 38

```
so..... there's nothing I can do?
```

---
## \#10 Posted by: Andy87 Posted at: 2018-08-31T12:53:17.963Z Reads: 40

```
you can sent it back.
you have guarantee on it?

if no, you could ask somebody to replace the drv, in case you can´t make it by your own

but the question is also, what caused the DRV to fry
```

---
## \#11 Posted by: Davo Posted at: 2018-08-31T13:00:42.944Z Reads: 39

```
I hope so.... honestly I haven't run the board at all, and I followed the instructions given..
what could the reason of the drv to die? I'm using an antispark loopkey
```

---
## \#12 Posted by: Kug3lis Posted at: 2018-08-31T13:04:07.022Z Reads: 38

```
Maybe faulty, or just conditions met the right moment...
```

---
## \#13 Posted by: visnu777 Posted at: 2018-08-31T13:10:40.662Z Reads: 37

```
Are you 100% percent sure its not the antispark plug? I had similar symptoms not long ago, blamed the motors but it was actually the antispark plug not having enough contact with its counterpart.
```

---
## \#14 Posted by: Kug3lis Posted at: 2018-08-31T13:11:17.570Z Reads: 37

```
Well DRV itself reports error so I doubt it will be spark plug...
```

---
## \#15 Posted by: visnu777 Posted at: 2018-08-31T13:18:22.161Z Reads: 36

```
I didn't check for the error codes but everything else sounded similar to my case :)
```

---
## \#16 Posted by: Davo Posted at: 2018-08-31T16:13:10.154Z Reads: 29

```
I don't think its the spark plug, how can I be sure about it? If I use the tester everything is fine, and the slave shouldn't work at all like master vesc, am I wrong?
```

---
## \#17 Posted by: Davo Posted at: 2018-08-31T16:14:22.047Z Reads: 29

```
What's the other error? ABS over current, what does it mean?
```

---
## \#18 Posted by: Kug3lis Posted at: 2018-08-31T16:18:53.507Z Reads: 29

```
ABS = Absolute its like the maximum current the vesc should see, according log it measured 144A which is bit bullshit or just one phase is broken and that's why it doesn't work as it was practically shortening one phase
```

---
## \#19 Posted by: Davo Posted at: 2018-08-31T16:31:20.899Z Reads: 28

```
bullshit for sure, my battery should give max 100A and as I said I didn't ride at all so I don't think I could reach that power without even spinning motors. What do you mean the phase is broken? Sorry, completely newbie and I'm trying to learn as much as possible
```

---
