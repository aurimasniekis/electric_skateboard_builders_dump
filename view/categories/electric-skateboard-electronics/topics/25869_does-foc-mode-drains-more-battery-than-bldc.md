# Does FOC MODE drains more battery than BLDC?

### Replies: 19 Views: 1117

## \#1 Posted by: NAF Posted at: 2017-06-21T19:03:02.756Z Reads: 260

```
Guys today I tried FOC for the first time with my CARVON Single hub v 2.5. My question is if the FOC MODE drains more battery juice than BLDC mode ?? Maybe I am all wrong ..but I've got the feeling that it eats up a lot more juice. Has anyone noticed that ?
```

---
## \#2 Posted by: anorak234 Posted at: 2017-06-21T20:14:32.667Z Reads: 256

```
why would it...?
```

---
## \#3 Posted by: sl33py Posted at: 2017-06-21T20:30:39.326Z Reads: 247

```
As i understand it - one of the main advantages of FOC is more efficiency.  Typically 5%ish improvement.

The benefits are efficiency, silent, better startup torque, but slightly less top speed.

I suggest searching FOC to get a better understanding - quite a few threads on ES in the eBike forum.  Cutting edge stuff...
```

---
## \#4 Posted by: Michael319 Posted at: 2017-06-21T21:15:37.616Z Reads: 231

```
I don't know if I agree with slightly less top speed. I'm running a single carvon v2.5 with a 12s2p, and I can hit 34-36mph easy on foc. But maybe at that voltage the difference is negligible.
```

---
## \#5 Posted by: treenutter Posted at: 2017-06-21T21:32:33.687Z Reads: 217

```
@NAF anecdotally - I haven't noticed an efficiency difference between the two. There are so many other factors that impact efficiency that the 5% increase seems negligible.
```

---
## \#6 Posted by: gee Posted at: 2017-06-21T22:04:47.725Z Reads: 208

```
so what's the difference between BLDC and FOC and the other one? I'm using the BLDC like everyone else but if FOC gives me more efficiency than I rather switch since I don't even go over 20 mph.
```

---
## \#7 Posted by: sl33py Posted at: 2017-06-21T22:15:18.848Z Reads: 200

```
[quote="Michael319, post:4, topic:25869"]
I don't know if I agree with slightly less top speed.
[/quote]

Top speed is definitely impacted from what i read and saw compared several months ago.  unless you test back-to-back with BLDC you likely wouldn't notice the small difference, but the experts tested and said it was there.  And i think you have to go to actual "top speed" not where you slow down as a reasonable person would when doing 35+mph...  on a skateboard...  (wear good gear! if you do test)

Again - I'm not an expert, so feel free to google and read up on FOC.  The best resources seemed to be the eBike guys.
```

---
## \#8 Posted by: sl33py Posted at: 2017-06-21T22:17:16.301Z Reads: 189

```
agreed - i don't know if the bikes are more consistent in usage so they can see the improvement better.  Or if they are super data-driven and have history(data logging) to prove the difference.

I know my range varies and totally depends on me - lots of variables from kicking a time or two to start, hills, and just heavier on the throttle will wipe out a small few % easily.
```

---
## \#9 Posted by: sl33py Posted at: 2017-06-21T22:31:31.213Z Reads: 178

```
[quote="gee, post:6, topic:25869, full:true"]
so what's the difference between BLDC and FOC and the other one? I'm using the BLDC like everyone else but if FOC gives me more efficiency than I rather switch since I don't even go over 20 mph.
[/quote]

Unless you are savvy enough to swap a DRV chip, and repair a dead VESC (4.xx) - i'd stick with BLDC.  I know lots of folks run FOC w/o issue - but i think that works best when you are conservative on voltage and settings.  

I'm not sure if the FOCBOX actually runs FOC better than a regular 4.xx VESC?  Like on 12s which seems a guaranteed dead DRV on FOC.

I have VESC's to spare, but still run BLDC for reliability.  Looking forward to trying FOC w/ the new VESC Six.
```

---
## \#10 Posted by: Mikenopolis Posted at: 2017-06-21T22:39:18.832Z Reads: 172

```
I've been debating on my future CarvOn V3 build, I got everything ready except the motor and bullet connectors. So would you recommend FOC with Enertion's VESC-X? 

I'm really intrigued by the quietness,
```

---
## \#11 Posted by: gee Posted at: 2017-06-21T22:44:07.136Z Reads: 170

```
Lol I'm so noob I had no idea what you're saying. I'll stick with BLDC.
```

---
## \#12 Posted by: Michael319 Posted at: 2017-06-22T01:25:39.310Z Reads: 157

```
FOCBOX technically will run FOC better than a standard 4.12. I personally run Ollins Direct Vesc, which is very similar to the focbox. And I haven't had a single issue.
```

---
## \#13 Posted by: Michaelinvegas Posted at: 2017-06-22T05:49:34.558Z Reads: 135

```
It would be foolish not to run FOC.... it's a special kind of silent
```

---
## \#14 Posted by: NAF Posted at: 2017-06-22T06:55:19.386Z Reads: 127

```
It's good to know ...maybe the battery drain that happened was because I got too excited when riding FOC for the first time, as I was riding like a maniac full speed uphills. But to be honest ...the difference between BLDC and FOC is night and day...and it's not only the SILENCE that you get from foc ..it's everything else too..smoother acceleration, better startup torque, smoother breaking..everything was better. I am using AXLE vesc which they modified the same way as Chaka's vescs, and it all works without any problems.
```

---
## \#15 Posted by: Michael319 Posted at: 2017-06-22T06:57:03.387Z Reads: 128

```
Well, although axles is similar. It isn't the same as chakas new vesc. He uses direct FETS with a huge heats ink.
```

---
## \#16 Posted by: NAF Posted at: 2017-06-22T06:58:05.654Z Reads: 127

```
Yes that's true...I am talking about the previous changes that CHaka made. I know that now he made it even better. But it seems like even with the previous changes AXLE vesc works really well.
```

---
## \#17 Posted by: gee Posted at: 2017-06-22T10:46:41.563Z Reads: 112

```
So I have diy torque board vecs, can I click the FOC option? Do you think it's safe?
```

---
## \#18 Posted by: NAF Posted at: 2017-06-22T11:46:33.185Z Reads: 108

```
I wouldn't do it with Torque boards vesc. From what I know it hasn't been upgraded just as Ollin, Axle and Enertion vesc's. Beside that it's not just clicking on FOC ..you need to configure the motor in four steps, but it is very easy with Extended BLDC TOOL by @Ackmaniac
```

---
## \#19 Posted by: DevinG Posted at: 2018-05-24T21:17:31.675Z Reads: 49

```
Do the values for each item in bldc mode carry over to foc mode? is that safe is what im asking
```

---
