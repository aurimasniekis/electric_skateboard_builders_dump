# VESC not lighting up after running fine

### Replies: 11 Views: 171

## \#1 Posted by: hi-fi88 Posted at: 2019-04-01T16:21:29.166Z Reads: 57

```
I have just completed my build and I am running a 6364 190 kv motor 12s1p 8ah set up.
With a Maytech 4.12 VESC.(PPM) Every thing was running fine for the first twenty minutes. Then upon taking it to test. I rode it a few blocks to have it just die, and seemed to lose power. The RX was not lighting up while the VESC had a light on. So I walk home unplug it and try and sort it out. Only to get it working momentarily. Which point it stopped with some flashing red lights. So I unplugged it all, and let it sit. went to plug it in and nothing. no lights anywhere. And when I connect it to the battery I got a slight "ringing" noise. So I unpluged it and today I have it with my trying to sort the issue. So I connected it to the power and it worked okay. for a few minutes while I spun it up on the PC. 5 minutes tops and it just dies, no power, only fault I got in the tool was Status: Serial port error: The I/O operation has been aborted because of either a thread exit or an application request. Looking a the board it looks to be in fine condition. But I was hoping someone could help me work in the right direction, as I really don't want to buy another VESC.
```

---
## \#2 Posted by: threebysix Posted at: 2019-04-01T16:28:55.931Z Reads: 54

```
I don't have an answer for you but I have read about running the motor without load on the workbench is not recommended because it can reach max erpm. Apprently, the vesc can be damaged if there is no set limit for max erpm.
```

---
## \#3 Posted by: hi-fi88 Posted at: 2019-04-01T16:36:56.106Z Reads: 51

```
I was barely running it up to 30% throttle. with out any load or weight on the board. But my issue seems to be power going through the board, as  I had it working just fine, then all the lights went off, and it died. unplugged it for a bit, and it came back to life, only to die again, tried it again and it was alive shortly, but now I just get this humming like noise, and nothing. If I unplug the PPM the noise get louder. but no lights which makes me think there is a short somewhere on the board. which I am not able to determine.
```

---
## \#4 Posted by: threebysix Posted at: 2019-04-01T16:42:46.489Z Reads: 43

```
Do you have an anit-spark switch in there? Maybe it's faulty anti-spark?
```

---
## \#5 Posted by: hi-fi88 Posted at: 2019-04-01T16:46:30.387Z Reads: 42

```
I do not, I am getting 37 volts at the connection point to the VESC, just not getting any lights but a loud humming whistling noise that makes me believe something has blown on the board.
```

---
## \#6 Posted by: threebysix Posted at: 2019-04-01T16:54:49.157Z Reads: 41

```
Is there any burnt smell coming from the vesc? Does the DRV chip look physically intact (e.g. no tiny pit holes on the chip, no charred marks on the pins, etc..)?
```

---
## \#7 Posted by: hi-fi88 Posted at: 2019-04-01T16:57:11.981Z Reads: 40

```
The only thing I can see on the DRV chip is what appears to be a finger print in some from of glue that was on it when they put it together. But I am not seeing anything burnt or smelling burnt, there as no pop noise, just running running, dead, complete lose of power, no lights just the  noise.
```

---
## \#8 Posted by: hi-fi88 Posted at: 2019-04-01T17:04:07.689Z Reads: 39

```
So here is some pictures. But I get a ringing noise when I power it up. Like ding ding ding ding, etc very high pitch.![image|666x500](upload://wL9nrBtxisljrG03Da1Pt1YaQRY.jpeg) ![image|666x500](upload://xMClqa6OyvzLZebnGpbuF7lwL40.jpeg)
```

---
## \#9 Posted by: hi-fi88 Posted at: 2019-04-01T20:15:43.945Z Reads: 32

```
Got a charger on my batteries and got them back to full, and that seemed to get the VESC back on, but I ran it a little and got a few faults. 
Fault            : FAULT_CODE_DRV
Current          : 0.5
Current filtered : -12.2
Voltage          : 40.35
Duty             : 0.003
RPM              : 10290.6
Tacho            : 3207
Cycles running   : 1539
TIM duty         : 27
TIM val samp     : 2
TIM current samp : 4200
TIM top          : 8400
Comm step        : 0
Temperature      : 25.34
 
Fault            : FAULT_CODE_DRV
Current          : -3.9
Current filtered : 29.3
Voltage          : 40.02
Duty             : 0.036
RPM              : 6626.8
Tacho            : 22374
Cycles running   : 95
TIM duty         : 304
TIM val samp     : 2
TIM current samp : 4200
TIM top          : 8400
Comm step        : 0
Temperature      : 29.73
 
Fault            : FAULT_CODE_DRV
Current          : 5.8
Current filtered : 2.8
Voltage          : 39.99
Duty             : 0.039
RPM              : 5323.0
Tacho            : 34800
Cycles running   : 15
TIM duty         : 327
TIM val samp     : 2
TIM current samp : 4200
TIM top          : 8400
Comm step        : 0
Temperature      : 29.83
Can anyone tell me what these mite mean?
```

---
## \#10 Posted by: RedBaron Posted at: 2019-04-01T21:47:42.892Z Reads: 28

```
What did you set your battery max to on the esc? The battery leads look like they melted the solder on the vesc.
```

---
## \#11 Posted by: hi-fi88 Posted at: 2019-04-01T22:33:32.634Z Reads: 28

```
I have the max amps set to 40, with the max volts 57. The battery cutoff is at 30v absolute minimum 28volts. as I said not sure what issue if any I am experiencing as it seems to be in working order currently.
```

---
