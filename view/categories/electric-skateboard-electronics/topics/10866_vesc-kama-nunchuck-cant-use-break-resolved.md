# VESC + Kama nunchuck can&rsquo;t use break \[Resolved\]

### Replies: 10 Views: 1212

## \#1 Posted by: Thanhnd Posted at: 2016-10-09T15:00:10.818Z Reads: 62

```
Hi Builders.

**I can't use the break anymore.**

- The cruise control still work good (both acceleration and deceleration)
- The acceleration (no cruise control) work good.

Please help me find the way to fix this.


https://www.youtube.com/watch?v=iv7i_8pKn48

<img src="/uploads/db1493/original/3X/d/4/d47c9448dad8b6473fdeb53c00d7bb9fc504119b.png" width="689" height="397">

<img src="/uploads/db1493/original/3X/d/d/dd4d5b3d2cd27b7d87d44c225fe2301a2fef5f4c.png" width="690" height="388">

<img src="/uploads/db1493/original/3X/b/a/ba75e875f37011e74d5bac59f5fa88bebba0bbd6.png" width="690" height="397">
```

---
## \#2 Posted by: Maxid Posted at: 2016-10-09T15:19:33.080Z Reads: 52

```
Did you click on the "display" checkbox in the nunchuck tab and check if the brake throttle movement is recognized by the VESC?
```

---
## \#3 Posted by: Thanhnd Posted at: 2016-10-09T15:27:19.951Z Reads: 51

```
Yes, its recognized but still not break. The break only work when the wheel is not rolling (not have momentum). I know that when I try use my hand to rolling the wheel.

<img src="/uploads/db1493/original/3X/9/c/9cf3df72be6378b2941240bca31a56fda71fd588.png" width="673" height="500">
```

---
## \#4 Posted by: Maxid Posted at: 2016-10-09T15:29:29.148Z Reads: 49

```
does the VESC brake when you control it via the keyboard?
```

---
## \#5 Posted by: Thanhnd Posted at: 2016-10-09T15:31:21.278Z Reads: 45

```
I haven't try and I not sure how to break by using keyboard. Press forward then backward?
```

---
## \#6 Posted by: Goombaacez84 Posted at: 2016-10-09T16:59:51.543Z Reads: 38

```
Yep, when the VESC is hooked up to your computer you can control the motor with the <- and -> arrow keys
```

---
## \#7 Posted by: lowGuido Posted at: 2016-10-09T18:33:48.444Z Reads: 35

```
that graph looks like its way too far back if that's at neutral.
```

---
## \#8 Posted by: Namasaki Posted at: 2016-10-09T22:50:37.300Z Reads: 31

```
This is unrelated to you question but I noticed that you seem to have the Max current step bug in your firmware.
Look at the setting on the motor config/advanced page.
Its reading .4 and should be .04
The bug multiplies the value by 10 every time you write to the vesc.
It will eventually damage the Drv chip.
The current download of bldc tool with firmware has the bug fixed.
if your not able to update the firmware then you'll need to set the value to .004 before writing to the vesc.
http://www.electric-skateboard.builders/t/psa-remember-to-reset-your-max-current-ramp-step-when-programming-your-vesc/6262
```

---
## \#9 Posted by: Jinra Posted at: 2016-10-09T23:10:22.307Z Reads: 28

```
Just FYI your battery cut off end should always be lower than start. Right now, it's higher.
```

---
## \#10 Posted by: Thanhnd Posted at: 2016-10-10T03:11:48.140Z Reads: 24

```
I've resolved by re-upload firmware 2.18 for PBC 4.10. Thank you guys.
```

---
