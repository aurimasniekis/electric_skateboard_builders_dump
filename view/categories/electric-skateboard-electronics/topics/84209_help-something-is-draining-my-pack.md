# Help, something is draining my pack

### Replies: 16 Views: 387

## \#1 Posted by: ervinelin Posted at: 2019-02-14T16:26:44.434Z Reads: 172

```
So some time ago I took my spud out for a spin... but for some reason it wouldn't fire up.

Went back and found out that my 10S2P had been completely drained.... 0.3V per cell left... At that time I thought perhaps my BMS was busted.

So I replaced it with a new 10S2P and new BMS and monitored it. For some reason, the pack was still slowly draining at about 0.5V per day. So I thought maybe it was my anti-spark switch (electricskateboard repair), I swapped that to a brand new flipsky smart anti-spark switch and the same thing is happening, 0.5V draining off each day.

I tried leaving the pack unplugged and voltage was stable, I also tried connecting it to a different VESC and it started to drain slowly again.

Any ideas what the hell is going on?

Thanks in advance!
Erv.
```

---
## \#2 Posted by: bevilacqua Posted at: 2019-02-14T17:07:33.926Z Reads: 162

```
maybe you could post a pic of your internals?

very strange indeed
```

---
## \#3 Posted by: banjaxxed Posted at: 2019-02-14T17:26:38.496Z Reads: 154

```
Bad bms? Maybe, or short? Weird
```

---
## \#4 Posted by: thisguyhere Posted at: 2019-02-14T17:33:19.453Z Reads: 154

```
what kind of bms?

which vesc?

my suspicion in on the anti-spark switch.  not sure if possible, but if you replaced that with a loop key, i'd bet money the slow drain will be gone.
```

---
## \#5 Posted by: ervinelin Posted at: 2019-02-15T01:29:28.251Z Reads: 136

```
@banjaxxed I think the instance when the pack got drained to zero in a matter of a few days might have been BMS issue. But I have since changed to BMS.

 @thisguyhere

It's the cheap waterproof red colour one from China.

VESC is hobbyking 4.12 and flipsky dual 4.2... both still drain slowly. As does new BMS.

I have it now transplanted to another enclosure with an antispark I know works.. voltage is stable...

Now what I don't get is why two brand new antispark from different manufactures would have the same problem... Is it something I did?

This is in no way a high powered board... Single 6374 on 10S...

My current option is to change to a loopkey but that means having to open a larger hole in the enclosure... And also the hassle of a loopkey...

I measured both antispark outputs when the switch was off and both exhibited a small less than 1V leak... WTH...
```

---
## \#6 Posted by: ervinelin Posted at: 2019-02-15T13:15:42.024Z Reads: 105

```
Transferred battery and BMS to another deck with an antispark I know doesn't leak... Voltage stable again...

So basically I have 2 brand new antisparks which are leaking... Why did this happen?
```

---
## \#7 Posted by: Komamtb Posted at: 2019-02-15T14:54:33.562Z Reads: 88

```
Interesting find! So who knows the answer?
```

---
## \#8 Posted by: linsus Posted at: 2019-02-15T15:29:07.078Z Reads: 83

```
Antisparks:

1. Meassure what resistance the the FETs show when off. (Should be Mega Ohm or "overload")
2. Meassure on "OUT" terminals with battery connected, if you have any active output.
```

---
## \#9 Posted by: thisguyhere Posted at: 2019-02-15T16:07:12.380Z Reads: 77

```
this would be better answered by an electrical engineer, but here goes.

antispark switches uses mosFET(s) in the open position to complete the circuit.  the gate that determines on / off is the thinnest filament and could allow the tiniest amount of current despite it being in the off position:

![image|466x317](upload://yuLhUOY5TNHarXbOzc8wtYa7RYW.png) 

that's my guess.  please tell me how i'm wrong.  i'd actually like to know as well.

anyway, this is why i never use antispark switches that have this tradition design.
```

---
## \#10 Posted by: linsus Posted at: 2019-02-15T16:19:38.257Z Reads: 70

```
Lets say the off state is 1Mohm. You'll have a "tiny current" of 0.0042mA(10s). So..from full to empty would be...2000+ years something for a 10Ah battery?

Lol hang on, let me get a calculator.

calculator said 27 years, few zeros wrong xD
```

---
## \#11 Posted by: ervinelin Posted at: 2019-02-15T16:54:27.678Z Reads: 64

```
How I measure the FET resistance?

As for the OUT terminals I connected a 4S battery, when the switch is off one anti-spark shows 0.2V, the other 0.5V.... I'm pretty sure this is not supposed to happen...
```

---
## \#12 Posted by: ervinelin Posted at: 2019-02-15T16:55:35.985Z Reads: 64

```
Yes it should be negligible in real world terms.. but I'm seeing my pack being drained noticeably...
```

---
## \#13 Posted by: ervinelin Posted at: 2019-02-15T16:57:01.373Z Reads: 63

```
I tried every combination to weed out the problem, pretty sure it's the anti-sparks leaking.. and somehow both of them (from different manufacturers)  are exhibiting the same problem....
```

---
## \#14 Posted by: linsus Posted at: 2019-02-15T17:01:45.054Z Reads: 60

```
[quote="ervinelin, post:11, topic:84209"]
How I measure the FET resistance?
[/quote]

just meassure between source and drain, nothing connected.
```

---
## \#15 Posted by: ervinelin Posted at: 2019-02-16T00:01:45.842Z Reads: 41

```
Across the positive terminal both problematic switches show zero ohms.. it's completely pass thru...

Across ground, one of them was OL.

The other was weird. When I first measured it read 5Mohms... Then after I probed it more it went over limit...
```

---
## \#16 Posted by: ervinelin Posted at: 2019-02-21T09:35:04.980Z Reads: 27

```
Gave up... 100% sure both my almost brand new antisparks are the cause of the leaks. 

Have since gone back to the primitive but proven XT90 loopkey... no more antisparks for me...

![IMG20190221164250|281x500](upload://5FsScKqsJmHOWJHWSPhOd8zfbdn.jpeg)
```

---
