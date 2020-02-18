# Battery experts, question for you guys

### Replies: 14 Views: 266

## \#1 Posted by: Taliesin Posted at: 2018-09-15T16:14:23.601Z Reads: 125

```
I am running a 12s4p 18650 pack.  I am charging with a voltage protector and I don’t let it charge past 49.9 volts.

When I start charging the battery meter rises at a steady pace, maybe 1% every few minutes.  But when the meter hits my max set voltage, and usually right around 90%, the chatging slows wayyyy down. Like 1% every 20-30 minutes. 

Is this because I have the voltage protector set at 49.9v?

Should I just consider the board fully charged at 90% or should I just be waiting an extra 3-4 hours for that last 10%? I realize that’s a subjective question but I guess I wanna make sure it’s not forcing the batteries to charge beyond 90% if I shouldn’t be, if that makes sense.
```

---
## \#2 Posted by: Acido Posted at: 2018-09-15T16:16:34.405Z Reads: 119

```
use volts not % 12s battery full charge at 4.2v is 50.4volts
at 4.1( studies saydouble life span) its 49.2
```

---
## \#3 Posted by: Okami Posted at: 2018-09-15T16:18:17.341Z Reads: 116

```
I guess it hits constant voltage phase so current goes down.. this is normal.

What 'voltage protector' do u use?
```

---
## \#4 Posted by: Taliesin Posted at: 2018-09-15T18:28:42.972Z Reads: 96

```
![image|281x500](upload://zdGkwMguhkcrJzoi9eYOSjMnIjJ.jpg)
```

---
## \#5 Posted by: Taliesin Posted at: 2018-09-15T18:29:04.141Z Reads: 87

```
Okay so basically harge it to 49.2 and call it a day
```

---
## \#6 Posted by: Okami Posted at: 2018-09-15T18:44:39.946Z Reads: 85

```
I guess u dont use bms, right? In that case it would go and balance cells at that level.

But yeh i guess u saturate battery quickly and it moves in its last charging stage, thats why its so slow at end..

Do u see amps also? At which level u start?

![IMG_20180618_114455|690x403](upload://gai80pHScRIK9tjPbF9FaV75Ohf.jpg)
Costs 10usd and lets see amperage / wattage / time / charged capacity
```

---
## \#7 Posted by: Taliesin Posted at: 2018-09-15T19:08:19.299Z Reads: 77

```
I believe I’m charging at 3 amps. I use a d596 80A bestech BMS
```

---
## \#8 Posted by: danielz Posted at: 2018-09-15T19:46:25.040Z Reads: 69

```
My bms for another project doesn't balance until the very end, so restricting the max voltage meant it wouldnt ever balance the cells, so i had get rid of the voltage limiter and charge to 100% Im not sure how other BMSs behave, maybe the point at which it balances it settable.
```

---
## \#9 Posted by: Taliesin Posted at: 2018-09-15T20:24:37.819Z Reads: 64

```
Interesting. How do I tell if my cells are getting balanced at the end or not?
```

---
## \#10 Posted by: trancejunkiexxl Posted at: 2018-09-15T20:30:00.155Z Reads: 64

```
i meaured p group in mine directly, and waited till i had different shrink, or just wrap with kapton (traps heat tho) meantime.
```

---
## \#11 Posted by: danielz Posted at: 2018-09-15T20:41:09.728Z Reads: 59

```
[quote="Taliesin, post:7, topic:68123"]
d596 80A bestech BMS
[/quote]
http://www.bestechpower.com/222v6spcmbmspcbforli-ionli-polymerbatterypack/PCM-D596.html

Says on there battery has to be fully charged to balance, is that yours?
```

---
## \#12 Posted by: Taliesin Posted at: 2018-09-15T21:00:45.772Z Reads: 52

```
Yes. So what I set my voltage protector at? The guy who built my battery said don’t go over 50v
```

---
## \#13 Posted by: danielz Posted at: 2018-09-15T21:43:59.237Z Reads: 46

```
I only have experience with one BMS, and it terminates the charge once balancing has complete. If you connect a multimeter inline in current mode you will see what the BMS is doing. I charge my cells with a simple cc/cv pcb. Its set to the maximum voltage of my pack. 4.2 x number of cells. 

I wanted to charge to 90% only, but id have lost the BMS balance function. So scrapped that idea.
```

---
## \#14 Posted by: kuphjr Posted at: 2018-09-16T01:35:24.630Z Reads: 36

```
I'm not sure why the person you bought it from told you this, but it is not correct (unless he meant to say 50.4V and not 50V).  You need to charge all the way to 50.4V for the balancing to work on that BMS.
```

---
