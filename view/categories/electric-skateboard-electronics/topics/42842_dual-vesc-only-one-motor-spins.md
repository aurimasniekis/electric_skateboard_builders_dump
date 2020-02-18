# Dual vesc, only one motor spins?

### Replies: 9 Views: 744

## \#1 Posted by: BadleyBoarding Posted at: 2018-01-05T10:45:23.756Z Reads: 111

```
I've got a dual setup but only one motor, the one connected to the master vesc, spins. Settings are

Vesc (master) 
Vesc id: 0
PPM
send status over can - No 
multiple esc over can - Yes

Vesc (slave)
Vesc id:1 
NO APP
send status over can - Yes
multiple esc over can - No 

Ive already tired messing around with send status over can ticked for both and checked the CAN cable with a multimeter, any suggestions??
```

---
## \#2 Posted by: Namasaki Posted at: 2018-01-05T16:09:46.455Z Reads: 97

```
For Focbox or any Vesc 4

Forget canbus and use a split ppm 
Run both Vescs as masters
```

---
## \#3 Posted by: BadleyBoarding Posted at: 2018-01-05T16:12:08.374Z Reads: 93

```
So run both as masters and connect the receiver to both with no CAN cable?
```

---
## \#4 Posted by: abenny Posted at: 2018-01-05T16:12:35.062Z Reads: 91

```
i fully agree with @Namasaki i burned a vesc first time trying to do canbus and decided to just use a y-split cable and haven't had an issue since.
```

---
## \#5 Posted by: abenny Posted at: 2018-01-05T16:13:46.914Z Reads: 85

```
yes, configure each vesc individually to its motor, and run a y split servo cable from both vescs into the reciever. also make sure you cut one of the 5v wires so you only have 1 input of 5v from the vescs.
```

---
## \#6 Posted by: Colson003 Posted at: 2018-01-05T16:14:54.509Z Reads: 79

```
Did you setup using the BLDC tool or VESC tool?
For some reason I couldn't get it to work using the BLDC tool. It's been working great with the VESC tool.
```

---
## \#7 Posted by: BadleyBoarding Posted at: 2018-01-05T16:15:40.283Z Reads: 78

```
Thank you ill try that, been messing about with this for hours trying to get CAN to work XD
```

---
## \#8 Posted by: BadleyBoarding Posted at: 2018-01-05T16:21:01.608Z Reads: 77

```
Setup both with the vesc tool, honestly I think the CAN is broken on at least one as when I try the command can_devs on the aster it doesn't appear to be able to see the slave
```

---
## \#9 Posted by: Namasaki Posted at: 2018-01-05T20:09:38.145Z Reads: 68

```
[quote="BadleyBoarding, post:3, topic:42842, full:true"]
So run both as masters and connect the receiver to both with no CAN cable?
[/quote]

@abenny beat me to the punch. 
And I agree with everything he said. 
Split ppm is much safer than canbus unless you have a Vesc6
```

---
