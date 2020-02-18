# Is my VESC toast? ABS Over current

### Replies: 8 Views: 221

## \#1 Posted by: Anubis Posted at: 2018-11-05T00:31:33.934Z Reads: 69

```
Edit: Caused by a poor bullet connector solder. Beneath the shrink wrap, one of the bullet connectors attached to the vesc must have become disconnected or had a poor connection. Eventually i pulled it off completely which revealed the issue

My vesc cannot do FOC or BDLC Motor detection. I have a 12S5P 30Q Battery with a 80A BMS Inside from eskating.eu. I cannot see any physical signs on the PCB that would indicate things have gone wrong, when comparing the VESC to a working 6.6 I have. 

Vesc settings: 
MOTOR: http://prntscr.com/lef9nq

With no other vesc plugged in, motor detection will spin the motor for 1 microsecond and stop instantly, such that it makes a blip then spins off whatever speed it had. This is on a testbench with no belts on the motor at all. the vesc does this with both motors i have tested. 

I think there is a chance that the phase wires may have touched during an earlier test. Could this fry the VESC? Is there anything I can do to have this repaired?

VESC Error:
The following faults were registered since start:

Fault            : FAULT_CODE_ABS_OVER_CURRENT
Current          : 34.7
Current filtered : 154.9
Voltage          : 47.00
Duty             : 0.011
RPM              : 184.3
Tacho            : 16
Cycles running   : 6598
TIM duty         : 554
TIM val samp     : 277
TIM current samp : 24859
TIM top          : 49165
Comm step        : 1
Temperature      : 28.40

Is produced by running a motor detection or pushing the trigger in any way on the testbench.
```

---
## \#2 Posted by: brenternet Posted at: 2018-11-05T00:38:07.892Z Reads: 65

```
[quote="Anubis, post:1, topic:73468"]
I think there is a chance that the phase wires may have touched during an earlier test. Could this fry the VESC?
[/quote]

Yes, this can kill an esc. @Martinsp may be able to help
```

---
## \#3 Posted by: J0ker3366 Posted at: 2018-11-05T00:41:27.213Z Reads: 63

```
Or @ThermalM16
```

---
## \#4 Posted by: Anubis Posted at: 2018-11-05T00:42:42.862Z Reads: 63

```
He is USA I'm EU
```

---
## \#5 Posted by: Deodand Posted at: 2018-11-05T01:05:55.380Z Reads: 59

```
run it with no motor plugged in, if it faults then its definitely fried.
```

---
## \#6 Posted by: Anubis Posted at: 2018-11-05T07:47:54.907Z Reads: 48

```
No faults when pushing the trigger and running BDLC tests with no motors plugged in.
```

---
## \#7 Posted by: SPIRITRON Posted at: 2018-12-20T16:51:02.002Z Reads: 29

```
What was the outcome of this? I have exact same thing on one of my 4.12 maytech
```

---
## \#8 Posted by: Anubis Posted at: 2018-12-21T08:55:14.194Z Reads: 23

```
Under one of my bullet connectors shrinkwraps, the connection had come off. Nearly completely so effectively it wasnt connected
```

---
