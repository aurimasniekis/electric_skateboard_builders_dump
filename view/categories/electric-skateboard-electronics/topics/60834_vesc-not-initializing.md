# VESC not initializing

### Replies: 17 Views: 347

## \#1 Posted by: Dkroes Posted at: 2018-07-03T21:45:20.250Z Reads: 49

```
I have a problem that I've tried to troubleshoot for about a month now, but I simply cannot figure it out. Basically, my VESC doesn't initialize properly... The red light does not blink three times, but the blue one comes on and a dim green one does. When I give throttle to my remote, the green LED lights up making me think there isn't any problem on the control side. I have gotten brand new batteries, and reprogrammed the VESC numerous times, but to no avail. I have also tried a different motor and that doesn't seem to work either. Any suggestions on what I should try? I should also mention that when trying to measure the sensored measurements on my Torque motor, the VESC disconnects.
```

---
## \#2 Posted by: wafflejock Posted at: 2018-07-03T21:51:50.050Z Reads: 47

```
Couple things to check, after the VESC disconnects does it stay booted? are you able to reconnect? if so go into vesc/bldc-tool again and go to the terminal section/tab and type `faults` to see if it is reporting any error.  When you say you reprogrammed the VESC multiple times do you mean you changed values in the tool and wrote config multiple times or that you rewrote the firmware multiple times? (if you haven't tried a firmware flash and faults isn't showing anything probably worth a shot)
```

---
## \#3 Posted by: Dkroes Posted at: 2018-07-03T22:06:29.712Z Reads: 43

```
I have just updated the firmware to the newest. It stays connected still, but what happens now is that I measure the R and L and wavelength, and when I press the button, the green light comes on, but the motor does not spin, nor does it make any sounds for either of the measurements. I typed faults, and nothing came up. I have both rewritten the firmware/updated it, and rewrote my settings on to the VESC.
```

---
## \#4 Posted by: wafflejock Posted at: 2018-07-03T22:20:30.415Z Reads: 36

```
Sounds like you're trying to do detection in FOC mode, would go with BLDC mode detection first to see if that works out since it tends to have less issues for people.  So long as your voltage cut offs are correct and there's nothing stopping the motor from spinning (no belt attached) then BLDC motor detection should work and should spin the motor, give it a shot and let me know how it goes.
```

---
## \#5 Posted by: Dkroes Posted at: 2018-07-03T22:27:20.576Z Reads: 33

```
I just tried BLDC and it didn't work. I still can't get the motor to spin even in BLDC to detect the parameters. The green light goes on when I try, but still no rotation.  In the Debug menu, there is a bad detection received, but I would assume its because the motor doesn't spin.
```

---
## \#6 Posted by: wafflejock Posted at: 2018-07-03T22:34:01.331Z Reads: 31

```
Double check the voltage from the batteries with a voltmeter and make sure the battery cut off start and end (in the vesc config) are lower than your actual voltage, also double check phase wire connections.

If it's none of those things you could try increasing the amperage it uses to do the test spin but I'd start to suspect a defect in the motor at this point.  You should be able to turn the motor easily by hand and should feel more resistance if you short any two of the three phase wires.
```

---
## \#7 Posted by: banjaxxed Posted at: 2018-07-03T22:41:59.015Z Reads: 29

```
Is there any visible damage to the DRV chip?
```

---
## \#8 Posted by: Dkroes Posted at: 2018-07-03T22:44:06.041Z Reads: 27

```
No visible damage to the chip. I've burnt one out before in FOC mode so I keep a close eye on it.
```

---
## \#9 Posted by: Dkroes Posted at: 2018-07-03T22:46:46.633Z Reads: 26

```
I have a custom 10s flat lipo reading at 37v. I have the soft cutoff at 30v and the hard at 28v(low I know).  And still no luck. I cut the connectors off of the phase wires and soldered them directly to eliminate any failure points other than the motor and VESC itself, and that didn't work either.
```

---
## \#10 Posted by: wafflejock Posted at: 2018-07-03T22:52:43.589Z Reads: 24

```
Does the motor turn easily by hand when connected (should feel like small amount of consistent resistance, but shouldn't feel like it is braking at all)? also can you paste the output from the VESC tool terminal after typing `faults` and hitting enter (ideally after trying to run detection to see if it gives us any more hints)
```

---
## \#11 Posted by: Dkroes Posted at: 2018-07-03T23:21:37.541Z Reads: 20

```
The motor does turn easily. I am familiar with how they should feel, and this one feels normal/ a little on the draggy side. The terminal only says: No faults registered since startup.
```

---
## \#12 Posted by: Dkroes Posted at: 2018-07-03T23:22:59.165Z Reads: 22

```
I'm wondering if there is a fault in startup.
```

---
## \#13 Posted by: wafflejock Posted at: 2018-07-03T23:25:42.238Z Reads: 21

```
If you toggle on the real-time data and then open the real-time view does it show the voltage and temp correctly?  I imagine you'd get some error or more weird responses from faults and attempting detection if the vesc was having a startup issue, if the real-time data doesn't work would lean more towards that possibility (or at least an issue with the vesc itself).
```

---
## \#14 Posted by: wafflejock Posted at: 2018-07-03T23:30:01.326Z Reads: 18

```
This thread sounds like similar behavior but strange it doesn't report a drv_fault thought it would do that anytime the stm chip couldn't communicate with the drv chip
https://www.electric-skateboard.builders/t/vesc-does-not-blink-red-and-doesnt-give-speed-but-it-registers-when-you-move-it-by-hand/31073/4
```

---
## \#15 Posted by: Dkroes Posted at: 2018-07-03T23:33:41.470Z Reads: 17

```
The data plots aren't getting any reading. Even when I spin the motor by hand, I can't see any changes, or data for that matter.
```

---
## \#16 Posted by: wafflejock Posted at: 2018-07-03T23:40:54.429Z Reads: 16

```
There's a toggle that turns green if you have real-time data enabled and believe there is one for app (believe right side of the vesc tool) and one for other basically make sure that's toggled on otherwise you won't see any data.  Still from the other thread it doesn't sound great.
```

---
## \#17 Posted by: Dkroes Posted at: 2018-07-03T23:47:53.448Z Reads: 16

```
Yeah might have to get a new one. I just wanted to make sure it wasn't the motor/or wasn't a quick fix. Toggled on the realtime data and everything seems correct to me. When I use the arrow keys, there are big spikes in the data plot, but the motor doesn't move still. I also really appreciate your help so thank you!
```

---
