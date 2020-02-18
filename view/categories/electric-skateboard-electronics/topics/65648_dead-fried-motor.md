# Dead/Fried Motor

### Replies: 23 Views: 440

## \#1 Posted by: Ryguy Posted at: 2018-08-21T23:20:40.114Z Reads: 126

```
I went on first ride today and everything was going smoothly until I went full throttle uphill. The when I reached the top and attempted to brake I had to jump of the board as the motor locked up, there was also a terrible smell emitting from the motor. I think the motor is fried, and when I try to turn the motor with my hand it is deficiently harder to turn than before but still turns. When using the remote it no longer spins just throbs back and forth. I think it was fried as I made the motor and battery cutoffs on the "safe" (low) side which I believed overheated my motor after going full throttle uphill. I lost the exact values but they were around 30A for motor current max/max brake and battery current max/max regen off maybe 35/20 A. 

Not sure if this is any issue or just glue
![IMG_3725%202|375x500](upload://dltGIFe9iAGPo5i0PTajZJXQOL4.JPG)

My setup is a 9S2P battery, torque boards 5055/190KV Motor, torque boards nano remote and a torque ESC BLDC.
![IMG_3727%202|374x500](upload://dEiUPJGbXel4FAZe2YKAcgpz56u.JPG)
![IMG_3732|666x500](upload://3uWr06I10NxiHARz36asSXFNYaD.JPG)
This last picture is what the default setting on the speed controller was, should I have kept these?
![IMG_3734|666x500](upload://ftbGLjJWP4WklmUsiLQxK4kg3lQ.JPG)
Pretty new to this stuff obviously, so I'm just wondering if my motor is completely dead, (ESC seems fine) and what my values should have been, assuming those were what caused the overheat. Any help would mean a ton, thanks.
```

---
## \#2 Posted by: Rinzler Posted at: 2018-08-21T23:30:41.418Z Reads: 110

```
If it smells bad it is fried, for sure try looking for a black part on the winding. You can rewind it, but take it off your board trying to ride a shorted motor will certainly fry the VESC. Same thing happened to me, the solution is to switch to a bigger motor, the smaller motors may have the power but they dont have enough mass so they heat up fast.
```

---
## \#3 Posted by: Ryguy Posted at: 2018-08-22T18:29:37.133Z Reads: 77

```
What size motor would you recommend/you use?
```

---
## \#4 Posted by: dareno Posted at: 2018-08-22T18:45:59.165Z Reads: 72

```
Have you run the motor detection?
```

---
## \#5 Posted by: Silverline Posted at: 2018-08-22T18:50:27.162Z Reads: 72

```
And the screws holdning the motor, is not to Long and touching the windings in the motor ?
```

---
## \#6 Posted by: b264 Posted at: 2018-08-22T18:53:08.636Z Reads: 67

```
[quote="Ryguy, post:3, topic:65648, full:true"]
What size motor would you recommend/you use?
[/quote]

5055 or 5065 for quad

6355 for dual

6374 or 6384 for single
```

---
## \#7 Posted by: longhairedboy Posted at: 2018-08-22T18:55:40.280Z Reads: 65

```
hmmm.. i wonder what a quad 5055 feels like...
```

---
## \#8 Posted by: Brdchris Posted at: 2018-08-22T18:58:48.149Z Reads: 66

```
Like a single 20,220.
```

---
## \#9 Posted by: b264 Posted at: 2018-08-22T18:59:53.015Z Reads: 67

```
[quote="Brdchris, post:8, topic:65648, full:true"]
Like a single 20,220.
[/quote]

@MoeStooge has made some similar to that with inrunners, but they are dual
```

---
## \#10 Posted by: longhairedboy Posted at: 2018-08-22T19:01:41.299Z Reads: 69

```
@Ryguy  Do not run detection on that motor. You could end up frying your ESC as well. @b264 is right. Get a much larger motor for single drive. The SK3 6374 is a classic and a known good single drive solution if you can find one.

Your belt width should be just fine for single drive in case you were wondering.
```

---
## \#11 Posted by: b264 Posted at: 2018-08-22T19:03:45.882Z Reads: 64

```
Here is how I test a motor:

Disconnect motor from anything else
Connect phase A to B and verify choppy brakes
Connect phase A to C and verify choppy brakes
Connect phase B to C and verify choppy brakes
Connect phase A to B to C and verify smooth, strong brakes

If the first three are not all the same strength and feel, and the last one is not noticeably stronger and smooth, then you have a winding problem in your motor.
```

---
## \#12 Posted by: dareno Posted at: 2018-08-22T19:10:42.145Z Reads: 62

```
Yeah sorry should have worded that better i meant had he ran detection on it.  My bad its v early over here. :expressionless:
```

---
## \#13 Posted by: longhairedboy Posted at: 2018-08-22T19:14:20.039Z Reads: 57

```
i figured that's what you meant, but it needed to be clarified immediately... some people would see that and be like "oh i better do that.." and then poof. 

i have a drawer full of poof. lol
```

---
## \#14 Posted by: dareno Posted at: 2018-08-22T19:16:57.562Z Reads: 56

```
Same, lots of paperweights round here.  Thanks for that!!
```

---
## \#15 Posted by: MoeStooge Posted at: 2018-08-22T19:22:50.716Z Reads: 52

```
Single, single single.! I made a single  [IMG_20170930_204406131_HDR|281x499](upload://ayuFlrca7FY4Y7W1B9NHrk7kGQ4.jpg) ! 

![IMG_20170119_201927218|690x388](upload://a905ykNRgBTHJYEzEJV8ADXCbom.jpg) ![IMG_20170402_132027604|281x499](upload://rnnQgIqCggn0Rcq55Y9IsKJvhiD.jpg) ![IMG_20170520_105252860_HDR|690x388](upload://yjXghntQYBuBsp0dc0YPIgrncik.jpg) ![IMG_20180815_201713_769|500x500](upload://kDEaml38vGcVhTbcWHphiYgc6fi.jpg)
```

---
## \#16 Posted by: Blitz Posted at: 2018-08-22T19:40:32.035Z Reads: 47

```
Hows braking on a single motor with 0 skips?
```

---
## \#17 Posted by: Ryguy Posted at: 2018-08-22T19:45:36.725Z Reads: 46

```
Thanks @dareno @longhairedboy @b264 I'll get SK3 6374.
```

---
## \#18 Posted by: Brdchris Posted at: 2018-08-22T19:45:51.419Z Reads: 49

```
That’s good, but you could also just verify with a meter. Phase to phase should all have the same resistance and no phase should have a path to ground I.e. the motor case or shaft etc.
```

---
## \#19 Posted by: dareno Posted at: 2018-08-22T19:50:54.687Z Reads: 47

```
Thanks man just glad I didn't make it worse.  6374 all the way.  The sk8 is an option too, I've had 3 running for about 6 months. 2 on a dual and one on a single with no issues so far.
```

---
## \#20 Posted by: longhairedboy Posted at: 2018-08-22T19:54:54.781Z Reads: 47

```
Its a field diagnostic tactic that's incredibly effective when you don't have a volt meter on hand. We use this exact method all the time out of laziness because it works so well at determining if the motor is a candidate for The Drawer.
```

---
## \#21 Posted by: MoeStooge Posted at: 2018-08-22T20:16:21.396Z Reads: 45

```
On a urethane wheel single rear drive I could lock-up the rear under hard decel.  Bigger the motor better the braking.  Gotta put the heat somewhere.
```

---
## \#22 Posted by: Blitz Posted at: 2018-08-22T20:20:03.732Z Reads: 47

```
@MoeStooge Traction wise is it fine? Say you have a 6380 would you be golden?
```

---
## \#23 Posted by: MoeStooge Posted at: 2018-08-22T20:26:37.402Z Reads: 45

```
Can't say on the outrunner can. I imagine it would work out very well @ 4100watts.  traction is better on a front drive single
```

---
