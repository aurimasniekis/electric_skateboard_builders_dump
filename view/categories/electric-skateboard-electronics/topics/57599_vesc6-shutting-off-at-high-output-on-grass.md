# VESC6 shutting off at high output (on grass)

### Replies: 17 Views: 478

## \#1 Posted by: ripcurldog Posted at: 2018-06-02T23:18:46.317Z Reads: 183

```
Does anyone know what would cause my VESC6's to shut down anytime I am on grass and apply too much power (if I get to the top of the range during a quick burst of torque, it seems that the VESC's are cutting power to the motors (so I go from full speed forward, to no power at all, which throws me from the board)?
```

---
## \#2 Posted by: ARetardedPillow Posted at: 2018-06-02T23:56:59.296Z Reads: 174

```
Check for any loose conections and check the fault codes when the problem occurs
```

---
## \#3 Posted by: Cobber Posted at: 2018-06-03T00:27:32.397Z Reads: 167

```
could be hitting the thermal cutoff?
```

---
## \#4 Posted by: Deckoz Posted at: 2018-06-03T00:40:39.478Z Reads: 159

```
Logs will help.. could be thermal cutoff. Or your battery is to small relatively to your load and or wheel reduction.  

You could be hitting voltage cut off, thermal cutoff, over current cutoff(depending on what your motor amps is vs your battery)

We need more details...

Battery specs
Reduction
Wheel size
Your weight
Motor max and battery max settings.

Logs if you have them.
```

---
## \#5 Posted by: bloke900 Posted at: 2018-06-03T01:08:39.209Z Reads: 149

```
Could be interference to the signal the receiver is getting.  Make sure the receiver and wires are no where near main power or motor phase leads.
```

---
## \#6 Posted by: CamBo Posted at: 2018-06-03T01:54:07.787Z Reads: 148

```
The ‘Grass’ component makes me think the problem could be traction control related.  

Just one more thing to check.
```

---
## \#7 Posted by: ripcurldog Posted at: 2018-06-03T04:51:40.551Z Reads: 139

```
Thanks for replying.  I did lower the battery/motor amp output.  But if the output is hit, should that really cut power altogether.  Seems that the safer way to go would be to limit power to the max output, not cut power altogether.  I almost ate shat twice because of this.  If the cutoff is reached, does it in fact shut down the power instantly, or should it limit maximum power to the max that you set?  I'm guessing that this is the issue because for the first week of using this Trampa board, it was fine, even on grass, dirt, etc.  But I made some changes to the VESC6 settings, and now this issue has come up.  I'll double check settings.  I think I lowered the Max amp output from 60 to 50, so i'll go back up to 60.

I also have a clicking sound coming from either the motor or the wheels.  WHat is the common cause of clicking?  

My spec's are:

battery:  4 * 6200mah 40C 6 cel lipo's (12S 2P).
```

---
## \#8 Posted by: ripcurldog Posted at: 2018-06-03T04:55:40.592Z Reads: 131

```
The VESC6 were setup so that if I gun it, the tires peel out (I wanted it that way).  The first week I used the board, it was great.  But I lowered the max motor amp output from 60 to 50, so maybe that is the issue.  I'll be really surprised if that's the case.  I would have thought that if the limit were hit, it would simply not allow more power to be exerted and continue to move forward at max speed/torque.  Instead, the power is completely shutting down all of a sudden, which is dangerous because it throws me off the board.  I dont think traction control makes sense.
```

---
## \#9 Posted by: ripcurldog Posted at: 2018-06-03T04:56:13.477Z Reads: 126

```
Does the VESC6 save the fault codes even after the board is powered down??
```

---
## \#10 Posted by: Cobber Posted at: 2018-06-03T04:59:52.925Z Reads: 119

```
At 50 or 60A motor max. you shouldn't be reaching thermal cut off. Your vesc 6 should be able to run that constant. 
What is your battery voltage cut off set at? had you been ridding a while?
```

---
## \#11 Posted by: Eboosted Posted at: 2018-06-03T07:15:00.673Z Reads: 103

```
Does the vesc 6 reboots itself, no power for acceleration or braking for 3 seconds, when the problem occurs? Or its just a power loss for a split second?

The vesc 6 should have no problem even at 120A motor amps so if you are getting issues at 60A then you must find the culprit somewhere else. 

Do you have any fault when the problem occurs? 

I would bet you have broken leg on one of the caps, I had this issue on V6.4 ESC develar times.

Open your VESC and make an inspection. 

Use hot glue to lock the caps in place
```

---
## \#12 Posted by: ripcurldog Posted at: 2018-06-03T16:01:50.792Z Reads: 74

```
What do you mean by ‘broken caps’?   The power cuts out for a split second.
```

---
## \#13 Posted by: trampa Posted at: 2018-06-03T17:35:18.463Z Reads: 63

```
On the VESC 6 the caps don't fall off the PCB. The VESC 6 has a quite complex, moulded silicone part, preventing that parts move or vibrate. The knockoffs don't have the that part and therefore they will get issues one day. 

The described cutout issue is probably traction control related. Switch that feature off and test things again.
```

---
## \#14 Posted by: Eboosted Posted at: 2018-06-03T18:38:24.386Z Reads: 63

```
[quote="ripcurldog, post:12, topic:57599, full:true"]
What do you mean by ‘broken caps’?   The power cuts out for a split second.
[/quote]

This is what I'm refering to:

[img]http://www.electric-skateboard.builders/uploads/db1493/original/3X/3/f/3fbbf279ea91571987ed2e4f09e76f683a762354.jpeg[/img]

I'd wouldn't hurt to open it for inspection
```

---
## \#15 Posted by: hexakopter Posted at: 2018-06-04T13:41:18.995Z Reads: 50

```
Looks like my VESC 6 is missing that moulded silicone part. So its not true for all trampa VESC 6.
```

---
## \#16 Posted by: trampa Posted at: 2018-06-04T14:40:52.742Z Reads: 46

```
Yours has enough silicone parts inside to prevent any vibrations. We never shipped one without necessary components.
```

---
## \#17 Posted by: ripcurldog Posted at: 2018-06-04T16:26:54.076Z Reads: 42

```
Thanks for letting me know Frank!  I have not yet turned off the traction control, so I will give that a try and see if it fixes the issue.
```

---
