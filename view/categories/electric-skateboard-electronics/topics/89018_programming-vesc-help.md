# Programming Vesc help!

### Replies: 8 Views: 162

## \#1 Posted by: WoahColors Posted at: 2019-04-01T20:42:30.032Z Reads: 50

```
Hey guys!

I recently built my very first electric longboard (parts list below), and after taking it out for a test run I had some performance issues I'd like ask for some help on!

Parts list (the important stuff):
2x 6374 motors from Flipsky.
2x Fsesc 6.6 based on Vesc 6.6 Flipsky.
12S4P battery pack from TorqueBoards.

The main issue I had with the board was that it seemed like the top speed of the board dropped significantly when the battery reached around 75%.
As far as I can tell the board was performing fine at 100% battery but I never really used the full throttle, however as I said earlier when the battery was at 75% I was using full throttle to barely even keep up with my friend on a boosted board using around half...

I'm under the assumption all my hardware is working fine and I wanted to ask what would the ideal programming be for this setup?

The settings I input originally was 75A max motor current, 30A max battery current (Torque boards live chat told me 60A but I don't believe that's safe for 2x vescs).

I feel like the problem might be in my voltage settings, I currently have the cutoff at like 44.7 volts which I know is much too high considering you can safely discharge until ~35 volts or so but would this actually have caused the performance problem?

I'm also not convinced that's the end of the story because on pure intuition seeing the motors spin (no load) with my current settings even at 100% battery it doesn't look like the ~30 mph estimate that the esk8 speed calculator suggests I should have.

Any help would be great! I've read all over the forums about voltage settings and ERPM and such and just want to see some direct answers to my problem before I re-assemble the board, Thanks!
```

---
## \#2 Posted by: Benjamin899 Posted at: 2019-04-01T21:13:28.462Z Reads: 43

```
The Cutoff is way to high, you are above Nominal Voltage for a Li-Ion, which 3.6v. So yes, when you are at 75% you are basicly already at your cutoff and the vesc starts to slow you down, as programmed.
The speed is also dependent on your wheel diameter and gearing.
Also what type of Cells are build into the Battery?
```

---
## \#3 Posted by: goldrabe Posted at: 2019-04-01T21:20:09.715Z Reads: 39

```
Try battery cut off start 41V and cut off end 37V and look if the board performs better.
You don´t want to discharge your cells lower then 3.1V multiply this times 12 gives you 37.2V. To not have a abrupt shut off put 3-4V on top of that for your soft cut off eg.41V
```

---
## \#4 Posted by: WoahColors Posted at: 2019-04-01T21:33:44.919Z Reads: 33

```
Hey thanks for the quick reply!
I'll definitely try changing the cut off voltage, to answer your questions TB uses the samsung 30Q cells in their packs, and the gearing/wheels is 16T to 36T on orangatang caguama 85mm wheels.
```

---
## \#5 Posted by: WoahColors Posted at: 2019-04-01T21:34:27.578Z Reads: 30

```
Thanks I'll definitely try that!
Any chance you could explain to me a bit better what the cutoff actually does?
```

---
## \#6 Posted by: Benjamin899 Posted at: 2019-04-01T21:47:55.161Z Reads: 27

```
it stops the vesc from pulling amps from the battery, you have a soft and hardcut off.
```

---
## \#7 Posted by: goldrabe Posted at: 2019-04-01T21:48:48.833Z Reads: 28

```
The cutoff prevents you from overdischarging your battery. Usually BMS´s will shut down your pack when reaching 2.8V per cell.
To prevent a sudden shut down, which could throw you off, you set the cutoff values. This settings are taking also Voltage Sag in to account. Under load (acceleration, hillclimb) your batterys Voltage will drop by 1-2V or even more, to prevent a sudden shut down, your ESC will lower the Amps fed to the motors and slow you down until you reach the final cutoff value.
```

---
## \#8 Posted by: WoahColors Posted at: 2019-04-01T21:58:26.459Z Reads: 25

```
Thanks guys!
I'll definitely change the cutoff settings asap and see if that changes anything.
Still, have my doubts about the 30mph estimated top speed, but won't know without testing haha!

I know it's unrelated to this topic but would you happen to know why it seems at about half throttle to 100% throttle there seems to be no change in the motor rpms? I have it set on current no reverse brake, I checked the ppm throttle graph and setup the remote correctly. If anything I'll just be extremely gentle on the throttle!
```

---
