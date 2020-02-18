# 10S4P Wiring Diagram, Bypass BMS, Does this look right?

### Replies: 11 Views: 5452

## \#1 Posted by: johnny_261 Posted at: 2016-11-12T04:30:21.236Z Reads: 483

```
Building a 10s4p and want to use the BMS for only charging as it is rated for low amps.

I haven't bypassed a BMS before, so wanted to verify if I'm supposed to wire the dotted line in my diagram or not.

Also, I didn't want to have a super long row of 20 cells x2 (these are 26650 cells), so I thought this layout, while wider, would be more space efficient.  How have you guys arranged your 10s4p? Just wondering if there are any other alternatives out there.

I think I got the rest down, since I did do a 6s2p with a BMS before, but any other tips are appreciated!<img src="/uploads/db1493/original/3X/e/3/e39f397b47d679aae50cd0023b3470d246e71ce3.jpg" width="496" height="500">
```

---
## \#2 Posted by: ch3m1st Posted at: 2016-11-13T04:13:05.716Z Reads: 412

```
Wouldn't the dotted line provide the ground, for the cells, while the charger is plugged in?
```

---
## \#3 Posted by: Jinra Posted at: 2016-11-13T07:47:37.796Z Reads: 401

```
Looks good, just make sure your breaker is anti-spark. the main B- may depend on how the BMS is wired.
```

---
## \#4 Posted by: johnny_261 Posted at: 2016-11-13T08:09:49.649Z Reads: 389

```
Yeah, but connection 0 also goes to negative, so that's why I'm not sure if B- is negative.
```

---
## \#5 Posted by: johnny_261 Posted at: 2016-11-13T08:14:20.810Z Reads: 376

```
Thanks, do you know how to test this?  connection 0 goes to negative, so I'm not sure if that is used for charging and B- is only for the discharge...Not really sure how to go about testing it
```

---
## \#6 Posted by: Jinra Posted at: 2016-11-13T08:32:36.455Z Reads: 362

```
B- isn't for discharge, only P- is. I think you'll need to use it to balance charge correctly.
```

---
## \#7 Posted by: gkeefe10 Posted at: 2017-11-16T03:16:00.629Z Reads: 250

```
So the dotted line has to be wired or the battery wont balance charge properly
```

---
## \#8 Posted by: clvnng Posted at: 2017-12-01T23:06:02.204Z Reads: 226

```
@Jinra
i'm interested to know this as well.
```

---
## \#9 Posted by: Jinra Posted at: 2017-12-01T23:26:02.614Z Reads: 224

```
It depends on the BMS, some will charge fine, some won't.
```

---
## \#10 Posted by: WillVill Posted at: 2019-03-11T12:07:22.886Z Reads: 87

```
Would it be possible to do the series connection with 0.15mm nickel strips? How many would I have to use for each series connection?
```

---
## \#11 Posted by: ESK8Erock Posted at: 2019-03-23T15:12:01.553Z Reads: 69

```
Depends on how many amps you are trying to supply.
```

---
