# Balanced battery dies in 2 minutes

### Replies: 19 Views: 231

## \#1 Posted by: Jordan12 Posted at: 2019-05-01T16:00:12.834Z Reads: 114

```
Weirdest thing started happening. My battery goes from cut off voltage(or near) to fully charged in matters of an hour. All the cells are at 3.6V when the charger says it’s at full charge of 25.2. I’ll unplug the charger and the battery reads 21.6. Why won’t the battery fully charge anymore?
```

---
## \#2 Posted by: Namasaki Posted at: 2019-05-01T16:05:17.187Z Reads: 110

```
How many cells does your battery have in series
```

---
## \#3 Posted by: Jordan12 Posted at: 2019-05-01T16:09:51.203Z Reads: 107

```
6s2p battery
```

---
## \#4 Posted by: StefanMe Posted at: 2019-05-01T16:11:09.811Z Reads: 105

```
[quote="Jordan12, post:1, topic:92444"]
All the cells are at 3.6V when the charger says it’s at full charge of 25.2
[/quote]

Charger is broken... 

The full load voltage is 4.2 per cell. 3.6 is the nominal voltage.
```

---
## \#5 Posted by: Jinra Posted at: 2019-05-01T16:12:11.538Z Reads: 102

```
It's reading 25.2 when it's plugged in because it's reading the chargers output voltage. Likely an issue with your BMS. Read the voltage for each parallel group individually.
```

---
## \#6 Posted by: Jordan12 Posted at: 2019-05-01T16:17:15.570Z Reads: 94

```
Well I thought so so I stuck my bolt meter to just the charger it and it shows 25.5 on the meter. On the back of the charger it says Output 25.2V

Another thing to is if I test the battery, unplugged after the light turns green, it says 21.2. Then I’ll plug the battery back into the charger and test the battery leads it says it’s now at 25.5, as soon as I unplug, back to 21.2

I tested each series and they all show 3.6
```

---
## \#7 Posted by: Jinra Posted at: 2019-05-01T16:20:25.109Z Reads: 85

```
Yea still sounds like a defective BMS, or perhaps an incorrectly hooked up BMS.
```

---
## \#8 Posted by: Jordan12 Posted at: 2019-05-01T16:24:16.178Z Reads: 80

```
Probably defective, it worked fine for months. 
But the battery also started acting weird before this.
About a week leading up to this it would basically skip the low voltage protection set by the vesc and the vesc would completely shut off cause the bolts drop so quick. Now even with it at 21.2 I can run it with no load for maybe 5 mins and it drops to 18V

Could the cells be bad too?
```

---
## \#9 Posted by: Jinra Posted at: 2019-05-01T16:26:21.480Z Reads: 74

```
Are you discharging through BMS? If so, perhaps it's related.
```

---
## \#10 Posted by: StefanMe Posted at: 2019-05-01T16:26:49.811Z Reads: 72

```
No, looks more like an defect BMS... All cells have the same voltage. The cells are not the problem.
```

---
## \#11 Posted by: Jordan12 Posted at: 2019-05-01T16:30:11.477Z Reads: 72

```
Thanks all of y’all for the quick responses.
Discharge is through the bms. 
Should good working cells go from 20.2V to 18V with no load in 3 mins? Just timed it while watching it on the vesc tool. I hope the cells are good I wouldn’t mind turning 2 6S batteries in a 8S3P with a quality bms.
```

---
## \#12 Posted by: Jinra Posted at: 2019-05-01T16:31:18.094Z Reads: 66

```
Sounds about right, depending on the specific cell, you probably hit the voltage cliff.
```

---
## \#13 Posted by: Jordan12 Posted at: 2019-05-01T16:35:34.631Z Reads: 62

```
So just a new bms should do the trick essentially?
```

---
## \#14 Posted by: Jinra Posted at: 2019-05-01T16:37:43.956Z Reads: 55

```
That's what I'd try.
```

---
## \#15 Posted by: Jordan12 Posted at: 2019-05-01T16:39:26.689Z Reads: 52

```
Awesome, I’ll give it a shot
```

---
## \#16 Posted by: Jordan12 Posted at: 2019-05-01T23:23:48.860Z Reads: 27

```
Left it unplugged for several hours, decided to plug it in again, now it’s decided to charge over 4v and counting?! I’m more confused now.
```

---
## \#17 Posted by: Andy87 Posted at: 2019-05-02T00:56:32.697Z Reads: 24

```
Check the voltage of each p-group. The voltage of each should be close to be the same.
```

---
## \#18 Posted by: Jordan12 Posted at: 2019-05-02T17:03:34.977Z Reads: 16

```
They are, they are exactly the same. The battery is balanced. It’s taken a day but it’s reached 23.9V the charger is going green and red. Not sure what’s going on with it
```

---
## \#19 Posted by: Jinra Posted at: 2019-05-02T17:16:43.779Z Reads: 14

```
again.. probably defective bms
```

---
