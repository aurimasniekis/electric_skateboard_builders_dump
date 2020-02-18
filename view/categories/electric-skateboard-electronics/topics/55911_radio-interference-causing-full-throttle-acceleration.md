# Radio Interference Causing Full Throttle Acceleration?

### Replies: 8 Views: 452

## \#1 Posted by: TrainRider Posted at: 2018-05-18T18:22:25.077Z Reads: 92

```
So yesterday I was taking my board to the shops in the village for the first rather than testing down a bridal way and I think I got some sort of radio interference causing my board to go full throttle.

I had to bale and got a black eye and fucked up shoulder for my troubles.

I use a GT2b with a Mad Munkey enclosure. I have the receiver antena outside of the board enclosure, stuck to the board.

I put the board in the passenger seat of my car, turned it and my remote on and drove it around a residential area today to see how it would behave and I was getting random periods of full throttle.

Has anyone experience anything like this or know how I could fix it?

Thanks
```

---
## \#2 Posted by: i2oadsweepei2 Posted at: 2018-05-18T18:35:45.138Z Reads: 80

```
That really blows man. Let’s start with a bit more info then. 


1 - Did you set the failsafe for the radio and receiver? In most cases we don’t use brake as the failsafe. We just use neutral. That way you don’t get thrown off if you loose signal. 
Find the manual here: https://www.manualslib.com/manual/1145194/Fly-Sky-Fs-Gt2b.html

2- Did you calibrate the remote in vesc/bldc tool if that’s what you are using?

Post screenshots of the app settings in the vesc/bldc too if you can. 

This will be a good start. Before that make sure all of the wires are plugged in fully. You can try to wiggle them while the board is on to see if they are too loose.

GL
```

---
## \#3 Posted by: TrainRider Posted at: 2018-05-18T18:52:02.488Z Reads: 68

```
1. Yes, I have set the failsafe of the radio and receiver.

2. I did calibrate my FOCBOX's/remote with the bldc tool latest software.

I don't think it is a loose cable but I will take the enclosures off and check all the connections tomorrow + take screenshots of my app settings.

The issue never happened before, only when I started riding in residential areas, which is why I think it is related to radio interference.
```

---
## \#4 Posted by: TehAtheist Posted at: 2018-05-18T19:20:53.225Z Reads: 63

```
Bench test your board and turn off your remote, see if the board accelerates or not. If it does not, the issue is not due to signal interference. If it is, it's due to interference and a bad failsafe.
```

---
## \#5 Posted by: b264 Posted at: 2018-05-18T19:39:38.129Z Reads: 58

```
See what happens when your board is on at half throttle and you slowly wrap aluminum foil around the remote.  What does the board do?
```

---
## \#6 Posted by: onepunchboard Posted at: 2018-05-18T22:17:10.184Z Reads: 47

```
DO NOT USE FAIL SAFE ON RECEIVER.
This cause full acceleration. Please disable it
Use fail safe on VESC Setting as neutral, not brake. 

fail safe on gt2b is made for glow engine cutout. So in electric motors it is best not to use. I'm not sure why but it always full accelerate in some esc including vesc
```

---
## \#7 Posted by: danielz Posted at: 2018-05-18T22:23:15.504Z Reads: 45

```
Yep, relying on gt2b failsafe can be dangerous. I explained why in this thread and the work around.

https://www.electric-skateboard.builders/t/failsafe-issue-never-seen-this-before/53057/11

Original posters problem could also be troubleshooted with an arduino too.
```

---
## \#8 Posted by: i2oadsweepei2 Posted at: 2018-05-18T23:37:17.073Z Reads: 43

```
Strange the gt2b has been very solid.  There is some really good advice below my first post. Try those out then post the screen shots when you can. I’m also curious to know what happens when you turn off the remote while everything is on. If it accelerates then, the failsafe is set wrong and you are having signal issues as others have said too.

Good luck
```

---
