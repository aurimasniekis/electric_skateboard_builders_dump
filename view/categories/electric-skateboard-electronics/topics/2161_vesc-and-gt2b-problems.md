# VESC and GT2B problems

### Replies: 10 Views: 1630

## \#1 Posted by: NerijusM Posted at: 2016-04-04T19:58:38.183Z Reads: 154

```
Hello,

I have one big problem - VESC brakes motor when GT-2B transmiter is off.
How to make VESC not do anything when I turn off transmiter?
In BLDC tool I have 0A current in field about Timeout (when no control signal is received) and 10000ms delay.
I`m getting kind of glitches and today I hit a groud badly with my eMTB board.
I will check hardware, but it is possible to make VESC not do brakes when transmiter is off?

Thank you
```

---
## \#2 Posted by: laurnts Posted at: 2016-04-04T20:21:54.352Z Reads: 151

```
Theres somewhere setting to set the baud / gauss at 1500 upon signal lost from transmitter.
```

---
## \#3 Posted by: elkick Posted at: 2016-04-04T20:25:26.230Z Reads: 151

```
In the main app tab: "Brake current to use…” can be set to make the motor brake with a certain current when a timeout occurs instead of just releasing it. 

This needs to be set to 0,00.
```

---
## \#4 Posted by: NerijusM Posted at: 2016-04-04T20:31:03.442Z Reads: 149

```
Yes, this is already 0,00 but I get really hard wheel lockup when I shut down transmiter. I checked this today 2-3 times. That lockup goes away after 20 seconds or so and then wheel with motor spins easy.
```

---
## \#5 Posted by: elkick Posted at: 2016-04-04T20:33:33.576Z Reads: 138

```
Did you try to adjust the settings on the transmitter itself? There are some things that can be easily dis adjusted during usage.

It might send a brake signal to the VESC.
```

---
## \#6 Posted by: NerijusM Posted at: 2016-04-04T20:36:24.827Z Reads: 133

```
Fail-safe? 
Maybe.
I will test this with simple servo.
And also why I get dropouts and I get to ground...

Thank you.
```

---
## \#7 Posted by: Haimindo Posted at: 2016-04-04T21:16:17.960Z Reads: 127

```
Yeah, check the receivers fail-safe thingie, that helped me
```

---
## \#8 Posted by: NerijusM Posted at: 2016-04-05T17:54:30.517Z Reads: 119

```
Yes, got solved everything.
Firstly - receiver antena ground wire was broken from PCB. Soldered back.
Secondly - receiver fail-safe was kicking full brakes with no signal. Removed that with this tutorial - http://ibuyrc.com/manual/79P-FSGT2B-2CH-Car.pdf

Take care with your fail-safe because you will end up flat on ground....
```

---
## \#9 Posted by: samusaki Posted at: 2016-05-30T05:46:05.762Z Reads: 100

```
Hey again. Can i get in touch with you, about vecs?
```

---
## \#10 Posted by: NerijusM Posted at: 2016-05-30T06:03:06.554Z Reads: 96

```
Yes, just write a PM.
```

---
