# VESC Redundancy&hellip;is it possible?

### Replies: 20 Views: 735

## \#1 Posted by: scepterr Posted at: 2017-09-13T04:38:18.189Z Reads: 133

```
Has anybody come up with anything that'll allow you to have a 2nd vesc hooked up as backup and switch over if the primary fails. This is common on drones, haven't found any mention about it for vesc.
```

---
## \#2 Posted by: Silverline Posted at: 2017-09-13T04:42:05.379Z Reads: 132

```
Not totally redundancy. But i'm using one receiver pr. Focbox. This gives me some sort of safety i think.
```

---
## \#3 Posted by: scepterr Posted at: 2017-09-13T04:43:04.580Z Reads: 131

```
I mean using 2 vescs on 1 motor, 1 vesc active, 1 backup
```

---
## \#4 Posted by: Cobber Posted at: 2017-09-13T04:52:15.385Z Reads: 129

```
No, sorry bro I have not heard of anything like that... I have a scorpion back up guard for my rx circuit... again its a heli thing. I have my switching regulator set at 6.5v and at just over 5v (5.15v) the back up battery (2s 500mah lipo) kicks in and keeps power up to the rx... Apparently fluctuations on this circuit are in part caused by inductance supply variations, or _brown outs_ as they are called. More back up for your TX/RX though than your speed controller...
I'm guessing you would need some kind of switch that can handle the load of your system and this in it self with a eSk8 could be another weakness?
```

---
## \#5 Posted by: scepterr Posted at: 2017-09-13T04:54:33.098Z Reads: 115

```
The phase wires and battery would need to be on relays. 
I want to be able to blow a vesc and automatically switch to another
```

---
## \#6 Posted by: Cobber Posted at: 2017-09-13T04:56:54.143Z Reads: 105

```
I get that bro, what is you system max, cont/peak v/amp loads?
```

---
## \#7 Posted by: scepterr Posted at: 2017-09-13T04:57:52.939Z Reads: 103

```
8S 30A cont
```

---
## \#8 Posted by: Cobber Posted at: 2017-09-13T05:12:43.872Z Reads: 98

```
33.6v/30A well that isn't a lot, I have never had good luck with relays being reliable at any significant amp... I think you will need lots of headroom and my brief search gave me quite large components? I think it might be cheaper just to buy a VESC6 than a 4.xx with the switching system, add in the second vesc 4.xx and it will be a more expensive route?
VESC6 is looking pretty un-breakable at this point :punch:
```

---
## \#9 Posted by: scepterr Posted at: 2017-09-13T05:14:12.524Z Reads: 86

```
I agree but for me a half dozen vesc4 cost as much as 1 vesc6. Waiting to see price on vesc6 bom and PCB
```

---
## \#10 Posted by: Cobber Posted at: 2017-09-13T05:17:25.713Z Reads: 83

```
what HW variation are you using?
might be easier to upgrade mosfets...
```

---
## \#11 Posted by: scepterr Posted at: 2017-09-13T05:18:41.820Z Reads: 82

```
4.12 with irf7530 atm
Waiting on directfet PCBs
```

---
## \#12 Posted by: Cobber Posted at: 2017-09-13T05:24:29.533Z Reads: 80

```
at 8s/30A are you cooking vesc's?
```

---
## \#13 Posted by: scepterr Posted at: 2017-09-13T05:26:01.878Z Reads: 75

```
I can if I try
```

---
## \#14 Posted by: Cobber Posted at: 2017-09-13T05:28:53.891Z Reads: 78

```
sorry a bit diverted, but... do you know what sort of peak amp numbers you are hitting?

[quote="scepterr, post:13, topic:33015, full:true"]
I can if I try
[/quote]
(that is a bit disappointing)
```

---
## \#15 Posted by: scepterr Posted at: 2017-09-13T05:31:24.971Z Reads: 74

```
40-45 I think. I abuse it in every way possible. Full break from full accel and accel again, start from incline. Just punish it.
I keep tweaking it to make it take more abuse
Running 8-10c less under load with this latest addition 😀
<img src="/uploads/db1493/original/3X/4/2/42808bb0d43e04e5db128bebeafbaaa514889351.jpg" width="666" height="500">
I'll be doing some tests with 400watt peltier cooler
```

---
## \#16 Posted by: Cobber Posted at: 2017-09-13T05:50:35.639Z Reads: 72

```
sounds cool :sunglasses: I just have little fans on my aluminium esc case...
```

---
## \#17 Posted by: scepterr Posted at: 2017-09-13T05:53:23.689Z Reads: 70

```
<img src="/uploads/db1493/original/3X/7/e/7e96bba9c3343e2ad17ef81e5507e2b587e9ef68.jpg" width="140" height="250">
```

---
## \#18 Posted by: banjaxxed Posted at: 2017-09-13T09:10:37.232Z Reads: 58

```
As far as I understand if in dual focbox setup and you want redundancy against a problem with the master focbox then if using CAN for focbox comms should te master go down it will take the slave vesc as well - dead board.

But you can use a recevier Y-splitter and configure each vesc seperately instead, but you lose at least one feature - traction control afaik.
```

---
## \#19 Posted by: Nordle Posted at: 2017-09-13T10:19:31.441Z Reads: 50

```
Read again
```

---
## \#20 Posted by: FredSaberhagen Posted at: 2017-09-13T15:20:03.238Z Reads: 35

```
Peltier can only move the heat a little ways for you and is very inefficient .  You can spend 400w on a Peltier and only move 40w worth of heat.  You need a large heat sink or something on the hot side of the peltier to dump into, or you will quickly hit your delta-temp.  And then, why not put that heat sink directly on the vesc??

If you wanted to really get effective use of those 400w consider ripping a liquid cooled system out of a computer (gaming rig)  or a vapor chamber heat pipe from an old tablet/hybrid computer

Or, a big ass piece of graftech or similar TIM material , in proper compression, and use your whole enclosure or board as a heat sink

At the end of the day you will have a hard time creating a dual-vesc switchover as detecting the fault may be the hangup.  Any switch you put into the circuit on the phase wires will be costing you efficiency and creating heat as well :-(
```

---
