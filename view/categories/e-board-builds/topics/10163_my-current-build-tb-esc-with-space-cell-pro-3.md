# My Current Build: TB ESC with Space Cell Pro 3

### Replies: 20 Views: 750

## \#1 Posted by: roonydagoony Posted at: 2016-09-26T14:18:32.326Z Reads: 120

```
I'm currently working on this build and would like to know if anyone things there'll be any issues?

TB 12S ESC
DIY 6055 motor (w/ mount)
Enertion Wireless Controller
Enertion Space Cell Pro 3 with enclosure/switch
Kebbek 43" deck

My only concern here is with the signal wires
Back when I had the TB mini wireless controller, the receiver used both the signal wire AND the UBEC power 
However the TB receiver only has 1 port, so do I only connect signal wire? or something else?

Any help would be appreciated!
```

---
## \#2 Posted by: Mark Posted at: 2016-09-26T15:03:40.382Z Reads: 108

```
You need a motor mount, also I would go for a VESC for better braking and performance :)
```

---
## \#3 Posted by: roonydagoony Posted at: 2016-09-26T15:27:35.959Z Reads: 103

```
I have a vesc, but I'm not able to get it working for some reason :/ 
which is why i gave in a got the 12s esc
```

---
## \#4 Posted by: Namasaki Posted at: 2016-09-26T15:39:08.251Z Reads: 91

```
[quote="roonydagoony, post:1, topic:10163"]
Kebbek
[/quote]
Where did you get your vesc?
And what seems to be the problem?
```

---
## \#5 Posted by: roonydagoony Posted at: 2016-09-26T15:45:25.308Z Reads: 79

```
For some guy in Long Island, it works with the **Neo 6364 motor**(it spins at 1 speed when I use the controlled), but doesn't do anything with my **diy 6055 motor**(doesn't spin at all, only shakes a little for a second)
I am basically not able to read it with the BLDC tool, but it does load with ST Link utility
```

---
## \#6 Posted by: i2oadsweepei2 Posted at: 2016-09-26T15:53:30.196Z Reads: 74

```
Is it the Twinkix? I really like that one. I almost bought that deck but decided on the Omen Tango instead. It was a really good deal.
```

---
## \#7 Posted by: roonydagoony Posted at: 2016-09-26T15:55:04.648Z Reads: 71

```
Yes @i2oadsweepei2 that's the one!
```

---
## \#8 Posted by: roonydagoony Posted at: 2016-09-26T15:55:58.419Z Reads: 70

```
I used the deck with my previous build, and it really rocked my socks off. amazing ride quality, super smooth
```

---
## \#9 Posted by: i2oadsweepei2 Posted at: 2016-09-26T16:00:54.552Z Reads: 70

```
Very nice. How stiff is it? I ended up putting 2 layers of Carbon Fiber on the tango to stiffen it up for torqueboards 12s3p battery. It's a Cadillac now :)
```

---
## \#10 Posted by: roonydagoony Posted at: 2016-09-26T16:03:25.408Z Reads: 62

```
it's pretty stiff so far. but I'll know more once I ride it for a week. That's a good idea with the Carbon fiber, I'll take a look into that

Any chance you know if a cheap and good gps tracker that I can stick inside?
```

---
## \#11 Posted by: i2oadsweepei2 Posted at: 2016-09-26T16:07:56.654Z Reads: 62

```
To map your ride or for security? I just use my phone and an app called map my ride. For security I use the trust no one approach.
```

---
## \#12 Posted by: roonydagoony Posted at: 2016-09-26T16:14:44.640Z Reads: 63

```
for security haha
I got my last one robbed in nyc, so I wanna put a tracker on it incase it happens again (won't happen again with this knuckle rings I now own)
```

---
## \#13 Posted by: Namasaki Posted at: 2016-09-26T16:41:29.121Z Reads: 64

```
It's normal to only spin at one speed on the bench. 
That's because of current control. 
If it works with the 6374, then it should work with the 6055. 
But you'll need to do motor detection with the 6055 and apply its parameters before running it with your controller.
```

---
## \#14 Posted by: roonydagoony Posted at: 2016-09-26T18:05:24.309Z Reads: 56

```
That's where the issue is. I'm not able to run motor detection in the tool. the vesc is not recognizable for some reason
```

---
## \#15 Posted by: Namasaki Posted at: 2016-09-26T18:53:08.394Z Reads: 51

```
Are you on windows or mac?
```

---
## \#16 Posted by: roonydagoony Posted at: 2016-09-26T19:16:17.639Z Reads: 53

```
I was using windows (running on parallel on a mac)
```

---
## \#17 Posted by: Namasaki Posted at: 2016-09-26T20:06:59.473Z Reads: 50

```
You would do better running the mac version on mac
Then you don't have to worry bout comports and such.
```

---
## \#18 Posted by: roonydagoony Posted at: 2016-09-26T20:08:53.452Z Reads: 48

```
hmm, I'll try that out today.
not sure why I didn't try that in the first place :slight_smile:
```

---
## \#19 Posted by: Namasaki Posted at: 2016-09-26T21:01:22.433Z Reads: 45

```
Plug in USB cable to vesc and computer then open bldc tool.
```

---
## \#20 Posted by: Namasaki Posted at: 2016-09-26T21:02:23.818Z Reads: 44

```
 Mac is much more plug and play than windows
```

---
