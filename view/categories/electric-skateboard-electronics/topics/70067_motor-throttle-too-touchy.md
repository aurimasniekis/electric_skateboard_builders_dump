# Motor throttle too touchy

### Replies: 7 Views: 689

## \#1 Posted by: Pafrican Posted at: 2018-10-03T22:41:11.627Z Reads: 123

```
Hello,

My board is riding great, but the torque is too aggressive.

Specs:
(x2) 5S Turnigy 5000mAh Lipo batteries (linked in series)
Tunrnigy 6374 149kv BLDC motor
GT2B receiver/transmitter
TB VESC (running in BLDC mode)

The board behaves like it should; the motor gradually spools as I apply more and more throttle.
The VESC-Tool is showing me that full throttle is applied when I've got the trigger pulled all the way, so my transmitter is properly calibrated.
My problem is that when I'm riding at say... 15mph... and I pull on the throttle a bit too suddenly then the board pulls forward aggressively and I struggle to keep balance. At those speeds, I don't want the board to go shooting from underneath my feet because I accidentally blipped the throttle.

Is there a way that I can limit the torque using the VESC-tool, even if it means lowering my top speed overall?

Thank you
```

---
## \#2 Posted by: thiswasandy Posted at: 2018-10-03T22:42:20.564Z Reads: 118

```
Adjust your throttle curve. I do -25% on both with a natural curve.
```

---
## \#3 Posted by: thiswasandy Posted at: 2018-10-03T22:43:25.654Z Reads: 121

```
https://www.electric-skateboard.builders/t/ackmaniacs-fw-lets-talk-throttle-curves/64173

That thread says ackmaniac fw, but even without you can still adjust the curve.
```

---
## \#4 Posted by: Jmding Posted at: 2018-10-03T23:30:05.701Z Reads: 106

```
VESC Tool -> App Settings -> PPM -> Positive Ramping Time and Negative Ramping Time

Increase these value of these numbers.  These basically average out your throttle input, smoothing it out.
```

---
## \#5 Posted by: Pafrican Posted at: 2018-10-04T01:45:26.603Z Reads: 97

```
Awesome, thanks!

Before I start tinkering with the values, I'd like to know what these variables are exactly.
I'm assuming Positive Ramping Time is the time it takes for the motor to match throttle response when accelerating
Does Negative Ramping Time apply for braking/decelerating?
```

---
## \#6 Posted by: thiswasandy Posted at: 2018-10-04T01:59:19.371Z Reads: 95

```
https://www.electric-skateboard.builders/t/better-throttle-performance-through-more-responsive-ramping/29356/30

I'm not familiar, but maybe this will help.

Personally I use FOC and from what I understand the ramp times don't work in FOC, But maybe I misread.
```

---
## \#7 Posted by: Jmding Posted at: 2018-10-04T16:43:54.858Z Reads: 73

```
Yeah, ramping is the amount of time it takes to get from 0 throttle, to full throttle, or basically how quickly the VESC ramps up the current.  Longer ramp time, more gradual current ramping, less jerky ride.
```

---
