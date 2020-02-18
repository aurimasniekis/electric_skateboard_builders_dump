# Is the VESC 4.12 energy measurements reliable?

### Replies: 3 Views: 425

## \#1 Posted by: Fatglottis Posted at: 2017-09-16T13:57:42.988Z Reads: 67

```
Hi guys!
I have some issues regarding energy measurements.

I have a 15Ah battery connected to two VESCs 4.12 (different brands). According to them they each consume ~1,2Ah on a 7,8km ride (~5miles). That is a total of 2,4Ah. If I use 12Ah of my battery, that should then give me a range of 50km (~30 miles). This is far from the truth unfortunately. It's like a factor 2 wrong.

When I charge the battery after a 7,8km (5miles) ride with initially fully charged battery, **I get ~4,3Ah!!** into the battery according to the IMAX b6 clone. **Not the 2,4Ah stated by the VESCs.**
Using 4,3Ah in my calculations makes much more sense since I have around 25km range (15miles).
( 12Ah / 4,3) * 7,8km =  22km. 

To add confusion.. I don't actually know the status of the cells. It is possible that they were aged before I got them and it would explain that I don't get the 50km range. However, my two IMAX b6 clones I use for charging tells me another story. Not sure what to believe now. Either both IMAX chargers measures wrong, or both VESCs measures wrong..  or my thinking is wrong :D 

**So two questions:**
**1. Are the VESC energy measurment accurate and if so, what am I doing wrong?**
**2. I can only see two current shunts and they are for the phase current measurement. Does it mean the I_DC is calculated and not measured?**

Here is a screen shot of energy calculations for a typical 7,8km ride. 
3,5 *2,24 = 7,8km. 
Don't mind the 0,4V battery voltage offset on VESC 2.<img src="/uploads/db1493/original/3X/a/f/af81c953cb69a346e7b90185b52e47df9ecec62c.png" width="690" height="225">
```

---
## \#2 Posted by: Chewie Posted at: 2017-09-16T14:07:15.371Z Reads: 60

```
Interesting, sure sounds like your VESC measurement isn't accurate.  I might have to go back to my Lipo setup so I can charge them on my RC charger and test mine...
```

---
## \#3 Posted by: ThierryGTLTS Posted at: 2017-09-16T15:37:12.044Z Reads: 50

```
My VESC battery current measurement is not accurate!

Tested with an very old but good HP power supply.

Thierry
```

---
