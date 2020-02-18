# I have shorted B0 and B1 on evolve BMS

### Replies: 9 Views: 257

## \#1 Posted by: Eretron Posted at: 2018-07-08T20:12:58.988Z Reads: 82

```
Hello in the process of replacing evolve battery with 18650 10s4p pack I have accidentally shorted B0 and B1 pins on a BMS. 

Since then the board won't turn on, but is charging regularly. 

Any ideas how to address this issue, is there any way to order just a BMS or I am screwed and my only option is to order brand new battery?

Thanks in advance.
```

---
## \#2 Posted by: PickSix24 Posted at: 2018-09-09T15:22:58.427Z Reads: 47

```
 @Eretron Any update on this ? I just installed a 18650 pack and didn’t realized the new charge port  lead I bought was wired backwards, Shorted something when I plugged in. Now the board won’t turn off/on using power switch. I can get it to turn on and motors will works by power cycling the main bat plug, but then I can’t turn the board off.
```

---
## \#3 Posted by: Eretron Posted at: 2018-09-09T15:40:41.409Z Reads: 44

```
Damn, sorry to hear that...

Unfortunately I didn't bother with this, I just got second hand BMS from one of forum members...

I just hope that you didn't screw up the ESC alongside with BMS... Do you have spare BMS so you can check if everything else is ok?
```

---
## \#4 Posted by: PickSix24 Posted at: 2018-09-09T16:40:26.741Z Reads: 35

```
Unfortunately not. Funny thing is I can get motors, everything to work if I power cycle the main battery plug, Go figure it will work just can’t turn it on/off normally... 😆
```

---
## \#5 Posted by: Acido Posted at: 2018-09-09T17:23:43.831Z Reads: 32

```
are you sure that the bms is still balancing your cells?
```

---
## \#6 Posted by: b264 Posted at: 2018-09-09T17:29:11.039Z Reads: 29

```
[quote="PickSix24, post:2, topic:61277"]
I can get it to turn on and motors will works by power cycling the main bat plug, but then I can’t turn the board off.
[/quote]

No problem, the 5 minute "f- you" timer will turn it off for you :stuck_out_tongue:

LoL the real problem is how to turn it on again without pressing "brake" on the remote every 2 minutes the entire time you're not riding it
```

---
## \#7 Posted by: PickSix24 Posted at: 2018-09-09T18:40:04.315Z Reads: 23

```
@Acido yes , I plugged in the charger and went into the battery diagnostics screen. I can see they are balanced
```

---
## \#8 Posted by: PickSix24 Posted at: 2018-09-09T18:47:26.446Z Reads: 23

```
Looks like I have solved my issue. Did some probing with my multimeter on BMS. Noticed not all of the soldered leads have continuity. Which tells me that one of  grounds are part of the switch circuit. Then I looked at some photos I took and noticed I had P- on the other main ground backwards. Re soldered them correctly and presto ! A functioning board !!!!
```

---
## \#9 Posted by: Eretron Posted at: 2018-09-09T18:53:36.558Z Reads: 21

```
Nice. Glad u made it
```

---
