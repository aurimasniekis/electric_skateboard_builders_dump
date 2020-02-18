# How do I go about connecting 4 Focbox&rsquo;s together?

### Replies: 12 Views: 1571

## \#1 Posted by: BoostedBuilder Posted at: 2017-08-02T17:06:30.433Z Reads: 187

```
Hello everyone, 

I want to build a 4WD board and have no idea how to do it. I spent a few hours researching and even contacted Chaka but no luck)

Any help will be appreciated!!!
```

---
## \#2 Posted by: WARMAN Posted at: 2017-08-02T17:08:25.306Z Reads: 189

```
@BigBoyToys think he has a 4wd setup
```

---
## \#3 Posted by: BigBoyToys Posted at: 2017-08-02T18:03:13.969Z Reads: 183

```
Hi, 

You can make a 4 way split ppm signal harness to control them, and/or make a daisy chain CAN bus cable harness to connect all 4.  I use ppm for control and CAN bus for tuning.

Word of warning with the Can bus connections. While your vescs are connected via the can bus, be sure to power off all vescs before plugging another in. If you dont you will blow the CAN transceiver on all of them at the same time.
```

---
## \#4 Posted by: JTAG Posted at: 2017-08-02T18:15:01.826Z Reads: 172

```
The same for PPM. 

All VESC gnd's should at all times be connected to each other when signal (either PPM or CAN) are connected.

And don't use PPM to use multiple ESC's on a single receiver, that will kill them, always use CAN. 

When using you daisy chain all CAN-H and CAN-L 's of all VESC's in parallel. You most likely have to remove the CAN termination resistor of the middle two VESC's (or else the impedance on the bus will be to low for the transceiver to drive it). When all VESC's are connected the resistance between CAN-H and CAN-L should be 60Ohm ish. 

https://en.wikipedia.org/wiki/CAN_bus

@trampa did you ever encounter someone using 4 vesc's on can with regards to removing the termination resistors?
```

---
## \#5 Posted by: BoostedBuilder Posted at: 2017-08-02T19:01:40.245Z Reads: 150

```
Could I maybe connect 2 VESC's with can bus on each side and then chose any VESC on each side and connect them with the male to male Y cable to the receiver?
```

---
## \#6 Posted by: BoostedBuilder Posted at: 2017-08-02T19:09:48.632Z Reads: 141

```
Something like this: 
<img src="/uploads/db1493/original/3X/e/4/e40e39b99b337e8894e7ac6d1291aeb95907f797.jpg" width="690" height="379">
```

---
## \#7 Posted by: trampa Posted at: 2017-08-02T19:10:30.502Z Reads: 135

```
Never use a Y! The new Vesc designs will get damaged for sure. Y-PPM should not be used at all, nor on HW 4.xx, nor on the new designs.

4 VESC Six on Can should work just fine. 

Frank
```

---
## \#8 Posted by: BoostedBuilder Posted at: 2017-08-02T19:11:27.133Z Reads: 133

```
Ok)) thank you!! Saved me $400
```

---
## \#9 Posted by: BoostedBuilder Posted at: 2017-08-02T19:12:10.830Z Reads: 133

```
Could you maybe also consult me on the battery I should use? I wanted to use a 12s1p. would that work at all?
```

---
## \#10 Posted by: BigBoyToys Posted at: 2017-08-02T19:23:56.001Z Reads: 129

```
I havent removed the terminal resistor, I actually have a  higher ohm resistors at R401 on all my VESC's for the 4wd, but to be honest though, its worked fine with with out them. Using a ppm spitter hasnt caused me issues either.  Ill take your word for it though.
```

---
## \#11 Posted by: Jinra Posted at: 2017-08-02T19:25:47.714Z Reads: 128

```
I don't know anyone who's ever blown their VESC using split PPM, but I always see people warning that it will.
```

---
## \#12 Posted by: BigBoyToys Posted at: 2017-08-02T19:47:06.596Z Reads: 125

```
Right, i do only power the receiver off of one vesc though so its the signal and ground that are shared between all 4.
```

---
