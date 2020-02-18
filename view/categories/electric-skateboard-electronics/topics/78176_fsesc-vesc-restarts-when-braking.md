# Fsesc VESC restarts when braking

### Replies: 16 Views: 353

## \#1 Posted by: skaterscooter Posted at: 2018-12-16T16:49:16.467Z Reads: 122

```
Ok so I bought a VESC made by flipsky off eBay a week ago and it arrived yesterday. I've been having a play with it and plan to use it on an ebike. It was working fine controlling it via up down left right on they keyboard untill suddenly it disconnected when I braked or swithed I to reverse. Upon further inspection I've noticed that the entire VESC is disabled for a few seconds and the green led goes off for a few seconds then comes back on again. I've tried fiddling with current limit settings but that changed nothing. The only thing that temporarily world was reducing some sort of delay to do with errors. Weirdly no errors showed up in the console and the red led did t blink at all. Same applies to using a throttle knob for control.

Any help appreciated
```

---
## \#2 Posted by: Benjamin899 Posted at: 2018-12-16T16:55:36.076Z Reads: 117

```
What FSESC? Also post all your seetings with screenshots pls.
```

---
## \#3 Posted by: skaterscooter Posted at: 2018-12-16T17:04:34.535Z Reads: 116

```
It's an FSESC 4.12. I'm out at the moment but will post screenshots when back. Which sections shall I post?
```

---
## \#4 Posted by: Ixf Posted at: 2018-12-16T17:20:14.725Z Reads: 111

```
are you running 12s?
Sounds like overvoltage...
```

---
## \#5 Posted by: briman05 Posted at: 2018-12-16T17:22:04.457Z Reads: 104

```
Are you running 12s FOC
```

---
## \#6 Posted by: skaterscooter Posted at: 2018-12-16T17:52:42.379Z Reads: 95

```
Running 10s BLDC
```

---
## \#7 Posted by: Unsounder Posted at: 2018-12-16T20:19:14.744Z Reads: 83

```
Does this happen when the battery is not fully charged?
```

---
## \#8 Posted by: skaterscooter Posted at: 2018-12-16T20:34:34.329Z Reads: 78

```
No I charged the battery fully and have also tested with a power supply however that can't be used with braking as charge can't be put back in to it.
```

---
## \#9 Posted by: Unsounder Posted at: 2018-12-16T21:22:29.523Z Reads: 78

```
That's kind of why I'm asking. If the VESC goes into regen and tries to send power to a fully charged battery the BMS can cut power to protect the battery killing the circuit momentarily.
```

---
## \#10 Posted by: alexnz Posted at: 2018-12-16T21:37:44.556Z Reads: 74

```
Yes sounds like it's the battery BMS that is cutting off. Either because your battery is already full, or because you're sending back too many amps for what your battery can handle.
```

---
## \#11 Posted by: ElectricCoast Posted at: 2018-12-16T23:14:13.688Z Reads: 65

```
My Flipsky 6.6's dual drive 6380 170kv motors do the same thing.  Only during a full battery running 12s FOC it's an over voltage from regeneration during braking is what I believe is the cause.  Once the battery has ran down some the problem goes away.  I was suggested to run no Hardware limits version of firmware. Of course run this at your own risk.
```

---
## \#12 Posted by: RedBaron Posted at: 2018-12-17T00:00:08.090Z Reads: 61

```
I had the same issue here with 2 dual 6.6's. I was going crazy trying to figure out what I did wrong. Brakes would cut out momentarily after coasting at 41.2v and getting fault code over voltage.  Checked and rechecked every connection down to the parallel groups. Interested in a safe workaround. I haven't explored no hw limits.
```

---
## \#13 Posted by: DeathCookies Posted at: 2018-12-17T03:02:49.146Z Reads: 48

```


[quote="ElectricCoast, post:11, topic:78176"]
My Flipsky 6.6’s dual drive 6380 170kv motors do the same thing. Only during a full battery running 12s FOC it’s an over voltage from regeneration during braking is what I believe is the cause. Once the battery has ran down some the problem goes away.
[/quote]

Maybe it is about the voltage reading in the fs6.6's. Many people reported that they get massive over voltage spikes. only suggestion so far: add capacitors
```

---
## \#14 Posted by: lrdesigns Posted at: 2018-12-17T03:05:12.673Z Reads: 48

```
@skaterscooter what is your "max input voltage" set at? 

![image|690x200](upload://fodM9U5s3MBvmAVwgvErAoxcsrC.png)
```

---
## \#15 Posted by: skaterscooter Posted at: 2018-12-17T08:32:18.457Z Reads: 38

```
Right I'm back now. Seems most people are suggesting over voltage which would make sense as before when it was working, that pack was only at about 38v. I'll send screen shots and test with a lower voltage at some point this morning.

Thanks for helping!
```

---
## \#16 Posted by: skaterscooter Posted at: 2018-12-17T10:32:30.182Z Reads: 36

```
Also just to be clear, I'm not using a BMS whilst testing.
```

---
