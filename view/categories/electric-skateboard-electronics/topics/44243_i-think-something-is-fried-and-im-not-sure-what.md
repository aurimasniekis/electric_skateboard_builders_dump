# I think something is fried and I&rsquo;m not sure what

### Replies: 10 Views: 525

## \#1 Posted by: DragonSwagin Posted at: 2018-01-21T05:18:35.544Z Reads: 145

```
So back story, I wanted to swap decks that I was using and I had the power button mounted on the deck using JB weld since it wasn't tall enough to use the screw... basically not getting that button back. So I cut the wires under it and ordered a new mechanical button on amazon. 

I have a 12s battery, a power switch, and an OESC all from miami electric. After cutting the wires, I made a bad decision and left everything plugged in (minus the motor). Now the battery is pretty much permanently supplying power to the OESC no matter what. I got the new power button, wired it up, pressed it, depressed it, unplugged the button completely, and in all 3 instances the battery continued supplying power to the OESC. It's like the power switch isn't even there.

So I tried some trouble shooting. I unplugged the battery and plugged it back in (everything goes through XT60 connectors) and there was a mildly loud "pop." 

I unplugged it immediately and took the power switch out of the circuit. I plugged the battery straight into the OESC and the same "pop" happened again. I currently have everything unplugged and am a little afraid to try anything. 

As far as I know, even after the "pop" when things are plugged back in, the OESC functions perfectly normal. 

Any thoughts?
```

---
## \#2 Posted by: b264 Posted at: 2018-01-21T06:30:27.362Z Reads: 130

```
The pop is normal and that's why folks use antispark switches.  The esc has a large capacitor on the supply side -- it's like a reserve reservoir.  When you first plug it in, the ESC's reservoir is empty and fills up instantly -- this is the "spark" or "pop" -- then it is ready to supply spikes of power to the ESC if it can't pull power from the battery fast enough through the length of wire.
```

---
## \#3 Posted by: MysticalDork Posted at: 2018-01-21T07:17:15.056Z Reads: 118

```
Is the "Power switch" actually switching power to the esc? or is it controlling an antispark switch or eswitch on the bms?
```

---
## \#4 Posted by: ThermalM16 Posted at: 2018-01-21T07:23:10.592Z Reads: 115

```
The power switch is turning the anti spark switch on and off. It sounds like your anti spark switch went bad, mine did the same thing not too long ago. When those go bad they get stuck in the on position regardless of what position your physical switch is in. If you’re interested in repairing it, I may be able to help.
```

---
## \#5 Posted by: Acido Posted at: 2018-01-21T08:35:48.246Z Reads: 97

```
Check the ressistance with a multimeter on 3.3v and ground, simmilar thing happened to me, probably your 3.3v converter is fried, plug it in the battery and see if the lights turn on, if not from my experience its that

Probbably its just the switch died,becase they like to
```

---
## \#6 Posted by: DragonSwagin Posted at: 2018-01-21T16:58:01.831Z Reads: 85

```
I took some pictures of the power switch and am interested in repairing it. The only problem is circuits and wiring are pretty foreign to me. Any help is greatly appreciated!

![IMG_8976|666x500](upload://a8v5fLHvYtLaQO725ZV1TbgGSDM.JPG)![IMG_8977|666x500](upload://p0RWdrMdXlJRmguIrKqszvvyXf2.JPG)
```

---
## \#7 Posted by: b264 Posted at: 2018-01-21T23:37:36.268Z Reads: 69

```
I think it's more helpful to think about -- if you repair it, you won't have fixed what caused it to fail, which means it will probably fail again

Is it just not able to handle that much current?
```

---
## \#8 Posted by: DragonSwagin Posted at: 2018-01-22T00:02:36.925Z Reads: 62

```
It should be able to handle the current, as it came bundled with the battery and OESC all from the same place.
```

---
## \#9 Posted by: DragonSwagin Posted at: 2018-01-22T00:35:48.606Z Reads: 54

```
Update! Miami electric is replacing the switch entirely so I don't have to worry about it. Thanks everyone for the help!
```

---
## \#10 Posted by: Eboosted Posted at: 2018-01-22T01:07:18.717Z Reads: 48

```
There are still no reliable antispark switches, just buy an antispark and additional mosfets from mouser, everytime your antispark stays in the closed position just replace the mosfet.
```

---
