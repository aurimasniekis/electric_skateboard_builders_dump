# Checking and correcting voltage drift in a battery pack

### Replies: 20 Views: 394

## \#1 Posted by: thisguyhere Posted at: 2019-03-15T18:30:40.411Z Reads: 127

```
Thought this could help:

https://medium.com/@esk8life.orders/checking-and-correcting-voltage-drift-in-a-battery-pack-616e139d2e3b?source=friends_link&sk=74dfb8f3c0bc9f505743d1eee74a704b
```

---
## \#2 Posted by: ryansinatra Posted at: 2019-03-15T18:58:40.136Z Reads: 114

```
Bookmarking to read later. Thanks for the contribution
```

---
## \#3 Posted by: Octave Posted at: 2019-03-15T19:01:37.683Z Reads: 109

```
Very well written and was interesting to read :slight_smile:
```

---
## \#4 Posted by: mccloed Posted at: 2019-03-15T19:20:20.977Z Reads: 102

```
Very nice write up! We use a little 5v fan to discharge cells.
```

---
## \#5 Posted by: thisguyhere Posted at: 2019-03-15T19:37:08.015Z Reads: 97

```
ooh yea, that too.
```

---
## \#6 Posted by: Mudders Posted at: 2019-03-15T20:04:22.968Z Reads: 91

```
Interesting that cell 1 is the highest reading, my bms (d140) has cell 1 as the lowest reading and cell 12 at 50.4v. Its a new pack i have just built, should i switch the wires?
```

---
## \#7 Posted by: thisguyhere Posted at: 2019-03-15T20:25:50.449Z Reads: 86

```
It depends on which direction you're measuring. I suspect you've got voltmeter negative to pack negative, then using positive probe to measure each cell. If so, that'd work in the opposite direction.
```

---
## \#8 Posted by: Mudders Posted at: 2019-03-15T20:30:34.792Z Reads: 85

```
Ahh i see, yes thats what i was doing, glad its all good!
```

---
## \#9 Posted by: Lionpuncher Posted at: 2019-03-15T20:53:43.290Z Reads: 82

```
Awesome write up @thisguyhere. Couldn’t come at a better time, as I am about to correct some drift on my 10s4p pack. Was planning on doing this with a bench power supply. Question tho; on you example, you say cell 3 is the drifting one, how come you’re applying the voltage to cell 7? Or am I seeing this wrong?
```

---
## \#10 Posted by: thisguyhere Posted at: 2019-03-15T20:55:38.547Z Reads: 78

```
omg, this is why people need editors.

you're absolutely right, that's cell 7...

brb

edit- fixed it, thanks
```

---
## \#11 Posted by: Hummie Posted at: 2019-03-16T09:04:52.793Z Reads: 68

```
Think this needs an edit as it seems a lot:
“Variance in voltage readings in the “Cell Voltage” column should be no more than 0.75v.”




I was just asking for ideas to do this. U can also hook cells up to a toaster or hairdryer to discharge. 


And u could throw all cells in parallel. I just did this to a bunch of cells and with a huge voltage spectrum 4.65-3.4.  Barely got warm and took longer than I thought it would.  They are 30q cells.  How I got (3) to 4.65 was due to charging imbalanced cells after ONE charge.   Some cells in parallel had become disconnected during discharge and due to that.  Without a bms u have to be on it. With ur hand testing for heat at least.
```

---
## \#12 Posted by: thisguyhere Posted at: 2019-03-16T17:39:00.186Z Reads: 55

```
[quote="Hummie, post:11, topic:87250"]
Think this needs an edit as it seems a lot
[/quote]

what do you think it should be, less than 0.75v?  0.4v?  i noticed balance charge definitely did NOT kick in at 0.1v, but it did at 0.05v.

i just took the median of the two from experience, because technically it should balance within 0.1v, but that wasn't the case for me.

[quote="Hummie, post:11, topic:87250"]
I was just asking for ideas to do this. U can also hook cells up to a toaster or hairdryer to discharge.
[/quote]

for sure, there's many ways to create a load...i was just naming the most common, probably the easiest way.

[quote="Hummie, post:11, topic:87250"]
And u could throw all cells in parallel
[/quote]

of course, again, i'm trying to describe the simplest way to do this.  it's kind of impractical to parallel additional cells onto a P group when it's already assembled in a pack.
```

---
## \#13 Posted by: thisguyhere Posted at: 2019-03-16T17:39:32.732Z Reads: 49

```
thanks @Lionpuncher for the edit, this diagram is on cell 9, not cell 7.  corrected.

![image|690x261](upload://efWoLmS76udgBTuD8i9lKsFrLhT.jpeg)
```

---
## \#14 Posted by: Hummie Posted at: 2019-03-16T18:22:15.478Z Reads: 47

```
o i didn't understand that a variation of .7 volts being before attached to a bms.    maybe not as clear as it could be and I thought it meant generally when building the battery and running with or without bms.  whatever.    but get that board out going to the po right now.
```

---
## \#15 Posted by: Lionpuncher Posted at: 2019-03-16T20:42:27.567Z Reads: 45

```
I’m doing this atm. Works like a hot damn!

![image|375x500](upload://5vGiYxAT2lh5VbTGC5w3Fn1E9DP.jpeg) 
![image|375x500](upload://wbTsoBkIjrxAPTvzeK4x2dUdB7S.jpeg)
```

---
## \#16 Posted by: thisguyhere Posted at: 2019-03-16T20:57:04.157Z Reads: 41

```
Niice 

A bench dc power supply definitely makes it easier.

Also, them tesla cells 🤩
```

---
## \#17 Posted by: Lionpuncher Posted at: 2019-03-16T22:43:29.482Z Reads: 36

```
They’re tremendous cells, but in the future, if I use them again, it will be for a larger build, aka 12s6+p. Built for ev’s tho so more safety involved in the construction for vibration apparently.
```

---
## \#18 Posted by: Jumpman Posted at: 2019-03-16T23:43:50.174Z Reads: 33

```
[quote="thisguyhere, post:12, topic:87250"]
what do you think it should be, less than 0.75v? 0.4v? i noticed balance charge definitely did NOT kick in at 0.1v, but it did at 0.05v.
[/quote]

Perhaps you meant 0.075V?
```

---
## \#19 Posted by: thisguyhere Posted at: 2019-03-16T23:50:38.781Z Reads: 34

```
You're right!

Fixing....
```

---
## \#20 Posted by: deucesdown Posted at: 2019-03-17T18:32:47.170Z Reads: 27

```
I just found my 13s pack that was reading 3.85/cell on the charger terminals, was 4.13/cell for 12 groups, and 0.0v on 1 group. I'm blaming the 13s bms. At least it prevented charging, which let me know to take a look...

Some stuff that helped me.

https://en.wikipedia.org/wiki/Four-terminal_sensing

I found when pushing the voltage up on a pack with a lab PSU, the greater the current, the greater the voltage difference as sensed by the PSU vs the battery terminals. I ended up leaving a good multimeter hooked up to the battery terminals.

https://www.aliexpress.com/item/150W-Constant-Current-Electronic-Load-60V-10A-Battery-Discharge-Capacity-Tester-ammeter-voltage-meter/32725711985.html

This thing is cheap and really helpful -- the flip side to the lab PSU. Careful there are lots of lookalikes and clones. You can digitally set the parameters you want. It has 4 wire sense on the load connectors. In theory you can set the voltage you want to drain to, and the rate (amps) at which to drain, then walk away. Looks like they added tx/rx ports, hmmm...

![IMG_20190317_142557|666x500](upload://tDa5eEeXsnGsxcczVW0yvlME0BC.jpeg) 

Rigging this test lead really took away a lot of tedium and danger.

![IMG_20190317_142627|666x500](upload://ns3uoHtGhENPMKOzwpr3OyVH5SX.jpeg) 

This splitter (15s => 8s,7s) and meter (8s, not super accurate) also very helpful. I made it to balance charge, but it's very convenient when troubleshooting.

Here's another meter that can do 8s, and shows all cell voltages at once. Only 2 decimal places, and accuracy is meh. Not as nice as the other meter.

https://www.amazon.com/Venom-RC-Checker-Discharge-Function/dp/B073SNZH4K/

Both meters come in many look-alike styles. The CellMeter style can be bought with light bulbs for decently rapid discharge function.
```

---
