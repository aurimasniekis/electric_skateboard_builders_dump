# Brand new motor and VESC throwing Over-Current fault when hitting bumps?

### Replies: 17 Views: 828

## \#1 Posted by: t0m_r1dd1e Posted at: 2017-06-27T00:03:33.314Z Reads: 95

```
I'm a pretty decent problem-solver but this one just baffles me. I just replaced a motor and VESC  on my dual motor board and it's throwing ABS_OVER_CURRENT and rebooting when I hit bumps. Not even huge bumps, even cracks in the sidewalk. All my VESC settings are identical to how they were on my last motor and VESC, which I put 500 miles on, so I know they're good. I just don't know know how to troubleshoot this one. All the components are from DIY. It does it both when using a servo cable splitter for signal and when using control over CAN-BUS from the master VESC. 

The weird thing is that my last motor and VESC were doing the exact same thing right before the motor completely died and fried the VESC. 

Has anyone heard of anything like this before? @torqueboards maybe you have some ideas?
```

---
## \#2 Posted by: Jinra Posted at: 2017-06-27T00:07:03.511Z Reads: 92

```
You gotta post vesc screenshots if you want answers for questions like these
```

---
## \#3 Posted by: t0m_r1dd1e Posted at: 2017-06-27T00:18:52.518Z Reads: 88

```
You got it.

http://imgur.com/a/vJGLX
```

---
## \#4 Posted by: t0m_r1dd1e Posted at: 2017-06-27T00:23:43.558Z Reads: 80

```
The only things that look weird to me is that Tacho: 50k and Temperature: 3 on the fault log. I know I wasn't going nearly that fast and it's definitely not winter here. Maybe the sensor is messed up?
```

---
## \#5 Posted by: Jinra Posted at: 2017-06-27T00:49:11.202Z Reads: 77

```
Hmm yea maybe the sensor is wonky, though your bemf coupling is too high. Maybe try setting that correctly and try again.
```

---
## \#6 Posted by: t0m_r1dd1e Posted at: 2017-06-27T01:21:22.124Z Reads: 76

```
Hmm I just re ran calibration (after taking the pulley off, so with nothing on the motor shaft) three times and it read 960, 970, and 965 for BEMF. Is that bad?
```

---
## \#7 Posted by: Jinra Posted at: 2017-06-27T01:23:59.081Z Reads: 75

```
Should be fine then. It just seems a little high compared to what I've seen.
```

---
## \#8 Posted by: t0m_r1dd1e Posted at: 2017-06-27T01:32:35.783Z Reads: 73

```
I just tried it in sensorless mode and it's still doing it. I'm thinking either the motor or the VESC is faulty at this point.
```

---
## \#9 Posted by: Jinra Posted at: 2017-06-27T01:33:21.196Z Reads: 72

```
Well sensorless just disables the hall sensors, not the current/temp sensors on the VESC. It might be the onboard sensors that are messed up.
```

---
## \#10 Posted by: Jinra Posted at: 2017-06-27T01:34:39.661Z Reads: 68

```
Maybe try reflashing stock firmware and give it a shot
```

---
## \#11 Posted by: t0m_r1dd1e Posted at: 2017-06-27T01:42:46.453Z Reads: 66

```
Yeah will do and if that doesn't work I'll swap motors and see what happens.
```

---
## \#12 Posted by: t0m_r1dd1e Posted at: 2017-06-27T02:16:13.352Z Reads: 65

```
Stock firmware behaved exactly the same and I didn't have a chance to try the other motor because now it's throwing drv8302 :( 

I don't get it, it was brand new. I know I didn't do anything stupid to fry it. I guess I'll talk to Dexter.
```

---
## \#13 Posted by: Jinra Posted at: 2017-06-27T02:16:52.754Z Reads: 63

```
That sucks, could just be a lemon, it happens
```

---
## \#14 Posted by: Alanhunt123 Posted at: 2017-06-27T02:49:23.604Z Reads: 61

```
Could it be a short that only happens when you go over bumps? That would surly cause some current spikes!
```

---
## \#15 Posted by: t0m_r1dd1e Posted at: 2017-06-27T14:24:15.296Z Reads: 50

```
I thought about that too, but the motor is brand new and I covered the leads with heat shrink after connecting them so idk.
```

---
## \#16 Posted by: rich Posted at: 2017-07-13T03:18:47.324Z Reads: 44

```
Hey @t0m_r1dd1e, did you solve the problem? 
If not maybe i can help.
On my longboard my vesc had the same behavior, even small cracks and the vesc was absent for like 2-3 seconds.
I put a bit of foam under the vesc (+receiver) and i've never had problems again, not the biggest bump was a problem (but for my motor :wink:)
```

---
## \#17 Posted by: t0m_r1dd1e Posted at: 2017-07-13T15:14:50.245Z Reads: 29

```
Oh interesting that you seem to be having the same problem. I wasn't able to continue troubleshooting once the vesc starting throwing the DRV fault. But Dexter contacted me and had me send it in as an RMA. That was last week and I'm waiting to hear back. I'll post back here when it's resolved.
```

---
