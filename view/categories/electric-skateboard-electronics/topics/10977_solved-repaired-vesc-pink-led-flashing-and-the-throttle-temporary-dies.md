# Solved/repaired! VESC pink led flashing and the throttle temporary dies

### Replies: 6 Views: 717

## \#1 Posted by: SvantePanter Posted at: 2016-10-11T19:37:21.408Z Reads: 87

```
Hi!
I've had my @torqueboards VESC for a couple of days now. After some minutes of use, the throttle just dies for a moment and the pink led starts to flash. Then I'm back again, and the the error repeats. Could it be an error within the VESC?
 https://youtu.be/5sM5ooahCLE
```

---
## \#2 Posted by: Blasto Posted at: 2016-10-11T19:42:01.325Z Reads: 90

```
post your setting and check the errors the vesc throws. in the terminal type "faults" dont turn the vesc off before or the error messages will reset
```

---
## \#3 Posted by: rpn314 Posted at: 2016-10-11T19:55:08.271Z Reads: 82

```
I see that most often with over voltage errors, but it could be anything. Given that you're quickly accelerating and then braking (at least that's what it looks like in the video), and that it then comes back, over voltage is my first guess.
```

---
## \#4 Posted by: SvantePanter Posted at: 2016-10-11T20:12:52.211Z Reads: 75

```
Great I will post my BLDC Tools-settings when I have access to my laptop again... Although yesterday I quickly (for a second) got the DRV8302 fault code when running the VESC with USB-cable/BLDC Tools. The DRV8302-error really scares me, there are some threads about that and they all contains comments like "the VESC is dead, replace the chip"...
```

---
## \#5 Posted by: rpn314 Posted at: 2016-10-11T21:31:13.277Z Reads: 62

```
Yeah, if you ever got a drv8032 error, from what I've seen, it's dead or dying and will soon be dead (the drv chip). 

Though personal recommendation, I wouldn't do the quick acceleration with quick braking in succession. I have heard of that blowing drv chips.
```

---
## \#6 Posted by: SvantePanter Posted at: 2016-10-25T19:42:21.390Z Reads: 39

```
I<img src="/uploads/db1493/original/3X/b/7/b78734104fabd5077b5108f7b604a7190c1c2505.JPG" width="375" height="500">

Update! I found a great guy in Germany that fixed my VESC quick and inexpensive.
I don't really understand what was wrong with the VESC, but it was not the DRV8302-chip that was the problem. Seems like something was wrong when the board was manufactered.

Link to the repair guy: http://www.lp-electronic.com/vesc/
```

---
