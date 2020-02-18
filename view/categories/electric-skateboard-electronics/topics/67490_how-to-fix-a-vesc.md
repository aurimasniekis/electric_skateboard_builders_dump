# How to fix a VESC

### Replies: 24 Views: 540

## \#1 Posted by: Davo Posted at: 2018-09-09T09:38:05.620Z Reads: 125

```
Hey there! I got a doubl![20180909_113706|374x500](upload://6n9MwlgeHNbTS1R8TVO1BzjZ5cw.jpg)e flipsky VESC, but unfortunately it is a faulty one... I keep getting from master ABS overcurrent, it cannot spin at all, and the prices with UPS to send it back are madness.... latest firmware, never used, how can I check what's the real problem?
```

---
## \#2 Posted by: brenternet Posted at: 2018-09-09T10:04:22.397Z Reads: 117

```

[details="Summary"]
The real problem is that Flipsky isn't accepting the return cost as their own. Demand free return and resolution.

You shouldn't need to be here asking how to fix a new product that arrived faulty.
[/details]


While we're on the topic though, whats going on with the wire reduction and electrical tape onto XT 60 there?
```

---
## \#3 Posted by: dareno Posted at: 2018-09-09T10:08:39.607Z Reads: 116

```
The real problem is that you did some half arsed diy crap and broke it.   @brenternet double take on the pic? lol
```

---
## \#4 Posted by: brenternet Posted at: 2018-09-09T10:10:02.359Z Reads: 115

```
Yeah haha, Flipsky not to blame here.
```

---
## \#5 Posted by: dareno Posted at: 2018-09-09T10:10:44.388Z Reads: 115

```
Christ that shit pisses me off.
```

---
## \#6 Posted by: Davo Posted at: 2018-09-09T10:19:23.251Z Reads: 113

```
Ok I feel like a complete idiot.... I didn't know that wire reduction could do this stuff...
```

---
## \#7 Posted by: brenternet Posted at: 2018-09-09T10:22:22.658Z Reads: 109

```
Eeek, you've gone from 12awg to like 20awg, it's more than likely causing your issue here because it can only handle 1/3rd of the load. Also get some heat shrink and make sure you solder well.
```

---
## \#8 Posted by: Davo Posted at: 2018-09-09T10:24:06.768Z Reads: 108

```
Thanks for the help, I should've studied a bit more, before jump on diy...
```

---
## \#9 Posted by: dareno Posted at: 2018-09-09T11:30:24.440Z Reads: 95

```
Apologies for the harsh words my friend but we rely on real life testing of products here so when someone comes on and is detrimental to a unit that we are hoping is good and it turns out to be user error its a bit frustrating. Flipsky is just on the radar right now so if there is news it has to be informed.  
Good luck and welcome to the club.
```

---
## \#10 Posted by: Davo Posted at: 2018-09-09T13:09:55.026Z Reads: 82

```
no need to apologize, you made me realize that I've been too much in a hurry to try... I'm desoldering the XT60 and tomorrow I'll solder it in a proper way, but from the battery the wires are still 20awg, would it be  still a problem? And do you have any idea of why my setup doesn't work on the master and works fine with slave?
```

---
## \#11 Posted by: mynamesmatt Posted at: 2018-09-09T13:34:11.787Z Reads: 77

```
what sort of a battery are you using!? if it's using 20awg it probably can't push the power you need bud
```

---
## \#12 Posted by: Andy87 Posted at: 2018-09-09T13:40:34.370Z Reads: 72

```
Where you get a battery with 20 awg wires?
Yes there you need to change it too. It’s a week spot. Maybe you can let us know which battery you have and where you got it from?

The abs over current fault shouldn’t be a reason why it’s not working. A reason for this can be a bad solder join or lose components.
Make sure you double check your connections and solder joins, and please take away that 20awg wires. For Esk8 you want to go with min 12awg depending on the current you want to draw from your battery.
```

---
## \#13 Posted by: Davo Posted at: 2018-09-09T15:39:39.237Z Reads: 57

```
I got my first board from APS, which lately I discovered it's similar to ninestep but with differences.
So I?m using the battery of the previous board 10s5p samsung cells, 460Wh 10 C 11Ah
```

---
## \#14 Posted by: Andy87 Posted at: 2018-09-09T15:45:34.103Z Reads: 58

```
I never had a aps pack.
Just to get it right, on your battery, capable to output 110a were 20awg wires for the main plus and minus wires soldered?
Could understand 20awg for the charge wires, but for the main it’s a bit less
```

---
## \#15 Posted by: Davo Posted at: 2018-09-09T15:48:02.465Z Reads: 58

```
Yep, I've never changed the wires, the ESC mounted was set to 30A each ESC, I think Bruno get it from some chinese factory
```

---
## \#16 Posted by: Andy87 Posted at: 2018-09-09T15:54:03.751Z Reads: 56

```
https://www.powerstream.com/Wire_Size.htm

20awg 11a... i would be a bit worry that my wires burn while riding up a hill...

But seems it was working before without issues, right?
```

---
## \#17 Posted by: Davo Posted at: 2018-09-09T15:57:04.625Z Reads: 55

```
Yes it was, no problems at all except for the ESCs, probably killed by the heat riding uphill... I'll change the wires anyway after seeing which cables are better for me
```

---
## \#18 Posted by: Andy87 Posted at: 2018-09-09T15:59:05.002Z Reads: 51

```
And back on our initial problem.
One side was working you said.
What was with the other? You couldn’t even run a motor detection?
```

---
## \#19 Posted by: Davo Posted at: 2018-09-09T16:04:38.199Z Reads: 48

```
Exactly, with the master finished the wizard I run motor setup and it's giving me bad detection error. So I double checked if it was the motor, but it isn't, and If I do the same on the slave motor detection is fine, both FOC and BLCD. Probably bad soldering (my fault) could give me ABS error, but I don't understand why isn't happening the same to the slave. I keep getting 4 flashes from red light
```

---
## \#20 Posted by: Andy87 Posted at: 2018-09-09T16:07:47.775Z Reads: 46

```
Try if you get the fault also without sensor wires plugged. I had once the problem that I got that fault on my master vesc but only if plugged in sensor wires and it was there also not the motor.

Unfortunately I don’t know anything about which led flashing means which problem.
Maybe somebody else here can help?
```

---
## \#21 Posted by: Davo Posted at: 2018-09-09T16:10:37.625Z Reads: 46

```
No sensor wires, sorry, I forgot to say that. A weird thing once or twice the VESC tool has given me 
Fault            : FAULT_CODE_DRV
Current          : -150.2
Current filtered : -17.0
Voltage          : 38.26
Duty             : 0.712
RPM              : 347.0
Tacho            : 5
Cycles running   : 19
TIM duty         : 4076
TIM val samp     : 2038
TIM current samp : 4899
TIM top          : 5723
Comm step        : 3
Temperature      : 30.97
but then it has just disappeared giving me just ABS fault
Fault            : FAULT_CODE_ABS_OVER_CURRENT
Current          : 151.4
Current filtered : 133.5
Voltage          : 38.20
Duty             : 0.001
RPM              : 40173.6
Tacho            : 3
Cycles running   : 0
TIM duty         : 2
TIM val samp     : 1050
TIM current samp : 3150
TIM top          : 4200
Comm step        : 6
Temperature      : 30.60
```

---
## \#22 Posted by: Andy87 Posted at: 2018-09-09T16:14:22.048Z Reads: 44

```
Drv error always bad sign 😬
Where you located?
Maybe you have a local repair service around the corner?
```

---
## \#23 Posted by: Davo Posted at: 2018-09-09T16:23:06.284Z Reads: 41

```
yeah I know, but why has it disappeared? The support team told me that if I can upgrade the firmware DRV is fine...I'm located in Italy, I should take 40 min driive to get in a computer repair shop...
```

---
## \#24 Posted by: Andy87 Posted at: 2018-09-09T16:25:13.282Z Reads: 40

```
Shoot @Martinsp a pm. He repairs all kind of vesc. Maybe you can work something out together.
```

---
