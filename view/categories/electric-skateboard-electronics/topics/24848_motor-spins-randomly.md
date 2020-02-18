# Motor spins randomly!?

### Replies: 6 Views: 595

## \#1 Posted by: bartroosen12 Posted at: 2017-06-07T22:10:56.479Z Reads: 89

```
Hi, I have tested every part before starting making my esk8.
But today I was just testing if everything was still fine and nowp, I really don't understand why :frowning:
I connected everything right and the motor ''beeps'' are sounding very late, and after that, the motor does super random spins.
I'm even not touching the trigger and he's accelerating, braking starting again just so weird...

Everyone else who had this problem before?

The ESC is a FVT 120A and I'm using a 6S pack with an SK3-236kV.

Here's a video of the weird things.
https://www.youtube.com/watch?v=oQ3TlzCuSNQ&t
```

---
## \#2 Posted by: laurnts Posted at: 2017-06-08T11:51:50.038Z Reads: 66

```
recalibrate remote. it could also be that the remote runs out of battery. if those two ruled out, use the ESC programmer to recheck everything.
```

---
## \#3 Posted by: Montiey Posted at: 2017-06-08T12:22:06.564Z Reads: 58

```
First, make sure the remote has full batteries. Also, make sure that your failsafe is calibrated. From what it looks like, it's set to mid-throttle or something, and so when the remote disconnects, it spins up. Turn on the board with the remote @ neutral, and wait for the ESC to sound. Maybe read the manual for other programming features.

Also, check your wiring. Try to solder all your connections- your PPM link is critical. You don't want it rattling around and sending false pulses to the ESC, making it go crazy.
```

---
## \#4 Posted by: SilentException Posted at: 2017-06-08T12:33:19.577Z Reads: 53

```
PPM receivers are sensitive. Use short wires to ESC, try not to use wire length that are multiplier of 1/4 of 2.4Ghz wave length as they could act as antenna. Check the connections and/or soldering. Lastly, do a few wraps of wire from RX to ESC over the ferrite core. Best of luck! :)
```

---
## \#5 Posted by: bartroosen12 Posted at: 2017-06-08T16:16:43.945Z Reads: 48

```
Firstly I switched to some new batteries from the remote, so they're fully charged right now.
I have the manual for the receiver and it's connected succesfully with the binding/pair steps.

Secondly I tried to calibrate the full throttle and brakes so I found a manual about that but that won't work, the esc shows a red LED and I can't preceed the proces like mentioned in the manual.

Also if I power on the board, normaly the motor beeps a few times to let you know everything is fine but he does nothing...
I have another ''big'' and older remote from an rc car and I plugged in that receiver and it works so I'm happy that the problem isn't the esc.

Have you ever calibrated this remote before(also the failsafe function)? Because I really don't know where to find or how to do it :D
```

---
## \#6 Posted by: bartroosen12 Posted at: 2017-06-10T18:17:22.258Z Reads: 29

```
Problem solved!
I don't understand I could be so stupid.
The wires to the receiver were plugged in the wrong direction...
But the blue receiver LED was also flashing so I thought there was no problem :smiley:
```

---
