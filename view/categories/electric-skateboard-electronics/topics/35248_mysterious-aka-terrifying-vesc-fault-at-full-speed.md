# Mysterious *aka terrifying* VESC fault at full speed

### Replies: 13 Views: 655

## \#1 Posted by: Bazingazunga Posted at: 2017-10-10T16:53:39.612Z Reads: 179

```
Hi all,

So I'd been out for a half hour ride today, and on my way back i was blasting down a steady, small gradient. I wasn't at full throttle (I don't think) but hell I was flying.  Anyway I went to apply the brakes, slowly and gently, and they worked for about half a second. Then nothing. I kept gently squeezing the brakes in the hope that the VESC just had a wobble and reset itself, but no, no brakes. 

Managed to coast it off a bit and foot brake to safety but jesus my heart leapt!

So I flip the board over to have a look, and there's no visible damage. No excessive heat, no smell of burning, plus the clear heatshrink round the VESC doesnt even look like it's warped. Lights on the VESC are as usual, one blue one green. The only fault I can see is whenever i try to give it some throttle or brake, it flashes red three times, twice (six in total) 

Walked home, plugged into BLDC, FAULT_CODE_NONE. 

Im a bit at a loss here - little bit scared it could happen again. Anyone experienced this? I had a search for threads but can't find any similar.

Cheers
```

---
## \#2 Posted by: Hummie Posted at: 2017-10-10T16:58:27.237Z Reads: 170

```
What is ur max powered speed and were u above it?  At least the throttle will behave like a brake above the no-load speed but don't remember how throttle is  affected
```

---
## \#3 Posted by: Bazingazunga Posted at: 2017-10-10T17:00:25.561Z Reads: 170

```
Ok great, managed to go to Realtime data -> Activate Sampling and replicate the throttle issue.

You guessed it: DRV8302!

Ding ding ding we have a winner!
```

---
## \#4 Posted by: Bazingazunga Posted at: 2017-10-10T17:01:05.447Z Reads: 166

```
Thanks for you reply man, I have a stinking suspicion I just went above ~60k :weary:
```

---
## \#5 Posted by: Hummie Posted at: 2017-10-10T17:03:31.628Z Reads: 163

```
Are brakes affected when going over the no-load speed?
```

---
## \#6 Posted by: Bazingazunga Posted at: 2017-10-10T17:05:50.317Z Reads: 159

```
Couldn't even guess, hopefully someone else can chip in? 

FYI I was on a 260kv 8s @ 83mm, ~31mph is no-load max
```

---
## \#7 Posted by: Jinra Posted at: 2017-10-10T17:47:48.568Z Reads: 141

```
FOC or BLDC?
```

---
## \#8 Posted by: JohnnyMeduse Posted at: 2017-10-10T17:53:28.123Z Reads: 138

```
What Brand of Vesc and which Firmware?
```

---
## \#9 Posted by: Deckoz Posted at: 2017-10-10T22:17:25.897Z Reads: 106

```
This is how my second 4.12 died. Going downhill, hit the brakes at the end going about 40mph(metre.at on my watch said 39), worked for half a second then no brakes. Master died, I foot braked. Coulda been erpm, or overvoltage. Lesson learned, if your making a cruising/downhill combo board, gear it for the speeds you'll achieve downhill - as erpm doesn't seem to matter. There's things like vesc6 which is 150kerpm sure. But two 190kV motors spinning fast enough to be above 60V will still kill all versions of a VESC. So you have to keep your motor speed down.
```

---
## \#10 Posted by: Bazingazunga Posted at: 2017-10-11T19:05:38.240Z Reads: 69

```
BLDC 10char
```

---
## \#11 Posted by: Bazingazunga Posted at: 2017-10-11T19:06:29.934Z Reads: 66

```
Just a maytech, 4.12 on 2.18 :joy: good job i bought a FOCbox a few weeks ago.. buy cheap buy twice!
```

---
## \#12 Posted by: evoheyax Posted at: 2017-10-11T19:31:22.895Z Reads: 59

```
[quote="Bazingazunga, post:11, topic:35248"]
buy cheap buy twice!
[/quote]

This is something I try hard to share.

Unless your an engineer, and you know how to measure and calculate everything to a tee (and even then, low quality can still bite you), you should over engineer your system. Cheap is never an over engineering (and unusually, is under engineering).

I wasted almost $800 on my first board before I started to buy quality. focbox or chaka vesc are the standard right now.
```

---
## \#13 Posted by: JohnnyMeduse Posted at: 2017-10-11T21:21:37.400Z Reads: 38

```
Well, the Maytech Vesc are not renoun for their quality, also the older one has a bug inside their firmware, that ramp up the current too fast and burn DRV
```

---
