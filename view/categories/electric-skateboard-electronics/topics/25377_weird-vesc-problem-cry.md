# Weird VESC Problem :cry:

### Replies: 10 Views: 1234

## \#1 Posted by: NickTheDude Posted at: 2017-06-14T16:39:02.292Z Reads: 106

```
So a couple days ago I went for a long ride on my board, and everything was fine. But when I went to use it today, the second I tried to take off it would cut out.

I bench tested it and found that even while on the bench under hard breaking and hard acceleration it would cut out. Watching the realtime data on the VESC I saw that I was getting FAULT_CODE_OVER_VOLTAGE when it cut out under breaking, and FAULT_CODE_ABS_OVER_CURRENT when it cut out accelerating.

Fault            : FAULT_CODE_ABS_OVER_CURRENT
Current          : 64.3
Current filtered : 85.5
Voltage          : 25.17
Duty             : 0.09
RPM              : 642.5
Tacho            : 81088
Cycles running   : 477
TIM duty         : 2432
TIM val samp     : 1151
TIM current samp : 14154
TIM top          : 26006
Comm step        : 6
Temperature      : 26.64

Fault            : FAULT_CODE_OVER_VOLTAGE
Current          : -16.1
Current filtered : -16.3
Voltage          : 57.51
Duty             : 0.38
RPM              : 32104.0
Tacho            : 41208
Cycles running   : 485
TIM duty         : 3745
TIM val samp     : 1869
TIM current samp : 6771
TIM top          : 9805
Comm step        : 6
Temperature      : 25.82

These are my VESC settings:

<img src="/uploads/db1493/original/3X/0/9/0974309ca30c6b7fb095e474a0b612344bab372a.png" width="690" height="388">

<img src="/uploads/db1493/original/3X/0/d/0d7743a6990f044727d3faaa2d31193371fe1626.png" width="690" height="388">

<img src="/uploads/db1493/original/3X/1/f/1f9e97a2c2492ed32ff70afa948a1d9d038c968b.png" width="690" height="388">

<img src="/uploads/db1493/original/3X/1/f/1f9e97a2c2492ed32ff70afa948a1d9d038c968b.png" width="690" height="388">

<img src="/uploads/db1493/original/3X/8/2/82bd0d487f06d3b397535fb61a97253c02d74337.png" width="690" height="388">
```

---
## \#2 Posted by: TehAtheist Posted at: 2017-06-14T16:52:15.125Z Reads: 88

```
I don't own a VESC but (Well I actually own two but I have yet to use them to create my first board.) but something deep inside tells me that it's odd to see "80A" as max motor current, if the VESC can only deliver 60A...

I mean, I'm pretty sure you just have to lower that to 60A. Cause I think atm your VESC lets current through till 80A's but shutsdown because it's higher than 60A.
```

---
## \#3 Posted by: jaykup Posted at: 2017-06-14T16:57:18.836Z Reads: 87

```
Absolute max (first page) should be left default at 130 or so.

Battery min seems low at -6, but I don't know what pack you are running.
```

---
## \#4 Posted by: NickTheDude Posted at: 2017-06-14T17:10:24.925Z Reads: 82

```
Weird, it came set to 80A Absolute max. I changed it to 130A and it seems to have fixed the FAULT_CODE_ABS_OVER_CURRENT problem but the FAULT_CODE_OVER_VOLTAGE issue persists.
```

---
## \#5 Posted by: rpn314 Posted at: 2017-06-14T18:18:18.118Z Reads: 69

```
1. Max current ramp step is way too high. If you've been running it at that (4) you may (I'd say almost guaranteed) develop a DRV error in the future
2. What is your battery situation? That first error shows a ton of current (60 Amps, when you've set it for 40) and then you've got some serious votlage sag. The second error shows the voltage hitting just over 57 volts, which leads me to ask, are you using a BMS? I know some aren't very happy about regen braking and so they just go over-voltage instead of letting much current back into the pack.
```

---
## \#6 Posted by: NickTheDude Posted at: 2017-06-14T18:31:02.140Z Reads: 70

```
I'm using 2 5S 5000mAh 25C lipos wired in series with no BMS. Also, what would you suggest for the current ramp step?
```

---
## \#7 Posted by: jaykup Posted at: 2017-06-14T18:50:26.162Z Reads: 66

```
Agreed - good catch @rpn314.  Read this

http://www.electric-skateboard.builders/t/psa-remember-to-reset-your-max-current-ramp-step-when-programming-your-vesc/6262

Set it to 0.004, write, then read the config and see where it's at.  

If you upgrade your BLDC tool and VESC firmware with Akmaniac's updated version it will prevent this from happening

https://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286
```

---
## \#8 Posted by: rpn314 Posted at: 2017-06-14T18:50:46.623Z Reads: 64

```
The default current ramp step is 0.04. If you're at 4 (and didn't set that yourself, which I can't see why you would have), then you almost certainly have an old buggy firmware which multiplies that parameter by 10 every time you write changes from BLDC tool. It was quickly fixed (about a year ago) but seems that the firmware is still lingering around. See this thread: 

http://www.electric-skateboard.builders/t/psa-remember-to-reset-your-max-current-ramp-step-when-programming-your-vesc/6262

As to your battery situation....10s should pretty much never hit the 57 volt limit we usually set, even when braking. What is the exact circumstance where you saw those errors? (ie. riding up a hill, etc).

Is this your ["Street Weaver"](http://www.electric-skateboard.builders/t/street-weaver-landyachtz-dodger-190kv-6355-10s-5ah-vesc/24303?u=rpn314) build? You mentioned in that thread that you'd used 2 modified 6s batteries (because of a single failure in each)....are you still using those batteries? And how did they have issue originally? I'm starting to wonder if some other cells are starting to go as well. A high internal resistance due to aging or defective cells could cause that over-voltage issue.
```

---
## \#9 Posted by: NickTheDude Posted at: 2017-06-14T19:16:23.719Z Reads: 55

```
The errors only started happening after I hadn't ridden it in a couple days and tried to use it. It would cut out whenever I tried to break and had very little power, and yeah, that's the build. Initially I figured the batteries were the problem but every cell is around 3.7V. Weird that the VESC still has old firmware, its a brand new one from Torqueboards. 

Can I test the internal resistance of the cells using a volt meter?
```

---
## \#10 Posted by: rpn314 Posted at: 2017-06-14T19:19:27.431Z Reads: 51

```
Interesting. If that's the case, I may suggest you contact torqueboards about that. He may be liable for DRV errors if your firmware came with the buggy version of 2.18 (they didn't change the revision number when they fixed the issue, unfortunately, so it's not easy to see which version you have besides trying it)

I think you need something like the iMaxB6 balance charger to get IR. I don't believe it's as simple as just DC resistance (which is what a standard volt meter would measure)
```

---
