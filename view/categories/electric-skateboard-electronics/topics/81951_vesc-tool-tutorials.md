# Vesc tool tutorials

### Replies: 15 Views: 649

## \#1 Posted by: joeadams101 Posted at: 2019-01-24T19:13:35.740Z Reads: 143

```
Anyone had links for VESC tool tutorials ? Tried looking them up but no luck. Will be great for one that goes over setting up from scratch. Thanks!
```

---
## \#2 Posted by: Skunk Posted at: 2019-01-24T19:14:57.153Z Reads: 142

```
https://youtu.be/qpovd2XRKqc
```

---
## \#3 Posted by: joeadams101 Posted at: 2019-01-24T19:17:20.754Z Reads: 133

```
Thanks!!!!!
```

---
## \#4 Posted by: Skunk Posted at: 2019-01-24T19:19:18.801Z Reads: 123

```
No problem. I keep that bookmarked.
```

---
## \#5 Posted by: trampa Posted at: 2019-01-24T19:38:15.577Z Reads: 120

```
Vesc-project.com 
Click on documentation, then select manuals
```

---
## \#6 Posted by: High-roller Posted at: 2019-02-25T11:38:47.837Z Reads: 87

```
Do I still have to limit the ERPM to 60000? I didn't see anything about changing that value so I wonder if it's still necessary or can I leave it at +100000 \ -100000?
```

---
## \#7 Posted by: Andy87 Posted at: 2019-02-25T11:41:35.416Z Reads: 81

```
It depends on your vesc hw version.
```

---
## \#8 Posted by: High-roller Posted at: 2019-02-25T11:45:45.142Z Reads: 83

```
Flipsky mini FSESC 4.12. The tool updated the firmware without issue and then a few minutes later the vesc burned out while I was testing the remote trigger. I had forgotten to remove the binding key from the receiver first so I figure it's either that or the ERPM.
```

---
## \#9 Posted by: Andy87 Posted at: 2019-02-25T11:48:31.576Z Reads: 75

```
4.12 hw should be limited to 60000 erpm.
Focbox is an exception here.
Which motor kV and battery you had when it happened?
If under 12s 190kV than it wasn’t the erpm Limit probably
```

---
## \#10 Posted by: High-roller Posted at: 2019-02-25T12:09:13.049Z Reads: 68

```
Correct, it was 10s 190kv, the motor is also from flipsky. Any other possibilities? I was using the wizard for  a single vesc which I later was going to pair through ppm. I was trying to get a response with the remote but had nothing. That's when I heard a fizzling noise and saw smoke coming from the vesc. I disconnected everything and other than the vesc there's no damage. Now I'm about to try the second one and I'd not have to replace both.
```

---
## \#11 Posted by: Andy87 Posted at: 2019-02-25T12:13:53.872Z Reads: 66

```
but you made it successful through the wizard?
Maybe there is a short in your phase wires or somewhere.
maybe your bullet connectors touched each other, or did you isolate them?
```

---
## \#12 Posted by: High-roller Posted at: 2019-02-25T12:20:39.143Z Reads: 64

```
I didn't finish the tutorial, the burnout happened before I got there.
The bullet connectors are placed in holes in a 3d printed plate and held there with hot glue. They were partially shrink tubed, I was going to color code the last part once I knew the right order for the phase wires. They can't short through cured hot glue, can they?
![15510971948866054435319940076694|375x499](upload://zsoOnOPHNcPnvUOsjvC5lbEsONX.jpeg)
```

---
## \#13 Posted by: Andy87 Posted at: 2019-02-25T13:03:14.123Z Reads: 59

```
I don´t like hot glue inbetween of electric parts, but it shouldn´t be the cause of the fault.
I would non the less meassure the phase wires one by one to the ground of the motor. which should be all open end.
and than measure the phase wires inbetween of each other. the resistance there should be all the same.

PS: you can invert the spin direction of your motor with only one click in the vesc tool.
no need to swap the phase wires.
```

---
## \#14 Posted by: High-roller Posted at: 2019-02-25T13:16:17.763Z Reads: 58

```
Alright, I'll try those. Thanks!
```

---
## \#15 Posted by: High-roller Posted at: 2019-02-28T19:03:35.698Z Reads: 50

```
Update: I reviewed the tutorial and rebinded the receiver properly. 
On the second vesc, after the firmware update I first changed the erpm just in case and only then started the wizards. Everything worked perfectly.
The first vesc is definitely dead. Just plugging it in (with the loopkey) caused a loud pop and nothing else. Opening it up I can see that one of the mosfets is fried:
![IMG_20190228_204505|375x499](upload://qh76rIpYemAmoadp2sQdLiOt2Oh.jpeg) 
I couldn't find any of the parts online to replace it and I don't know anyone nearby who can in any case. I'll probably just try to sell it for the hardware to someone who knows what to do with it.
```

---
