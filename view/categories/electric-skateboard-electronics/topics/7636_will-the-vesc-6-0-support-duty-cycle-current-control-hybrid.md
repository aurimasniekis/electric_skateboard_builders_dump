# Will the VESC 6.0 support duty cycle/current control hybrid?

### Replies: 10 Views: 833

## \#1 Posted by: Jinra Posted at: 2016-08-14T18:59:52.240Z Reads: 121

```
I suppose might actually be possible on the current 4.12 hardware, but I was wondering if it could provide the benefits of position based speed control while having the benefits of on demand current for torque and acceleration.

Evolve seems to do something like this as speed is determined by throttle position, but the torque and acceleration potential on the GT is insane. It accelerates much faster than my DIY board which is why I'm pretty curious about it.
```

---
## \#2 Posted by: makevoid Posted at: 2016-08-14T19:08:46.496Z Reads: 120

```
I think that if you increase motor max a bit you will have faster acceleration than evolve without many doubts, maybe from 45 go in steps of 5 until you reach 60/65?
```

---
## \#3 Posted by: Jinra Posted at: 2016-08-14T19:14:45.962Z Reads: 118

```
oh for sure if i increase it, the acceleration would be better, but I'd like the benefits of throttle dependent speed. I have my settings a little lower to not beat up my battery too much
```

---
## \#4 Posted by: chaka Posted at: 2016-08-14T19:21:18.870Z Reads: 113

```
Yeah when I set my motors to 80 amps they rocket! But.....it isn't healthy for the system. That is often the case with anything "high performance".  I have also noticed that there are many gt owners complaining of failing packs, I would be willing to bet these are the same people who flog there boards pretty hard. Also, I am not convinced that the gt is not using lipos...whos willing to cut open the heat shrink on their pack. :stuck_out_tongue:
```

---
## \#5 Posted by: Jinra Posted at: 2016-08-14T19:24:47.014Z Reads: 109

```
i felt it around and pretty sure they're 18650s
```

---
## \#6 Posted by: Hummie Posted at: 2016-08-14T19:24:57.413Z Reads: 109

```
I challenge ur GT to a race from 0-20mph! Or 0-25mph if u think it will really go that fast.  Or race any hill any distance 8 blocks or less. From what I remember I should I was quicker.
Yea we all looked together and 18650s. How many was it?
```

---
## \#7 Posted by: chaka Posted at: 2016-08-14T19:27:46.480Z Reads: 108

```
The gt also has a lower kv, I think it is around 140kv. That will give it a little more punch if gear ratios are the same. The pack could also have less resistance resulting in less voltage sag under load. Also the gt has a larger pack right? If it does that will play a large role in available "punch".
```

---
## \#8 Posted by: Jinra Posted at: 2016-08-14T19:29:02.040Z Reads: 104

```
yep about 140kv from my calculations. it's running a ridiculous 15/32 ratio. It's a 10s4p pack
```

---
## \#9 Posted by: Jinra Posted at: 2016-08-14T19:30:09.303Z Reads: 106

```
sure! i didn't full throttle from start last time because i usually fly off if i do.
```

---
## \#10 Posted by: onloop Posted at: 2016-08-15T13:48:26.504Z Reads: 86

```
[quote="Jinra, post:3, topic:7636"]
I'd like the benefits of throttle dependent speed.
[/quote]

yeah, i would have to agree with you on this one.... normally i don't mind current control.. 90% of the time it is fine.... but when approaching an incline with varying angles of steepness as you increase in elevation.... & whilst at slow-ish "half-throttle" speeds.... the current control sort of sucks....

because you need to keep adjusting the throttle in sync with the varying steepness grades if you want your speed to be consistent during the climb.... in most cases you never get it right.... during the steep section you apply the throttle, but it takes time to get the speed increasing, by the time your speed has increased you reach a less aggressive incline which means you would rapidly accelerate at that throttle position, so you back off the throttle.... which means the next steep section you need to pump the throttle again.... etc....etc....

so normally I just hammer the throttle hard before any steep sections to ensure i have ample moment which helps you maintain speeds, lessens the motor load and often means less throttle fiddling is required.

this phenomenon is most noticeable when you are trying to "ride-slow" when you are with kids or inexperienced riders....

the simple answer is just-ride-fast-always.
```

---
