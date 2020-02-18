# 1 charging plug for 2 BMS&rsquo;s? (2x 6S LiPos)

### Replies: 17 Views: 2236

## \#1 Posted by: Tijmen Posted at: 2016-12-10T20:02:23.210Z Reads: 162

```
Hey guys. Would really appreciate some help here.

I want to build a dual motor board, so I will need 2 ESC's. I also want it to be chargeable through a BMS and therefore one charging plug for a plug-in and forget solution.

I will be using 4 batteries in total. 4x  30C 8000mAh 3S batteries. Two wired together to be 6S, and then I assume each 6S pack has to go to one ESC and one motor. But I want to be able to charge all batteries with one plug.

I have no idea how I'd even begin to wire this. Is it possible to wire one BMS to each 6S battery, and then splitting power from the charger input on the board to each BMS, and using a higher voltage and amperage charger?
```

---
## \#2 Posted by: jmasta Posted at: 2016-12-10T20:09:30.467Z Reads: 158

```
Your 2x ESC's should be hooked up to the battery pack in parallel, so that they see identical voltages and the current is split between the two.  Then you only need one BMS and one total battery pack (consisting of multiple batteries)
```

---
## \#3 Posted by: rpn314 Posted at: 2016-12-10T20:09:39.766Z Reads: 154

```
I would make it one big pack. So if you want a total of 6s, then a 6s2p. So the black and red of the two 6s packs will be connect to each other (a parallel connection) and then you split that to each ESC
```

---
## \#4 Posted by: Tijmen Posted at: 2016-12-10T20:13:53.646Z Reads: 140

```
So the combined battery pack would be 12S, but would be split across 2 ESC resulting in each receiving 6S voltage right?
```

---
## \#5 Posted by: rpn314 Posted at: 2016-12-10T20:14:38.575Z Reads: 133

```
you could do 12s if you'd like (all of them end to end) or 6s and have half of them be in parallel (2 sets of 2 end to end, and then 2 sets of those side by side)
```

---
## \#6 Posted by: jmasta Posted at: 2016-12-10T20:24:29.039Z Reads: 126

```
[quote="Tijmen, post:4, topic:14475, full:true"]
So the combined battery pack would be 12S, but would be split across 2 ESC resulting in each receiving 6S voltage right?
[/quote]

No. Maybe it'd be more clear with numbers.   For example, if you had a 12S battery pack delivering 60A to two ESC's in parallel, each ESC would get 12S 30A
```

---
## \#7 Posted by: rpn314 Posted at: 2016-12-10T20:32:39.747Z Reads: 111

```
Oh, yeah, that's correct.
```

---
## \#8 Posted by: Tijmen Posted at: 2016-12-10T20:36:42.881Z Reads: 109

```
Man I wish I was better at this kind of stuff.

Basically I'd be using two motors requiring 6S, two 6S ESC's and two 6S battery packs.
Do I wire the two battery packs in parallel then? Wouldn't that simply increase my mAh and not my output amperage? 
Basically I need 6S going into each ESC, and each motor needs to be able to draw at least 60A. And all batteries need to be wired so I can charge them through one charging plug into a BMS but I'm so confused as to how it'd all be wired...
```

---
## \#9 Posted by: jmasta Posted at: 2016-12-10T20:44:33.283Z Reads: 101

```
Is there any particular reason you want 6S?  I'd recommend a higher voltage to reduce your current draw, which decreases the amount of heat generated.  

If you put two identical battery packs in parallel, it doubles the capacity (Ah) and also doubles the max current output (A), but the voltage stays the the same.

Side note:  If you are only running 6S, you don't even need a BMS since you could use a 6S balance charger
```

---
## \#10 Posted by: rpn314 Posted at: 2016-12-10T20:45:01.733Z Reads: 94

```
Batteries in parallel add their amperage together. Batteries in series add their voltage together.
```

---
## \#11 Posted by: rpn314 Posted at: 2016-12-10T20:45:46.238Z Reads: 92

```
@jmasta Wow. I'm litterly about 20 seconds slower on these responses
```

---
## \#12 Posted by: Tijmen Posted at: 2016-12-10T20:47:38.769Z Reads: 92

```
I specifically want a laptop style charging solution though so a charger like the imax b6 is out of the question.
Only reason I'm so focused on 6S is because with my current board I'm using a 6S ESC and the motor runs fine on 6S, so I thought it'd make everything easier to just stick with that
```

---
## \#13 Posted by: jmasta Posted at: 2016-12-10T20:50:06.124Z Reads: 92

```
[quote="rpn314, post:11, topic:14475, full:true"]
@jmasta Wow. I'm litterly about 20 seconds slower on these responses
[/quote]


Gotta step your game up!  Haha, just kidding 

Signing off now. I should be studying continuum mechanics, not teaching electric circuits on the internet :grin:
```

---
## \#14 Posted by: Tijmen Posted at: 2016-12-10T20:55:54.871Z Reads: 92

```
Is this even remotely correct?
<img src="/uploads/db1493/original/3X/3/a/3aeae8f2b79f07c791c9724af6a495abbcb15c91.JPG" width="374" height="500">
```

---
## \#15 Posted by: anorak234 Posted at: 2016-12-11T20:12:26.990Z Reads: 74

```
Here ya go:
<img src="/uploads/db1493/original/3X/0/a/0ad944c936a12334832c0247c44f183a77d60577.png" width="659" height="500">

Balance leads go directly to bms as well this was just a quick sketch
```

---
## \#16 Posted by: Tijmen Posted at: 2016-12-11T20:24:55.326Z Reads: 70

```
Hey I think that's actually what I drew! :D Thanks!

Soz for the double post btw

Edit: Think my drawing is slightly different actually
```

---
## \#17 Posted by: HillRipper21 Posted at: 2018-07-13T15:14:27.764Z Reads: 22

```
I'm in a similar situaiton, I have 4 Zippy 3s batteries, I want to run 6S2P. I have one iMax B6 V2 charger which can only handle 6s, so I bought a balance board (https://www.banggood.com/Power-Genius-PG-Parallel-Charging-Board-Supports-5-Packs-of-2-6S-Lipo-Battery-XT60-T-Plug-p-1141232.html?rmmds=myorder).

Here is my wiring diagram, does this look correct?

![Battery%20Wiring%20Diagram|666x500](upload://l083Cd8zQ7iVHPH8MssFUNXzhq8.jpg)

Also, this is my first time with wiring stuff, what is the best way to make the T junction because it seems like you have to tee off at some point with one branch going to the charger and the other branch going to the vesc.
```

---
