# Ebay BMS, where da batteries go?

### Replies: 9 Views: 626

## \#1 Posted by: mmaner Posted at: 2017-08-14T17:21:32.141Z Reads: 104

```
So I'm looking at this [BMS](http://www.ebay.com/itm/60A-Lithium-Ion-7S10S13SBleeding-BMS-30A-60A-with-electronic-Switch-BMSOn-Off-/222373438930?var=&hash=item33c67d65d2) on Ebay, looks decent for $22.  But I cannot understand this diagram...

<img src="/uploads/db1493/original/3X/9/e/9ea5e3c8718b9ccf784052e56cd161fc80251331.png" width="500" height="421">
Normally the **B-** port is usually the **NEG from the battery** pack, the **C-** port is usually the **NEG for the charge port**, the **P-** port is usually the **NEG for the LOAD**, or VESC's in this case.  If that can be assumed to be true then I assume I would connect as normal and the POS does not connect to the BMS at all, but then it says "the common positive B+", and It just got confusing as hell.  Plus the color codes are non-standard, so I'm not sure if the black or the blue is POS or if any of them are POS!

Any advice would be greatly appreciated.
```

---
## \#2 Posted by: darkkevind Posted at: 2017-08-14T17:35:08.252Z Reads: 89

```
This looks right to me. The positive (the last wire connected,  B10?) Gets used by the BMS for all the positives of the other cells for balancing...

Mine's the same if I remember correctly.

Although I actually bypassed discharge from the BMS in the end and let the VESC handle discharge limits. Even though my BMS is rated for 80A discharge! :confused:
```

---
## \#3 Posted by: mmaner Posted at: 2017-08-14T17:53:09.416Z Reads: 81

```
[quote="darkkevind, post:2, topic:30603"]
The positive (the last wire connected,  B10?) Gets used by the BMS for all the positives of the other cells for balancing
[/quote]

That's what I thought too, but the BMS color codes have me all confused :slight_smile:. 

The only reason I'm not bypassing discharge is because I want to use the switch...maybe...not sure yet.  Still working through how I'm gonna do this.
```

---
## \#4 Posted by: darkkevind Posted at: 2017-08-14T18:05:06.374Z Reads: 74

```
Yeah I think you may have to ignore colours and just go with labels... Lol.

No I get that, the switch is super handy. You may as well go with the discharge if you're not going to be drawing more than 60A.
```

---
## \#5 Posted by: mmaner Posted at: 2017-08-14T18:06:12.646Z Reads: 71

```
[quote="darkkevind, post:4, topic:30603"]
You may as well go with the discharge if you're not going to be drawing more than 60A.
[/quote]

That's the thing, not sure if  am or not.  Ill post more when I have the thing assembled and tested.  This is a new type of build for me, so I'm trying to take my time.
```

---
## \#6 Posted by: mmaner Posted at: 2017-08-14T21:03:20.343Z Reads: 56

```
Here's the diagram for use with x2 5s Lipo(s)...if you good folks wouldn't mind double checking me.  thanks

<img src="/uploads/db1493/original/3X/1/6/165e3937454525d36d984803b5984bb83a34c11d.jpg" width="254" height="500">
```

---
## \#7 Posted by: pat.speed Posted at: 2017-08-14T21:59:54.335Z Reads: 41

```
Yes, that looks fine to me. Although I don't have a bms
```

---
## \#8 Posted by: mmaner Posted at: 2017-08-15T02:54:28.837Z Reads: 31

```
What about you @Namasaki, does this look correct?
```

---
## \#9 Posted by: Namasaki Posted at: 2017-08-15T03:19:21.322Z Reads: 30

```
both diagrams look correct to me
```

---
