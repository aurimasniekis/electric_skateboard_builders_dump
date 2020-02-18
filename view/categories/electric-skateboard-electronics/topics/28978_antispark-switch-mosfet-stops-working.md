# AntiSpark Switch (MOSFET) stops working

### Replies: 12 Views: 836

## \#1 Posted by: Sander Posted at: 2017-07-28T21:53:12.066Z Reads: 138

```
Hi my AntiSpark Switch stops working for some reason.
Yesterday and early today I didn't have no problem turning it on and off with the push button.
I went for a 3km ride with no steep hills and when I come home I noticed it won't turn off, so I opened it and checked why didn't find the reason. The MOSFET wasn't even hot, it was cold, the VESC MOSFETs were hotter. Is it a bad MOSFET again or the push button? Thanks in advance.

This has happened to me before, I replaced the MOSFET and got it working again, suddenly it stopped working like now..

<img src="/uploads/db1493/original/3X/5/2/52aa043b0f5acc11964c169bd60e2ff62cedd895.JPG" width="375" height="500">

<img src="/uploads/db1493/original/3X/5/f/5f0e39d527fb2d5f4e250e8113e1f9199b0f73f2.jpg" width="375" height="500">

<img src="/uploads/db1493/original/3X/c/0/c0b83e934e900be0741c80a42ab33bb27f7ec54a.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/d/6/d65052e8f414e402f6a55bb240d3f0ed9f7b947b.JPG" width="666" height="500">
```

---
## \#2 Posted by: sl33py Posted at: 2017-07-28T22:27:07.935Z Reads: 129

```
[quote="Sander, post:1, topic:28978"]
This has happened to me before, I replaced the MOSFET and got it working again, suddenly it stopped working like now..
[/quote]


you usually want to replace both mosfets if one fails...  likely the other one died, overstressed the new and both dead.  I'd test and swap both.

when they fail they usually fail "closed" - passing current.  there are some videos on how to test i don't have handy, but i'd google really quick to find and test.

GL!
```

---
## \#3 Posted by: Eboosted Posted at: 2017-07-28T22:40:31.435Z Reads: 122

```
I'm looking for a more reliable solution for an antispark switch, I found pricy ones only with direct fets.
```

---
## \#4 Posted by: ShaunPieso Posted at: 2017-07-28T23:09:00.338Z Reads: 117

```
Test the resistance between the source and drain of the mosfets, if you have a short it is bad mosfets if it is not a short mosfets are fine. I had the sme issue and it was the diode so check that. There is nothing else that could go wrong because the cap and resistor does not see a while lot of stress.
```

---
## \#5 Posted by: Sander Posted at: 2017-07-28T23:51:02.741Z Reads: 106

```
I replaced both ;) But I think it may got destroyed while I rode the board today, I accidentally hit the power button and I turned it on again?
```

---
## \#6 Posted by: Sander Posted at: 2017-07-28T23:52:44.410Z Reads: 95

```
I replaced the diode and the mosfets, the mosfet is shorted.
```

---
## \#7 Posted by: sl33py Posted at: 2017-07-29T20:12:58.641Z Reads: 84

```
I'm testing a triple Fet solution from a guy here w/ a higher voltage set of fets.  Will see how it goes...

@goldenHusky has a nice direct Fet solution too.

More robust/reliable - a simple anti-spark loop key is pretty bulletproof.  Only time i've heard one failed i'd assume a QC issue when assembled (faulty), or more likely user error (not fully seated and try to push 50A though it under load).
```

---
## \#8 Posted by: Eboosted Posted at: 2017-09-23T17:21:49.648Z Reads: 66

```
Can someone point me to the correct mosfet to replace the one on my antispark switch?
```

---
## \#9 Posted by: goldenHusky Posted at: 2017-09-23T21:23:11.365Z Reads: 62

```
@Eboosted Which anti spark do you have? Ollin, diy, lhb, aps?
```

---
## \#10 Posted by: Eboosted Posted at: 2017-09-23T21:38:37.136Z Reads: 60

```
I have some DIY switches I'd like to fix them and if possible upgrade components
```

---
## \#11 Posted by: goldenHusky Posted at: 2017-09-23T21:59:23.563Z Reads: 58

```
I have no info on that one, sorry
Maybe @JdogAwesome can help, I think he took a diy switch apart some time ago
```

---
## \#12 Posted by: JdogAwesome Posted at: 2017-09-24T08:02:19.017Z Reads: 50

```
Hey @Eboosted sorry for the late reply and thanks @goldenHusky for tagging me. Hopefully I can help you out, can you post some pics of what switch/MOSFET'S your trying to replace or upgrade? Also try to explain a little more what exactly your trying to do.
```

---
