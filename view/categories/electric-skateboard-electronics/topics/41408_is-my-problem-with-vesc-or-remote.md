# Is my Problem with vesc or remote?

### Replies: 17 Views: 617

## \#1 Posted by: Daniel828 Posted at: 2017-12-19T03:26:25.942Z Reads: 74

```
I’m new to eskateboarding, I just put together an old vanguard with single torque board 6374 and 12s1p a123 pack. It’s an older pack from an ebike project. My problem is a stuttering/jerking when I apply power. I fooled around with some vesc settings and that didn’t seem to change any of the problems. It happens during braking too.  I have a maytech 1712 remote and the recover is mount close to the vesc. Any help would be greatly appreciated<img src="/uploads/db1493/original/3X/a/8/a84153a01033ecbdbe6cdfb4fca74af1a8b6c94d.jpg" width="669" height="499"><img src="/uploads/db1493/original/3X/e/9/e90ac2308487ef627804b7192ba339b350fb6358.jpg" width="669" height="499"><img src="/uploads/db1493/original/3X/a/5/a5e36f1def1c8b8f9ae0e2ba0b4458113db481b2.jpg" width="669" height="499"><img src="/uploads/db1493/original/3X/e/d/ed13661bb94f71c21f4c15465f606f3a6889502d.jpg" width="669" height="499">
```

---
## \#2 Posted by: JLabs Posted at: 2017-12-19T03:31:41.032Z Reads: 65

```
The stuttering is coming from the VESC. Do you have it setup in Sensored mode or Hybrid? Sounds like you motor/batt amps are too low or the sensors aren’t setup
```

---
## \#3 Posted by: Daniel828 Posted at: 2017-12-19T03:35:12.757Z Reads: 65

```
I tried senorless, sensored, and hybrid.  Also set motor detection with no load, not even the pinion gear was on. My motor max is 70a and I’ve changed my batt amps from 40a up to 70a.  Brake regen is 30a. It seems to get worse after each change
```

---
## \#4 Posted by: Daniel828 Posted at: 2017-12-19T03:37:18.115Z Reads: 64

```
Also, the maytech remote stays on even if I let go of the thumb trigger. It’s only about a split second but it’s a bit unnerving   And as it’s jerking/sputtering it seems to all of sudden take off sometimes too
```

---
## \#5 Posted by: michaelcpg Posted at: 2017-12-19T03:45:07.878Z Reads: 63

```
Does it stutter if you kick push first to get some momentum before you apply any power?
```

---
## \#6 Posted by: scepterr Posted at: 2017-12-19T03:47:26.193Z Reads: 61

```
Did you calibrate remote/ppm settings?
If there's a high/low mode switch make sure it's in high for all setup
```

---
## \#7 Posted by: Bensaida Posted at: 2017-12-19T03:52:41.837Z Reads: 56

```
receiver defect. Happened with my board. Get a new remote and receiver
```

---
## \#8 Posted by: Daniel828 Posted at: 2017-12-19T03:53:43.210Z Reads: 55

```
Yup setup the remote in high mode. It doesn’t seem to do it starting off, but once I get going it’s stuttering   If I floor it off the line it will stutter   If I ease into it off the line it starts nicely but will go into the stuttering problem
```

---
## \#9 Posted by: Daniel828 Posted at: 2017-12-19T03:55:27.391Z Reads: 53

```
Interesting Ben,  what did you end up doing? Replaced rcvr, ?
```

---
## \#10 Posted by: Daniel828 Posted at: 2017-12-19T03:56:29.569Z Reads: 52

```
Sorry, I meant to say, did you get a different manufacturer rcvr or another maytech?
```

---
## \#11 Posted by: Exiledd_Top Posted at: 2017-12-19T04:02:47.719Z Reads: 51

```
Have u tried rebinding the remote
```

---
## \#12 Posted by: Daniel828 Posted at: 2017-12-19T04:04:35.740Z Reads: 50

```
No I didn’t. I’ll give it a try tomorrow. I think the user manual mentions how to do it? I never bind it when I first turned it on. It just worked
```

---
## \#13 Posted by: Exiledd_Top Posted at: 2017-12-19T04:06:38.843Z Reads: 48

```
My gt2b was working and then out of know where the motors would do would you said rebinded not a single issue now
```

---
## \#14 Posted by: Bensaida Posted at: 2017-12-19T04:07:51.430Z Reads: 45

```
hold the remote power button for 3 seconds, then turn on board, to re-pair Also, my board is not a DIY, its a production board, so i am waiting for the company to send us new receivers and remotes so we can install them
```

---
## \#15 Posted by: Daniel828 Posted at: 2017-12-19T04:14:00.968Z Reads: 42

```
Awesome, thank you guys.  I’ll let you know tomorrow how it turns out
```

---
## \#16 Posted by: Daniel828 Posted at: 2017-12-19T04:22:48.648Z Reads: 38

```
I couldn’t go to bed with out trying to rebind.  Didn’t work
```

---
## \#17 Posted by: Daniel828 Posted at: 2017-12-19T15:03:44.591Z Reads: 25

```
SOLVED........  I had the receiver mounted in the same enclosure as the vesc.  I moved the rcvr as far away as possible.  Working great now.  Thanks everyone
Ps. I was wondering why the cable for the rcvr was so long!??  Lol
```

---
