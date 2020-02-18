# Arduino regen messes - drawing power from the same source (help)

### Replies: 21 Views: 647

## \#1 Posted by: evoheyax Posted at: 2018-04-11T18:18:03.462Z Reads: 73

```
I'm having a bit of an issue with the ardunio nano freezing up when regen current is applied to the battery pack. I have a buck converting kicking out 7.5v, pulling from the same battery as my VESCs.

Anyone have ideas as to what could cause this? Do I need a separate battery?
```

---
## \#2 Posted by: Bor.inc Posted at: 2018-04-11T18:38:43.618Z Reads: 70

```
You can maybe hookup a diode between the buck converter and the batteries so no reversed voltage can occur, furthermore you can try hooking up the arduino to the ubec + - of the vescs if it doesnt draw too much amps

there are probably much more options but I can't think of one, hope this helped you! :smile:
```

---
## \#3 Posted by: Deckoz Posted at: 2018-04-11T18:40:07.074Z Reads: 61

```
Lc filter before the buck. 

Inductor & capacitor in series, likely transients are over volting your switching buck, limit it with an LC
```

---
## \#4 Posted by: evoheyax Posted at: 2018-04-11T18:46:36.525Z Reads: 57

```
[quote="Deckoz, post:3, topic:51968"]
Lc filter
[/quote]


so something like this?

https://www.amazon.com/Crazepony-Reverse-Polarity-Protection-Quadcopter/dp/B018X744TO/ref=sr_1_2?ie=UTF8&qid=1523472353&sr=8-2&keywords=Lc+filter&dpID=414wPW2OAFL&preST=_SX300_QL70_&dpSrc=srch
```

---
## \#5 Posted by: Deckoz Posted at: 2018-04-11T18:50:36.217Z Reads: 51

```
Yea..but you'll need to make one probably. The voltage on quad lc filters is typically only up to 25 or 32v..

Just grab a cap and inductor for your board voltage and make one for a few pennies..
```

---
## \#6 Posted by: evoheyax Posted at: 2018-04-11T18:51:41.178Z Reads: 50

```
[quote="Bor.inc, post:2, topic:51968"]
try hooking up the arduino to the ubec + - of the vescs
[/quote]


Do you mean stealing power from the ppm port?
```

---
## \#7 Posted by: Bor.inc Posted at: 2018-04-11T18:53:37.984Z Reads: 47

```
I don't realy know vescs but you always have a ubec port nowadays on an esc which delivers 5v's for the reciever, maybe you could tap that a bit. But @Deckoz has the best solution i think
```

---
## \#8 Posted by: Deckoz Posted at: 2018-04-11T18:57:11.811Z Reads: 46

```
No eliminator BEC on vesc :(
```

---
## \#9 Posted by: evoheyax Posted at: 2018-04-11T18:57:13.771Z Reads: 46

```
THe issue seems to actually not be the arduino. Cause I get good values. But I'm powering the screen from the arduino. So I'm thinking if I use the ubec on the vesc to power the oled screen, my issues might go away.
```

---
## \#10 Posted by: evoheyax Posted at: 2018-04-11T19:35:40.149Z Reads: 44

```
Well I have 60v caps from old vescs. However, I don't have an inductors, so I guess It'll mean I need to wait a bit to get this going.
```

---
## \#11 Posted by: evoheyax Posted at: 2018-04-11T23:31:41.261Z Reads: 30

```
@Deckoz Sorry, I'm kinda a n00b when it comes to electronic component ratings. What am I looking for in an inductor? I have extra 60v caps, in many different lengths. I run 12s btw.
```

---
## \#12 Posted by: Deckoz Posted at: 2018-04-11T23:39:44.400Z Reads: 26

```
Inductor is just wound wire. You can get some smd conductors off of digikey, pick one double the mA you are trying to.push through it... Your voltage is small so don't worry to much about the rest, you are just trying to bring down noise on the line, before it goes to your switching ubec, as the Bec will reintroduce noise, the noisier the input to the Bec, the noisier it's switching. Lc helps smooth the input so the Bec switching frequency is constant..

Inductor helps keep the current from fast change, while the cap helps keep the voltage from fast change.
```

---
## \#13 Posted by: evoheyax Posted at: 2018-04-11T23:56:14.904Z Reads: 25

```
So wire them in series before the buck, on the + wire, correct?

Would it be hard to make my own inductor? I have tons of motor wire, which is what it seems they use...
```

---
## \#14 Posted by: Deckoz Posted at: 2018-04-12T00:00:32.807Z Reads: 24

```
![main-qimg-ba23e4668f25de5216c3865ed567ae84|340x193](upload://2sHH95HmHtrXtwjuCCudFy9Z4Rb.gif)

Sorry when I said series earlier I mean in the Daisy chain

Battery - > lc filter - > Bec -> Arduino


Yea you could if you wrap extremely thin wire around a ferrite toroid or conductive metal. Not sure how well it would perform though as it's super high frequency noise from the motors you are trying to filter out..
```

---
## \#15 Posted by: evoheyax Posted at: 2018-04-12T00:04:20.457Z Reads: 22

```
Ok, just trying to find the quickest solution, since I don't think I can find these anywheres locally anymore. All the local electronic places got pushed out from high rent. And mouser would be at least a week. Is it possible I'm blowing out arduinos or oled displaysAfter a bunch of testing today, the screen won't light up anymore and I had this happen once before a few days ago in testing. Replaced the screen and mega and now I seem to have the same issue again.

Since I need less than 2 amps, would this work?
https://www.amazon.com/Uxcell-a13071500ux0192-Toroid-Inductor-40mOhm/dp/B00EZC70M0/ref=sr_1_1?ie=UTF8&qid=1523491648&sr=8-1&keywords=2+amp+inductor+coil
```

---
## \#16 Posted by: Deckoz Posted at: 2018-04-12T00:11:30.457Z Reads: 21

```
Yea...either that or buy the one on Amazon you linked before. And replace the cap(25v)... I believe the one was 2A as well..
```

---
## \#17 Posted by: scepterr Posted at: 2018-04-12T00:49:52.001Z Reads: 20

```
Is the Arduino drawing power from the vesc and stepdown or just stepdown?
```

---
## \#18 Posted by: evoheyax Posted at: 2018-04-12T01:44:58.613Z Reads: 18

```
just step down. Step down is in parallel with vescs.
```

---
## \#19 Posted by: evoheyax Posted at: 2018-04-12T01:50:24.529Z Reads: 19

```
I just bought those so I have more for the future. I'm just wondering why my nano doesn't have this issue. I use 2 buck converters, one for a nano (lighting system) and one for a mega (speedometer). The nano has no issues, pwm from receiver for brake lights and turn signals work. No glitchs or anything. But the oled display has consistently been an issue. I had it working the other day with out any glitching. and then today, it started glitching after modifying the nano for turn signals.
```

---
## \#20 Posted by: scepterr Posted at: 2018-04-12T02:01:59.145Z Reads: 20

```
Maybe not enough power?
```

---
## \#21 Posted by: evoheyax Posted at: 2018-04-12T04:50:15.180Z Reads: 18

```
Maybe, but it’s weird that it almost always glitches when I brake. Going to try an external battery to verify while I wait for inductors.
```

---
