# Mini fsesc recommended settings according to Flipsky - can someone verify?

### Replies: 8 Views: 601

## \#1 Posted by: High-roller Posted at: 2019-03-07T06:04:21.811Z Reads: 101

```
Having burned one vesc through stupidity I'm ordering a second one and I received these guidelines from flipsky.
![Screenshot_20190307-075640|281x500](upload://k3ncqA4SGefHZYZEUfwPjScqldN.jpeg) 
They also wrote: "Due to two phase design, the ESC has strict requirement on parameter setting. If not match well, it will cause over-current cut off during hard brake or hard accelerate for about 0.2s, but after 0.2s it will recover the power."

My battery is 10s4p Samsung 30q and according to them these settings should work even on dual (I'm running ppm, not canbus).
Do these make sense? I ask mainly because the battery regen rate seems very high, I always thought that it should be about 12-15 amps?
```

---
## \#2 Posted by: jun1208 Posted at: 2019-03-07T06:21:32.460Z Reads: 90

```
With 10s4p 30Q, iinm you are able to push 45A in and out :thinking:

But that also depending on whether are you running on dual drive or single drive, if you're on dual drive aka 2 VESC then you actually need to half the value meaning only 22A per side max..

I hope I understand it properly :+1:
```

---
## \#3 Posted by: High-roller Posted at: 2019-03-07T06:28:49.496Z Reads: 88

```
Thanks, that's more or less what I thought too. 
I'll probably play it safe and do half of their recommended on each side. I mean, they would presumably know what their vescs can do but this still looked slightly off.
```

---
## \#4 Posted by: Andy87 Posted at: 2019-03-07T06:41:38.917Z Reads: 85

```
Noob question, but what is the mini fsesc?
The 4.20 dual? Dual plus? Or a single vesc?
```

---
## \#5 Posted by: High-roller Posted at: 2019-03-07T06:59:18.906Z Reads: 80

```
https://flipsky.net/collections/electronic-products/products/mini-fsesc4-20-50a-base-on-vesc-widely-used-in-eskateboard-escooter-ebike
Redesigned single vesc 4.12. It's more compact, has a heatsink and is their cheapest vesc at $75.
They also have an article explaining the differences:
https://flipsky.net/blogs/vesc-tool/whats-the-main-difference-between-mini-fsesc4-20-and-fsesc4-12-is-mini-fsesc4-20-reliable

I still want to know what independent, unbiased people think though.
```

---
## \#6 Posted by: Gamer43 Posted at: 2019-03-07T09:31:12.009Z Reads: 68

```
Motor current settings look good. What control mode (BLDC, FOC, sensors?) are you running?
I'd recommend setting positive ramping time to 0.8s in the app config.

Many users have reported problematic cutouts due to DRV faults; I am working with another user on esk8 to get to the bottom of the issue, and so far, we've discovered that simply changing the value of 6 resistors allows +-50A motor current at 12s no cutouts. (Basically, he tried some of the craziest settings on sensored FOC and it performs better than stock 4.12 hardware after the change).


I'd be more than happy to provide the details of the rework if you're interested.
```

---
## \#7 Posted by: High-roller Posted at: 2019-03-07T09:37:02.143Z Reads: 69

```
Thanks, that would be great!
I'm using bldc, no sensors. I'd rather keep it simple.
```

---
## \#8 Posted by: Bjork3n Posted at: 2019-03-07T09:53:49.562Z Reads: 62

```
Battery current max regen -40A seems very high. 
Not even sure if that's safe.... 
I'm running A total of -18A on my dual setup (-8 each vesc)

10s4p samsung 30Q
```

---
