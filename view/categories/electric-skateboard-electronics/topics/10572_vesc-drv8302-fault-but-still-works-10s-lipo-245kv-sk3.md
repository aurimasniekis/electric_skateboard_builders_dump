# VESC DRV8302 Fault but still works 10s Lipo 245kv SK3

### Replies: 12 Views: 1172

## \#1 Posted by: Jobbel Posted at: 2016-10-03T16:27:27.878Z Reads: 147

```
So I used my VESC from enertion for about 2 weeks in FOC mode. Then today on a small ride suddenly my brakes did not work anymore. I stopped looked at the VESC but everything seemed to be fine so I drove on. After about 2 km it happend again, once I got home I connected the VESC to BLDC-Tool and got the following output upon typing faults:

Fault            : FAULT_CODE_DRV8302
Current          : 0.3
Current filtered : 0.0
Voltage          : 39.40
Duty             : 0.00
RPM              : 109.1
Tacho            : 1897215
Cycles running   : 1
TIM duty         : 26
TIM val samp     : 5
TIM current samp : 8398
TIM top          : 8400
Comm step        : 0
Temperature      : 41.11

Fault            : FAULT_CODE_DRV8302
Current          : 0.1
Current filtered : -0.0
Voltage          : 39.12
Duty             : 0.09
RPM              : 5968.7
Tacho            : 2464606
Cycles running   : 2
TIM duty         : 763
TIM val samp     : 5
TIM current samp : 8398
TIM top          : 8400
Comm step        : 0
Temperature      : 71.95

Fault            : FAULT_CODE_DRV8302
Current          : -2.5
Current filtered : -0.3
Voltage          : 39.09
Duty             : 0.00
RPM              : 73.9
Tacho            : 2608636
Cycles running   : 1
TIM duty         : 35
TIM val samp     : 5
TIM current samp : 8398
TIM top          : 8400
Comm step        : 0
Temperature      : 74.21


After l hooked everything up on my bench, sometimes when i press the throttle it starts spinning sometimes it does not and delivers a drv fault. The rate is about 50% to 50 %, but when it starts spinning it wont stop. Is there a chance of a bad solder joint which causes this problem ?<img src="/uploads/db1493/original/3X/9/4/947e8878c1c4f4fe0989647ffdef4d6420298cb0.JPG" width="375" height="500">

Compared to my roommates VESC who is using BLDC mode my VESC with FOC gets much hotter
```

---
## \#2 Posted by: Jinra Posted at: 2016-10-03T16:42:42.723Z Reads: 132

```
Sounds like FOC killed your DRV. You'll have to get it replaced. Also, whats that goopy looking stuff on the chip? Maybe it shorted out the pins?
```

---
## \#3 Posted by: Jobbel Posted at: 2016-10-03T16:51:13.826Z Reads: 130

```
That is because I used Duct tape :D 
once i drive and don't stop holding the throttle it runs like a charm, only from a dead stop it fails.
But you might be right  no more FOC for me :cry:

Edit: I just switched  back to BLDC, same problem here
```

---
## \#4 Posted by: Blasto Posted at: 2016-10-03T16:55:58.806Z Reads: 128

```
Sounds like one of you fets failled, probe the drain-source to see if you have a low impedance on one of them
```

---
## \#5 Posted by: Jobbel Posted at: 2016-10-03T17:00:08.989Z Reads: 125

```
But if one of the FETs would have failed, the motor would not be able to spin anymore would it ?
Blasto how do you get to that conclusion ?
```

---
## \#6 Posted by: Blasto Posted at: 2016-10-03T17:07:08.602Z Reads: 121

```
The lack of brakes is the hint, check your shunts also.
```

---
## \#7 Posted by: Jobbel Posted at: 2016-11-07T00:14:48.677Z Reads: 98

```
I replaced the broken DRV Chip and the VESC does work again :grinning:
I will not try FOC a second time.

There was one time when I got the ABS over current fault at 130 amps
, but it didn't happen a second time in 2 weeks.
The problem is not the mosfets or the shunts because I measured and re-soldered all of them :confused:
```

---
## \#8 Posted by: Jinra Posted at: 2016-11-07T00:24:18.316Z Reads: 97

```
great to hear you got it fixed up. Keep in mind 245kv at 10s goes over the eRPM limit and that may burn out your DRV again even on BLDC mode.
```

---
## \#9 Posted by: Jobbel Posted at: 2016-11-07T00:34:23.109Z Reads: 95

```
Thanks for you quick reply, can you tell me what the eRPM limit is on the VESC ?
10s -> 10*4,2 = 42V at 245kv 
-> 245*42 = 10290 eRPM
Is it a good Idea to limit the eRPM in BLDC Tool to a sane amount, to evade burning the DRV again. I would'nt mind driving a little bit slower, if my system would be overall more reliable.
```

---
## \#10 Posted by: Jinra Posted at: 2016-11-07T00:36:44.699Z Reads: 88

```
erpm limit is about 60k. You have to multiply RPM by your motor's pole pairs (usually 7) to get the eRPM.

Common 50-63mm motors have 7 pole pairs which mean you're hitting 72,000 erpm max, though at 95% duty cycle that's more like 68,400.

You can limit the erpm on the app configuration tab, there should be a "soft erpm limit" option, however, this isn't very efficient. Best thing to do would be to get a <200kv motor for your setup.
```

---
## \#11 Posted by: Jobbel Posted at: 2016-11-07T00:42:03.687Z Reads: 85

```
Ok, thank you very much.
For now I'll limit the erpm to 60,000, because I use my board every day, and don't want it to break again. And I'll look out for a sub 200 kv motor :slight_smile:

Thanks again
```

---
## \#12 Posted by: Jobbel Posted at: 2016-12-03T19:12:25.110Z Reads: 60

```
Update on the DRV:
 after several weeks of daily use my vesc decided to throw me off at 20 kph due to a DRV Error (instant break). It happened at an evening ride and I wasn't hurt much. That evening I did not get it to run again, DRV Faults all over the place. The next day however everything worked like a charm. the accident happened 1 week ago and my board worked since then. That is why i think there is a bad solder joint somewhere on my VESC. I thought about reflowing the DRV with a lot of flux and then again check every pin under a microscope with micro-probes. Are there any other Components that may have a bad solder joint and should be fixed ?

I limited the ERPM to 58000 and never drove full speed that's why I'd say the too high kv of my motor should not be a Problem
```

---
