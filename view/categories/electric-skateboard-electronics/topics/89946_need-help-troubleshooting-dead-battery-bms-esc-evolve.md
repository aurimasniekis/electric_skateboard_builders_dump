# Need help - troubleshooting dead battery / bms / esc - evolve

### Replies: 13 Views: 354

## \#1 Posted by: davidbonde Posted at: 2019-04-09T17:18:15.753Z Reads: 55

```
I have this evolve system that have been exposed to water. The battery is dead and I have made a new one. Both the bms and the esc seem to have avoided the water. But that’s not certain. 

When I plugged in the battery it nothing happened could not turn on the board or charge either. 

The battery measure 34V (its not fully charged fully yet) before the bms. After the bms it measure 20V. So the bms is not completely dead something happens there. 

How do I know if the bms is the problem? 

Any suggestions in how to troubleshoot this and find the solution / part to change?

How do I know if the esc has taken damage. Any suggestions?

![image|666x500](upload://qFFyojupO8yD31ZLJgxxobnR4SL.jpeg)
```

---
## \#2 Posted by: olestra Posted at: 2019-04-09T17:36:31.041Z Reads: 49

```
Do the easy stuff first, then work your way forward. 

Are all connection secure including all the balance leads? are there any melted wires? does any circuit board smell burnt --unless you have a really good trained eye, you'll likely smell a damaged circuit board long before you'll see the failure.

working your way from the start forward:
Measure each cell, are they within normal range (3.2-4.0)? are they within about .1v of each other? If not, fix that first.

Bypass the BMS, for testing. Does the ESC power up, and motors run? if so, BMS has a problem. if not, ESC has an problem, and the BMS is unknown.
```

---
## \#3 Posted by: davidbonde Posted at: 2019-04-09T17:59:14.347Z Reads: 44

```
Thanks. All the easy stuff have been tested nothing seems wrong there. It´s a new pack and all the cells and p-groups do measure within 0.01 (34.5) of each other.

I think next thing to do could be to bypass the bms and probably also the switch . Do you know if the evolve esc can run without the bms. They are connected with an awful lot of wires.
```

---
## \#4 Posted by: olestra Posted at: 2019-04-09T18:14:19.663Z Reads: 42

```
I have no idea about evolve's proprietary systems, so I'm clueless to the specific quirks here

There shouldn't be connections between a BMS and an ESC. other than + and -, so unless you can identify what those do... you probably need to find a wiring diagram

The easiest way to bypass the BMS would likely be to use a jumper from the negative of the battery to the negative of the ESC. but given the other connections between BMS and ESC, doing so might be catastrophic, idk.
```

---
## \#5 Posted by: davidbonde Posted at: 2019-04-09T18:21:51.754Z Reads: 37

```
Maybe the excessive wiring between bms and esc is only for information to the display in the remote. If thats the case it could be bypassed. But if the receiver for the remote sits in the bms and not the esc (it must sit in either of these) its not possible. Maybe someone knows @longhairedboy?
![image|375x500](upload://tyFKcfx1tNE6n7xy2Au3BnSUnMb.jpeg)
```

---
## \#6 Posted by: olestra Posted at: 2019-04-09T18:30:10.002Z Reads: 32

```
look for the receiver antenna? it's either a  wire about 25-31mm long, connected at on end only or it's a area on a circuit board that goes |_|¯| like that
```

---
## \#7 Posted by: davidbonde Posted at: 2019-04-09T18:40:11.456Z Reads: 33

```
Could be this one. But I always thought this was some kind of temp. measuring wire. It was tape to the battery! It sits on the bms. I have worked to much on this today. Will continue tomorrow. 
![image|375x500](upload://2C6jI79YPGK5hNowMrULyP6rUs1.jpeg)
```

---
## \#8 Posted by: longhairedboy Posted at: 2019-04-09T19:01:40.446Z Reads: 33

```
yeah the uart connections are so the ESC and BMS can work together to lock out competition. I mean to display information on the proprietary remote.
```

---
## \#9 Posted by: davidbonde Posted at: 2019-04-09T19:04:37.480Z Reads: 30

```
:) so the bms can not be bypassed?
```

---
## \#10 Posted by: longhairedboy Posted at: 2019-04-09T19:08:09.327Z Reads: 30

```
in my experience the ESC won't fire up without it.
```

---
## \#11 Posted by: olestra Posted at: 2019-04-09T19:14:13.486Z Reads: 28

```
that's definitely a thermistor, not an antenna -- two wires, under the plastic would be a glass bead
```

---
## \#12 Posted by: Kram720 Posted at: 2019-09-28T02:08:47.746Z Reads: 15

```
Bypassing with power direct to the esc will work fine. Without the uart connected the esc will be stuck in slow mode. But for testing that’s ok.

How is OP going with this.
```

---
## \#13 Posted by: davidbonde Posted at: 2019-09-28T05:45:08.571Z Reads: 13

```
I ended up changing everything. New batt. New VESC. New bms. New remote.
```

---
