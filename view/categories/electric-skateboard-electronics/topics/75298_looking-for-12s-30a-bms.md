# Looking for 12s 30a BMS

### Replies: 19 Views: 191

## \#1 Posted by: lambievu0916 Posted at: 2018-11-20T02:48:05.959Z Reads: 63

```
Hello everyone, 

Forsome reason my bms started to get suoer hot at a certain spot, and my one of the cells were super hot ass well. Anyone knows whats going with that?
```

---
## \#2 Posted by: Sn4pz Posted at: 2018-11-20T02:57:28.538Z Reads: 62

```
check your battery welds, might not be the BMS. 

if it is your BMS you can do a charge only BMS, and bypass discharge
```

---
## \#3 Posted by: lambievu0916 Posted at: 2018-11-20T03:09:27.100Z Reads: 58

```
It might be my welds, but what could be the reason with the welding? I had to re weld everything so the prior nickle strips had the dots left over so i can barely get a good sticking weld. Should i just get new batteries to be safe?
```

---
## \#4 Posted by: mynamesmatt Posted at: 2018-11-20T05:37:40.045Z Reads: 52

```
are you looking for a bms or having issues with your current one or...?
```

---
## \#5 Posted by: lambievu0916 Posted at: 2018-11-20T05:48:30.802Z Reads: 48

```
If i can fix it yes! But not then ill buy a new bms
```

---
## \#6 Posted by: Mikenopolis Posted at: 2018-11-20T05:59:35.841Z Reads: 43

```
No idea what is happening with yours. I had an issue with my 12s3p battery where my thermal camera showed part of it being hotter than the rest of the pack. Turns out one of the series packs was at 0.0vand not charging. psychotiller helped me put in new cells replacements. And also changed my BMS to charge only because it was cutting me off when I pushed the board a bit hard. 

Anyway. The 12s BMS would be a bit warm even after charging is done, read it up as BMS doing its job but over the week it would drain the 100% pack to 39% before the warming/draining would stop. Really annoying as I can’t have a 80-90% ready to go board ever.
```

---
## \#7 Posted by: lambievu0916 Posted at: 2018-11-20T06:14:05.887Z Reads: 44

```
My bms from diyelectric was nice and didnt loose its charge at all but cant seem to find where they got it
```

---
## \#8 Posted by: thisguyhere Posted at: 2018-11-20T07:14:55.336Z Reads: 41

```
measure each P group voltage, i bet there's one that's way out of balance.

stick your voltmeter positive on pack positive, then measure each balance lead.

record that on a spreadsheet or something, subtract each subsequent voltage reading, that'll give you each P group voltage.

once you isolate which P group is gone bad, inspect that area closely to ensure no shorts or anything out of the ordinary.  make sure balance leads are installed correctly, nothing exposed or wires crossing over each other.

if pack looks ok, you may have a bad bms.
```

---
## \#9 Posted by: Mikenopolis Posted at: 2018-11-20T07:20:52.034Z Reads: 40

```
Found the picture of the 3 cell that got hotter than the rest of the pack. This 3p was reading 0.0V. Not sure the physics of my it turned hot after a short ride. 

![flir_20180928T095937|640x480](upload://jYACBHsFlXdbSt4HXFoeV5zenrF.jpeg)
```

---
## \#10 Posted by: lambievu0916 Posted at: 2018-11-20T08:09:50.629Z Reads: 36

```
I think there was a p group that didnt have a good weld, in there which was the one that was getting super hot. 

Should i just getna new set of batteries and rebuild from there? And repurpose the old ones since its hard to get the surface to be clean for a nice weld?
```

---
## \#11 Posted by: pat.speed Posted at: 2018-11-20T08:47:40.431Z Reads: 31

```
No, not yet. All you need to do is measure the voltage across the balance leads. All cells should be closely balanced, if not that might be your problem and it will be a lot cheaper than buying new batteries
```

---
## \#12 Posted by: accrobrandon Posted at: 2018-11-20T14:16:10.853Z Reads: 26

```
well if you can get the cells free of the pack...or atleast get the nickel strip off if theres any burrs you cant manually get you could use a dremel  with the round ball like file attachments and ever so lightly and graciously file off the burr to get a smooth surface again right where you need it...
```

---
## \#13 Posted by: lambievu0916 Posted at: 2018-11-20T18:01:59.689Z Reads: 22

```
Loving the ideas, but i was an idiot when i made my pack and kinda touch the positives and negatives together a couple times, so ik not sure if i mest up some cells there. But worst case scenario ill try the dremel thing and test the voltage as i out it back together
```

---
## \#14 Posted by: lambievu0916 Posted at: 2018-11-20T18:40:20.843Z Reads: 20

```
so i just measured the p groups, i found that 3 of them came out to be 2.4 volts and the rest were 3.4 volts. Also one of the 2.4 groups i dismantled and check the voltage, but it came out one was battery was 2.4 and the other one was at .6 volts
```

---
## \#15 Posted by: thisguyhere Posted at: 2018-11-20T19:01:59.955Z Reads: 18

```
ok, so that one P group with the near zero volt cell is dead, you should just get rid of it.

generally liion cells can be drained down to 2.5v without damage so the groups at 2.4v _may_ be ok to salvage.

but consider, taking cells to their extremes will prematurely alter / increase their internal resistance so you may find they drift more easily.  if this happens it's important to keep them balanced, so charging to 100% and letting the bms complete its float charge.
```

---
## \#16 Posted by: lambievu0916 Posted at: 2018-11-20T19:28:01.641Z Reads: 19

```
okay gotcha gotta get some replacements then and ill rebuild the pack to see if i get problems with the bms.
```

---
## \#17 Posted by: thisguyhere Posted at: 2018-11-20T20:27:23.202Z Reads: 16

```
i've got 30q cells if you need em, in US

https://www.esk8life.com/samsung-30q-18650-cell
```

---
## \#18 Posted by: lambievu0916 Posted at: 2018-11-20T20:46:21.011Z Reads: 16

```
How much are the cells?
```

---
## \#19 Posted by: lambievu0916 Posted at: 2018-11-28T08:51:26.378Z Reads: 10

```
UPDATE: i replaced the cells and everything is welded correctly and voltage is 46V but my bms is still heating up. Does that mean my bms isn't working properly? Or it is working properly and i just didnt do a good job at checking my welds
```

---
