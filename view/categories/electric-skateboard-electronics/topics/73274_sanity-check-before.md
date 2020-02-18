# Sanity check before :fire:

### Replies: 18 Views: 414

## \#1 Posted by: longboardshort Posted at: 2018-11-03T17:53:38.317Z Reads: 172

```
About to setup a 12s bestech lipo bms (hex-d223v1) on my trampa. I have four 6s identical lipos, two series and two parallel. I am paralleling two groups then putting those in series. All of the connections are going to remain the exact same except for  only having the balance leads and main power leads in parallel, correct?

Thank you in advance.
```

---
## \#2 Posted by: kuphjr Posted at: 2018-11-03T17:58:42.186Z Reads: 167

```
Sounds correct to me, but feel free to post pictures and people will definitely confirm that you have it set up right.
```

---
## \#3 Posted by: kuphjr Posted at: 2018-11-03T17:59:46.556Z Reads: 152

```
Make sure to check the voltages of each battery cell is the same before hooking the balance leads up in parallel though!
```

---
## \#4 Posted by: Hummie Posted at: 2018-11-03T18:05:53.531Z Reads: 137

```
N a pic.  BalNce leads in parallel sounds like a short if they’re all in series as well
```

---
## \#5 Posted by: pixelsilva Posted at: 2018-11-03T18:15:04.403Z Reads: 117

```
Experts, please follow this one very careful.
```

---
## \#6 Posted by: longboardshort Posted at: 2018-11-03T18:32:30.903Z Reads: 109

```
Pics incoming:

This is how everything is to be wired up, not pretty but it helps me conceptualize it. I know my balance leads are junmbled but I have a multimeter to verify b1 is 4.2 and b12 is 50.4v.

![image|690x379](upload://rbiVem7niFDodPREpSJw1Oxwm2s.jpeg)
```

---
## \#7 Posted by: Sedmii Posted at: 2018-11-03T19:04:04.658Z Reads: 102

```
[quote="longboardshort, post:6, topic:73274"]
p, not pretty but it helps me conceptualize it. I know my balance leads are junmbled but I have a multimeter t
[/quote]

[*note - im no expert in this, but i will give my opinion anyway, please correct me if im wrong, and dont connect based only on my advice :P ]
Looks good to me, although very messy xD. If it helps you conceptualize thats great. For the parallel pack you put balance leads in parallel and those two connectors you put side by side in BMS. I would recommend to first connect one battery into BMS and figure out how it works, and which wire is what, then go do this mumbo jumbo. 
Why didnt you connect B- on BMS? I think it should be connected to GND of battery (first wire of your first battery balance connector, the first wire of your second pack you dont connect, bacause the wire is at B6 you dont connect)
```

---
## \#8 Posted by: Sedmii Posted at: 2018-11-03T19:07:33.957Z Reads: 89

```
[quote="Sedmii, post:7, topic:73274"]
ect B- on BMS? I think it should be connected to GND of battery (first wire of your first battery balance con
[/quote]

Take a look on 
https://www.electric-skateboard.builders/t/10s-balance-connector-series-harness/33051
and 
https://www.electric-skateboard.builders/uploads/db1493/optimized/3X/7/8/782ff289069542c5a6c42c33f1c25047664e83c2_1_512x500.jpg
```

---
## \#9 Posted by: b264 Posted at: 2018-11-03T19:08:19.221Z Reads: 83

```
[quote="longboardshort, post:6, topic:73274"]
but I have a multimeter to verify
[/quote]

This is the most important of all.  Before you make every single connection, tell yourself what voltage this wire is supposed to be, then check with the multimeter.  If it's not what you think, stop and put everything down and figure out why.  A difference of 0.1V is not a big deal.
```

---
## \#10 Posted by: Sedmii Posted at: 2018-11-03T19:10:51.306Z Reads: 79

```

DISCONNECT last connection you made before last checking and then

[quote="b264, post:9, topic:73274"]
If it’s not what you think, stop and put everything down and figure out why.
[/quote]
```

---
## \#11 Posted by: b264 Posted at: 2018-11-03T19:12:35.925Z Reads: 75

```
Also same advice for when cooking with hot oil with a gas flame--

Stop frequently and think -- if this thing in front of me turned into a fireball right now, do I know what I would do first?

Just always know the answer to that in your head.  Then proceed.

This is how people stay safe :smiley:
```

---
## \#12 Posted by: longboardshort Posted at: 2018-11-03T21:35:51.234Z Reads: 64

```
Awesome thank you all for the advice. Also one more question.. is there any certain order that needs to be followed as far as plugging things in.. ie balance leads first, battery gnd last or the like?

Also someone said not to plug in wire for b6 I believe? So I know not to connect the gnd of the seconds battery in series, but I should still plug in b6 which should actually be the last balance wire in the first 6s batt.  Lastly I was not planning on connecting anything to the b- wire because I read somewhere, I think from Namasakis post, disregard that connection because the first battery’s main (gnd) aka the thick black wire connects to B- so it’s taken care of from that.
```

---
## \#13 Posted by: longboardshort Posted at: 2018-11-05T03:19:02.761Z Reads: 42

```
Update.. everything is hooked up and works for the most part, and there were no sparks or fires 🤞👍😬. Works when riding fine, but it got down to 60% and when I plugged it in to charge, get nothing. 

Has anyone experienced this before by chance or could maybe suggest what to check? And yes I made sure the e-sw was on (closed circuit) for charging. Thank you in advance
```

---
## \#14 Posted by: longboardshort Posted at: 2018-11-05T18:50:10.474Z Reads: 36

```
Bump

10cha
```

---
## \#15 Posted by: J0ker3366 Posted at: 2018-11-05T19:24:04.576Z Reads: 31

```
[quote="b264, post:11, topic:73274"]
do I know what I would do first?
[/quote]

Get some popcorn
```

---
## \#16 Posted by: b264 Posted at: 2018-11-05T19:49:54.666Z Reads: 29

```
[quote="longboardshort, post:12, topic:73274"]
is there any certain order that needs to be followed as far as plugging things in… ie balance leads first, battery gnd last or the like?
[/quote]

Yes, start with the most negative balance lead and go through up to the most positive balance lead and then B- if needed

But the balance wires should be connected to a plug, so you can plug them all in simultaneously.

Don't work on more than one wire at a time on a battery -- completely finish and insulate each wire before you strip the next one
```

---
## \#17 Posted by: longboardshort Posted at: 2018-11-05T20:34:35.003Z Reads: 27

```
I appreciate the tip, but I have done that already. Everything is  connected and I tested it by riding it, which went well. 

My issue is that it won’t charge for some reason. I made sure the e-sw is on for charging, checked individual cell voltages and they are consistent. 

When I try to charge though, it stays at 60% and doesn’t seem to be charging at all. Discharge seemed to work fine though.

One thing I noticed is my other board which has the same bms (just 10s version) turns the board on when I turn on the charger (indicated by the battery % meter turning on) before I press the power switch (aka e-sw) which needs to be on for the bms to charge. 

Now when I turn on the charger for this board, the battery % indicator stays off until I press the power switch (e-sw) but then doesn’t charge.  Any ideas? This is the second bestech bms I’ve tried this with this week (both brand new) and same issue. Im thinking it could be a defective batch, but I ordered from buildkitboards which likely makes this an even bigger mess if it is a bad batch. 

😤
```

---
## \#18 Posted by: b264 Posted at: 2018-11-05T20:56:19.038Z Reads: 24

```
Post a photograph of where all the wires are connected
```

---
