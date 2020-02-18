# Nunchuck Cutoff Question

### Replies: 9 Views: 1078

## \#1 Posted by: rasmukri Posted at: 2016-11-06T19:25:15.597Z Reads: 90

```
So I got my nunchuck all wired in and it seems to work good. Ive only bench tested it as I'm still working on the case for electronics. But when i tested the cutout it doesn't work. Like i have the nunchuck at full throttle and pull one of the batteries to simulate the battery died and the skateboard motor still keeps going at full speed. But when i was using my RC remote if i switched it off while full throttle it cut gas off to the VESC. The timeout no signal received (ms) block on the BLDC tool is set to 500, I've adjusted that and still no dice. 
Also it seems like the nunchuck doesn't register correctly. Like when i am in the nunchuck part of the screen i click display and it idles at 50% but once i get to about 65% the motor is at full speed. Is this because its bench tested and not enough weight to make it go right? because my RC controller did it right on the bench at 75% it was only going half speed. But with the nunchuck the bar goes to 99% and 0% but it feels like something is off. Is there a way to adjust the nunchuck settings?
```

---
## \#2 Posted by: Jobbel Posted at: 2016-11-07T01:25:42.954Z Reads: 71

```
I can't tell you why your cutoff does not work, but you are right about the bench test, you are using current control, which behaves exactly as you'd expect it, as soon as you stand on the board. That is because for example 5 amps without load are enough to reach a pretty high rpm, but with you on the board it'll be quite low and you'll go much slower.
```

---
## \#3 Posted by: JLabs Posted at: 2016-11-07T02:12:43.322Z Reads: 64

```
[quote="rasmukri, post:1, topic:12594"]
Like i have the nunchuck at full throttle and pull one of the batteries to simulate the battery died and the skateboard motor still keeps going at full speed
[/quote]

How does the motor keep spinning at full speed if there is no battery power? Of you have batteries wired in series and unplug on there is no complete circuit, which means no power.
```

---
## \#4 Posted by: rasmukri Posted at: 2016-11-07T02:15:16.860Z Reads: 55

```
Guess i wasn't specific enough.
The battery for the board stays connected, I removed the battery from the nunchuck and the board kept spinning full speed.
```

---
## \#5 Posted by: JLabs Posted at: 2016-11-07T02:17:37.991Z Reads: 47

```
Oh ok, makes sense. Seems like the problem is with the Vesc settings, which I am not an expert in.
```

---
## \#6 Posted by: chinzw Posted at: 2016-11-08T17:45:18.896Z Reads: 31

```
Do you have the VESC connected to your computer by any chance? If so, disconnect it, power cycle the VESC and try again.
I had the same problem, it was driving me crazy! BLDC tool sends a keepalive packet to the vesc, and that overrides the timeout.
```

---
## \#7 Posted by: rasmukri Posted at: 2016-11-08T18:25:38.379Z Reads: 32

```
HAHA thanks bro that totally was it. Just tried it here at work and it cut off right after I pulled the battery. Silly that I didn't think of that before.

Another problem has come up though, unrelated to the previous.
I am having cutout issues from my nunchuck while riding down the road. just random intermittent hesitations while cruising along. I thought I fixed it by putting a ferrite ring on the cable that goes to the RX for the nunchuck but its still doing it. It gives me a bit of a scars as I'm riding down the road and it doesn't stop when I release the gas or gives it more gas than I wanted.
I soldered the cables to the VESC so there is no clip to be lose or anything they are solid connections.
```

---
## \#8 Posted by: chinzw Posted at: 2016-11-08T18:33:04.467Z Reads: 29

```
From what i hear, nunchucks are not particularly reliable. I read on vedder's forum that he's working on a new communication protocol for the nunchuck for VESC6 that will add some more layers of protection and failsafe, but that wont be ready for a while.
```

---
## \#9 Posted by: raxell Posted at: 2016-12-21T17:39:26.542Z Reads: 22

```
@rasmukri  I have been riding with nunchuck for 3 months with zero issues. I don't know why, a week ago it has become uncontrollable. Lot of random cutoff, random lose of power, smalls accelerations... Like you. It is dangerous to ride like this

I thing it is time to try other controller for me.
```

---
