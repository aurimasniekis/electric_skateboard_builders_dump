# Soldering vedders antispark switch

### Replies: 21 Views: 1615

## \#1 Posted by: brandon Posted at: 2016-12-21T22:16:23.408Z Reads: 157

```
I'm pretty sure I fried the fets while soldering them on. I get 12v on the output side not matter if the switch is turned on or off. I've checked for solder bridges but I can't find any. I'm getting continuity between the 5 ground legs of each get and the single gate leg, which I'm fairly sure is bad and means I broke them. If anyone has any suggestions for things to check im open to them.

Otherwise I guess I'll just order some more fets. Any recommendations on soldering them without burning them up?
```

---
## \#2 Posted by: IDVert3X Posted at: 2016-12-21T22:35:34.129Z Reads: 154

```
Do it quickly with high power soldering iron.
Use bigger tips with high thermal capacity.
```

---
## \#3 Posted by: mccloed Posted at: 2016-12-21T22:35:56.163Z Reads: 155

```
I have had good luck soldering these and I'm not very careful. Have yet to burn out one of the mosfets. Are you putting 12v through it, or is it a higher voltage?
```

---
## \#4 Posted by: brandon Posted at: 2016-12-21T22:41:03.089Z Reads: 140

```
I've tried 12 and 24, always get out what I put in. I thought maybe if missed a solder bridge, my fuse popped the first time I plugged it in.
```

---
## \#5 Posted by: mccloed Posted at: 2016-12-21T22:44:43.246Z Reads: 132

```
Yup. Sounds like the mosfets failed. :cry:
```

---
## \#6 Posted by: brandon Posted at: 2016-12-21T23:00:24.100Z Reads: 129

```
Any idea why the fuse might have popped?
```

---
## \#7 Posted by: lox897 Posted at: 2016-12-22T01:06:29.785Z Reads: 114

```
Could you please send some pictures?
```

---
## \#8 Posted by: brandon Posted at: 2016-12-22T17:49:35.270Z Reads: 98

```
If there's anything you'd like a better shot of, let me know. I don't think there's much to see though. Soldered together the ground pins on the fets but there is definitely no bridge to the control pin.

<img src="/uploads/db1493/original/3X/8/b/8b5efc161bdcef72f62bd04d7b220372fc6bc408.jpg" width="281" height="500"><img src="/uploads/db1493/original/3X/f/d/fd4888687a696cadbbaee0b579efc3971b13d3cb.jpg" width="690" height="388">
```

---
## \#9 Posted by: lox897 Posted at: 2016-12-22T20:28:55.585Z Reads: 87

```
And you got the polarity of the 12v zener diode right?
```

---
## \#10 Posted by: chaka Posted at: 2016-12-22T21:13:15.359Z Reads: 83

```
You have a small bridge on the gate pin.  That MOSFET is probably dead or will fail soon after some use.

Do you know what type of toggel switch that is?

<img src="/uploads/db1493/original/3X/a/d/ad33245fa99a1f0a7ed65d5469021d865ba60b45.png" width="690" height="388">
```

---
## \#11 Posted by: brandon Posted at: 2016-12-22T21:17:59.195Z Reads: 84

```
I noticed that, just the light reflecting off the flux residue, no bridge there or on the other one. It's spdt as in the BOM. I tried just desoldering it, which should result in the fets closing, correct? I still get voltage on the output though so I think I may have just overheated the fets when soldering.
```

---
## \#12 Posted by: brandon Posted at: 2016-12-22T21:18:45.584Z Reads: 82

```
I just assumed smd diodes work the same as regular, I matched the stripe with the one on the pcb, seems to match the schematic as well.
```

---
## \#13 Posted by: chaka Posted at: 2016-12-22T21:34:22.037Z Reads: 79

```
Just noticed you said you were blowing fuses too. You probably have a short on you positive output or somewhere down stream.  Not much to go wrong with these switches. One or both of the fets were probably ruined too.

But what would I know. It's not like I have ever made one. :wink:
```

---
## \#14 Posted by: lox897 Posted at: 2016-12-22T21:34:37.509Z Reads: 73

```
Well you assumed right. I have no idea what else could have caused it, maybe too much heat on the fets
```

---
## \#15 Posted by: brandon Posted at: 2016-12-22T21:39:47.735Z Reads: 75

```
Okay so, it turns out in my infinite wisdom that I have been plugging my battery into the output side of the switch the entire time. Unfortunately plugging it into the correct side has not remedied the situation. I now get 0v on the output no matter if I turn the switch on or off. If I flip the switch with my meter attatched, it stays at 0, but if I change the switch and then attatch my meter, I get 12v for a brief second before it drops, so I'm guessing the voltage from the cap is getting through one fet or the other? At this point I'm sure something has been burnt up but I'm not sure what.
```

---
## \#16 Posted by: chaka Posted at: 2016-12-22T21:47:04.183Z Reads: 71

```
Try it with 24v. I am not sure how well the switch functions at 12v, if at all. Now that I know you had it hooked up backwards everything is telling me your switch is fine.

Don't forget to let the switch turn on, it takes a second. Don't toggle the switch like a crackhead. :grin:
```

---
## \#17 Posted by: brandon Posted at: 2016-12-22T21:55:08.019Z Reads: 73

```
Same phenomena with 24v. Resistors read correct values, diode seems to be working correctly, cap is charging up fine (these little caps are not polarized right? I see no markings) and since I'm getting 0 volts I guess that means both of my fets are dead?
```

---
## \#18 Posted by: chaka Posted at: 2016-12-22T22:09:50.955Z Reads: 71

```
What you have now is a symptom of having a shorted gate pin or a bad toggle switch. Still doesn't explain the blown fuse.
```

---
## \#19 Posted by: brandon Posted at: 2016-12-22T22:16:55.695Z Reads: 69

```
Toggle switch is working as expected, tried shorting the pads anyways and that doesn't work either. Could I have shorted the gate pin internally? I'm not reading a dead short between the gate and the other 5 pins.
```

---
## \#20 Posted by: chaka Posted at: 2016-12-22T22:46:04.398Z Reads: 67

```
The only other thing I noticed was some possible cold joints on your resistors. You cold add some flux and reflow.
```

---
## \#21 Posted by: brandon Posted at: 2016-12-22T22:58:04.934Z Reads: 63

```
I'll give it a go, but I cleaned with isopropyl and fluxed everything so my feelings are still on the burnt fets :frowning:
```

---
