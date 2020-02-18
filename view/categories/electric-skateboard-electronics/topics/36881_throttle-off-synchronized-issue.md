# Throttle off synchronized issue

### Replies: 15 Views: 424

## \#1 Posted by: shaohad Posted at: 2017-10-30T15:26:39.657Z Reads: 70

```
Hi guys .
i have an issue with my diy board.
when i press throttle for speed up or brake it seems like the remote control and the receiver do not communicate very good.
i don't get the motion when i press, it might be with slight delay or not even react at all for few moments.
any idea what's the problem or how can i find the problem?

here is my setup:
10S4P samsung 30q battery pack wit intergratd BMS.
maytec 6365 sensored 170kv motor
maytech 2.4ghz remote control
chinese vesc.

thanks in advanced.
```

---
## \#2 Posted by: dg798 Posted at: 2017-10-30T15:33:35.863Z Reads: 67

```
Go to bldc tool and go to app settings-ppm- and at the bottom there’s a checkbox that says display-check it and there’s a green line and percentage.
See what it look like when the throttle is at neutral, it should be at 50-51%
```

---
## \#3 Posted by: dg798 Posted at: 2017-10-30T15:34:26.590Z Reads: 59

```
Then make sure that ppm is enabled **strong text**
```

---
## \#4 Posted by: shaohad Posted at: 2017-10-30T15:45:20.767Z Reads: 50

```
so i have check and PPM is enabled - current no reverse with brake
and the display shows 50-51% at standby , so it ain't it.
any ideas??
```

---
## \#5 Posted by: wafflejock Posted at: 2017-10-30T16:03:13.982Z Reads: 44

```
Does the display/progress bar react quickly and consistently when you're monitoring the VESC connected to the computer?  If you rev the motor and brake while bench testing does it cause the signal to get messed up?  You might consider moving the receiver if you're getting noise when the motor is running or when braking or add a ferrite bead and/or shielding on the signal line so it doesn't get EMI from other electronics.
```

---
## \#6 Posted by: Deckoz Posted at: 2017-10-30T16:03:20.090Z Reads: 41

```
Set your ppm endpoints and center point

-disable control mode SL motor doesn't spin
Hold full throttle, set ppm max (mine is 2.06)
Hold full brake, set ppm min(mine is 1.03)
Let go, read the green bar, set ppm center(mine is 1.55)
Set deadband (mine is 0.07 as .15 is to much deadband)
```

---
## \#7 Posted by: shaohad Posted at: 2017-10-30T16:18:39.889Z Reads: 39

```
yes the bar repose quickly i don't get any delays or mess up with the signal while using bldc tool.
```

---
## \#8 Posted by: wafflejock Posted at: 2017-10-30T16:23:38.863Z Reads: 38

```
Only other thing I can think of really is when my board is under load the power coming off the vesc for the receiver wasn't completely consistent from me (I'm not sure which regulator on the VESC is responsible for that might be the one in the DRV) adding a capacitor on my custom receiver power input seemed to help smooth that out, but really shouldn't be an issue with a prebuilt receiver I don't think.  The nrf chips pull more amps than the arduino can supply so I have a cap on the power going into there and also added a cap on the power/gnd going in the arduino I use for doing the receiver logic/sending out the PWM signals.

---

I guess a simpler thing to check is either hot gluing the pwm connector or soldering those connections to make sure something isn't just shaking loose while riding.
```

---
## \#9 Posted by: shaohad Posted at: 2017-10-30T16:31:41.082Z Reads: 34

```
already done the wires are soldred to the reciver
```

---
## \#10 Posted by: shaohad Posted at: 2017-10-30T16:36:06.357Z Reads: 28

```
i do not understand 
how do you know which number is the correct one
and where do i change the ppm center?
```

---
## \#11 Posted by: Deckoz Posted at: 2017-10-30T16:37:27.873Z Reads: 27

```
Do the steps I posted above.

Ie when you hold full throttle the green bar has a number on the right, set that number to ppm max, repeat for ppm min(full brake), center(no thumb on throttle)
```

---
## \#12 Posted by: wafflejock Posted at: 2017-10-30T16:38:09.182Z Reads: 22

```
Version of the BLDC tool I have only had min and max think center is introduced in later versions.
```

---
## \#13 Posted by: shaohad Posted at: 2017-10-30T17:19:28.645Z Reads: 21

```
don't have center.
but the number shown when not touching the thumb 45%-46% 1.5-1.6
```

---
## \#14 Posted by: Deckoz Posted at: 2017-10-30T17:22:36.396Z Reads: 23

```
Center should be there with the rest of the settings<img src="/uploads/db1493/original/3X/b/f/bf382749e7a8e5711608e0afdb5895a58db3ac6e.jpg" width="281" height="500">
```

---
## \#15 Posted by: wafflejock Posted at: 2017-10-30T18:09:41.336Z Reads: 22

```
Weird I just pulled the latest source and rebuilt and still not seeing it here:

<img src="/uploads/db1493/original/3X/d/4/d453e568150deac837dab377af9729b387245f5b.jpg" width="690" height="360">

Either way though having an offset on the center will mess up the ability for it to idle correctly but shouldn't result in a delayed signal.

---

Latest source of bldc-tool not the vesc_tool just tried that but getting some serial port library errors trying to compile.

---

@shaohad if you have 45% then you want the deadband to be at least .10 maybe .15 is good the deadband in my firmware acts as a percentage so if you want 5% up and down or 10% total to be "dead" not count as input then use .10 if you want 15% (7.5% up and down to not count) then you'd use .15  That said though the deadband just affects how much of the "center" position on the trigger is ignored, in order to get the idle position closer to 50% if you don't have the middle value just top and bottom you can either raise the top one or raise the bottom one to shift the center closer to the correct value for idle.
```

---
