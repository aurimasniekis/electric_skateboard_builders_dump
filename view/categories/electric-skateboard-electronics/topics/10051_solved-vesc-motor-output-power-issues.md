# \[SOLVED\]VESC Motor output power issues

### Replies: 36 Views: 3122

## \#1 Posted by: coloncancer Posted at: 2016-09-23T23:25:33.107Z Reads: 132

```
Hi, I am very new to making e-boards, but have worked in making RC planes and quad copters. The issue that I ran across when trying to make my e-board is that my VESC seems to not be outputting nearly enough current to the motors. 

_sorry for the potato quality vids..._

When having the board upside down and no load on the wheels the VESC is able to get the wheel spinning. When doing this the current draw is around 1-2 amps. When the board is upside down like this and the wheel is spinning at full throttle, I am able to grab the wheel and stop it with my bare hand.
Video of what I mean:
 https://drive.google.com/file/d/0B8E6-v_xdAngN1A1OGpQVlJ1Nk0/view?usp=sharing

When the board is right side up, but only under the load of the weight of the board, it is not able to to move itself.
https://drive.google.com/file/d/0B8E6-v_xdAngOXVFeVRLV0E1WDQ/view?usp=sharing

If you do however give the board a push, it is able to move a little bit, but not sustain the movement.
https://drive.google.com/file/d/0B8E6-v_xdAngdF9FMEFZWTZQOVU/view?usp=sharing

In all of the videos the throttle remained at full.

In the BLDC tool, the motor detection fails.

A little about my setup: 

* Turnigy aerodrive 63-64 245kv
* Enertion VESC ver. 4.12
* HK GT2E transmitter and receiver combo
* BLDC firmware ver. 2.18
* 2 Turnigy 5000mAh lipo's in series

Some screenshots of my BLDC setup:
<img src="/uploads/db1493/original/3X/e/0/e0f5c89d3d1af2b6146cee01a0dae0fde01cc89a.jpg" width="690" height="390">
<img src="/uploads/db1493/original/3X/4/1/419b77d8b6bb8528b7cc704ff2e8674d4e5718cd.jpg" width="690" height="399">
<img src="/uploads/db1493/original/3X/e/e/eecc456ffbef30a30982752c7d2fc395da1faff3.jpg" width="690" height="385">
<img src="/uploads/db1493/original/3X/9/4/94d7be4a6be407795e1e73e69b2accdfebcad10a.jpg" width="690" height="388">

Thanks for any help!
```

---
## \#2 Posted by: chinzw Posted at: 2016-09-23T23:32:44.502Z Reads: 98

```
Can you post a picture of your Advanced section? Also, where did you get your VESC from?
```

---
## \#3 Posted by: Jinra Posted at: 2016-09-23T23:32:45.646Z Reads: 100

```
did you do a motor detection and apply the values?
```

---
## \#4 Posted by: Jinra Posted at: 2016-09-23T23:49:39.314Z Reads: 102

```
Also, if you're not running multiple VESCs, unchecked "multiple escs over can" and "send status over can". These settings should never both be checked on the same VESC.
```

---
## \#5 Posted by: coloncancer Posted at: 2016-09-24T00:22:24.286Z Reads: 100

```
Here is the Advance section:<img src="/uploads/db1493/original/3X/5/1/5160db452eb273df3f1641df98a8fa98de2f82a7.png" width="690" height="384">

I ordered the Basic VESC from enertion boards about 2 weeks ago

Thanks for the speedy replies
```

---
## \#6 Posted by: chinzw Posted at: 2016-09-24T00:25:17.287Z Reads: 95

```
You need to Read Settings before, all 0's doesnt look right
```

---
## \#7 Posted by: coloncancer Posted at: 2016-09-24T00:26:43.680Z Reads: 99

```
I ran the motor detection, but it failed. I then ran it again looking at the real time data with active sampling on and got no error codes... So I do not know what exactly is going on with that. I am not running a dual motor set up, so I think that I need to have both "multiple ESC's over CAN" and "Send status over CAN" unchecked... Correct?

Thanks for the help!
```

---
## \#8 Posted by: coloncancer Posted at: 2016-09-24T00:31:43.981Z Reads: 98

```
Ok, so the advance screenshot in my previous post had the VESC not connected, here is the correct one with the read values... sorry for the confusion
<img src="/uploads/db1493/original/3X/b/f/bfeb5e46a2c371a017a9e8a5c798edebd99f79a9.jpg" width="690" height="375">
```

---
## \#9 Posted by: chinzw Posted at: 2016-09-24T00:33:32.714Z Reads: 92

```
Hmm, that looks fine. But if motor detection failed then you will have problems.
```

---
## \#10 Posted by: coloncancer Posted at: 2016-09-24T00:35:17.096Z Reads: 86

```
I read somewhere that the motor detection should be done with a lab power supply and not just the batteries. When I tried it, I was just using the batteries, do you know if that is what is causing it to fail or what.
```

---
## \#11 Posted by: chinzw Posted at: 2016-09-24T00:36:56.997Z Reads: 83

```
The lab power supply is for the first power on, to prevent as much component damage as possible in the case of a short or other problem.
```

---
## \#12 Posted by: Jinra Posted at: 2016-09-24T00:37:15.654Z Reads: 82

```
batteries is fine if you know the batteries are good. Yes have both options unchecked. You need to be able to do motor detection, so don't use the board until that gets sorted out. Does the motor spin at all during detection?
```

---
## \#13 Posted by: coloncancer Posted at: 2016-09-24T00:40:26.783Z Reads: 80

```
Ok, so I have both unchecked now. I'll make a video of the motor detection really quick because its kinda hard to explain...
```

---
## \#14 Posted by: coloncancer Posted at: 2016-09-24T00:44:22.617Z Reads: 79

```
Ok, here is the video,
https://drive.google.com/file/d/0B8E6-v_xdAngMldPOVZxVEUxaDA/view?usp=sharing

It says "detection failed" in the output box for it... forgot to show that in the video
```

---
## \#15 Posted by: JohnnyMeduse Posted at: 2016-09-24T00:48:57.054Z Reads: 79

```
did you "read configuration" before trying a motor detection.
```

---
## \#16 Posted by: coloncancer Posted at: 2016-09-24T00:49:29.572Z Reads: 78

```
lol nope, I'll try that right now
```

---
## \#17 Posted by: coloncancer Posted at: 2016-09-24T00:51:26.688Z Reads: 80

```
Still failed, "bad detection, results failed" is what the words highlighted in red said down at the lower right
```

---
## \#18 Posted by: chinzw Posted at: 2016-09-24T00:54:31.451Z Reads: 79

```
You could try flash the latest firmware.
```

---
## \#19 Posted by: Jinra Posted at: 2016-09-24T00:54:54.409Z Reads: 80

```
what's the voltage you're running?
```

---
## \#20 Posted by: anon33082420 Posted at: 2016-09-24T00:57:53.440Z Reads: 80

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#21 Posted by: coloncancer Posted at: 2016-09-24T00:59:12.531Z Reads: 83

```
I flashed the latest firmware last night, and I think that I did that properly, are there any drivers that I need to get to make everything run properly?

I am running a 6s lipo... so i think around 24 ish volts
```

---
## \#22 Posted by: chinzw Posted at: 2016-09-24T01:00:02.675Z Reads: 84

```
OH!! Thats it then, your voltage cutoff start and end are wrong.
```

---
## \#23 Posted by: Jinra Posted at: 2016-09-24T01:02:11.427Z Reads: 83

```
This. Put battery cutoffs below current working voltage. you can even use 0 for now
```

---
## \#24 Posted by: Namasaki Posted at: 2016-09-24T01:06:37.868Z Reads: 81

```
Your battery regen min might be too high. What is the C rating on your Lipos for charging.
You are currently regen charging your batteries at over 2C
```

---
## \#25 Posted by: anon33082420 Posted at: 2016-09-24T01:07:12.230Z Reads: 80

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#26 Posted by: coloncancer Posted at: 2016-09-24T01:07:44.213Z Reads: 79

```
THANK YOU ALL!!! That just fixed it <3 peace
```

---
## \#27 Posted by: Namasaki Posted at: 2016-09-24T01:08:21.584Z Reads: 79

```
wait a min, you need to check your regen so you don't blow your batteries up
What is the max charge rate for your batteries. or what batteries do you have?
```

---
## \#28 Posted by: coloncancer Posted at: 2016-09-25T00:16:38.899Z Reads: 71

```
Sorry for the late reply, yesterday was my accounts first day so they limit the number of posts you can make. I am not sure what the max charge rate for the lipos are. Here is a link to the ones i bought...

http://www.hobbyking.com/hobbyking/store/__9184__Turnigy_5000mAh_3S_20C_Lipo_Pack.html

Thanks for all the great help!
```

---
## \#29 Posted by: lox897 Posted at: 2016-09-25T00:42:27.133Z Reads: 73

```
Most lipos are only supposed to charge at up to 1c so you could charge it at 5 amps but 0.75c is better.
```

---
## \#30 Posted by: Namasaki Posted at: 2016-09-25T01:26:59.009Z Reads: 71

```
According to hobby king, the max charge rate for those batteries is 2C or 10amps
So you can set your max battery regen at -10 or less.
```

---
## \#31 Posted by: coloncancer Posted at: 2016-09-25T01:35:04.302Z Reads: 71

```
Okay will do, thanks for all the awesome help and such a great community!
```

---
## \#32 Posted by: Ultimat3ging3r Posted at: 2016-10-24T18:43:55.097Z Reads: 58

```
How do you find the max charge rate? I have 2- 8000mah 30c 4s lipo. So 8amps? What would that be on batt regen?
```

---
## \#33 Posted by: Namasaki Posted at: 2016-10-24T20:10:48.744Z Reads: 57

```
It depends on the batteries. 
Usually batteries with a higher C rating for discharge will also have a higher C rating for charge. 
Look up the specs on your particular battery and they should include max charge rate. 
If you can't find the specs, then charging at 1C is always a safe bet. 
So, 8ah x 1C= 8amp charge rate.
```

---
## \#34 Posted by: Ultimat3ging3r Posted at: 2016-10-24T21:39:05.058Z Reads: 53

```
Thanks. Do you know what that would be for regen?
```

---
## \#35 Posted by: Namasaki Posted at: 2016-10-24T21:52:35.244Z Reads: 49

```
If your using zippy flight max the max charge rate is 5C
5Cx8ah=40a
Or -40 on battery regen
I would recommend setting it  to -10 and trying that. 
If you want stronger brakes then adjust it from there

<img src="/uploads/db1493/original/3X/2/0/2075caa6ff2565c95eff40bb50124eb646e8612f.PNG" width="281" height="499">
```

---
## \#36 Posted by: Ultimat3ging3r Posted at: 2016-10-24T22:17:40.766Z Reads: 45

```
Thanks brother
```

---
