# VESC 4.12 braking randomly even when applying throttle

### Replies: 17 Views: 664

## \#1 Posted by: Money Posted at: 2018-03-03T02:48:47.458Z Reads: 111

```
Hi eSk8 builders, 

I'm hoping someone can help me with some guidance here. I am experiencing something I have not seen before.

I just put together a new build, and it starts ok, but then it seems to be braking on it's own randomly. Sometimes even when I apply throttle. 

At first, I was also getting remote signal drop outs very frequently, in addition to the random braking. I tried a different nyko kama nunchuck (I've never had any issues with either of these two remotes in the past) but the problem persisted. Then I thought it was a problem with the nunchuck receiver, so I swapped that out. The remote doesn't drop out any more, but the braking still happens randomly, and rather frequently. Everytime it happens, giving it more throttle feels like it increases the braking force, and once the board brakes to a stop, the braking releases and the throttle becomes a throttle again. At least until 30 seconds or so later when it starts braking again.

I thought maybe it was an issue with the VESC, so I swapped it out with a new VESC, but still having the same problems. Both VESC's were configured using the new BLDC tool. They are both 4.12 hardware with the latest firmware (3.34 if I recall correctly).

I dont see how this could be caused by anything other than the remote, receiver or the VESC, and since they have all been replaced and the glitch is still there, I am at a loss on what to do now.
Any help would be greatly appreciated. Is it possible that there is a problem with the latest VESC firmware? I have looked online but have not seen anyone else reporting this. 

Thank you in advance.
```

---
## \#2 Posted by: Exiledd_Top Posted at: 2018-03-03T02:56:18.583Z Reads: 106

```
Post your vesc settings,  it could also be your enclosure if it's made out of carbon fiber known to mess with signal.
```

---
## \#3 Posted by: ZackoryCramer Posted at: 2018-03-03T03:24:47.787Z Reads: 100

```
Are you sure they are charged? I had random ppm signals kicking in with my old transmitters until I realized they were under charged. :jack_o_lantern:
```

---
## \#4 Posted by: E1Allen Posted at: 2018-03-03T03:46:43.227Z Reads: 95

```
Any metal to metal exposed on your motor phase wires? If so bumps could cause braking
```

---
## \#5 Posted by: pennyboard Posted at: 2018-03-03T04:36:53.500Z Reads: 90

```
I second this. I had this issue a while back and tore my board apart trying to figure out what it was only to realize that the remote just needed to be charged :joy:
```

---
## \#6 Posted by: Money Posted at: 2018-03-05T08:26:06.418Z Reads: 62

```
Thank you everybody for your input. 

I took some screen caps of the settings in the VESC tool. They are mostly all default settings. I didnt change anything other than running motor detection and setting it up for Nyko Kama nunchuk control.

But now I'm having a new problem. The board was being completely unresponsive to the nunchuk. When I press the bind button on the nunchuk the red light next to it comes on solid showing it is connected. But the board does nothing in response to any input. I tried re-configuring everything (motor setup and app setup), and then tested to see if the keyboard controls worked. They work fine. So then I disconnected the VESC, shut it down and then powered it back on. This time I was able to get the motor to spin up using the nunchuk, but then 30 seconds later it stopped. I reconnected it to my computer and checked for faults and it says there are none.

I'll post screen caps of my settings in just a moment.

Some of you suggested that it was likely the remote not being charged. Or blocked or weak signal. I have replaced the batteries twice in both nunchuks that I have tried. And the enclosure is plastic, and the deck is maple. And when bench testing I have the remote within a foot from the receiver, with literally nothing in between the two.

And the phase wires are well insulated with no cuts in the insulation and no metal exposed or contacting. 

Seeing as how I have swapped out each electrical component (VESC, Nyko Kama remote, Nyko Kama receiver) one at a time and tested each time in between and the issue still remains, I am thinking it is probably something with the settings or software configuration. 

Two days ago I tried configuring it for BLDC and not FOC, and the random braking still occurred. (I also was reminded how loud BLDC mode is. Yikes.) Now it's set back at FOC. 

I'll upload my screen caps in just a few minutes.

Thank you so much to anyone/everyone that is reading this. All input and suggestions are welcomed. I really appreciate the help.
```

---
## \#7 Posted by: Exiledd_Top Posted at: 2018-03-05T08:30:27.802Z Reads: 52

```
Define tested because my focbox were only being held by shrink  tubing as soon as I took that out they came right off. Just because u can't pull it off with the tubing doesn't mean it's a good solder.
```

---
## \#8 Posted by: snorren Posted at: 2018-03-05T08:36:13.602Z Reads: 51

```
Does it happen "always", like running it on the bench with no load?
Are the signal cables shielded from Electromagnetic interference?
```

---
## \#9 Posted by: snorren Posted at: 2018-03-05T08:38:26.995Z Reads: 52

```
I'm thinking perhaps the motor is inducing interference in receiver cables or in hall sensor cables (if you're using it) causing the motor to "correct" for thinking it's out of phase.
```

---
## \#10 Posted by: Money Posted at: 2018-03-05T08:49:35.816Z Reads: 51

```
I'm not sure which component you are referring. The receiver? That's the only part that required soldering. 

When I soldered the new leads onto the Nyko receiver, I thread the wire through the holes. As opposed to just being soldered to the pad.
```

---
## \#11 Posted by: Exiledd_Top Posted at: 2018-03-05T08:50:39.048Z Reads: 50

```
I was trying to say maybe a loose solder
```

---
## \#12 Posted by: Money Posted at: 2018-03-05T08:55:19.063Z Reads: 50

```
When the board was at least being responsive to the nunchuk, I did not notice it braking when testing on the bench with no load. Only when I went out side and tried riding it. It was fine for the first 20-30 seconds, and then i felt it gradually increasing the brake. Eventually it would release and i would get another 20-30 seconds before it would happen again. 

The receiver wires are not shielded from EM interference. I have some copper sheeting that I can try using to shield them. 

The motor I'm using is not sensored. And it doesn't feel like it's just out of phase because the braking is fairly smooth and gradual. And it occurs even when the throttle is in neutral.
```

---
## \#13 Posted by: Money Posted at: 2018-03-05T08:56:51.312Z Reads: 46

```
Gotcha, thanks. But the solder connections on the receiver are all solid.
```

---
## \#14 Posted by: snorren Posted at: 2018-03-05T09:04:07.851Z Reads: 46

```
Ok the problem didn't occur under no load (bench) when the current and therefor EI was very low.
It could also be EI caused by low current but at high frequency (motor at high rpm).

I would test:
Run your vesc from just a 5v signal/pwm to remove one error source.
Wrap this signal cable + vesc in aluminum foil. 
Twist the power cables to the motor.

It's just a guess but at least it excludes some error sources.
```

---
## \#15 Posted by: Money Posted at: 2018-03-05T09:23:17.404Z Reads: 43

```
Thanks for the suggestions. I will try these out.

To be clear, what do you mean by "Run your vesc from just a 5v signal/pwm"

Are you saying to try using a 5v receiver? Like a hobby receiver on the 3 pins on the vesc?
```

---
## \#16 Posted by: snorren Posted at: 2018-03-05T12:00:59.061Z Reads: 41

```
Aha sorry that was a bit unclear. What i mean if you have any testing pwm signal, I usually use Arduino to control/test things on the bench and only connect the remote once everything is working.
```

---
## \#17 Posted by: Money Posted at: 2018-03-11T22:34:30.748Z Reads: 26

```
I reloaded all default settings, again, in vesc tool. Then configured everything like before and viola, it works perfectly now. 

Thanks everybody for your suggestions!
```

---
