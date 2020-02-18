# Losing Eboard control, 2.4ghz mini controller not responding correctly

### Replies: 29 Views: 1748

## \#1 Posted by: Tampaesk8er Posted at: 2017-07-06T21:40:49.127Z Reads: 102

```
 2 VERY DANGEROUS ISSUES! When I squeeze trigger, the motor starts rolling upto full speed, and when squeezed to the max, the motor dies out. WHEN I SHUTT CONTROLLER POWER OFF, THE MOTOR STARTS GOING FULL SPEED, VERY DANGEROUS if still standing on Eboard. PLEASE HELP, DONT KNOW WHATS CAUSING THIS. I tried rebinding controller, but that didnt work.
```

---
## \#2 Posted by: wafflejock Posted at: 2017-07-06T21:41:58.243Z Reads: 104

```
What kind of ESC are you using... have you configured it?
```

---
## \#3 Posted by: psychotiller Posted at: 2017-07-06T21:45:16.885Z Reads: 103

```
Are you using a boat, helecopter or airplane esc? Other issue is your failsafe needs to be set to coast.
```

---
## \#4 Posted by: Tampaesk8er Posted at: 2017-07-06T22:00:50.869Z Reads: 97

```
A vesc, here are my vesc and bldc tool settings.

<img src="/uploads/db1493/original/3X/c/0/c0c79099f2aa598a51d944b6f61a1f0537da55d5.JPG" width="669" height="499"><img src="/uploads/db1493/original/3X/4/2/42c2d049dcf8c1057654858f39e488570123cf11.JPG" width="669" height="499"><img src="/uploads/db1493/original/3X/5/0/508bdc959dc2ebfd2578a259a5b62595833297b0.JPG" width="669" height="499">
```

---
## \#5 Posted by: Tampaesk8er Posted at: 2017-07-06T22:03:35.839Z Reads: 87

```
vesc is 4.12 running 2.18 firmware
```

---
## \#6 Posted by: wafflejock Posted at: 2017-07-06T22:11:47.627Z Reads: 86

```
Watch the display as you pull the throttle up to full or as you disconnect the controller and see what pulse width it's actually reading in those scenarios can see if it's the controller/receiver not doing the right thing in the display, if it's the VESC doing something weird it will behave how you want in terms of the display (only go up when you pull the trigger, go to idle when you disconnect).

---

You can set the control to disabled while you're testing the input to avoid revving the motor all over too.
```

---
## \#7 Posted by: Tampaesk8er Posted at: 2017-07-06T22:20:08.194Z Reads: 79

```
When controller disabled, the pulsewidth goes to 2.0 at full squeezed trigger, heres pics, enlarge pics so you can see settings
<img src="/uploads/db1493/original/3X/1/2/1246e296447c409dca4ea09b94ed20f797b23375.JPG" width="669" height="499"><img src="/uploads/db1493/original/3X/e/9/e904b3ce357de359d0424e1dd8482344562bbad2.JPG" width="669" height="499">
```

---
## \#8 Posted by: Tampaesk8er Posted at: 2017-07-06T22:21:03.339Z Reads: 74

```
How do I set failsafe to coast?
```

---
## \#9 Posted by: Jinra Posted at: 2017-07-06T22:21:13.595Z Reads: 72

```
Uh why is your eRPM limit start/end 1.75/2.00? It's asking for eRPM not pulsewidth signal.
```

---
## \#10 Posted by: wafflejock Posted at: 2017-07-06T22:27:05.114Z Reads: 79

```
The time out in the app configuration should make it go idle in 1 second (1000ms) if no signal for control is received.  So it seems the receiver is sending something but the wrong thing or there's some other error in the config possible the erpm values but don't think I have that limit enabled (I have a pretty low kv motor so didn't mess with that)
```

---
## \#11 Posted by: Tampaesk8er Posted at: 2017-07-06T22:35:22.815Z Reads: 76

```
@Jinra ah, ha, didnt noticed that, i input 0.00 to both, controller stopped acting crazy when i shutt it off now. Thank you,

How do i set the failsafe to coast?
```

---
## \#12 Posted by: Jinra Posted at: 2017-07-06T22:36:55.387Z Reads: 73

```
I'm not sure 0 is a good value either. I would uncheck the option if you dont need it or dont know what it does.
```

---
## \#13 Posted by: wafflejock Posted at: 2017-07-06T22:37:39.799Z Reads: 68

```
See my response above, looks like you already have it set, can test by throttling up a small amount and disconnecting. It should coast to a stop.  The failsafe on the VESC side should be good, but make sure your receiver doesn't have some other failsafe config for if it loses connection to the transmitter for whatever reason and you should be fine.
```

---
## \#14 Posted by: Tampaesk8er Posted at: 2017-07-06T22:38:56.648Z Reads: 62

```
This is my sons eboard, a little scared he gonna get hurt. I'll ask psycotiller, thank you for catching that for me.
```

---
## \#15 Posted by: Tampaesk8er Posted at: 2017-07-06T22:40:50.079Z Reads: 63

```
Ok, i fixed the values to 0.00 in the soft erpm limits, thats one issue fix, how do i set failsafe to coast? thank you for your help.
```

---
## \#16 Posted by: darkkevind Posted at: 2017-07-06T22:42:33.903Z Reads: 62

```
Sounds like the parameters aren't set up correctly and you don't have a big enough dead zone.

Squeeze the trigger in 'disabled' mode and note the value in the display box, place that value in the max field. Put on full brakes and note that value, put that in the min field, then try it out. If it's still cutting out and/or running when back in the middle then increase the dead zone.
```

---
## \#17 Posted by: Tampaesk8er Posted at: 2017-07-06T22:44:52.906Z Reads: 59

```
OH, it turns out that when I walked away before, my son accidently hit the keyboard from my computer while it was connected to bldc tool, it probably changed settings by accident when he picked it up from floor and he says he pushed some buttons when picking it up from floor, SMH.
```

---
## \#18 Posted by: Tampaesk8er Posted at: 2017-07-06T23:01:59.131Z Reads: 58

```
its not cutting out nomore, soft ERPM values were wrong, i changed them to 0.00. How can i set fail safe to coast?
```

---
## \#19 Posted by: Tampaesk8er Posted at: 2017-07-06T23:10:25.877Z Reads: 54

```
Yea, i know that part, how can i setup failsafe to coast?
```

---
## \#20 Posted by: Tampaesk8er Posted at: 2017-07-06T23:11:36.398Z Reads: 58

```
its working now, but, how do i setup failsafe to coast?
```

---
## \#21 Posted by: psychotiller Posted at: 2017-07-06T23:14:19.693Z Reads: 53

```
Ok. What you need to do is put the bind plug in your receiver. Then turn on your board, then turn on your remote while pushing the bind button. When the light goes solid you are bound.  Then rev up your board. While it is coasting to a stop, pull the bind plug. Now just turn everything off and then back on.

To test, throttle up your board and turn off your remote at the same time. If you're board coasts your good
```

---
## \#22 Posted by: Tampaesk8er Posted at: 2017-07-06T23:17:34.690Z Reads: 55

```
ok, i'll try it, thank you.
```

---
## \#23 Posted by: Montiey Posted at: 2017-07-06T23:22:46.867Z Reads: 59

```
There are 3 kinds of failsafe: Through the VESC, the RX, and one that you really, really don't want. You need to figure out how the receiver responds when the TX disconnects. 

If the RX goes into it's own failsafe, you cannot configure a failsafe on the VESC, but rather you depend on what PPM value the RX outputs when the TX disconnects. This should the same value output when the motor is at an idle.

Now, if the RX doesn't have fallback, it can do one of two things: Hold the current value indefinitely, or stop outputting a value. The former can be disastrous. Do _NOT_ use an RX that holds the value. This will leave you full-throttle down the road with no control. Too many people get hurt due to controller failsafe malfunctions. 

However, some receivers will just cut their output. In this case, it's up to the VESC to detect the 'no signal' state on the PPM line and engage the failsafe state (set the motor to idle).
```

---
## \#24 Posted by: Tampaesk8er Posted at: 2017-07-06T23:27:27.446Z Reads: 56

```
I currently have ppm settings on (current, no reverse with brake), when i letgo the trigger on remote, it doesnt coast, the motor just stops sudenly, how can i make it coast?
```

---
## \#25 Posted by: psychotiller Posted at: 2017-07-07T00:42:27.160Z Reads: 54

```
How tight are your belts? Does it stop because of tension? or brakes?
```

---
## \#26 Posted by: psychotiller Posted at: 2017-07-07T00:44:20.065Z Reads: 55

```
Also, Did you turn off your remote to see what happens when your board loses signal?
```

---
## \#27 Posted by: Montiey Posted at: 2017-07-10T23:59:32.102Z Reads: 47

```
The VESC *should* idle if the RX signal is at 1500µs. (assuming that your endpoints are 1000 and 2000)

When released, the remote's signal value in BLDCTool should be: 
(upper+lower) / 2
You should tweak the endpoints to make sure that the center falls on this value, or tweak the deadband if all else fails.

Next, try [THIS](http://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286) custom fork of the VESC firmware and its matching BLDC tool version. I say this because you can individually adjust the two endpoints, _and_ the center. Then you can make sure that your remote is working properly. Especially if you do any modding, like the SPARKLE mod, or replacing any potentiometers, you'll need to use really weird PPM settings where the center is not necessarily proportional.
```

---
## \#28 Posted by: Montiey Posted at: 2017-07-31T13:01:28.699Z Reads: 33

```
@Tampaesk8er, could you describe your new problem a bit further? Is it possible you simply bumped the trim pots on the GT2B?
```

---
## \#29 Posted by: Tampaesk8er Posted at: 2017-07-31T20:48:31.310Z Reads: 26

```
I just resetted the vesc by reinstalling the firmware and everything is working properly. I use the 2.4ghz mini controller, not the GT2B.
```

---
