# Testing battery pack with multimeter, is it safe?

### Replies: 9 Views: 400

## \#1 Posted by: RazzleDazzle Posted at: 2018-11-30T16:46:48.233Z Reads: 133

```
Hey guys, i have a fairly cheap 20 dollar multimeter and i went through and tested all my individual 18650 batters (samsung 25r) after i charged them and they're between 4.08-4.12.  I've built up my 10S4P battery pack, i want to do a last check to see what the overall juice of the pack is reading.  Is it safe if i connect my multimeter to it?  I dont want to blow it up with 40V
```

---
## \#2 Posted by: Acido Posted at: 2018-11-30T16:51:13.830Z Reads: 129

```
like the cheapest multi meters are rated for at least 500v or so
it should say somewhere on your multi meter how much amps and volts it can handle
```

---
## \#3 Posted by: skatardude10 Posted at: 2018-11-30T16:56:07.286Z Reads: 124

```
It will read a packs voltage just fine. 

I know this isn't your question, but still a good PSA, don't make the same mistake as me trying to measure amps though, I'm going to guess your meter is rated for somewhere around 10A. To measure amps you don't just switch the lead plugs, swap to amp measurement and measure like you do in voltage on positive and negative lead. You will short your battery this way, it needs to be hooked up in series on the positive or negative lead alone.
```

---
## \#4 Posted by: RazzleDazzle Posted at: 2018-11-30T16:58:07.433Z Reads: 113

```
I did that two days ago and blew my previous multimeter, hence me asking just to be safe :stuck_out_tongue:
```

---
## \#5 Posted by: RazzleDazzle Posted at: 2018-11-30T17:02:06.116Z Reads: 102

```
Quick update.  I just tested it and it was fine.  Pack is reading 41v.  Thats good right for a 10S4P.  Next step is to do the motor config for my VESCs (via VESC tool) with the batter pack connected to test the motors out.  Wish me luck, i'm sooo close to finally finishing this thing.
```

---
## \#6 Posted by: Fiori Posted at: 2018-11-30T18:01:02.565Z Reads: 83

```
You are safe to use it to check voltage yes. Do not try to use it as an inline amperage meter though.
```

---
## \#7 Posted by: thisguyhere Posted at: 2018-11-30T18:23:41.596Z Reads: 76

```
make sure your probes are connected to the correct ports on your multimeter.

i use this one, probes are connected in the circled ports.

![image|288x457](upload://by79kqaYnO15bEQMnqRlTMvzmgm.jpeg) 

the port on the left is for measuring current flow and will burn up the device if you try to measure high voltage / current.
```

---
## \#8 Posted by: RazzleDazzle Posted at: 2018-11-30T18:37:54.296Z Reads: 66

```
Yup, i blew my old multimeter yesterday doing it the wrong way.  I got a new one today and did it right, yay! learning!
```

---
## \#9 Posted by: Fiori Posted at: 2018-11-30T18:40:04.727Z Reads: 66

```
I have that same cheepo. It's been great for the price. I use a Fluke at work, but for home use these are totally fine.
```

---
