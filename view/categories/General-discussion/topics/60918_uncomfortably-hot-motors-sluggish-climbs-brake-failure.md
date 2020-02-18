# Uncomfortably hot motors, sluggish climbs, brake failure

### Replies: 7 Views: 298

## \#1 Posted by: ervinelin Posted at: 2018-07-04T23:23:13.019Z Reads: 124

```
So I finally found time to take my board out for a longer ride (20km) and midway through it I noticed the motors got uncomfortably warm. Not scalding hot but warmer than I would have expected considering I was cruising at 5A or so only.

Then there were 2 instances which the board became very sluggish going upslope. On other slopes they would have no issue at all, these 2 instances they just felt like they were struggling to go up although the incline was all roughly the same. On my remote this climb was roughly at 12A only...

Then the last straw came when after the second slope, my brakes failed completely. No response whatsoever. I nearly peeed my pants but thankfully I managed to ride out the slope, once it reached the bottom my brakes worked again.

Running dual Focboxes on FOC at 12S
8" wheels
6734 BKB motors

Anyone know what I should be checking?
```

---
## \#2 Posted by: Sender Posted at: 2018-07-04T23:51:09.909Z Reads: 111

```
Where are you located?  How hot is it?
```

---
## \#3 Posted by: ervinelin Posted at: 2018-07-04T23:52:48.674Z Reads: 111

```
Singapore, but I was riding at midnight.

I don't know exactly how hot but hot to the touch without being scalding hot. Like holding a very warm cup of coffee... I can keep my fingers on it but it's not comfortable.
```

---
## \#4 Posted by: Kug3lis Posted at: 2018-07-04T23:54:12.202Z Reads: 102

```
What about your FocBox temperatures?
```

---
## \#5 Posted by: ervinelin Posted at: 2018-07-04T23:56:42.997Z Reads: 100

```
Don't have telemetry setup to monitor them.

How should I go about it?
```

---
## \#6 Posted by: ervinelin Posted at: 2018-07-05T00:16:07.170Z Reads: 94

```
https://vesc-project.com/node/371 this problem sounds like what I might have encountered
```

---
## \#7 Posted by: ervinelin Posted at: 2018-07-05T16:46:14.153Z Reads: 61

```
Okay so I realised my firmware was out of date. Updated to latest firmware, increased FOC frequency from 20 to 30 and went out for a quick 5km test.

So far so good, motors seem to run a little cooler (based on unscientific hand touch) but essentially they are warm but not toasty. Hill climbs were a walk in the park, brakes all worked as expected.

Will find time to do a longer ride again to do more testing but I think for now it should resolved.
```

---
