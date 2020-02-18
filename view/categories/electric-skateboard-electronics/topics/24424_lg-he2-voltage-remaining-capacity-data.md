# LG HE2 voltage/remaining capacity data

### Replies: 3 Views: 554

## \#1 Posted by: t0m_r1dd1e Posted at: 2017-06-02T15:47:12.563Z Reads: 60

```
I've been wanting to get a more accurate scale to estimate remaining battery percent based on its voltage. Since my battery is made from HE2's, I bought an extra one for testing. 

What I wanted to know: 
-Actual usable capacity
-At what point my VESC will go into low power mode during actual riding current draw.

Methodology:
I did three charge and discharge cycles on my lipo balancer, noting the voltage every 100 mah discharged. I hooked a multimeter up to the battery for voltage measurement. The first discharge was done slowly at 1.4 amps, stopping for 30 seconds to a minute every 100 mah to let the voltage recover. This was my resting voltage measurement. The next two were done without stopping at 5 amps and 3 amps. 

Results:
<img src="/uploads/db1493/original/3X/a/b/abbfb18c4d653b91ace4fd6a0955046851f8bcc3.PNG" width="690" height="430">

Conclusions I draw:
My battery is a 12s4p and I know that 12 amps is plenty if I'm being conservative. So I'll hit low power mode at 1900 mah and battery cutoff at just over 2000 mah when the cells hit 3.2v. So my real-world battery scale is this: 10% capacity per 200 mah drained. 

I found similar data for other cells online but couldn't find anything for this battery so I wanted to share this in case it's helpful for anyone else.
```

---
## \#2 Posted by: Maxid Posted at: 2017-06-02T16:22:49.236Z Reads: 51

```
There is your graph for all kinds of discharge currents:
http://lygte-info.dk/review/batteries2012/LG%2018650%20HE2%202500mAh%20(Red)%20UK.html

For easier reading maybe use this and choose your HE2
http://lygte-info.dk/review/batteries2012/Common18650comparator.php
```

---
## \#3 Posted by: t0m_r1dd1e Posted at: 2017-06-02T16:24:45.447Z Reads: 50

```
Oh nice! Wish I had found this a week ago haha
```

---
