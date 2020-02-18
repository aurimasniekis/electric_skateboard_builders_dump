# \[SOLVED\] Getting FULL Brakes when trigger is released

### Replies: 16 Views: 807

## \#1 Posted by: Mikenopolis Posted at: 2017-03-25T11:07:50.597Z Reads: 117

```
I just replaced one and repaired one Enertion 6355 motor on a Raptor. Bench test was fine using a Winning remote, wheels turned and SLOWED to a stop when I released the "trigger" and halt to a stop when I pulled it back.....the next step was replacing the reciever and remote to the Nano-X. It paired fast and easy, BUT now  when I let go of the trigger it brakes immediately. ALSO the second the board is turned on the brakes are on. What did I miss in BLDC?
```

---
## \#2 Posted by: lowGuido Posted at: 2017-03-25T14:28:47.618Z Reads: 109

```
have you changed the PWM settings?
```

---
## \#3 Posted by: PXSS Posted at: 2017-03-25T15:08:12.470Z Reads: 100

```
You need to calibrate your remote
```

---
## \#4 Posted by: Mikenopolis Posted at: 2017-03-27T06:24:10.415Z Reads: 73

```
I'm not sure if I'm doing something wrong. the remote binds with the receiver and I can control the motors. Within BLDC tools I DISABLED the Control Mode and clicked write, rebooted and read....it shows the disabled, but the remote would still work.
```

---
## \#5 Posted by: laurnts Posted at: 2017-03-27T06:31:17.948Z Reads: 68

```
Seems to me and others this is configuration issue within the esc or the vesc.
```

---
## \#6 Posted by: Mikenopolis Posted at: 2017-03-27T06:32:51.733Z Reads: 64

```
what does that mean? I have a faulty vesc?
```

---
## \#7 Posted by: laurnts Posted at: 2017-03-27T06:36:41.563Z Reads: 66

```
No. Like others said you need to configure your vesc pwm setting. You might need to recalibrate your remote.
```

---
## \#8 Posted by: Mikenopolis Posted at: 2017-03-27T06:48:49.019Z Reads: 64

```
I did everything Jacob's video showed and I still have the same issue. I did the same thing for my other board and it works....can this be a Nano-X problem?

https://www.youtube.com/watch?v=PVx72c7Ya3s
```

---
## \#9 Posted by: Mikenopolis Posted at: 2017-03-27T07:52:49.846Z Reads: 57

```
Also, BLDC doesn't display the pulse rate so there's nothing to adjust
```

---
## \#10 Posted by: JLabs Posted at: 2017-03-27T16:46:33.195Z Reads: 51

```
[quote="Mikenopolis, post:9, topic:19654, full:true"]
Also, BLDC doesn't display the pulse rate so there's nothing to adjust
[/quote]

It should, make sure you check the box that says show pulse (or something like that). @Ackmaniac's software actually has a wizard for setting it up.
```

---
## \#11 Posted by: Mikenopolis Posted at: 2017-03-27T17:01:46.259Z Reads: 48

```
[quote="JLabs, post:10, topic:19654"]
ake sure you check the box that sa
[/quote]

Yeah, I clicked the DISPLAY box. but nothing shows up. I clicked the disable button, wrote to vesc, rebooted then reconnected, but the remote still works. I'll pair the vesc back to a winning remote and see it it changes anything. I have a feeling the Nano-x is my problem right now
```

---
## \#12 Posted by: boards Posted at: 2017-03-27T23:55:23.169Z Reads: 40

```
plugged into wrong vesc?
```

---
## \#13 Posted by: Mikenopolis Posted at: 2017-03-28T05:13:01.830Z Reads: 42

```
this evening's finding...I clicked on [START DETECTION] and only one motor (the one connected to the VESC my usb cable is connected into). ****EDIT**** found out this is normal as each vesc needed to be programmed individually.


@boards I'm connected the VESC that seems most obvious. They are glued into the case by Enertion (Raptor) and the other VESC's usb port is not accessible without cutting the glue
```

---
## \#14 Posted by: Mikenopolis Posted at: 2017-03-28T05:31:35.392Z Reads: 41

```
@boards well well well. it looks like I was connected to the wrong VESC afterall....which begs the question of why the hell whould Enertion make the correct VESC to connect to so hard to get to?!? 

I now was able to see the pulsewidth move up and down, BUT after entering the min and max, rebooting the VESC and re-enabling to "Current no reverse with brake" the remote no longer responds. ******EDIT****got it working FINALLY, but still not sure what order and how. I unchecked the [Send status over CAN] on both VESCs rebooted and rechecked each one and suddenly it worked.

totally trial and error.
```

---
## \#15 Posted by: Michaelinvegas Posted at: 2017-03-28T07:04:42.934Z Reads: 34

```
Maddening 

........
```

---
## \#16 Posted by: Mikenopolis Posted at: 2017-03-28T17:19:11.892Z Reads: 25

```
rode two miles on it this morning. running perfectly and didn't street my face. Nano-X's beginner mode made the Raptor easy to ride for slow test, but the brakes seems really hard compared to when it's in normal mode.

So what I probably did wrong was a combination of these things on a dual setup:

- Did not do BLDC setting on the "other" VESC assuming that if Enertion hot glued the vesc close to the point where you can't plug in a usb cable it much not been necessary. I literally cut all the rubber from a usb cable so I can plug it in. Having to program each vesc individually was new to me. I thought that was what the send status over can was for?

- Reenter the remote controller IDs on each VESC to 0 and 1

- Mirror all settings on both VESC 

- un-select and re-select "Send status over CAN"

- lots of cursing at myself

Side Note:I really like the even torque on dual 6355s compared to my single 6374 first build, I can't imagine the Raptor 2 being better, like how is that even possible?
```

---
