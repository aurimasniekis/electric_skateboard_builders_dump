# Weak Motor or VESC Issue?

### Replies: 21 Views: 1937

## \#1 Posted by: bill_f Posted at: 2016-12-03T11:31:30.721Z Reads: 215

```
Hi. Posted this on my build thread but got no views there. Apologies for repost here.
Board has been running great for most part but am getting an oscillation in right motor wheel as I speed up. I think it has to do with one motor becoming weaker than the other at lower rpms. Left motor is easier to stop by hand when at lower rpms. At higher rpms, seems to be fine. Right motor is hard to stop by hand at almost any rpm. The video below shows this. VESCs have not been changed since initial setup. They both have exact same settings. Any ideas? Do you think it's a motor issue or VESC issue? Or something else. Trying to figure out if I need a new motor. Thanks in advance.


https://www.youtube.com/watch?v=k2Z31dxptdg
```

---
## \#2 Posted by: saul Posted at: 2016-12-03T13:44:41.684Z Reads: 195

```
this is a weird one... :thinking:

did you check your connections? Can you make the motor can wobble by hand? could be lose..
```

---
## \#3 Posted by: bill_f Posted at: 2016-12-03T18:21:47.126Z Reads: 171

```
Hi. Motor can seems good as do bearings. No wobble.  Haven't checked connections but my guess is they are okay since the motor seems okay at higher rpms.  Not sure though.  Might have to see how things look using a voltmeter and compare both outputs on each VESC.  THanks
```

---
## \#4 Posted by: TURNROCK Posted at: 2016-12-11T06:54:49.602Z Reads: 154

```
@bill_f  did you figure out what was causing this? Im having a very similar problem.
```

---
## \#5 Posted by: bill_f Posted at: 2016-12-11T12:02:31.881Z Reads: 133

```
No. Haven't figured it out.  My guess is that it's a motor issue. Bought a new motor. Waiting for it to arrive. Will post what I find out once I swap the motor.
```

---
## \#6 Posted by: bill_f Posted at: 2017-03-12T13:47:15.183Z Reads: 123

```
Hi.  So I went and bought a new motor and plugged it in. Same problem. Which makes me think, it has something to do with the VESC, or maybe a bad connection somewhere.

Both VESCS are the same brand with same settings. I've never changed settings since first config.

Has anyone experienced one VESC delivering less power than the other?

How would I measure the voltage being supplied to the motor being that there are three wires leading to the BLDC motor? 

@TURNROCK  Did you manage to solve your similar issue? 

Thanks in advance.
```

---
## \#7 Posted by: Montiey Posted at: 2017-03-12T14:35:01.323Z Reads: 113

```
How are the VESCs connected? I believe this is something to do with traction control, or a problem with your master-slave configuration. I run a single drive so I couldn't tell you much about what the config _should_ be, but I think that's the best place to start.
```

---
## \#8 Posted by: bill_f Posted at: 2017-03-15T14:04:19.381Z Reads: 108

```
Hi. Thanks for the suggestion. Each VESC is actually connected through a Y splitter, so each is getting the exact same signal.  I haven't set up traction control or anything like that.  I'm thinking it's a VESC issue. Or maybe there is a weak connection somewhere in the circuit. I need to take a look at solder joints.
```

---
## \#9 Posted by: TarzanHBK Posted at: 2017-03-15T14:15:50.928Z Reads: 104

```
post a screenshot of your vesc settings
```

---
## \#10 Posted by: saul Posted at: 2017-03-16T06:38:08.152Z Reads: 106

```
reconfig both vescs.
then if it still happens. switch motors/vesc to see if its the motor or vesc.
if its the vesc/connection the opposite motor will have the problem. other wise its the motor....
```

---
## \#11 Posted by: bill_f Posted at: 2017-04-02T08:59:12.361Z Reads: 104

```
Hi. Has to be the VESC. I put a new motor on it and the same thing happens. Just checked settings on both VESCs in the BLDC tool. All looks okay.  Can't figure it out. 
Thanks
```

---
## \#12 Posted by: bill_f Posted at: 2017-04-14T13:38:00.452Z Reads: 94

```
So I keep trying to figure this one out. 
Not so sure it's the VESCs now. I checked both VESCs and the settings are where they are supposed to be. Ran motor detection with BLDC tool and all checks out.
One thing I did notice is that with the diyElectricSkateboard VESCs, the arrow keys do not make the motors move while connected to the BLDC tool (just clicking sound) but with the Ollins, they do move. Not sure what that means.

After riding for a while, I get the oscillations, like one motor is pulling harder than the other. This time, I stopped riding and would roll the board and I noticed that the motor (motors?) are cogging (making a sound and feeling "sticky"). I would roll the board a little more and then lift it off the ground to allow the wheels to spin at full throttle for a few seconds. Problem disappears (until it starts again after a few minutes of riding).  The problem seems to happen more often as the ride progresses.

Any ideas?
```

---
## \#13 Posted by: TarzanHBK Posted at: 2017-04-14T13:47:23.786Z Reads: 88

```
we still don´t have screenshots to help you out..
```

---
## \#14 Posted by: bill_f Posted at: 2017-04-14T15:17:52.576Z Reads: 90

```
Hi.  Here are a few. Stock settings except for what  says (in his video) need changing. Been running these settings for ever. Problem started with same settings. And continue. Ridable but annoying.  thx  <img src="/uploads/db1493/original/3X/a/3/a3bb270647f6ddb5d002a70e6c503c7a1b1bc8f9.png" width="690" height="408"><img src="/uploads/db1493/original/3X/9/b/9b33c0c35f7caf2fda1dae8150cbb6d0560aa2e9.PNG" width="690" height="400"><img src="/uploads/db1493/original/3X/6/3/634892e72ca95a906d8ecff8e3ea78a785366d49.PNG" width="690" height="407">
```

---
## \#15 Posted by: t0m_r1dd1e Posted at: 2017-04-14T15:46:21.284Z Reads: 88

```
[quote="bill_f, post:12, topic:14116"]
with the diyElectricSkateboard VESCs, the arrow keys do not make the motors move while connected to the BLDC tool
[/quote]

Mine from DIY respond to the arrow keys. Super weird. Have you tried swapping VESCs and motors yet to confirm that it's a problem with one of the VESCs?
```

---
## \#16 Posted by: bill_f Posted at: 2017-04-15T08:40:07.805Z Reads: 88

```
I've used an Ollin VESC with the same motor and the arrow keys worked.  With the DiY, it only makes a clicking sound and does not turn the motor. Same version VESCs with same settings on same BLDC tool. Otherwise, the DIY VESCs seem to be working okay (unless they are causing the original issue, but I'm not sure they are or if it's a motor issue). Will swap both motors for two new ones and see what happens.
```

---
## \#17 Posted by: bill_f Posted at: 2017-06-05T07:51:09.488Z Reads: 79

```
So it turns out it was one of the VESCs (diyelectricskateboard). I noticed that on the bad VESC, the LED would not light up when it got a throttle signal from the TX. The good one would light up. On both, the LEDs would blink on boot-up so I knew the LEDS on both were okay.  Not sure what the issue is with the bad VESC. It runs, but does not seem to provide enough power at low rpms. At high rpms, seems okay.  As mentioned above, when connected to BLDC tool, the arrow keys would not control motor--only makes clicking sounds.
Wrote to diyelectricskateboard about repairing VESC (I'd pay) but have gotten no response.
Any ideas on repairing this VESC or any ideas on what might be the issue with it?
I'm now using two Ollin VESCs and it's smooth like butter.
```

---
## \#18 Posted by: Sneaky_Troll Posted at: 2017-11-23T18:26:58.555Z Reads: 59

```
I'm having a similar problem when using the arrow keys. Motor detection works fine, but when I use the arrow keys the motors just click. I don't know why the arrow keys don't work.
My setup is:
10s4p
Dual RSPEC Enersion 190kv motors
VESC-6 boards
Nano-X controller
BLDC mode
I also get cogging and then the motors screech unless I kick off, which didn't happen on the 4.12 boards I used to run. But I hear this is a problem in BLDC mode.
Any advice?
```

---
## \#19 Posted by: bill_f Posted at: 2017-11-23T19:04:28.920Z Reads: 54

```
Never figured it out. Ended up switching my VESCs. Never heard back from  so never got it repaired. Had the Olin VESCs so just switched them out. Ollins are still working great.
```

---
## \#20 Posted by: Lloydd Posted at: 2018-06-27T13:42:01.891Z Reads: 36

```
I was having a very similar issue! Took motor apart and everything was fine, VESC and programming/ everything also fine but my issue started happening after I got a rock stuck in my motor pulley. This made me think it was something mechanical. Turns out my fix was the set screws from the motor body (don’t know correct terminology) that hold the motor body to the inner shaft came loose! Reinstalled with Loctite and good to go! (I know your problem was different just figured this might help others) cheers! 🍻
```

---
## \#21 Posted by: onepunchboard Posted at: 2018-06-29T12:45:57.082Z Reads: 30

```
did you set ppm guys?
and motor detection?
```

---
