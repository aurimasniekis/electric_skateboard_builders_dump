# Fault_code_drv help

### Replies: 33 Views: 775

## \#1 Posted by: luv2sk8te17 Posted at: 2018-09-25T02:46:13.045Z Reads: 127

```
Can someone please help me understand these fault codes? They shut off my flipsky dual 4.2 upon initial throttle/end of braking. If I accelerate slow everything is fine. Braking is fine until it is time to come to the last little bit of a complete stop. I have to let off and re apply brake slowly to keep from rolling forward.
Any help appreciated. I have tried my best to mess with all possible configuration settings. 

![1|690x387](upload://y3hIILzsyjtk8sUC8iQ1hjo45RE.jpeg) ![2|690x387](upload://pyEPNZHjAZSRPV8VPCsf4vslvnA.jpeg)
```

---
## \#2 Posted by: mmaner Posted at: 2018-09-25T03:16:46.881Z Reads: 120

```
https://www.electric-skateboard.builders/t/poll-flipsky-information-in-one-place/68940/10?u=mmaner
```

---
## \#3 Posted by: luv2sk8te17 Posted at: 2018-09-25T03:28:18.526Z Reads: 111

```
Thanks! Yes 10s as well here but lipo. I will try the lower motor current you have suggested. The feel of 60 motor is a lot of fun, but not worth the cutouts. Will try and post back.
```

---
## \#4 Posted by: linsus Posted at: 2018-09-25T14:55:11.438Z Reads: 103

```
Try change abs max to 140. If problem persists its a hardware problem.
```

---
## \#5 Posted by: luv2sk8te17 Posted at: 2018-09-25T15:02:18.754Z Reads: 100

```
Seems like it would send a drv_overcurrent if this was the issue. None the less I will def try and report back. I think it's just too much for a 4 series vesc. That or I need more than 5000mah lipos.
```

---
## \#6 Posted by: linsus Posted at: 2018-09-25T15:05:49.999Z Reads: 98

```
well, the fault reports 233A of current so it feels like a spiking issue. I have an open dialog with the manufacturer about this atm with vedder as support and the abs max value was his first response
```

---
## \#7 Posted by: luv2sk8te17 Posted at: 2018-09-25T15:22:30.356Z Reads: 89

```
That's what I was curious of. Thank you for clarifying that. So what setting controls this to where it limits it before just cutting out. I basically want to draw less. The vesc will handle 300a burst total/150a/single. 
Would this be a combination of batt max/motor max?
```

---
## \#8 Posted by: linsus Posted at: 2018-09-25T15:37:48.834Z Reads: 86

```
Well if abs max is reached or passed the fault will trigger. So if you want 300A then 150A on abs max is needed. Generally in electronics you want 25% headroom, never operate near limit. I'm unsure what peak currents the VESC is practically capable of but it sounds like you're close to the limits.

Batt max should be set to what your batteries can tolerate, same goes for motor. (max. allowed contineus thru VESC still applies tho) Batt current is not equal with motor current. (read about duty cycling)
```

---
## \#9 Posted by: linsus Posted at: 2018-09-25T15:40:19.086Z Reads: 79

```
50A con. 240A burst. So seems like you're in the scope after all
```

---
## \#10 Posted by: luv2sk8te17 Posted at: 2018-09-25T15:46:47.551Z Reads: 76

```
I'm def under the threshold and have a little room to spare. I just wish I could limit something else to not draw this many amps or self limit when it gets near. Why would one fault at 233a and the other at 174a? 
I have looked at duty cycle but man that is a thinker. 
So I guess I have to lower motor max to not draw as much? How do you tell this thing hey at higher amp draws(low speed take off) to self limit or slowly increase. Are we talking throttle curves now?

Your posts have given me the insight I have been looking for even though I have been reading night /day on other posts they are still somewhat confusing, but now I can relate to my situation so THANK YOU!
```

---
## \#11 Posted by: linsus Posted at: 2018-09-25T15:53:45.000Z Reads: 68

```
The behaviour you are seeing in your fault is something that (probably) shouldn't be there. Somehow the current sensing takes of like a rocket and it could have to do with cheap components or errors on the powerstage layout on the PCB. Its abit early to tell. From what I understand users have had a more stable experience below 40A con. so try that for now I guess.

If you apply full throttle from standstil, even uphill. Reaching anything above 60A is relativly hard to do. (not saying its impossible), you could set a less agressive throttle curve but if this is a hardware fault, its hard to tell if it will help at all.
```

---
## \#12 Posted by: luv2sk8te17 Posted at: 2018-09-25T17:05:03.548Z Reads: 60

```
Yeah probably hardware. Even with abs max at 130amp I somehow hit 328. Probably almost blew up the esc. I just don't get it. It's like the settings aren't 100% set in stone. I saw another forum a guy set his motor max to 40 but he still hit a peak of 56.
![3|690x387](upload://lxQlQzHN2Qav9jvByWFA0dnhg5H.jpeg)
```

---
## \#13 Posted by: luv2sk8te17 Posted at: 2018-09-25T17:08:38.304Z Reads: 59

```
Is there a reason it is negative? This is during throttle not braking.
```

---
## \#14 Posted by: briman05 Posted at: 2018-09-25T17:48:22.738Z Reads: 59

```
You did a motor detection right?
```

---
## \#15 Posted by: luv2sk8te17 Posted at: 2018-09-25T18:03:11.246Z Reads: 58

```
For sure. I've also tried bldc but have same results. I'm just going to run waaay lower values than I expected to be able to. This brand must be the reason it was cheaper than others.
```

---
## \#16 Posted by: luv2sk8te17 Posted at: 2018-09-25T18:09:23.388Z Reads: 58

```
Should I do it with no resistance like take wheels off and everything?
```

---
## \#17 Posted by: briman05 Posted at: 2018-09-25T18:18:01.625Z Reads: 55

```
did you do this all with your wheels and belts?
```

---
## \#18 Posted by: luv2sk8te17 Posted at: 2018-09-25T18:22:08.972Z Reads: 53

```
I did. Possibly causing issues? I can take everything off and report back. Maybe we found a huge solution.
```

---
## \#19 Posted by: briman05 Posted at: 2018-09-25T18:24:16.573Z Reads: 55

```
Yes always do the set up not under load or with belts on
```

---
## \#20 Posted by: linsus Posted at: 2018-09-25T18:53:00.246Z Reads: 53

```
I doubt there actually is 380A there even tho it says there is. Thats just ridic. Something is causing anomelies. Power Electronic can behave really wierd if something is done wrong. Its not just connect stuff and hope it works. Alot of things to consider. Theres a reason most 4.2 hardware look a like. Its cause it works. And redesigning is a risk
```

---
## \#21 Posted by: bigmisan Posted at: 2018-10-06T18:48:28.370Z Reads: 49

```
I have the same issue with my flipsky dual 4.2 too. Also with lipos as 12S (max current can be 300A).
If I lower my cuurent setting, it is better, but still, there is some issue there...
Fault            : FAULT_CODE_DRV
Current          : 43.4
Current filtered : 40.0
Voltage          : 44.94
Duty             : 0.878
RPM              : 39479.1
Tacho            : 50115
Cycles running   : 3068
TIM duty         : 4155
TIM val samp     : 2078
TIM current samp : 4446
TIM top          : 4736
Comm step        : 3
Temperature      : 38.41
 
Fault            : FAULT_CODE_DRV
Current          : 48.3
Current filtered : 48.6
Voltage          : 45.82
Duty             : 0.873
RPM              : 39771.7
Tacho            : 53298
Cycles running   : 3178
TIM duty         : 4152
TIM val samp     : 2077
TIM current samp : 4456
TIM top          : 4758
Comm step        : 6
Temperature      : 38.71
 
Fault            : FAULT_CODE_DRV
Current          : 49.6
Current filtered : 42.1
Voltage          : 45.41
Duty             : 0.890
RPM              : 40390.1
Tacho            : 57013
Cycles running   : 3141
TIM duty         : 4158
TIM val samp     : 2080
TIM current samp : 4417
TIM top          : 4674
Comm step        : 1
Temperature      : 38.56
```

---
## \#22 Posted by: bigmisan Posted at: 2018-10-06T18:49:40.447Z Reads: 49

```
Motor curr max: 50A
ABS max 130A
Batt curr max 50A for each
```

---
## \#23 Posted by: bigmisan Posted at: 2018-10-06T19:23:49.868Z Reads: 50

```
It seems, that limit is 50A for Motor curr max.
When I use 40A, it is OK without issue, when I setup 50A, issue is there. No matter what is setup for battery (40 or 50A).
Test was done without load, just on deck...
I will try it on full load tomorrow...
```

---
## \#24 Posted by: Kug3lis Posted at: 2018-10-06T22:57:50.243Z Reads: 49

```
DRV error is reported by DRV either something is bad with mosfets cant turn on mosfets or internal temp is high of drv or etc stuff mostly is blown drv..
```

---
## \#25 Posted by: bigmisan Posted at: 2018-10-07T07:54:47.185Z Reads: 47

```
As you can see, temperature is OK. And it is weird that two units have the same problem.. :frowning:Fault : FAULT_CODE_DRV
Current : 49.6
Current filtered : 42.1
Voltage : 45.41
Duty : 0.890
RPM : 40390.1
Tacho : 57013
Cycles running : 3141
TIM duty : 4158
TIM val samp : 2080
TIM current samp : 4417
TIM top : 4674
Comm step : 1
Temperature : 38.56

This unit is new, used once for now...
Already send message to flipsky...
```

---
## \#26 Posted by: Kug3lis Posted at: 2018-10-07T08:15:02.268Z Reads: 45

```
I mean temperature of DRV itself
```

---
## \#27 Posted by: bigmisan Posted at: 2018-10-07T15:43:06.687Z Reads: 43

```
I think, it is not this problem. I am testing on table without load...
This issue is immediately from beginning, when I start vesc...
```

---
## \#28 Posted by: bigmisan Posted at: 2018-10-08T05:47:51.564Z Reads: 42

```
Do you have any progress on this issue? Is it fixed? I have the same issue.. thx for info
```

---
## \#29 Posted by: luv2sk8te17 Posted at: 2018-10-08T20:04:16.470Z Reads: 40

```
I just put the motor max at 35-37 and am satisfied with fewer cutouts. I also added in -15 throttle expo for a softer response and seems to help.  Basically if you want less issues go to the vesc 6 series. Good luck to you.
```

---
## \#30 Posted by: alexnz Posted at: 2018-10-08T21:35:57.504Z Reads: 41

```
Isn't there a limit with the VESC with 40000 RPM? Don't know if this is what applies here, but your logs show that it's around 40k that you have this fault.
Are your motors really meant to spin that fast?
```

---
## \#31 Posted by: bigmisan Posted at: 2018-10-09T06:05:41.483Z Reads: 38

```
Limit in VESC 4.12 is 60000 eRPM.
I have 190kv on 12S, so this limit is hit with fully battery. But I have setup limit in VESC as max 60000 with 80% hit. So, it should be OK. Because I can speed for max without problem.
Probelm is with torque, special for startup or full thortle from lower speed. When I need more Amper from motor (more than 40A) DRV fault is there.
I already apoke with guy from FlipSky and they have recommendation for 10S for this dual 4.12. But spec is max 60V and 50-100A.
I will send result from this issue ...
```

---
## \#32 Posted by: luv2sk8te17 Posted at: 2018-10-09T19:05:56.459Z Reads: 36

```
I am on 10s but still have the same issue. I have thought about going lower in gearing, but the drv code I reported at the beginning of this topic doesn't report any under voltage or over current so I am not sure that would help anything. My belief is this thing is just cheap and wimpy and was not meant to do what we expect it to do and most likely does nowhere near the amp rating stated. Much like cheap auto amplifier/stereo brands advertise higher watts than they really are. Overall, it's a great affordable vesc to get the job done, but not for performance.
```

---
## \#33 Posted by: bigmisan Posted at: 2018-10-10T06:15:18.321Z Reads: 34

```
I already spoke with flipsky and they recommend 10S for this dual 4.12. But, I use 12S.
I did lowering setup for Motor Curr max as for 40A only, so far good for me, without issue, but torque is missing there. So, discussed with them about refund, they offer me dual vesc 6.6 for half price as around 150$, so think about it...
```

---
