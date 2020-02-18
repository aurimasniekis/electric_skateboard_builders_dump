# Vedder fuse switch not working - Chaka revision

### Replies: 8 Views: 552

## \#1 Posted by: KTMinni Posted at: 2017-05-12T17:51:13.508Z Reads: 82

```
Basically, I have the switch connected and there is a resistance change when the button is depressed. But no voltage will pass over the positive side of the switch.
<img src="/uploads/db1493/original/3X/0/1/016793fe7527308f59ddfc7e8710d3f47e204d7e.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/a/7/a760708521b923babb3e2fc281e38c9939752daf.jpg" width="375" height="500">

Edit: and yes I have triple checked the wiring, it's correct.
```

---
## \#2 Posted by: longhairedboy Posted at: 2017-05-12T18:18:27.659Z Reads: 76

```
have you tried bypassing the pushbutton and putting the eswitch into ON position by shorting the switch wires?

Where is the thin red wire attached to the positive output going?
```

---
## \#3 Posted by: Jinra Posted at: 2017-05-12T18:32:35.168Z Reads: 72

```
My guess is volt meter, though they should really have both leads for it next to each other. I burned out 2 voltmeters by attaching them too far apart..
```

---
## \#4 Posted by: longhairedboy Posted at: 2017-05-12T18:36:03.308Z Reads: 68

```
agreed. volt meters should have both leads soldered to the output side of the eswitch or somewhere else on the output side. 

Since I couldn't tell which end was plugged in where, i also thought maybe it might be backwards, with the cells plugged into the output side. Its hard to tell in the picture. That would also make it not come on right.
```

---
## \#5 Posted by: Jinra Posted at: 2017-05-12T18:39:02.790Z Reads: 62

```
The side without the switch is the output. Since the supposed voltmeter is on the right side, I'm **assuming** they have it hooked it correctly.
```

---
## \#6 Posted by: longhairedboy Posted at: 2017-05-12T18:45:48.833Z Reads: 60

```
and that does look like the male connector on the input so that backs up your theory. 

hmmm.

it could easily be a problem with the pushbutton, which could be tested by shorting the ON to COMMON, or it could be an issue with the volt meter. Not having the volt meter leads on the same side of the switch is an issue, but that could also be a lead for whatever BEC is running the light in the pushbutton. 

as an aside, i make these little leads with servo jumpers that can be used to keep the eswitch in the on or off position. I use them to keep the switch off while the packs are sitting around waiting to go in a board so I don't have to dangle a button or rocker off of it. of course they can also be used to turn the pack on while testing stuff.
```

---
## \#7 Posted by: KTMinni Posted at: 2017-05-12T23:54:25.676Z Reads: 42

```
Thank you all for your comments the mysterious red wire is going to the LED on the push button(there is a resistor at the contact of the button, I don't know if you can see that though).  I will try shorting the switch without the push button right now.
```

---
## \#8 Posted by: KTMinni Posted at: 2017-05-13T00:15:26.264Z Reads: 36

```
So I tried shorting the pads and it's just dead.  I was told mosfet die open so I'm sending it back to shogu to see if he can figure out what's wrong.
```

---
