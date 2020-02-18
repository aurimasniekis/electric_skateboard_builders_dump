# VESC - PPM Throttle range issue

### Replies: 5 Views: 1020

## \#1 Posted by: yaca Posted at: 2016-10-09T17:09:45.908Z Reads: 118

```
I need help with my first DIY EBoard: I use dual hub motors with the Winning Nano Remote and for testing I use a 6s lipo, later I will go with 10s Lipo. My problem is the throttle range. I reach already full speed at about the half way of the trigger.

What I tried till now:
- Adjusting the trim at the remote and the min and max pulsewith at the BLDC-Tool (0% - 50% - 100%) On the display it works but not in real.
- rebinding the receiver 
- adjusted the Max RPM which is 19000 with 6s

and yes this is not just a bench test, the problem is in real with myself on the board.

Here are some pics from the BLDC-Tool:

Master VESC:

<img src="/uploads/db1493/original/3X/3/d/3d12a5ebe50746f1a61b1e3eff87c6560e1e2522.png" width="650" height="500">


<img src="/uploads/db1493/original/3X/a/6/a6e643be743b76cb483f1513cb55023baa3d5a05.png" width="650" height="500">


<img src="/uploads/db1493/original/3X/6/d/6dda634378c74681c425e4992f2aec551583c4d3.png" width="650" height="500">


<img src="/uploads/db1493/original/3X/f/f/ff753f5b0e5febf94fb6dbbabcd0c28c32c1f469.png" width="650" height="500">

<img src="/uploads/db1493/original/3X/0/a/0adffa2dcecc981ac589ca1bb2caf62efd3fb204.png" width="650" height="500">

Slave VESC:

<img src="/uploads/db1493/original/3X/a/c/ac10bb0b1e00e8e75d2250ad4620f1510c43935e.png" width="650" height="500">

<img src="/uploads/db1493/original/3X/4/9/499d9d4fa396c4df158288fa155c23b94cdefd3f.png" width="650" height="500">e
```

---
## \#2 Posted by: Blasto Posted at: 2016-10-09T17:44:11.572Z Reads: 98

```

second edit, 

you can try to increase your min max window

min 0.9
max 2.1

you'll still be centered at 1.5 (idle)
```

---
## \#3 Posted by: yaca Posted at: 2016-10-09T17:54:18.724Z Reads: 97

```
You mean min max pulsewith? I will try this but now here it's dark on the outside.
```

---
## \#4 Posted by: Blasto Posted at: 2016-10-09T17:56:00.515Z Reads: 97

```
yes pulse width of the master
```

---
## \#5 Posted by: yaca Posted at: 2016-10-13T10:25:41.696Z Reads: 65

```
I tested a lot with pulsewith but at the end it did not solve the problem. The acceleration feels different and the brakes will be less strong when you increase your min max window. I went up till the green bar was min 14% and max 84%. But I still reached max speed at about 50 or 60 % of the throttle range. So I went back and trimmed the remote to the middle and set the points to 1,12 and 2,20. Thats exactly 0% - 50% - 100%.

I red somewhere the value for "MOTOR MAX" will have an influence for the way of the trigger. Higher Amps is fiewer way of trigger and vice versa. I tried this and maybe because I just use 6s LIPO in the moment, I had to go down to about 16 Amps to reach almost the full way but still a few mm left. I will try now with 10s Lipo and will see how it works.

What is your opinion or experience in this case?
```

---
