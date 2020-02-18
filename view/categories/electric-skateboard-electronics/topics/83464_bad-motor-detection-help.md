# Bad motor detection help

### Replies: 23 Views: 259

## \#1 Posted by: WolfKnight Posted at: 2019-02-07T13:22:41.616Z Reads: 89

```
So just a preface, I'm new to all of this so if there is any extra info you need please ask and i'll try and provide it.
The parts for my board are all bought from https://eskating.eu/.
motor: 6365 190kv sensored
vesc: maytech vesc firmware 3.40 hardware 4.10
battery: 10s2p

So the problem is, I've been riding the board for a few weeks and on a ride the motor suddenly stopped spinning and wouldn't respond to the remote. Once it was home and there was no load on it, the motor would sort of stutter. Then I went into the VESC tool and tried to use that to spin the motor, it spins properly but then says bad detection results, detection failed. I've looked across the forums but nothing I've found so far has worked. Hoping someone can help with this. If i've missed something out please let me know.
```

---
## \#2 Posted by: Andy87 Posted at: 2019-02-07T13:25:09.810Z Reads: 86

```
I would check my sensor wires.
Maybe one of the wires broke, maybe one pin in the jst got lose etc etc.
Do you use an extension cable?
Like from the 1.5mm jst to the 2mm jst.
```

---
## \#3 Posted by: Friskies Posted at: 2019-02-07T13:36:48.341Z Reads: 83

```
Plug the controller into your computer and see if it throws any faults through the vesc tool. I'm aiming you have already checked all of the connections etc
```

---
## \#4 Posted by: dg798 Posted at: 2019-02-07T14:03:48.096Z Reads: 74

```
If the tool doesn’t show any faults type “faults” into the terminal and see what it says.
If it says there are no faults from startup try turning the motor manually and see if it spins normally or it’s giving you resistance.
```

---
## \#5 Posted by: banjaxxed Posted at: 2019-02-07T14:36:09.142Z Reads: 71

```
Try increasing the duty
```

---
## \#6 Posted by: Friskies Posted at: 2019-02-07T14:41:06.171Z Reads: 66

```
It will show if he has a drv error if he checks. He can also run motor detection and see if it errors too...
```

---
## \#7 Posted by: AlanZhou Posted at: 2019-02-07T14:44:18.374Z Reads: 61

```
I've also had issue when using sensored bldc on enertion hubs but did sensored foc without a hitch 

So mabye try different settings?
```

---
## \#9 Posted by: Friskies Posted at: 2019-02-07T14:51:07.437Z Reads: 56

```
Hmmm maybe he just needs to try running the board in sensorless mode to see if it works...
```

---
## \#10 Posted by: Andy87 Posted at: 2019-02-07T14:57:40.114Z Reads: 54

```
That’s a good idea to make sure it’s only an issue with the sensors or the wiring.
```

---
## \#11 Posted by: WolfKnight Posted at: 2019-02-07T15:32:17.094Z Reads: 50

```
I assume I need a multimeter or something else to check the wires for this? There's no visible damage on the sensor pins, although the VESC end was compressed to fit in the case so I could see one of them becoming damaged over time. I'll get something to check the wires and check back on this one
```

---
## \#12 Posted by: WolfKnight Posted at: 2019-02-07T15:35:49.654Z Reads: 48

```
It doesn't throw out any errors, even typing 'faults' into terminal it says no faults. It's just the bad detection message
```

---
## \#13 Posted by: WolfKnight Posted at: 2019-02-07T15:38:01.625Z Reads: 49

```
Just tried it in sensorless mode, it doesn't even spin, just stutters a few times and a red led flashes on the VESC
```

---
## \#14 Posted by: WolfKnight Posted at: 2019-02-07T15:40:49.412Z Reads: 49

```
also got these faults now:

Fault            : FAULT_CODE_ABS_OVER_CURRENT
Current          : 67.9
Current filtered : 130.1
Voltage          : 38.63
Duty             : 0.081
RPM              : 74.7
Tacho            : 8745
Cycles running   : 3592
TIM duty         : 2265
TIM val samp     : 1132
TIM current samp : 15165
TIM top          : 28065
Comm step        : 1
Temperature      : 27.31
 
Fault            : FAULT_CODE_ABS_OVER_CURRENT
Current          : 49.7
Current filtered : 131.7
Voltage          : 39.19
Duty             : 0.077
RPM              : 54.0
Tacho            : 8814
Cycles running   : 3288
TIM duty         : 2214
TIM val samp     : 1107
TIM current samp : 15456
TIM top          : 28698
Comm step        : 4
Temperature      : 27.75
```

---
## \#16 Posted by: Andy87 Posted at: 2019-02-07T15:45:04.537Z Reads: 47

```
Check your phase wires, solder joins.
Make sure the capacitors are fixed properly on the vesc etc.
Likely that the fault comes from a lose or bad connection.
```

---
## \#17 Posted by: Turboboard Posted at: 2019-02-07T15:52:36.194Z Reads: 48

```
I was getting the same results when I first hooked my motor to vesc. It was because I tried to hook one of the motor wires to vesc wire with an aluminium clamp deal and not enough current would reach the motor. Motor would stutter and vesc would flash red. Problem stopped once I connected the wires correctly
```

---
## \#18 Posted by: Friskies Posted at: 2019-02-07T16:23:28.952Z Reads: 44

```
Just checking here. Are you motor settings equal to or less than 25/-25 amps respectively? Most of these Chinese vesc copies can't support more than that. Also can be due to high resistance or a bad connection as above. Try switching motors and speed controllers around and seeing if that has any affect.
```

---
## \#19 Posted by: RedBaron Posted at: 2019-02-07T18:50:35.761Z Reads: 33

```
If your using a dischatge bms check that you didn't create a ground loop. I had a bms that had multiple shunts to connect battery wires. 4 on each side, I connected the battery - to all 4 shunts, when I would use the breaks I would get abs over current. I also got over current from a bad series connection once. Good luck.
```

---
## \#20 Posted by: dareno Posted at: 2019-02-07T19:03:46.084Z Reads: 31

```
I hate to be the bearer of doom and gloom but if that motor was defective then re doing the detect will have damaged the vesc.  Always check the motor first before hooking it back up to the vesc tool.
```

---
## \#21 Posted by: WolfKnight Posted at: 2019-02-08T17:56:04.545Z Reads: 27

```
checked wires today, everything seemed fine is  there anything else I could try?
```

---
## \#22 Posted by: WolfKnight Posted at: 2019-02-08T17:56:33.344Z Reads: 27

```
I'm not sure, how would I go about checking that?
```

---
## \#23 Posted by: Andy87 Posted at: 2019-02-08T18:02:51.689Z Reads: 24

```
I don’t know of anything else.
```

---
## \#24 Posted by: Friskies Posted at: 2019-02-08T19:30:26.813Z Reads: 19

```
Switch the phase wires from the working motor to the currently not working speed controller. Run detection etc and see if it will spin properly.
```

---
## \#25 Posted by: Bataleon Posted at: 2019-06-22T09:25:36.771Z Reads: 10

```
Did you mange to solve the issue @WolfKnight? My VESC has the exact same symptoms: giving any throttle results in the motor jittering, red light flashing then a `FAULT_CODE_ABS_OVER_CURRENT` error.

Using the keyboard keys (while connected to the BLDC Tool) also results in jittery/stuttering motor spinning. Running a motor detection fails. I have tried 3 different motors so it's not a motor issue. I've also tried different firmware without success.

It was running perfectly until yesterday morning when it just stopped for no reason.
```

---
