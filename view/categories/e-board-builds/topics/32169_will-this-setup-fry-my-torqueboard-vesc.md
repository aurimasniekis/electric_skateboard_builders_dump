# Will this setup fry my torqueboard vesc

### Replies: 29 Views: 1366

## \#1 Posted by: dg798 Posted at: 2017-09-03T17:00:36.428Z Reads: 207

```
6355 190 kv 2500 watt torqueboards motor
2 6s lipo batteries in series (each 5200 mah)
Totqueboards vesc 4.12.
I just want to make sure u won't like get my drv chip.
```

---
## \#2 Posted by: karma Posted at: 2017-09-03T17:01:15.924Z Reads: 210

```
Running 12S is always risky if you haven't done calculations.
```

---
## \#3 Posted by: dg798 Posted at: 2017-09-03T17:01:37.319Z Reads: 206

```
What do you mean by calculations?
```

---
## \#4 Posted by: karma Posted at: 2017-09-03T17:05:00.002Z Reads: 197

```
The drv chip is usually blown by going over 60k eRPM. That's why it's important to calculate the eRPM and make sure it doesn't go over 60k.
```

---
## \#5 Posted by: dg798 Posted at: 2017-09-03T17:10:57.167Z Reads: 187

```
Ok I will check
```

---
## \#6 Posted by: dg798 Posted at: 2017-09-03T17:12:26.627Z Reads: 184

```
This is the erpm 59052.
Is that cutting it too close 
Or should I just put in 60000 as the max in the bldc tool
```

---
## \#7 Posted by: Nix Posted at: 2017-09-03T17:12:31.211Z Reads: 180

```
I'm pretty sure you would need to go lower than 170 kv rating if you don't want to blow the drv chip...
```

---
## \#8 Posted by: dg798 Posted at: 2017-09-03T17:13:28.309Z Reads: 181

```
So I will fry my chip with this setup?
```

---
## \#9 Posted by: onepunchboard Posted at: 2017-09-03T17:15:45.759Z Reads: 176

```
batt full charge is 4.2 per cell.  so for that u probably go over 60k. for baseform vesc erpm is critical
```

---
## \#10 Posted by: dg798 Posted at: 2017-09-03T17:22:15.348Z Reads: 175

```
So I'm good??
```

---
## \#11 Posted by: jammin Posted at: 2017-09-03T17:24:03.224Z Reads: 170

```
you could always add the eRPM limit, but 170kv would be a safer choice. Both should work, though.
```

---
## \#12 Posted by: dg798 Posted at: 2017-09-03T17:24:45.627Z Reads: 168

```
I will add the limit and I only have 190 kv
So It should work
```

---
## \#13 Posted by: dg798 Posted at: 2017-09-03T17:25:18.215Z Reads: 157

```
Or is there a very big chance something will happen because I already had to replace one vesc
```

---
## \#14 Posted by: jammin Posted at: 2017-09-03T17:30:21.237Z Reads: 153

```
the eRPM limit is inefficient, but you'll only hit the upper bound when you're pushing it at max. Since you bought both the vesc and motor, it wouldn't hurt to ask DIYes / Dexter directly about the # of poles of that motor or if it's safe.

How did you destroy your last vesc?
```

---
## \#15 Posted by: dg798 Posted at: 2017-09-03T18:37:15.450Z Reads: 148

```
It came faulty
```

---
## \#16 Posted by: dg798 Posted at: 2017-09-03T18:40:44.216Z Reads: 146

```
Then it gave me the drv fault
```

---
## \#17 Posted by: Eboosted Posted at: 2017-09-03T18:46:38.492Z Reads: 138

```
I run 12s on 6355 190kv from @Torqueboards
```

---
## \#18 Posted by: torqueboards Posted at: 2017-09-03T19:01:36.295Z Reads: 138

```
We only test and ride on 12S. All the VESCs are also tested on 12S prior to being shipped out.

We specifically recommend 10S/12S for 190KV but we only offer 12S batteries.
```

---
## \#19 Posted by: dg798 Posted at: 2017-09-03T19:02:48.800Z Reads: 137

```
ok thanks guys
```

---
## \#20 Posted by: BenL Posted at: 2017-09-03T23:52:16.975Z Reads: 125

```
@torqueboards That's good information to know - I think it would help to avoid these questions if the listing for the VESC was updated to say that they are tested via 12S. The listing reads as if they are only tested on 10S:

"Our VESC ships to you tested multiple times during the production cycle. Pre-configured for a Single Motor Electric Skateboard with our 6355 190KV EPOWER Motor and our 10S3P EPOWER Pack. "
```

---
## \#21 Posted by: Sn4pz Posted at: 2017-09-05T15:35:04.953Z Reads: 109

```
would it be ok to use your 6s4p pack with a single 190kv motor?
```

---
## \#22 Posted by: GrecoMan Posted at: 2017-09-05T15:59:11.964Z Reads: 106

```
For 6s you will want to go with higher kV. 245-270kv will be better
```

---
## \#23 Posted by: Sn4pz Posted at: 2017-09-05T16:08:24.257Z Reads: 101

```
but will it hurt my batteries or anything? :stuck_out_tongue:

ive already got the 190kv motor so id like to not buy another
```

---
## \#24 Posted by: GrecoMan Posted at: 2017-09-05T16:12:54.042Z Reads: 91

```
Nah it won't do anything to the battery you'll just be hella slow
```

---
## \#25 Posted by: GrecoMan Posted at: 2017-09-05T16:13:13.835Z Reads: 91

```
If you can try to go with 10-12s for the best power for that motor
```

---
## \#26 Posted by: torqueboards Posted at: 2017-09-07T04:35:42.345Z Reads: 87

```
@sn4pz it's fine.. your setup will be slow though 15-18mph with 6S on 190KV. Ideally, you want 260KV or similar for about 20-24mph top speed.
```

---
## \#27 Posted by: Ixf Posted at: 2018-01-08T02:10:40.411Z Reads: 71

```
Do you guys test foc as well?  I feel like theres alot of comments on how TB vesc gets burned up on foc.  Should we just stay on BLDC?  BLDC sensored\hybrid OK to run?
```

---
## \#28 Posted by: torqueboards Posted at: 2018-01-08T02:22:20.369Z Reads: 67

```
We don't test FOC but I run FOC on almost all my setups with no issues.
```

---
## \#29 Posted by: Sparc Posted at: 2018-01-08T03:51:18.377Z Reads: 61

```
I have dual TB 6355 190kv motors on TB VESCs at 12S.  The setup has been rock solid and I haven't had any issues in BLDC mode.  It's a great setup and I wouldn't have any problems recommending TB 190kv motors on 12S.
```

---
