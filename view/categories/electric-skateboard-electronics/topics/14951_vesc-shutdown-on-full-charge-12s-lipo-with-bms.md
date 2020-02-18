# VESC Shutdown on full charge. (12s LIPO with BMS)

### Replies: 25 Views: 1765

## \#1 Posted by: jackw Posted at: 2016-12-19T23:07:53.822Z Reads: 153

```
Hey guys, so I swear there was a thread solving this from a while ago but I can't for the life of me find it with the search...

Basically, when I fully charge my board (12s LIPO with BMS) to 50.4v, 100% on the battery meter, I am finding that anytime I try to brake with a load, my VESC will restart until I have used the board a little bit (Down to maybe 98% - 97%) when it'll start acting and braking normally. Was there a fix for this in settings? Or should I just not fully charge my board?

Thanks in advance...
```

---
## \#2 Posted by: Esrapp21 Posted at: 2016-12-19T23:13:21.831Z Reads: 149

```
I don't know the fix, but I'm pretty sure it is along the lines of the regenatove braking is trying to over charge your battery, but the BMS is stoping it, and with all that extra energy it is shutting down the VESC. I may be wrong, but I think that was what happened to the boosted v2
```

---
## \#3 Posted by: Namasaki Posted at: 2016-12-19T23:15:39.381Z Reads: 143

```
Are you discharging through the BMS?
```

---
## \#4 Posted by: jackw Posted at: 2016-12-19T23:16:14.995Z Reads: 136

```
Yes, could that be it?
```

---
## \#5 Posted by: Namasaki Posted at: 2016-12-19T23:18:06.759Z Reads: 134

```
If your charging and discharging through the bms, then it should keep the battery from over charging during regen braking.
What brand of bms is it?
```

---
## \#6 Posted by: jackw Posted at: 2016-12-19T23:22:49.718Z Reads: 129

```
Battery Supports. Would that give me an over voltage error? That's whats thrown up on the VESC when it happens.
```

---
## \#7 Posted by: jmasta Posted at: 2016-12-19T23:23:42.760Z Reads: 131

```
What is your max voltage setting on the VESC?  It should be set to 57V for 12S
```

---
## \#8 Posted by: Ackmaniac Posted at: 2016-12-19T23:27:00.595Z Reads: 123

```
Post some screenshots of you settings. But jmasta is absolutely right.
```

---
## \#9 Posted by: jackw Posted at: 2016-12-19T23:34:03.564Z Reads: 123

```
I'll post up some screen shots, I'm 99% sure I have it set at 57v though. Will report back!
```

---
## \#10 Posted by: jackw Posted at: 2016-12-21T13:12:46.147Z Reads: 102

```
Yep, was already set at 57v. Any Ideas?
<img src="/uploads/db1493/original/3X/d/6/d666453915ee32c16caa08d07b03413774377a75.jpeg" width="690" height="369"><img src="/uploads/db1493/original/3X/2/0/2051e6655410dbc8d99ba869bd72b17801212f71.jpeg" width="690" height="366">
```

---
## \#11 Posted by: Ackmaniac Posted at: 2016-12-21T17:39:55.285Z Reads: 88

```
Looks good to me. Really could be the BMS. Just type "faults" in the terminal tab after the vesc shut down. Don't switch off the board on between the shutdown and the terminal entry.
```

---
## \#12 Posted by: jackw Posted at: 2016-12-21T17:51:17.913Z Reads: 91

```
Alright I'll full charge the board tonight and post the error code. Pretty sure that it was throwing up an OVER_VOLTAGE code last time I checked. Thanks btw!
```

---
## \#13 Posted by: Blasto Posted at: 2016-12-21T18:05:27.809Z Reads: 92

```
Give yourself a little bit more play in between your voltage cutoff start and end.

Because now how it is, you will most likely hit your cut end emmediatly after your start.

I would put your cutoff end around 36V
```

---
## \#14 Posted by: adriendod Posted at: 2016-12-21T19:23:59.674Z Reads: 86

```
I have the same problem with the 10S space cell... I'll check the max voltage setting and also check the error it gives me.. thanks
```

---
## \#15 Posted by: jackw Posted at: 2016-12-21T21:40:38.736Z Reads: 82

```
Ok just fully charged and grabbed this:

<img src="/uploads/db1493/original/3X/c/c/cc616c530b4696ce1e6ad8f4b047fa33b0c5a4e6.jpeg" width="690" height="368">

Any ideas, not 100% sure how to read the report.
```

---
## \#16 Posted by: Blasto Posted at: 2016-12-21T21:49:49.175Z Reads: 82

```
try to tune down your batt min to -15

not sure if this will solve the problem...
```

---
## \#17 Posted by: JohnnyMeduse Posted at: 2016-12-21T21:56:11.985Z Reads: 81

```
Have you try to bypass the bms
```

---
## \#18 Posted by: jackw Posted at: 2016-12-21T22:18:38.214Z Reads: 81

```
[quote="Blasto, post:16, topic:14951"]
try to tune down your batt min to -15
[/quote]


No change :slight_frown:

[quote="JohnnyMeduse, post:17, topic:14951, full:true"]
Have you try to bypass the bms
[/quote]

I think I'll try this next..!
```

---
## \#19 Posted by: adriendod Posted at: 2016-12-21T22:28:07.460Z Reads: 76

```
Just so you know I fixed mine. Max input voltage was set on 42. I put it on 47.5 and now it works fine! Is it the right number for 10S?

Thanks
```

---
## \#20 Posted by: Ackmaniac Posted at: 2016-12-21T22:57:37.017Z Reads: 75

```
57 is the right number.  This value is not to protect your battery.  It is to protect the Vesc because it can only handle 60V and by 57V it has a little buffer.
@jackw It is very likely that it is caused by the BMS which shuts down. But please also check with a multimeter that the battery is not above 50.4V without load.
```

---
## \#21 Posted by: jackw Posted at: 2016-12-21T23:36:59.144Z Reads: 75

```
Battery is sitting at about 49v with multimeter without load. I'll try bypassing the BMS (No real reason to discharge through it really) I just wired it up that way first for simplicity... Just trying to figure out in my head how the BMS restarts the VESC with an OVER_VOLTAGE by shutting down?
```

---
## \#22 Posted by: Ackmaniac Posted at: 2016-12-21T23:47:14.073Z Reads: 73

```
When you brake then you charge the battery. Because the motor produces power (regenerative).  But the battery is already full and the BMS detects that. So the BMS shuts down and doesn't except any power anymore. Now the VESC doesn't know where to send the power and runs into the overvoltage. And to protect itself it shuts down.
```

---
## \#23 Posted by: JohnnyMeduse Posted at: 2016-12-21T23:48:18.399Z Reads: 73

```
Sometime the ovevoltage error occurs, because the bms discharge capacity are not enought, so it is like the voltage loop back to the esc
```

---
## \#24 Posted by: adriendod Posted at: 2016-12-22T09:15:58.053Z Reads: 69

```
ahhhhhh right on! thanks!
```

---
## \#25 Posted by: jmasta Posted at: 2016-12-22T16:30:05.554Z Reads: 65

```
[quote="Blasto, post:13, topic:14951, full:true"]
Give yourself a little bit more play in between your voltage cutoff start and end.

Because now how it is, you will most likely hit your cut end emmediatly after your start.

I would put your cutoff end around 36V
[/quote]

36V, or 3.0V/cell, is way way too low of a cutoff for LiPos.  If you look at a discharge chart, there is very little energy left at 3.5-3.6 V/cell, and the voltage drops rapidly.  If anything, should raise your voltage cutoff start/end.

@jackw has 40.80 --> 39.60.   I'm currently using 42.6V (3.55V/cell) start --> 40.8V (3.4V/cell) end, but that may need some adjusting.  3.6V/cell (43.2V) might be a better starting point
```

---
