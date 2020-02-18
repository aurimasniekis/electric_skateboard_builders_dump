# Low voltage cutoff in VESC

### Replies: 11 Views: 842

## \#1 Posted by: lennarn Posted at: 2018-11-19T17:24:04.695Z Reads: 172

```
I'm running my 12s build with two Turnigy 5Ah 6s cells. Doing a test ride, my VESC did not cut off in time to prevent over discharge, and one of the cells got down to 2.7v. I managed to save it by slowly charging that cell up to match the others with a power supply in CC mode.
I think I've set the LVC wrong in VESC settings. At 37.2v LVC that's 3.1v/cell! Do I need to set cutoff start at nominal voltage? (3.7*12=44.4v) What is your LVC/cell?
Should I use an external voltage alarm? When I install a BMS, will that also have a LVC? Any more guidelines, tips and pointers about battery care and avoiding hiccups like this in the future?
![LVC|542x172](upload://xg8ApI39wzTbw0k53UsPvuGSZC9.png)
```

---
## \#2 Posted by: mynamesmatt Posted at: 2018-11-19T21:39:05.976Z Reads: 154

```
yes a bms has low voltage cutoff but for each individual cell. eg my board cut out the other day because one cell was at 3v while the others where at 3.7v. glad i didnt have a charge only bms because there would've been a problemo. Also just to be safe, set the start to 3.4v/cell and end to 3.2v/cell
```

---
## \#3 Posted by: Benjamin899 Posted at: 2018-11-19T22:00:38.234Z Reads: 146

```
yeah, i would also set the cutoff higher, it gives your vesc time to throttle down the amp draw, if that window is too small and you go full throttle it could still send you flying.
```

---
## \#4 Posted by: skatardude10 Posted at: 2018-11-19T22:32:16.271Z Reads: 140

```
I set mine to 3.2 start - 2.8 end... it's lower than I was originally comfortable with, seeing as my vape batteries discharge to 3.2/3.3v.

Most lithium ion 18650 cells can discharge safely down to 2.5v, some 2.75ish. 

The capacity that remains after 3v ish though is very minimal. Taking into account voltage sag, my cells at 3.5v may sag to 2.8... the vesc does a good job of cutting them off, and I've only ever ran my pack down to a total of 3.2v after many many miles... Only cutting off at 2.8 due to sag from the amp draw during acceleration.

I guess what I'm trying to say is, like @mynamesmatt, if you are running your BMS for discharge as well as charge, you should be safe per P group for low voltage cutoffs, and beyond decreasing your packs life a bit, it's within most batteries rated specs to be able to discharge very low safely, regardless of however few extra half a miles you will get by setting it low. So don't feel like you have to set your cutoffs above 3.3-3.4v unless you prioritize extending the lifespan of your battery a bit over gaining that extra couple miles of potential range you might be able to get. 

Me personally, I like having the headroom for additional range if I need it in a pinch, less range anxiety, since we can't change voltage cutoffs on the go unless you have USB headers on your enclosure and carry a laptop or Android port of vesc tool (I do have both but vesc tool on the road is a pain). I just watch and when I get to around 20-30% I call it a day or time for a charge to extend my packs life.
```

---
## \#5 Posted by: lrdesigns Posted at: 2018-11-19T22:49:23.331Z Reads: 113

```
With lipo 1p packs it’s advisabe to use voltage alarms for all cells or much higher vesc cutoff I think I have mine start at 3.6v. 

From my experience with lipo there always a cell or two in a 12s 1p pack that discharges faster then the rest. 

While a 4p 18650 pack is going to be much more closely matched between groups.
```

---
## \#6 Posted by: lrdesigns Posted at: 2018-11-20T00:16:33.785Z Reads: 109

```
Just last night it happened to me, ran the board down to the cut off and one cell got down to 2.7 while others where at 3.5 ish. 

Cutoff start 3.625v.   It really depends on the condition of your cells and how well matched they are. 

![image|690x141](upload://gMrgXO1jpjchLFeddGSMXSa2Wpb.png)
```

---
## \#7 Posted by: mynamesmatt Posted at: 2018-11-20T02:18:23.088Z Reads: 95

```
i agree with ya, just gotta be aware he's using lipo so the minimum you wanna ever really be at is 2.9v. anything below is not good at all. So you play it safe and go cutoff at 3.2v each
```

---
## \#8 Posted by: skatardude10 Posted at: 2018-11-20T02:44:05.364Z Reads: 97

```
Oh!!! Didn't catch that. Yeah I wouldn't want a lipo lower than 3.3v max or even higher! 

My bad 🦁
```

---
## \#9 Posted by: youseekcota Posted at: 2019-01-21T00:10:31.656Z Reads: 85

```
Did just that.
```

---
## \#10 Posted by: Benjamin899 Posted at: 2019-01-21T16:01:16.637Z Reads: 79

```
damn, are you alright? Learnt it the hard way. My soft cutoff starts at 3.4v/cell, so i have a nice buffer.
```

---
## \#11 Posted by: youseekcota Posted at: 2019-01-22T00:34:59.533Z Reads: 74

```
Yeah, thank God for my Dainese body armor. Put a big dent in the shoulder plate, and hit my knee so hard that it probably would have turned to hamburger meat without my D3O kneepads
```

---
