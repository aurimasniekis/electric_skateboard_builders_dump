# Please help! Vesc incorrectly reading voltage as 4-5v most of the time?!?!

### Replies: 9 Views: 293

## \#1 Posted by: BringDaRuckus Posted at: 2018-10-16T14:06:48.212Z Reads: 68

```
hello all,

I am using a hobbyking VESC in my build and it is showing some very erratic behavior. 95% of the time  the motor will not spin at all or is super weak. In the realtime data tab of the tool the VESC is showing as receiving the incorrect voltage so I get the UNDER_VOLTAGE fault.

at the moment it shows 4 volts (but its a full 6s pack which shows 24.6v on the voltmeter) so there is no spin at all. sometimes it shows 14 or 15 volts and i get a very weak spin, and very rarely, it shows the correct voltage and spins beautifully as it should. unfortunately the last case only occurs about once for every 50 times i plug it in!!!

does anyone have any suggestions as to why it only works 5% of the time and 95% of the time it just shows completely wrong voltage and faults out?

once it  was working fine, I go for a ride and it kept cutting off, then resuming 2 or 3 seconds later even.

ANY help/suggestions/known faults with the ESC and so on would be very greatly appreciated.
I've tried rebooting, reflashing etc and this silly VESC just will not read the voltage correctly.

Many Thanks for your suggestions.
```

---
## \#2 Posted by: Benjamin899 Posted at: 2018-10-16T14:11:05.455Z Reads: 64

```
get a refund from hobbyking. if your voltmeter is showing the true voltage but the vesc doesn't, then i guess the vesc is damaged.
```

---
## \#3 Posted by: BringDaRuckus Posted at: 2018-10-16T14:13:36.954Z Reads: 62

```
Sadly its not an option. it was received as a present and I have moved countries. Whats really confusing me is that sometimes its working, then if i unplug i t and re-plug it its wrong again. I do think you are right but was wondering if i am missing something obvious. Thanks for the quick response though!
```

---
## \#4 Posted by: Benjamin899 Posted at: 2018-10-16T14:33:31.625Z Reads: 54

```
well if that is the case, then maybe trying to find a repair service is feasible. if you have easy access to it, maybe put up some pictures and a more expierenced member can spot a problem on the pcb/components.
But make good ones.
```

---
## \#5 Posted by: BringDaRuckus Posted at: 2018-10-16T14:42:31.917Z Reads: 49

```
will do, thank you sir!!!
```

---
## \#6 Posted by: mynamesmatt Posted at: 2018-10-16T21:04:11.138Z Reads: 43

```
@JohnnyMeduse 
@Martinsp
would you guys maybe know what's up?
```

---
## \#7 Posted by: BringDaRuckus Posted at: 2018-10-27T20:13:34.432Z Reads: 32

```
hello again ladies and gents.

so I got my hands on another vesc and the issue went away and the board is running great. however, I have this duff VESC in my hands and I figure its worth trying to fix it rather than let it collect dust. so one close inspection following your advice above, I went over it with a magnifying glass and spotted two capacitors (I believe c44 and c49) are looking a little wonky and the solder looks like it has bridged them. I have tried capturing this in the pics attached - they are the ones at the centre of first photo right under the ground wire. they are clearly not supposed to be bridged but just wondering if someone can tell me, does it at least make sense that this bridge explains the behaviour I described above? (sorry for shoddy photography, but I dont want to take the shiny wrapper etc off unless this could truly be the cause before I destroy it any further!)

thanks for any responses.

![thumbnail_20181027_154311|690x388](upload://27wuVks093KHG6X64ibbMWIyBuC.jpeg) ![thumbnail_20181027_155225|281x500](upload://vCf9VDQkQCBl84ordGVLgA9c25e.jpeg) ![thumbnail_20181027_154344|690x388](upload://6g7E14aPYhxsrvsMKOXxy7jxtYe.jpeg)
```

---
## \#8 Posted by: Martinsp Posted at: 2018-11-21T18:35:23.892Z Reads: 27

```
Hi,

hope it is not too late, I have just gotten around to following up pretty much everything I was tagged in :D 
The capacitors are connected on PCB anyway, so that is not a problem. 

Did you try flashing a new (or the same) firmware? Id suggest 2.54 on 4.12 VESC worked well every time for me.
If that does not help you could measure the voltage divider if the values of the resistors are not wrong.
 
Not sure how much you trust yourself not shorting something out but you could measure the voltage in the voltage divider to see if the readout of the voltage is incorrect  or if the actual voltage divider is at fault.

It could also be an issue with the MCUs ADC which would be only solvable by replacing it...
```

---
## \#9 Posted by: BringDaRuckus Posted at: 2018-11-23T22:16:54.547Z Reads: 19

```
Thanks for the advice. I did get my hands on another vesc so I am up and running but this one may have to go to a repair service as your suggestions are beyond my skill level.
```

---
