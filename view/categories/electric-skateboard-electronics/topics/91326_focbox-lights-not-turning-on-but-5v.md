# FOCBOX Lights not turning on, but 5V

### Replies: 25 Views: 413

## \#1 Posted by: Jamie42 Posted at: 2019-04-21T17:23:23.827Z Reads: 94

```
Hi,

Today I plugged my FOCBOX into my computer and then powered my FOCBOX with a battery. The FOCBOX then didn't turn on while it worked 5 minutes before.

After reading a bit around here I took these measurements:
Measuring 5V on UART port: 5.12v
Measuring 3.3v on UART port: 0.3v 
When I put my multimeter in "check" mode and short the leads: 002
Measuring C25 on one end to ground (of can port): 008
Measuring C25 on the other end to ground (of can port): 002

I also took some pictures:

![FOCBOX%20bottom|375x500](upload://jh8VJmFly6ayn9lEGeq51XoqZ2G.jpeg) ![FOCBOX%20top|375x500](upload://balRNpSai8SnXmSVVWfq6L5CndQ.jpeg) 

Can anyone help me?
```

---
## \#2 Posted by: Sn4pz Posted at: 2019-04-21T23:10:01.981Z Reads: 71

```
As far as my (incredibly impaired) eyes can see, you should be fine :) 

I wonder if these two bigger bits are always that... crusty? Maybe that has something to do with your issue :thinking: ![image|690x255](upload://psYAW7FpwEMCF5oRdrih1TdAViy.jpeg)
```

---
## \#3 Posted by: dareno Posted at: 2019-04-22T00:22:18.740Z Reads: 66

```
Is it one of a pair or a single motor set up?
Are there any lights on at all?  Flashing?
Is it under warranty?
```

---
## \#4 Posted by: Dornacht Posted at: 2019-04-22T01:45:51.871Z Reads: 66

```
If knowledge serves correct, it is most likely the can chip, I have this problem on one of my focbox and replaced it but still doesn’t work
```

---
## \#5 Posted by: Jamie42 Posted at: 2019-04-22T08:26:07.013Z Reads: 57

```
Is is a single motor setup, so no connections through the CAN port. No lights on at all, except the one on my receier that gets 5V through thr COMM port. And I don't think it's under warranty.
```

---
## \#6 Posted by: Jamie42 Posted at: 2019-04-22T08:26:59.585Z Reads: 56

```
So what should I do, remove it? What will happen then? Can I only not use can or does it have other consequences?
```

---
## \#7 Posted by: dareno Posted at: 2019-04-22T09:24:17.088Z Reads: 50

```
You can remove the canbus chip and it will either work or it won't but if it was the chip that was causing the issue then the focbox will be alive again.  The can bus chip won't affect anything else or make things worse except linking another via can bus.
```

---
## \#8 Posted by: Jamie42 Posted at: 2019-04-22T10:16:35.949Z Reads: 40

```
Can it even be the CAN chip if it wasn't using CAN?
```

---
## \#9 Posted by: dareno Posted at: 2019-04-22T18:18:13.057Z Reads: 34

```
It could be any number of things to be honest but as i said it is behaving like a focbox with a blown can bus chip.  No lights but still retaining the bec voltage.  Its also something you can do yourself with a small pair of side cutters. If you want it repaired then there are a few guys that offer that service here.

I believe @Martinsp does focbox repairs in europe very reasonably priced.
```

---
## \#10 Posted by: Mich21050 Posted at: 2019-04-22T18:22:16.023Z Reads: 34

```
Maybe the wizard himself could shed some light on this... @JohnnyMeduse :slight_smile:
```

---
## \#11 Posted by: Jamie42 Posted at: 2019-04-22T19:22:09.217Z Reads: 33

```
Ok, guess I will try to remove the CAN chip then.
```

---
## \#12 Posted by: dareno Posted at: 2019-04-22T19:26:17.899Z Reads: 32

```
I brought 2 back to life by removing the chip.  It was a failing on the earlier versions of the focbox but they fixed it just before discontinuing them lol
Wait till one of the real experts chime in before attacking it though.
```

---
## \#13 Posted by: Jamie42 Posted at: 2019-04-22T19:28:53.655Z Reads: 32

```
Ow wow, that can chip should have protection from this kind of crap... Hope someone that really knows VESC's will help on this.

Just for the reference: Were you using the can port with the vesc's that had a broken can chip or not?
```

---
## \#14 Posted by: dareno Posted at: 2019-04-22T19:34:18.827Z Reads: 30

```
If you disconnected power to one vesc while the can bus was connected it blew both chips.  If you removed the can bus cable while powered up it blew one.  I did it trouble shooting a seperate issue and blew both.  I just use split ppm now.
```

---
## \#15 Posted by: Jamie42 Posted at: 2019-04-22T19:44:16.167Z Reads: 32

```
See and that's the thing, I read a lot about this here and it when it was the can chip, poeple used can...
```

---
## \#16 Posted by: dareno Posted at: 2019-04-22T19:52:04.951Z Reads: 32

```
But that doesn't mean it can't just fail on you.  I can only go on what the symptoms are without a good look at the board. Most other common faults display flashing lights although my focboxes have always been good in that regard.
```

---
## \#17 Posted by: Jamie42 Posted at: 2019-04-22T19:59:40.423Z Reads: 31

```
Yeah that's true, and I get that you can't further diagnose. 

Thanks!
```

---
## \#18 Posted by: dareno Posted at: 2019-04-22T20:02:07.238Z Reads: 30

```
I'm the sort that would have snipped them off by now because its already bricked and what have you got to lose?  But thats just me lol
and you are very welcome just sorry I couldn't have been more helpful.
```

---
## \#19 Posted by: Jamie42 Posted at: 2019-04-22T20:14:32.543Z Reads: 27

```
Heat gun and a tong right? Will try that tommorrow when I'm back home... 

And don't be sorry! You were more helpful than I was to myself!
```

---
## \#20 Posted by: dareno Posted at: 2019-04-22T20:21:00.914Z Reads: 25

```
I used a small pair of side cutters and snipped the tags off.  Its quite a big chip so you don't need to de solder it.  Good luck
```

---
## \#21 Posted by: Jamie42 Posted at: 2019-04-22T20:22:23.036Z Reads: 24

```
Tommorrow. I'Il report my results back here. Thanks!
```

---
## \#22 Posted by: dareno Posted at: 2019-04-22T20:29:11.387Z Reads: 23

```
In case you don't know this is the little bastard.
![image|640x480](upload://4Yt0pZY8G2qhiRxNGX2adimCnR5.jpeg)
```

---
## \#23 Posted by: Jamie42 Posted at: 2019-04-22T20:31:42.199Z Reads: 23

```
Yep I know, U401. One more question: Do I have to discharge any capacitors or anything?
```

---
## \#24 Posted by: dareno Posted at: 2019-04-22T20:33:20.224Z Reads: 23

```
I didn't but mine were powered down for ages before I did the deed.  Like you I was all over here asking questions before I got the right answers.
```

---
## \#25 Posted by: Jamie42 Posted at: 2019-04-22T20:34:41.166Z Reads: 22

```
Mine powered down for one day now, anyone here that can tell me whether to discharge the capcitors?
```

---
