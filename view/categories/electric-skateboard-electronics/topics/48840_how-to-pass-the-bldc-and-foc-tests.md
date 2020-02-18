# How to pass the bldc and foc tests

### Replies: 20 Views: 537

## \#1 Posted by: Hummie Posted at: 2018-03-12T05:24:34.522Z Reads: 149

```
I don't know much about the vesc or getting things to spin on it.  If any of you can help adjust what I can to get things spinning as they normally do that would be a big help

https://www.youtube.com/watch?v=fMHt2ZYOC0k
```

---
## \#2 Posted by: scepterr Posted at: 2018-03-12T05:43:13.205Z Reads: 141

```
Try detection at 10A,
What's your power source btw?
```

---
## \#3 Posted by: Hummie Posted at: 2018-03-12T05:44:10.579Z Reads: 138

```
tried 10 and even up to 12.   just using 4s lipos
```

---
## \#4 Posted by: scepterr Posted at: 2018-03-12T05:44:34.208Z Reads: 130

```
Are your cutoffs set accordingly?
```

---
## \#5 Posted by: Hummie Posted at: 2018-03-12T05:46:00.628Z Reads: 130

```
aha .  probably not.  ill do that.  anything else?
```

---
## \#6 Posted by: scepterr Posted at: 2018-03-12T05:46:27.577Z Reads: 125

```
If it's that then no 😋

Also I've never personally done detection at such a low voltage, only for just testing vescs
```

---
## \#7 Posted by: Hummie Posted at: 2018-03-12T06:48:07.870Z Reads: 118

```
wow that did a lot now its really smooth and no cogging even with low current and whatever else, but still wont pass!  really strange as it's super smooth and always spins.  very encouraging!!!  It posted the alpha or whatever it is in the foc too.

no wonder it kept shutting off.  the low voltage cut off does a lot
```

---
## \#8 Posted by: scepterr Posted at: 2018-03-12T06:53:24.654Z Reads: 113

```
I would restore to defaults, refix the cutoffs and try again
```

---
## \#9 Posted by: Hummie Posted at: 2018-03-12T06:59:10.351Z Reads: 109

```
I did.  page by page and then changed the low voltage cutoff way down again.  it spins great in fact more consistently than any other motors but it wont pass the bldc test.  foc it passed everything.  
really nice to see.  been ages assuming something was wrong...and this here now passes great with the big 10mm magnets!  so they weren't even the problem.  

but would like to pass the bldc test still...not that I ever ride in it but still
```

---
## \#10 Posted by: scepterr Posted at: 2018-03-12T07:00:00.499Z Reads: 105

```
Do you have a different previously tested in bldc motor you can try?
```

---
## \#11 Posted by: Hummie Posted at: 2018-03-12T07:01:11.180Z Reads: 102

```
not now.  too much trouble to set up right now.  but good idea.  so these motors I have are good!  I'm gunna try live data and see if I can get that going and figure a kv
```

---
## \#12 Posted by: telnoi Posted at: 2018-03-12T07:50:20.836Z Reads: 82

```
Does it stutter at the very end of the run/detection?
```

---
## \#13 Posted by: Hummie Posted at: 2018-03-12T15:08:00.792Z Reads: 66

```
No stutter. Really smooth n controlled but won’t pass bldc. But good on foc
```

---
## \#14 Posted by: Blasto Posted at: 2018-03-12T15:15:31.735Z Reads: 67

```
for BLDC detection, in the detection parameters, there's a min erpm, try lowering that value (since you are detecting with 4S and have a low KV motor)
```

---
## \#15 Posted by: Blasto Posted at: 2018-03-12T15:24:53.994Z Reads: 69

```
you shouldn't need to play around with all those values you are talking about in your video (start up boost etc) to get the detection to work

but you do need to make sure of this:

set your  voltage limits properly (what @scepterr said) 

![image|644x194](upload://qSftqLsGLCNQvpj7wxSy9fbMhUB.png)

if your motor stutters upon detection, increase you current

![image|584x174](upload://1og9dMSVgSbvwUGkteAvTGGmVMN.png)

if the motor gives a heavy knock at the end of your detection, inscrea your "low duty" to 0.1

if all goes well and still fail, decrease your "MIN ERPM"
```

---
## \#16 Posted by: Acido Posted at: 2018-03-12T15:39:59.526Z Reads: 60

```
i think 6s is minimal
```

---
## \#17 Posted by: Hummie Posted at: 2018-03-12T15:46:00.784Z Reads: 60

```
I think 4s is doable but thanks for all the info. On bldc no stuttee and solid and smooth everytime which makes me think some box needs be changed. Low voltage cut off fixed a lot.
```

---
## \#18 Posted by: Blasto Posted at: 2018-03-12T15:50:52.490Z Reads: 59

```
What is the kv of your motor?
```

---
## \#19 Posted by: Hummie Posted at: 2018-03-12T16:29:02.978Z Reads: 51

```
I tried two different rotors and surprisingly the rotor with wider magnets has a higher kv at 85 and the rotor with the smaller magnets is 72kv.  (stators with 9 turns of 17awg in wye).
I would've assumed the opposite.  I guess the bigger magnets are not making a clean magnetic connection to the teeth and actually reducing the productive magnetic field.  ..but the inductance number showing on the vesc foc test with the 10mm mags is higher so that also is confusing.

at like 72kv and likely not having a problem running at 85% of the no-load the top speed with a 83mm wheel, I'm guessing at about 30mph
so syched to run these!!  sooooon.  I'd assumed there were problems with them because of my lack of vesc knowhow and couldn't get it to spin nicely with either rotor.  think the bldc test wont be a problem based on how awesome it spins and will do some adjusting written above.
```

---
## \#20 Posted by: Blasto Posted at: 2018-03-12T16:48:47.960Z Reads: 47

```
try to drop the MIN ERPM to 400-500
```

---
