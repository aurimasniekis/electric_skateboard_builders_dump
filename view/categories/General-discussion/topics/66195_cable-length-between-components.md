# Cable length between components

### Replies: 25 Views: 292

## \#1 Posted by: malJohann Posted at: 2018-08-27T02:32:11.847Z Reads: 109

```
Hi guys, I'm about to embark on my first DIY build.

I need advice on cable length, as in what affects what electronically. If for example I wanted to relocate certain parts to the front, or in a backpack. You get the idea.

My main concerns being resistance and spikes/surges.

So, how much does electric cable length matter between:
1. Battery and ESC

2. ESC and Motors

Could I have:
1. Two ESCs mounted to the front behind the truck, batteries in the middle and motors at the back?

2. Two ESCs and batteries at the front and motors at the back?

3. Two ESCs at the front and batteries in a backpack with a breakaway connection on the board?

4. Two ESCs and batteries in a backpack with a breakaway connection on the board?

Thanks in advance for any advice.
```

---
## \#2 Posted by: dareno Posted at: 2018-08-27T02:42:00.376Z Reads: 104

```
This information is all here for the taking.  Search button.  Its a fountain of information if you use it.  There are so many different iterations of builds on here that everything that you have just asked is readily available for you if you just research.  With 6hrs of reading you haven't imo done enough.  Everyone on here has done the hard yards so members can access practically anything at the touch of a button.
```

---
## \#3 Posted by: kuphjr Posted at: 2018-08-27T02:44:48.534Z Reads: 98

```
Honestly unless you have like 5 feet of wire in your board for some random reason it does not matter at all. Just use 12 gauge wire for a single motor board and 10 for a dual as a general rule of thumb. Or just do what most people on the forum seem to do and use 10ga throughout. Its only a couple bucks extra.
```

---
## \#4 Posted by: malJohann Posted at: 2018-08-27T02:50:28.969Z Reads: 93

```
Thanks for pointing that out. Suppose nothing new under the sun.
```

---
## \#5 Posted by: malJohann Posted at: 2018-08-27T02:50:50.305Z Reads: 88

```
Good info, much appreciated.
```

---
## \#6 Posted by: mmaner Posted at: 2018-08-27T02:57:52.629Z Reads: 83

```
Typically you want to keep power to VESC's and phase wires to the motor as short as possible, I'm not saying only use 3cm of wire just keep it short.  Other than that you are pretty free. 

Also, don't use 3 feet of wire to a loop key, if your using one, that can be bad (learned the hard way).
```

---
## \#7 Posted by: dareno Posted at: 2018-08-27T03:04:09.638Z Reads: 82

```
Ignore me I've had a bad day :persevere:
```

---
## \#8 Posted by: kuphjr Posted at: 2018-08-27T03:08:07.787Z Reads: 82

```
well you weren't wrong about the search button...
```

---
## \#9 Posted by: dareno Posted at: 2018-08-27T03:14:21.698Z Reads: 77

```
True but when magic mike shames you you just have to eat humble pie :joy:
```

---
## \#10 Posted by: malJohann Posted at: 2018-08-27T03:15:24.083Z Reads: 74

```
I'm not eating anything offered to me by a half naked man.
```

---
## \#11 Posted by: dareno Posted at: 2018-08-27T03:15:55.867Z Reads: 72

```
probably the wrong analogy.
```

---
## \#12 Posted by: dareno Posted at: 2018-08-27T03:19:18.972Z Reads: 72

```
Trust me though the man does know his shit.  Listen and heed his words.  There are a few guys on here that are a level above the rest of us and you have just been lucky enough to hit the radar of one of them.
```

---
## \#13 Posted by: mmaner Posted at: 2018-08-27T03:25:59.623Z Reads: 67

```
1.  I'm frequently half naked, never in public.
2.  Didn't mean to shame you, just chilling an answering some questions.
3.  Thanks for the kind words, means a lot.
```

---
## \#14 Posted by: lrdesigns Posted at: 2018-08-27T03:27:58.439Z Reads: 67

```
As far as I know the only length that is critical is from the BATTERY --- to the --- ESC. Keep that as short as practical. Even if it means longer motor wires.

Under 12 inches should be fine.

If it has to be long then you can use extra capacitors to compensate.
```

---
## \#15 Posted by: dareno Posted at: 2018-08-27T03:47:59.360Z Reads: 61

```
time to be objective.
[quote="malJohann, post:1, topic:66195"]
1. Two ESCs mounted to the front behind the truck, batteries in the middle and motors at the back?
No worries
2. Two ESCs and batteries at the front and motors at the back?
no worries
3. Two ESCs at the front and batteries in a backpack with a breakaway connection on the board?
Why?
4. Two ESCs and batteries in a backpack with a breakaway connection on the board?
again why?
Thanks in advance for any advice.
[/quote]
most production boards have the battery and esc's at each end of the board with no issues and so do 2 of my own builds again with no issues.  It seems the length of your standard board will not cause problems with cable length but as for the whole back pack scenario then you've got me there.  
The only issues I've read about are the distance between battery and esc's so keep them within your boards dimensions and there shouldn't be an issue.
If you are connecting components over distance then resistance is something to be avoided and the longer your wiring the greater the resistance so if you are going to be spreading things out then make sure that the cabling used compensates for that.  Bigger the better.  keep the current flowing man!
```

---
## \#16 Posted by: Winfly Posted at: 2018-08-27T04:07:06.113Z Reads: 57

```
I don't understand why battery wire is "critical"? as long as you have the correct gauge wire (thick enough to carry your desire amperage), the copper wire resistance is basically insignificant at this length. if anything you shouldn't have long motor phase wire as it would affect the permutation of the ESC when your motor at high rpm.

http://hyperphysics.phy-astr.gsu.edu/hbase/Tables/wirega.html

I'm on @mmaner side on this one.
```

---
## \#17 Posted by: lrdesigns Posted at: 2018-08-27T04:27:46.316Z Reads: 56

```
It's not about resistance, its about inductive load and voltage spikes. 

Long DC power wires can become inductors which increase the severity of voltage spikes. The large caps on the esc is to smooth out the voltage spikes. 

If your caps are too small or the wires too long the voltage spikes will kill the esc over time.
```

---
## \#18 Posted by: malJohann Posted at: 2018-08-27T04:29:41.708Z Reads: 54

```
So if the ESC and batteries are close together, how would distance from the ESC to the motors affect the performance?
```

---
## \#19 Posted by: dareno Posted at: 2018-08-27T04:41:06.750Z Reads: 57

```
[quote="lrdesigns, post:17, topic:66195"]
It’s not about resistance, its about inductive load and voltage spikes.
[/quote]

Which is irrelevant over the distance he is talking about.  Unless we are getting into the backpack scenario and then I will say again why?
```

---
## \#20 Posted by: Andy87 Posted at: 2018-08-27T04:44:06.978Z Reads: 55

```
What you think would be the right size of capacitors for a usual mtb set up.
Batteries in the middle of the deck, esc on the end, cables about 50cm (routed over the binding add some length too). 12s battery and let’s say 5ah.
Is there an easy way to calculate?
```

---
## \#21 Posted by: lrdesigns Posted at: 2018-08-27T05:01:47.613Z Reads: 46

```
[quote="Andy87, post:20, topic:66195"]
Is there an easy way to calculate?
[/quote]

I'm sure there is some formula. But I'm no electrical engineer. If any of the legit electrical engineers on here could chime in that would be awesome.  [This thread on RCgroups](https://www.rcgroups.com/forums/showthread.php?952523-too-long-battery-wires-will-kill-ESC-over-time-precautions-solutions-workarounds) seems to suggest an extra 220uF every 10cm of aditional length. 

I have seen a few MTB guys use these [pre made cap banks](https://www.yge.de/en/accessories/) from YGE
```

---
## \#22 Posted by: Andy87 Posted at: 2018-08-27T05:05:29.096Z Reads: 48

```

[quote="lrdesigns, post:21, topic:66195"]
220uF every 10cm of aditional length.
[/quote]

With additional you mean everything over 30cm?
```

---
## \#23 Posted by: danielz Posted at: 2018-08-27T06:14:43.081Z Reads: 43

```
Inductance is certainly not irrelevant, it can and does kill electronic devices all the time and countless RC escs. Youtubes eevblog videos has many great videos on bypass/decoupling caps. The large caps only filter the low frequency stuff, but can easily be added to. The ceramics filter the high frequency stuff and arent easily added to. Which is probably why so many cheapo vescs die, the ones with upgraded higher rated ceramics tend to fair better.

Remember to tape or tie the + and  - together closely, to also reduce inductance.
```

---
## \#24 Posted by: AutoItKing Posted at: 2018-08-27T06:32:46.247Z Reads: 40

```
At the lengths we're talking about inductance will be pretty low, but it can still cause some nasty voltage spikes. A good rule of thumb is about 1 nH/cm. Basically what you want to do is give the spikes a place to go.
Inductors oppose change in current, say 20 amps are flowing through a wire and you suddenly stop pulling 20 amps (open the circuit). The inductance will want to keep that current flowing causing a voltage spike.
If I get bored I might do a quick simulation to see what difference it might make.
```

---
## \#25 Posted by: Winfly Posted at: 2018-08-27T06:42:34.973Z Reads: 39

```
you right. that's a very good link. _Rule of thumb caps everywhere_
```

---
