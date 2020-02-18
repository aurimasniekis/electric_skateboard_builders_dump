# 12S2P Battery Orientation Suggestions

### Replies: 7 Views: 991

## \#1 Posted by: Emerson Posted at: 2018-02-28T16:41:22.169Z Reads: 141

```
Hey all, I'm starting the process of building a 12S2P battery (30Q, BMS Charge Only) for my upcoming Icarus build.  My goal is to build a 1 stack, flat pack but I'm unsure as to the best layout. Here's what I'm planning on going with thus far...

 ![12s2p|535x499](upload://fKxPZSHzu8ujJAFdTuE2hpWpv0c.png)

I'll be using the boss spot welder with 10mm x .15mm pure nickel strips.  I've already placed fish paper ring/covers over each of the positive sides of the batteries but that's about it thus far.

I'm assuming I'll need to double stack the nickel strips for the series connections but don't seem to have much luck with getting a good spot weld (for double stacked strips only).  I'm running 2 x 3s 4AH 40C zippy lipos in parallel so I should have plenty of amps to draw.  My testing thus far has forced me to go rather high on the MS (10+) to get a decent weld and no real luck on double stack. 

Any suggestions for a different orientation? Nickel Strip usage? Spot Weld Suggestions?

Edit: 1.5mm to .15mm correction
```

---
## \#2 Posted by: chsknight Posted at: 2018-02-28T17:25:15.894Z Reads: 115

```
When double stacking strips, I like to first weld one strip to the batteries then weld the second to the first.
```

---
## \#3 Posted by: thisguyhere Posted at: 2018-02-28T17:29:59.435Z Reads: 120

```
i'm assuming you're using a sunko spot welder?

nickel to steel (cell) welds are fine, but nickel to nickel welds suck.  i've had to redo an entire set because the 2nd layer of nickel started to come off on its own.

since it's a 2p pack you should be ok with one strip, esp. since it's 10mm.

if you're uneasy about that, just use a higher gauge (> 14awg) copper stranded silicone wire on your series connections, that should bring your ampacity above whatever you pack can discharge.

in terms of layout, the diagram you have is the most common and would work fine.
```

---
## \#4 Posted by: ZackoryCramer Posted at: 2018-02-28T17:42:18.640Z Reads: 111

```
I used 12 awg wires on the sides. But for the bms, I would be careful on positioning it right on top of the pack. The bms I have has pins pointing right down which could easily stab the battery wrapping into the negative terminals.
```

---
## \#5 Posted by: Deckoz Posted at: 2018-02-28T18:56:03.204Z Reads: 96

```
[quote="Emerson, post:1, topic:47763"]
using the boss spot welder with 10mm x 1.5mm
[/quote]

I think you mean .15

What are your settings? 

If it's dual layer .15 try X3 4.0 Amp, 2.0ms between pulse rate. This should be able to weld through both to the terminal on 4s...

![1519844134471959942385|375x500](upload://layojpEin5RU0WGCdWEgq7cG32h.jpg)
```

---
## \#6 Posted by: Emerson Posted at: 2018-02-28T20:00:33.810Z Reads: 80

```
Correct with .15 mm...sorry about that (edited above).  I was using X1 10ms, *1ms.  But that was only using a high amp 3S.  Sadly I only have the two 3S lipos and one 6S.  My parallel cord isn't the small adapter but rather 6" long 12awg.  I'll probably make the small parallel adapter soon and hopefully that will increase performance a bit.
```

---
## \#7 Posted by: rojitor Posted at: 2018-03-01T14:10:49.809Z Reads: 56

```
If you are using wired parallel adaptor there you have your amps loss.
You MUST use short compact adaptor or really thick and short wired adaptor. You will have low performance otherwise
```

---
