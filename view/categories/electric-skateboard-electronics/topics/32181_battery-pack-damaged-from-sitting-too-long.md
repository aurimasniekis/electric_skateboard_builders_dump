# Battery pack damaged from sitting too long?

### Replies: 11 Views: 668

## \#1 Posted by: surprisebirthday Posted at: 2017-09-03T20:59:50.738Z Reads: 157

```
This summer I left my board with a friend while I walked the earth for 3 months.  The board was barely ridden, and my friend said he didn't ride it for the last 1.5 months.  Now that I'm back, I've started to ride again, but noticed that the board is shutting off early and seems to pack less punch.

Is it possible my battery drained and some cells are asleep now?  Is it possible some wires connecting the cells became loose?  Problem with BMS?  

I realize this might be a hard question to answer without opening things up, so if it's required, I'll definitely open this puppy up -- just wanted to avoid accidentally damaging something if not needed.

**Symptoms**:
- Board suddenly loses power when when the battery indicator shows around 46% left.  This is much earlier than I the board ever shut off on me before.  Same riding conditions as before.
- Board shuts off even on slow acceleration when the battery indicator is around 46%
- Board will not power back on immediately; requires resting for a few minutes or being charged
- Motors strain and cog at low speeds, something that did not happen before. Pushing off a little harder resolves the issue.

**Board Details:**
- 10s3p 18650
- Dual 1st gen Hummie Hubs
- Ollin 4.12 VESCs, 2.18 firmware

Thanks for any insight, guys!  

If all else fails, this will give me an excuse to learn how to build my own pack. :smile:
```

---
## \#2 Posted by: GrecoMan Posted at: 2017-09-04T00:22:37.609Z Reads: 134

```
Check the pack voltage. And if possible, check the voltage of each cell
```

---
## \#3 Posted by: thisguyhere Posted at: 2017-09-04T01:09:04.499Z Reads: 127

```
[quote="surprisebirthday, post:1, topic:32181"]
walked the earth
[/quote]

![alt text](http://1.bp.blogspot.com/-fJFwsl8AYoI/Ta5dRLZ0L1I/AAAAAAAAAaI/7emUaAlUM6g/s1600/pulpfiction00005.png "")
```

---
## \#4 Posted by: thisguyhere Posted at: 2017-09-04T01:12:06.500Z Reads: 125

```
Yea check each parallel group. 

Open it up, take balance leads out of bms, ground your voltmeter on battery negative and touch each balance lead in sequence. 

May or may not have a dead cell.
```

---
## \#5 Posted by: surprisebirthday Posted at: 2017-09-04T05:28:27.706Z Reads: 113

```
<img src="/uploads/db1493/original/3X/3/4/343ef5364b5088e9f633220ba503f49abb0d24c4.gif" width="500" height="250">
```

---
## \#6 Posted by: surprisebirthday Posted at: 2017-09-04T05:33:02.090Z Reads: 107

```
Okay, got it.  I wasn't sure how to test things without breaking apart my entire pack cell by cell, but this sounds like a good way to identify where the problem is.

Thanks for the guidance.
```

---
## \#7 Posted by: chuttney1 Posted at: 2017-09-04T05:35:41.853Z Reads: 104

```
Definitely, check the voltage of the pack. I revived my 10S5P Samsung 25R pack from 1.6 volts per cell. It was very stressful knowing this is bad for the battery and may result in a fire charging it back up to normal. Glad there is no fire. Not trying to push my luck.
```

---
## \#8 Posted by: Maxid Posted at: 2017-09-04T07:20:40.959Z Reads: 92

```
If the voltage of the voltage meter says 46% and it was close to that when you left, the pack itself should be fine. I'd check the vesc settings - maybe it resetted to default values after a certain amount of time without being powered and you are hitting a low voltage cut off.
```

---
## \#9 Posted by: surprisebirthday Posted at: 2017-10-28T16:08:42.673Z Reads: 62

```
First, thanks to everyone who has chimed-in with help.

I opened up the pack and used a multimeter to measure each of the cells.  The pack wasn't fully charged, maybe around 72%.  Most of the cells were about the same voltage, but there were a few that were off.  The biggest difference was 0.7.  

Here's my new theory on what happened: I was intentionally not charging my pack too 100%, because my morning commute starts downhill.  One time I lost my brakes after I had charged to 100%, so I started to charge it to around 90%.  I'd been doing this months.  I read that a BMS will balance charge AFTER the pack is charged to 100%, so my new theory is that my cells have drifted over time, and I haven't balanced my pack in a long time.

Questions:

* If I charge my pack to 100% and leave the charger plugged in, will the BMS balance my cells for me?
* How long should I leave it plugged in?  The charger light will turn green at some point, but I'm not sure whether I should continue to leave it plugged in.
* Is this safe to do given how far apart my cells are?  I'm happy to just try it out and report back as long as people think this is still safe to do.

In case, it's useful, here's the voltage readings on each of the cells.  This is a Spacecell 10s3p

4.06	
4.07	
4.08	
3.37	
3.94 
3.68	
4.07	
3.96	
4.08	
4.08

Thank you!  Looking forward to riding again without worrying that my board will go up in :fire:
```

---
## \#10 Posted by: ThierryGTLTS Posted at: 2017-10-28T16:55:14.604Z Reads: 50

```
Try to charge it longer than normal and check once again.

3.37V is almost dead, 3.68V can perhaps recover, others are good.

Thierry
```

---
## \#11 Posted by: Okami Posted at: 2017-10-28T17:04:30.272Z Reads: 49

```
I think he said spacecell.. so i think 3.4 is not that bad, bad would be close to 2.5v..

So i sure hope @surprisebirthday your cells recover, u should do periodic checks now to see whenever everything is good as that cell might be weaker..

I dont have the option to go into details but u should look up how to start balancing earlier or just attach battery monitor after a few balance charges to see at what level the cells are..
```

---
