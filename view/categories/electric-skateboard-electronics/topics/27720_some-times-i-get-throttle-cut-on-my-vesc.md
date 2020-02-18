# Some times i get throttle cut on my VESC

### Replies: 14 Views: 827

## \#1 Posted by: Silverline Posted at: 2017-07-15T21:01:59.457Z Reads: 95

```
Hallo

I have a esk8.de VESC on my 6s single motor build.

Some times when going up a little hill or driving fast for some times, the throttle suddenly just cut of a moment, then come back again.

I have now fault codes in BLDC tool, so i think it`s my battery settings.
Anybody who could help me ?
I´m runnig 6s Lipo battery (2x3s)

Also i´m new, so i dont like strong brakes, so my motor min(regen) is set to -40A and batt min (regen) -20A, is this okay for the vesc ??

Thanks Guys

<img src="/uploads/db1493/original/3X/9/e/9eb9c7da68b3cbc1cf071dc38f65c122a6b70a55.jpg" width="690" height="387">
```

---
## \#2 Posted by: Jinra Posted at: 2017-07-15T21:34:55.028Z Reads: 87

```
Looks like voltage sag may be cutting off power, you should leave the values at default 8/57
```

---
## \#3 Posted by: Silverline Posted at: 2017-07-15T22:17:52.305Z Reads: 83

```
Sorry 8 / 57 ?? where should i put in these numbers ?
```

---
## \#4 Posted by: Jinra Posted at: 2017-07-15T22:19:40.503Z Reads: 86

```
min max input voltage
```

---
## \#5 Posted by: kieraneboard Posted at: 2017-07-15T22:21:44.979Z Reads: 84

```
[quote="Silverline, post:1, topic:27720"]
motor min(regen) is set to -40
[/quote]

The battery is the problem but.  
I met throttle cut many many times when I build my Meepo Boards.
The easy solution is ESC seting.   You need to limit the current of the ESC, limit it down small until that its affordable for the battery.
The cut you have is definitely because the battery CANT supply as much current to the ESC.
That also happen when you accelarate on flat road. not only up hill.    Whenever you need high current for long time.  The battery cant supply constantly.
```

---
## \#6 Posted by: Silverline Posted at: 2017-07-15T22:29:43.766Z Reads: 78

```
Is it my battery max : 60amp, you think that i should turn a little down ?
And do you also think that i should change my current settings for input voltage and battery cutoff ?
```

---
## \#7 Posted by: kieraneboard Posted at: 2017-07-15T22:31:20.138Z Reads: 75

```
yes.  a battery claim to be 60 amp may not be able to output 60 amp constantly.  You try limit the ESC highest current to 30 AMPs,  if the problem gone.  you then adjust it higher and higher.
```

---
## \#8 Posted by: Silverline Posted at: 2017-07-15T22:34:56.116Z Reads: 69

```
Okay thanks
The only thing i will start change for now is the "Batt Max" then.......
```

---
## \#9 Posted by: SeanHacker Posted at: 2017-07-15T23:10:10.767Z Reads: 68

```
I would also set the default values at 8/57 also like @Jinra said before.
```

---
## \#10 Posted by: Silverline Posted at: 2017-07-15T23:12:24.707Z Reads: 66

```
So Minimum input voltage should be 8v
And Maximum input voltage 57v ??
```

---
## \#11 Posted by: SeanHacker Posted at: 2017-07-15T23:14:45.435Z Reads: 66

```
Yep. That's right.
```

---
## \#12 Posted by: Silverline Posted at: 2017-07-16T14:10:31.206Z Reads: 57

```
Thanks Guys
```

---
## \#13 Posted by: lrdesigns Posted at: 2017-07-16T14:41:48.981Z Reads: 56

```
If that does not fix it I once had this happen to me from the receiver being too close to the motor wires. The large current flow would make it cut out.
```

---
## \#14 Posted by: Silverline Posted at: 2017-07-17T22:00:29.831Z Reads: 43

```
Thanks guys...

After i did the battery max/min change

And chaged max erpm from default 100.000 to 60.000 i have no more throttle cuts 😎

And One thing i have noticed is, that the motor sounds a Lot more smooth , and is more quit. But how come exactly ?
```

---
