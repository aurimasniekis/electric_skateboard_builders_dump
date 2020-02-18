# Voltage sag? Board cuts out on full throttle during acceleration

### Replies: 29 Views: 1411

## \#1 Posted by: trigger4point7 Posted at: 2017-05-17T21:26:17.005Z Reads: 154

```
So I finally got my board up after months of work, and after riding for about a week (25 miles?) I'm now having an issue where my VESC-X restarts on full acceleration. If I accelerate more slowly then it does fine. It hasn't shown this issue until all of a sudden. I've included my settings. I've seen setting the "Max input voltage" to 57V is that recommended? Is that the Motor Max setting (just to be sure)?

I'm terrified I've killed my battery.

Motor max/min - 60A/-60A
Battery max/min - 30A/-12A
Absolute Max - 130A
```

---
## \#2 Posted by: Alextech Posted at: 2017-05-17T21:34:54.371Z Reads: 150

```
What battery are you using? Liion Lipo? Max Discharge? There have also been cases of bad Vesc x that have cut off due to low voltage from a bad resistor or something along those lines, and you may want to double check with the seller who sold you it
```

---
## \#3 Posted by: trigger4point7 Posted at: 2017-05-17T21:39:26.049Z Reads: 150

```
I bought most everything from Enertion (all except the motor, 6355 190kv TB) it is the Spacecell 4 (10S4P Li-ion), Absolute Max is 130A.

<img src="/uploads/db1493/original/3X/b/a/baf7b4f8e7cb25d52793cc08a9e1f2ea2b9eeaf5.jpg" width="375" height="500">
```

---
## \#4 Posted by: Jinra Posted at: 2017-05-17T21:47:17.113Z Reads: 138

```
whats your battery cutoff start/end?
```

---
## \#5 Posted by: trigger4point7 Posted at: 2017-05-17T22:34:49.035Z Reads: 133

```
Shoot, I can't get back to my computer right now. But it is the default, I haven't touched those settings at all.
```

---
## \#6 Posted by: trigger4point7 Posted at: 2017-05-17T22:34:59.778Z Reads: 130

```
I'll send them over the second I'm able.
```

---
## \#7 Posted by: Jinra Posted at: 2017-05-17T22:36:01.865Z Reads: 129

```
My guess is that punching the throttle is causing too much sag and it goes below the threshold for battery cutoff.
```

---
## \#8 Posted by: trigger4point7 Posted at: 2017-05-17T22:39:35.866Z Reads: 130

```
Any idea why it would start happening now? I've kept my riding style pretty consistant. Have I damaged the battery in some way?
```

---
## \#9 Posted by: Jinra Posted at: 2017-05-17T22:40:15.340Z Reads: 129

```
It's more likely you've damaged the VESC-x, but hard to say. Seeing all your settings would help.
```

---
## \#10 Posted by: trigger4point7 Posted at: 2017-05-17T22:57:23.605Z Reads: 126

```
Here we go! <img src="/uploads/db1493/original/3X/d/b/db8dba0a6f0beabd39409133a4c67704a9f8acc6.png" width="690" height="343">
```

---
## \#11 Posted by: Jinra Posted at: 2017-05-17T22:59:25.824Z Reads: 123

```
Try adjusting your battery cutoff start/end to something really low for testing (like 10/10) to see if you still have the problem.

Could you post your other pages as well? (BLDC, Advanced)
```

---
## \#12 Posted by: trigger4point7 Posted at: 2017-05-17T23:01:25.115Z Reads: 125

```
<img src="/uploads/db1493/original/3X/b/a/baee830132faadd92c6aaf68bcead08f784875e9.png" width="690" height="363">
<img src="/uploads/db1493/original/3X/3/2/32f20616975bfb973e7a126f02108a6390562eaa.png" width="690" height="367">
```

---
## \#13 Posted by: Jinra Posted at: 2017-05-17T23:11:00.583Z Reads: 118

```
Did you do motor detection? Those values look like they're default.
```

---
## \#14 Posted by: trigger4point7 Posted at: 2017-05-18T00:07:28.428Z Reads: 114

```
I didn't for that screenshot but here it is after a motor detection... <img src="/uploads/db1493/original/3X/6/a/6a1caacb276e98afb57773415d2071878bccf842.png" width="690" height="380">
```

---
## \#15 Posted by: Jinra Posted at: 2017-05-18T00:47:54.294Z Reads: 106

```
You didn't write the config for it. You have to do detection to get the values, hit "apply" or write the fields in manually, then hit "write config" to write it to the VESC
```

---
## \#16 Posted by: trigger4point7 Posted at: 2017-05-18T00:53:55.220Z Reads: 104

```
Ah, I thought you just wanted to see the readings, I had done a detection and apply before, but I'll do it again.
```

---
## \#17 Posted by: Jinra Posted at: 2017-05-18T00:54:44.415Z Reads: 103

```
Well you have to apply AND write config. Simply "applying" doesn't do anything besides write the numbers in the appropriate fields for you.
```

---
## \#18 Posted by: trigger4point7 Posted at: 2017-05-18T01:34:51.482Z Reads: 97

```
Applied and config written!
```

---
## \#19 Posted by: Jinra Posted at: 2017-05-18T01:41:48.012Z Reads: 95

```
Cool, have you tried adjusting the battery cutoff voltage to see if the problem persists?
```

---
## \#20 Posted by: trigger4point7 Posted at: 2017-05-18T03:43:14.313Z Reads: 93

```
I did, I set it super low 10/10 as you suggested, put one foot on it hit full throttle and same issue.
```

---
## \#21 Posted by: Jinra Posted at: 2017-05-18T03:45:56.244Z Reads: 92

```
Alright, so do it again, but this time make sure it doesn't turn off and plug it into your computer, go to terminal in BLDC tool, and type faults to see if you got any faults.
```

---
## \#22 Posted by: trigger4point7 Posted at: 2017-05-18T03:49:04.265Z Reads: 89

```
Fault            : FAULT_CODE_DRV8302
Current          : 156.0
Current filtered : -75.2
Voltage          : 39.07
Duty             : 0.56
RPM              : 14919.8
Tacho            : 623
Cycles running   : 735
TIM duty         : 3961
TIM val samp     : 1867
TIM current samp : 5436
TIM top          : 7137
Comm step        : 5
Temperature      : 28.63
```

---
## \#23 Posted by: Jinra Posted at: 2017-05-18T03:50:50.355Z Reads: 88

```
Oof, yea that sucks, you'll need a new DRV8302 chip. It's a bit tricky to solder on so you'll have to learn surface mount soldering or give it to someone who can do it for you.
```

---
## \#24 Posted by: JohnnyMeduse Posted at: 2017-05-18T04:14:52.231Z Reads: 85

```
Vesc-x can recover from DRV Error :wink: 

@trigger4point7 try to put your max current at round 150 at first if it does it again try 175.

Edit: If your are using a nano-x remote, be sure to open the remote first and then push the throttle Forward and Backward at there max first before opening the board.

Edit 2: Also @trigger4point7 don't push the throttle at max in one second when jump up on your board do it gradually, the nano-x remote is very responsive, and the transistor are faster to act on the vesc-x, so in some case it will over rush the current.
```

---
## \#25 Posted by: Jinra Posted at: 2017-05-18T04:31:02.214Z Reads: 83

```
What is this wizardly? The VESC-X can self heal? :dizzy_face:
```

---
## \#26 Posted by: JohnnyMeduse Posted at: 2017-05-18T04:34:21.207Z Reads: 81

```
Well, it's much more simple, the transistor are faster than the drv, so unlike the old version, they are doing there job wright, and cut before braking the drv :wink:
```

---
## \#27 Posted by: Jinra Posted at: 2017-05-18T04:38:39.740Z Reads: 81

```
ah is this why people are saying it's "FOC-proof"? On the other hand, it'd be harder to spot a legit burnt DRV8302 ya?
```

---
## \#28 Posted by: JohnnyMeduse Posted at: 2017-05-18T04:43:45.507Z Reads: 83

```
I've only see a hand full of legitimate burn drv... 

But if you look at the current (show around 156A, in the picture post over), on a real burn drv (on mosfet) it will show 0.0A
```

---
## \#29 Posted by: trigger4point7 Posted at: 2017-05-18T05:05:24.252Z Reads: 78

```
Thanks @JohnnyMeduse I gave it a shot, I set the Absolute Max to 150 and then 175 and saw the same issue. I'm religous about calibrating the remote before use. I had a "Phantom Throttle" issue (without touching the remote the throttle would just jump to max, calibrating the remote seemed to fix it). It seems odd that it would just start to happen, I've been riding with the same riding style for the one week I've had it working.
```

---
