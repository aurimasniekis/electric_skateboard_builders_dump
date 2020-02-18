# Tips for the LiPo batteries to last longer

### Replies: 25 Views: 2524

## \#1 Posted by: tueboard Posted at: 2016-09-16T10:41:43.057Z Reads: 231

```
i read some tips in this forum and others from internet, but i don't know if all of them are true.

note: i'm not an expert, i broke my first two lipo batteries.

1- don't fully charge the batteries, stop the charge at 4.19 because if you are using a VESC you can overcharge them when you use the brakes.
2- don't discharge them below 3.7v, if you want to charge them full the heat can break them.
3- don't charge the batteries quickly after use,  wait a while to cool them.
4- use a lipo alarm buzzer to control the charge.
5- don't use batteries in series with different specs.
6- don't use batteries with a lot of difference charge load.
7- charge batteries one by one.
8- charge batteries in series is dangerous.
9- don't charge above 4.2V.
10- for a longer lifespan is better to use the "balance charge" mode.
11- use the storage mode if you are not going to use the batteries in 3 days.
12- calibrate your balance charger before charging.
13- never leave a charger unattended.
14- if you battery has 2200mAh would be charged at no more than 2.2A, but it's better to charge at 1.1A.

what do you think? if do you know more tips share it on the comments below

thanks
```

---
## \#2 Posted by: 2-alex-2 Posted at: 2016-09-16T10:49:45.233Z Reads: 225

```
Most seem ok only one I don't agree with is charge in series as long as it's wired correctly should have no issue. But what I would say is I could be more dangerous to charge in parallel as you could get false reading if a sell is down, where as in series if a cell goes down it will show.
```

---
## \#3 Posted by: mattdig Posted at: 2016-09-16T11:22:27.352Z Reads: 211

```
I thought LiPos could be discharged down to around 3.4V.
```

---
## \#4 Posted by: PB1 Posted at: 2016-09-16T12:25:05.638Z Reads: 209

```
Hmm, there are some good points in there. I would correct some statements. 

1- don't fully charge the batteries, stop the charge at 4.19 because if you are using a VESC you can overcharge them when you use the brakes
*** agreed, this really extends the battery life. I would even suggest stopping at 4.15 or 4.17V (and has nothing to do with VESC)

2- don't discharge them below 3.7v, if you want to charge them full the heat can break them.
*** That is very conservative. You should be able to discharge your LiPos down to 3.3V. Personnaly I've set soft cutoff at 3.4V and hard cutoff at 3.1V. 

3- don't charge the batteries quickly after use, wait a while to cool them.
*** Yes, this is considered as best practice 

4- use a lipo alarm buzzer to control the charge.
*** You probably mean DIScharge. Yes, you "something" to control discharge (Buzzer, volt meter, VESC, ..)

5- don't use batteries in series with different specs.
*** Yes, because all of the current flows through every battery. IF you do use different specs batteries in series, your amp limit should be the "weakest" battery. 

6- don't use batteries with a lot of difference charge load.
*** Yes. 
And IF you do limit amps and volts to your weakest battery. 

7- charge batteries one by one.
*** Yes. Unless you know exactly what you're doing and then still double check that everything is connected properly. 

8- charge batteries in series is dangerous.
*** Yes, sort of. At least if you don't know what you're doing. 
And if you do, make sure you have the right control mechanisms in place (e.g. monitor every cell). 

9- don't charge above 4.2V.
*** Yes, correct, very important! Never ever charge above 4.2V! Never!

10- for a longer lifespan is better to use the "balance charge" mode.
*** Yes.
And if you're an impatient person, use balance charge every 2nd, 3rd or 4rd charge. Or if your cells have become unbalanced. 

11- use the storage mode if you are not going to use the batteries in 3 days.
*** This is very conservative. 
I would say use storage mode if you are not going to use the batteries in 3 months. 

12- calibrate your balance charger before charging.
*** Ok

13- never leave a charger unattended.
*** Yes, yes, yes
And you should also understand WHY as this could extend YOUR life or the life of your house. *)

14- if you battery has 2200mAh would be charged at no more than 2.2A, but it's better to charge at 1.1A.
*** General rule is that max battery charge amp limit is 1C (2200mAh => 2.2A). Unless the spec of the battery is different. 

*) if you overcharge Lipos or discharge them to a very low level and then draw many amps they can heat up. This heating up can result in a so-called thermal runaway where the Lipos can get very very hot. So hot that things around the Lipos can catch fire. 
This does normally not happen when you're charging your Lipos with a nice charger. 
However if your charger is broken or has a malfunction or even the wrong settings it could overcharge your Lipos. No good!
```

---
## \#5 Posted by: NNGG Posted at: 2016-09-16T21:55:17.433Z Reads: 151

```
There are some turnigy nanotechs that are 1500mah and an be charged at 5amps. It all depends on battery chemistry and if you want them to live long. I charge my lipos overnight at .5amps.
```

---
## \#6 Posted by: lowGuido Posted at: 2016-09-16T23:42:01.023Z Reads: 147

```
I don't agree with point 8.
everyone charges batteries in series every day. its the normal thing to do.
```

---
## \#7 Posted by: Namasaki Posted at: 2016-09-17T05:50:41.457Z Reads: 141

```
I disagree with three...
1>3.4 is a totally safe discharge limit.
2>Balance charging packs in series is perfectly fine as long as they are matched(mah and C rating) and each cell is monitored.
3>balance charging every 2nd, 3rd or 4th charge is not good enough. Lithium batteries need to be balanced in every charge cycle.
I always do a full charge 4.2v. Full Balancing occurs at full charge, not below full charge.
```

---
## \#8 Posted by: PB1 Posted at: 2016-09-17T10:31:16.302Z Reads: 134

```
[quote="Namasaki, post:7, topic:9683"]
I always do a full charge 4.2v. Full Balancing occurs at full charge, not below full charge.
[/quote]

You can extend battery life by not going the full 4.2v. I've set up my balance charger to 4.15, so you can balance below 4.2

As for balancing at every charge, I really don't see a reason. I only balance if my cells have drifted.
```

---
## \#9 Posted by: Jinra Posted at: 2016-09-17T10:41:21.362Z Reads: 132

```
I don't think this does anything. It's true not going to full charge extends cycle life, but i think .05v is too small. Common recommendation is 80% which is about 4.0v or so.
```

---
## \#10 Posted by: mattdig Posted at: 2016-09-17T13:16:31.393Z Reads: 127

```
Tesla considers "full charge" on its packs to be 80% for longevity.
```

---
## \#11 Posted by: Namasaki Posted at: 2016-09-17T14:47:15.893Z Reads: 120

```
Ok, your right. 
I forgot that you can adjust end voltage with a balance charger. 
I'm using a BMS and dumb charger and my BMS only balances when the battery is fully charged. 
But I'm ok with that. I'll get max performance and range and replace the batteries when they wear out.
```

---
## \#12 Posted by: Namasaki Posted at: 2016-09-17T21:44:08.085Z Reads: 122

```
[quote="mattdig, post:10, topic:9683, full:true"]
Tesla considers "full charge" on its packs to be 80% for longevity.
[/quote]

They have to do that. imagine what those batteries cost!
And they don't want to have to replace them under warranty.
Plus they need to have extra safety margin.
```

---
## \#13 Posted by: tueboard Posted at: 2016-09-30T15:53:23.619Z Reads: 98

```
i've 2 lipos x 6s = 12s, it's safe to ride if one lipo is charged at 3.90v per cell and the other 4.10v per cell?

there is any limit of the cell charge between different lipos without break them?
```

---
## \#14 Posted by: SORRENTINO Posted at: 2016-09-30T16:04:13.723Z Reads: 96

```
Always balance charge unless you want to burn your house down one day because of a bad or high internal resistance cell. Biggest threat to your lipo is over discharging it. This does the most damage and will shorten your life span for the lipo.
```

---
## \#15 Posted by: SORRENTINO Posted at: 2016-09-30T16:06:01.327Z Reads: 94

```
No that a serious problem. You need to balance your cells when you charge them. If one cell is struggling to charge of is constantly lower then the others that an indication of a failing cell. It should be replaced or the lipo pack is no good anymore.
```

---
## \#16 Posted by: tueboard Posted at: 2016-09-30T16:08:23.567Z Reads: 90

```
yes, always i do the balance charge, i've two big batteries of 8000mAh and takes a lot to charge and want to know if is safe to ride if one battery is 90% charged and the other is 85% charged. thank you
```

---
## \#17 Posted by: SORRENTINO Posted at: 2016-09-30T16:10:50.618Z Reads: 89

```
Extending battery life by not charging to 4.2 is a myth. You always balance charge because if your IR is off on the cells some cells will charge faster then others causing some cells to be higher then 4.2v at the end of the charge and this is how fires start.
```

---
## \#18 Posted by: SORRENTINO Posted at: 2016-09-30T16:16:07.647Z Reads: 85

```
Oh ok I read that wrong should be ok but I think its bad practice. You could throw it on a balance board ( connect them in Parallel)  for a few minutes and they should even out each other before riding.
```

---
## \#19 Posted by: maxchilton Posted at: 2016-09-30T16:29:53.952Z Reads: 83

```
[quote="SORRENTINO, post:17, topic:9683, full:true"]
Extending battery life by not charging to 4.2 is a myth. You always balance charge because if your IR is off on the cells some cells will charge faster then others causing some cells to be higher then 4.2v at the end of the charge and this is how fires start.
[/quote]

You are wrong, it's not a myth.  

http://batteryuniversity.com/learn/article/how_to_prolong_lithium_based_batteries
```

---
## \#20 Posted by: mattdig Posted at: 2016-09-30T16:34:05.852Z Reads: 80

```
You could do this for a short ride in an emergency, but I STRONGLY advise against it simply because you could think you've got lots of power left from the higher charged pack, while you're over draining the lower charged pack and ruin it completely. Always stick with equally charged packs.
```

---
## \#21 Posted by: Jinra Posted at: 2016-09-30T16:39:04.176Z Reads: 77

```
I knew it wasn't a myth but this is very interesting

> Most Li-ions charge to 4.20V/cell, and every reduction in peak charge voltage of 0.10V/cell is said to double the cycle life. For example, a lithium-ion cell charged to 4.20V/cell typically delivers 300–500 cycles. If charged to only 4.10V/cell, the life can be prolonged to 600–1,000 cycles;
```

---
## \#22 Posted by: tueboard Posted at: 2016-10-06T00:11:22.717Z Reads: 71

```
one dumb question... if the battery has higher c rating (ex. 35c vs 20c) the motor goes faster but lasts less time, this is right?
```

---
## \#23 Posted by: Jinra Posted at: 2016-10-06T00:32:09.078Z Reads: 68

```
Nope, voltage determines the speed of the motor. The C rating is merely the discharge potential of the pack. Higher C rate = less voltage sag.
```

---
## \#24 Posted by: DivenParker Posted at: 2016-11-04T03:09:11.650Z Reads: 60

```
 if you battery has 2200mAh would be charged at no more than 2.2A, but it's better to charge at 1.1A. I have a [2200mAh lipo battery](http://www.genstattu.com/ga-b-25c-2200-3s1p-deans.html), so I need charge low than 2.2A?
```

---
## \#25 Posted by: jmasta Posted at: 2016-11-04T03:45:52.975Z Reads: 58

```
It is generally recommended to charge Lipos at 0.5C
```

---
