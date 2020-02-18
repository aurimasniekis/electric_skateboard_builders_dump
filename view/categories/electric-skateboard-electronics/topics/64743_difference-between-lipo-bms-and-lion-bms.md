# Difference between Lipo BMS and Lion BMS

### Replies: 13 Views: 1213

## \#1 Posted by: Itsmedant Posted at: 2018-08-13T13:18:04.089Z Reads: 163

```
Hey all! I've done some searching on this and still a bit confused!

I currently have a Besttech  HCX-D223V1. When I bought it, there was a selection for Lion or Lipo (both being 10s)

I've seen this BMS used in a lipo build from @Namasaki as well as mulitple Lion builds.

Is there a certain one for lipos and a different one for Lion, or is it the same damn BMS just being used for different batteries that are all 10s?

The reason I'm asking is that I got my hands on a DieBieBMS and was going to give this BMS to a friend who wants to do a lipo build.


Thanks!!
```

---
## \#2 Posted by: longhairedboy Posted at: 2018-08-13T13:22:40.053Z Reads: 161

```
as long as the BMS specs are in line with the cell specs it doesn't really matter if its li-ion or li-poly. 

as long as the minimum charge, maximum charge, and nominals are the same or within spec of the BMS, cell chemistry is mostly irrelevant.
```

---
## \#3 Posted by: Itsmedant Posted at: 2018-08-13T13:27:52.272Z Reads: 158

```
Nice!!! Thanks man, that was my thought all along but I'm wrong more times than not.

As usual @longhairedboy saves the day
```

---
## \#4 Posted by: Namasaki Posted at: 2018-08-13T15:11:14.250Z Reads: 138

```
The main concern is the over discharge detection. 
It is adjustable at the factory but 2.8v is the default unless the buyer requests a different value. 
2.8 is ok for Li-ion but it’s too low for Lipos. 

Both chemistries have the same full voltage if 4.2v
The difference is the min safe voltage. 
Li-ions can go a lot lower than Lipos
```

---
## \#5 Posted by: Itsmedant Posted at: 2018-08-13T17:24:41.894Z Reads: 122

```
So as long as he isn't ridding till its 0% he should be okay??
```

---
## \#6 Posted by: Namasaki Posted at: 2018-08-13T19:09:20.550Z Reads: 108

```
I would not recommended taking Lipo’s below 3.4v 
If the bms is set for Li-ions at 2.8v cutoff, 
It can still be used for Lipos but it will not protect the cells against over discharge
```

---
## \#7 Posted by: longhairedboy Posted at: 2018-08-13T19:13:13.237Z Reads: 104

```
i didn't realize lipos had such a high recommended cutoff voltage. So weird.
```

---
## \#8 Posted by: Itsmedant Posted at: 2018-08-13T20:11:52.879Z Reads: 97

```
With the lipos, the charging is more important right? (As far as balancing goes)

He is huge in to drone racing so he knows battery safety, I'll just have to make him aware of over discharging his batteries. I've been trying to convince him to get 18650s but apparently he knows people that work for turnigy and may be able to get a better deal through them.

If he does, I told him to bring it to the forum and hook everyone up!
```

---
## \#9 Posted by: Namasaki Posted at: 2018-08-13T21:26:32.481Z Reads: 85

```
I believe 3.0v is rock bottom for Lipos. 
I always recommend to stay well above that.
```

---
## \#10 Posted by: Andy87 Posted at: 2018-08-13T21:31:43.199Z Reads: 88

```
If he run a vesc based controller he could set there the battery cut off to 3.4-3.5v. 
With it the vesc cut off before the bms cut off would start. Safe the lipos from over discharge too
```

---
## \#11 Posted by: Silverline Posted at: 2018-08-13T22:29:02.460Z Reads: 80

```
If the BMS is bypassed, it dosn't matter what the discharge cutoff is. So maybe it's best that way, since he want to use lipo's
```

---
## \#12 Posted by: Itsmedant Posted at: 2018-08-14T00:06:06.838Z Reads: 72

```
Thanks to everyone here! You all are rock stars, this is hands down the best forum I've ever been on.

I'll let him know he can handle it through the VESC
```

---
## \#13 Posted by: Namasaki Posted at: 2018-08-14T00:17:14.811Z Reads: 69

```
No need to bypass with an 80a bms and low voltage soft back off strategy of the Vesc
Set the  Vesc low voltage start at 36v 
And low voltage end at 34v
And you’ll be good to go
```

---
