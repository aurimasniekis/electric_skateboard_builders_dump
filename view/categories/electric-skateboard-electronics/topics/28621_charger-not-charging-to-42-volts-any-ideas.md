# Charger not charging to 42 volts&hellip;any ideas?

### Replies: 17 Views: 904

## \#1 Posted by: marcus Posted at: 2017-07-25T20:52:22.997Z Reads: 95

```
Hey guys,

So I tried out my second charger and it again is only charging to 40 volts when I plug it in...I bought one of the 42 volt balance board chargers off of Amazon and as you'll see in the photo, it turns green and registers as fully charged...yet that is clearly not true...do these chargers have internal voltage cutoffs?? I'm lost...my BMS is wired properly and everything😐Any help would be great...<img src="/uploads/db1493/original/3X/a/4/a4c658b46251045b7c90dd684ae8157eb86b9337.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/1/9/190fdd0960ab0a287774e0f17f85d9229631a299.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/e/f/efda53d893b4febfa8445cce8d996474a887fd83.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/c/2/c2b918aacf58a2a177b03aec16221ba1777e77f4.JPG" width="375" height="500">
```

---
## \#2 Posted by: Jinra Posted at: 2017-07-25T20:58:19.788Z Reads: 88

```
That BMS doesn't look like one with balance charging. Do you have a link? It could be hitting over voltage on a cell group and cutting off charging. Take out the JST header and measure the voltage of each group using the leads from the header.
```

---
## \#3 Posted by: marcus Posted at: 2017-07-25T21:04:22.366Z Reads: 87

```
here it is:
http://s.aliexpress.com/FrA7jqUr

I've bypassed it on discharge. It should be balancing though..all of the balance leads are covered by tape and I just measured each cell earlier and they are all the same voltage (3.6 at the time)
```

---
## \#4 Posted by: Jinra Posted at: 2017-07-25T21:06:13.296Z Reads: 82

```
I mean measure the balance leads when your charger cuts off to see if one group is higher voltage than the others.
```

---
## \#5 Posted by: Jinra Posted at: 2017-07-25T21:07:42.832Z Reads: 80

```
You have 3 cables going to battery negative right? Two on the BMS and one for discharge?
```

---
## \#6 Posted by: marcus Posted at: 2017-07-25T21:11:13.295Z Reads: 78

```
Yes I do. And every cell is 3.8 average...
```

---
## \#7 Posted by: Tuomalar Posted at: 2017-07-25T21:13:11.433Z Reads: 72

```
I had this same problem two times because spot welding failed so bms charged one 4p group as 3p. Bms stopped charging both times at 40v. I think bms cut it there because of over voltage in broken group.
```

---
## \#8 Posted by: marcus Posted at: 2017-07-25T21:13:14.827Z Reads: 71

```
Weird eh?..
```

---
## \#9 Posted by: Jinra Posted at: 2017-07-25T21:14:25.242Z Reads: 73

```
so then it's only charging to 38v? For some reason the BMS cut off charging thinking something went wrong.

If you made sure each group has not hit 4.2v then I'd suggest using the battery to trigger the overvoltage release and try charging again.
```

---
## \#10 Posted by: marcus Posted at: 2017-07-25T21:15:45.847Z Reads: 67

```
This happens every time I try to charge..how would I do that?
```

---
## \#11 Posted by: Jinra Posted at: 2017-07-25T21:16:21.239Z Reads: 64

```
So you've already discharged and charged the pack several times?
```

---
## \#12 Posted by: marcus Posted at: 2017-07-25T21:17:18.555Z Reads: 62

```
Yes. I'm thinking on of my parallel connections came loose...it is 10s3p pack..of that happened that could be the problem?
```

---
## \#13 Posted by: Jinra Posted at: 2017-07-25T21:18:42.908Z Reads: 59

```
Yea, that's why I asked you to check the voltage of every group. If a cell got loose and became a 2P or 1P group, it would get to 4.2v earlier than the rest of the groups causing and overvolt cutoff
```

---
## \#14 Posted by: marcus Posted at: 2017-07-25T21:24:26.875Z Reads: 62

```
Durp, stupid question I asked :smile: Update: so when I plugged  the JST balance connector back in it start charging again....the light is back to red! The saga continues...

Also: with this new charger it only charged to 38 volts and my old 42 volt charger charged to 40 volts before it stopped. Not sure why they differed but I guess I'll see what happens now as it started charging again!
```

---
## \#15 Posted by: marcus Posted at: 2017-07-25T21:39:53.676Z Reads: 62

```
Well one of the parallel connectors just may be broken..went back to check again and one cell reads 4.1 while the others are around 3.8...that may be it
```

---
## \#16 Posted by: Jinra Posted at: 2017-07-25T21:40:12.020Z Reads: 63

```
Yep, that's what it sounds like
```

---
## \#17 Posted by: ihatetopush Posted at: 2018-01-19T09:08:34.277Z Reads: 39

```
Had the same problem then i bought this 900w 15a DC Boost Converter 8-60v to 10-120v NC CC CV Power Module LED Solar![$_58|500x500](upload://jMzokJjdpL7Jmmszb5G3zQbq58H.JPG)


a few  video about it

https://www.youtube.com/watch?v=0Z5QWzSSvdI

https://www.youtube.com/watch?v=4HAQhN6_cnM


You still need to use a 12volt  power supply   out of old pc free  or 48volt  hp severe power supply  even better

I can charge my battery in less than 1 hour love it 

You should not have to disconect bms and you can charge right up to 42 i set mine to 41 volt
```

---
