# Interesting VESC problems

### Replies: 15 Views: 216

## \#1 Posted by: jojamcha Posted at: 2018-10-16T22:09:03.843Z Reads: 74

```
Hello. My VESC seems to be experiencing technical difficulties. Please Help! :sweat:
```

---
## \#2 Posted by: jojamcha Posted at: 2018-10-16T22:10:08.080Z Reads: 74

```
here are the pics for my setup (sorry about the glare)
![skate%201|640x480](upload://4QaDbhYET2VIIW0GDpfvcbJCL6Z.jpeg) ![skate%202|640x480](upload://8oHFjcMwo5CjDIRmuBV2lH2jYI4.jpeg) ![skate%203|640x480](upload://eFoswxcCWtHkEbb00f6fus1b5o8.jpeg) ![skate%204|640x480](upload://gX9Q22G5c78eisdohftETNLbmht.jpeg) 
and my settings
![skate%205|690x423](upload://hPzOmTaoq1a591I9FcmymMdueP3.png) 
![skate%206|690x416](upload://v80DNWxE9l4SBARoZWFpYmsaYH0.png) ymMdueP3.png) 
this is what I get when I run the motor detection
![skate%208|690x416](upload://wUZZxmGAQrPt30qho1L65u2EIgv.png) ![skate%207|283x47](upload://tta9MaHHh22tJPQF9GqIwiL1i4Y.png) 
and the fault code![skate%209|318x65](upload://4BxLAQok9RR1fblUP8nwzpd7Zy.png) 

Also, the VESC always blinks pink in sets of two blinks.
I'm stumped to what could be causing this problem.
```

---
## \#3 Posted by: Jake2k17 Posted at: 2018-10-16T22:18:05.098Z Reads: 61

```

1. Draw a diagram of your wiring and post that too. It’s hard to see what goes where with the wiring in your pictures.
```

---
## \#4 Posted by: Pmac Posted at: 2018-10-16T22:24:58.267Z Reads: 60

```
As per Jacob's comment.  It would be easier to see what is going on with a clearer image of your wiring to rule that out as an issue.

I have never seen a VESC flash pink so all I can say is check for fault codes in the VESC Tool to see if there is an issue with the VESC.

From personal experience I had issues detecting motor's and I had to lower D: 0.05 to D: 0.03 and it worked.  That is my own personal experience and as I have never seen the VESC flash Pink it may be a completely different issue that you are encountering.

Good Luck!
```

---
## \#5 Posted by: jojamcha Posted at: 2018-10-16T22:32:36.504Z Reads: 54

```
Thanks!
Here is the diagram ( i'm sorry i'm not much of an artist :sweat_smile: )
![skate%2010|640x480](upload://tWNUIr49jQMSgevcrVO7Z88q94V.jpeg)
```

---
## \#6 Posted by: jojamcha Posted at: 2018-10-16T22:33:14.490Z Reads: 50

```
I hope you can see that well enough. If not, I can try to get a clearer picture


The batteries are all with HXT 4mm series connector wires ( the wires are 12awg)
```

---
## \#7 Posted by: thisguyhere Posted at: 2018-10-16T22:39:48.195Z Reads: 50

```
are each of those lipo packs 2s?

you have cell count set to 6 in vesctool 

whatever the pack S count is, multiple that by three, put that number in series count
```

---
## \#8 Posted by: jojamcha Posted at: 2018-10-16T22:43:35.662Z Reads: 53

```
I changed the cell count, but that did not help. I have been working on this for a while and am starting to think my VESC is seriously messed up :(
```

---
## \#9 Posted by: alexnz Posted at: 2018-10-16T22:47:21.772Z Reads: 54

```
Well, if you have a FAULT_CODE_UNDER_VOLTAGE, the sensible thing to do would be to take a voltmeter and check what voltage you have out of your XT90.

You would also have other info in the VESC terminal if you type "faults".
```

---
## \#10 Posted by: jojamcha Posted at: 2018-10-16T22:50:47.573Z Reads: 50

```
nope. Nothing out of the terminal when I type "faults", just the UNDER_VOLTAGE one. I will try the voltometer though
```

---
## \#11 Posted by: alexnz Posted at: 2018-10-16T23:00:24.093Z Reads: 49

```
I just noticed in the ( Ackmaniac's) ESC Tool that the battery cutoff are different for Li-Ion and LiPo. Not that it would help in your case if it's an undervoltage, but you might want to set it right for the sake of keeping your  batteries safe-ish.
```

---
## \#12 Posted by: jojamcha Posted at: 2018-10-16T23:23:20.583Z Reads: 47

```
Ok thanks. I will catch up tomorrow when I can head to my workshop to check voltage output.
```

---
## \#13 Posted by: torqueboards Posted at: 2018-10-17T00:06:59.700Z Reads: 40

```
@jojamcha you can check in real time to see your actual voltage reading from your pack. It needs to be above 20.40v (which you set it at) otherwise it won't motor detect and will fail.
```

---
## \#14 Posted by: mynamesmatt Posted at: 2018-10-17T02:26:02.130Z Reads: 33

```
also turn your battery current wayyyyy down to anything below 40a
```

---
## \#15 Posted by: Jake2k17 Posted at: 2018-10-17T03:40:10.989Z Reads: 29

```
Yeah your cutoff may be too high, charge your batteries to full or close if you can and lower the cutoff
```

---
