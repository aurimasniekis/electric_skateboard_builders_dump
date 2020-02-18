# Focbox repairs- need advice from the gurus

### Replies: 19 Views: 309

## \#1 Posted by: samuelsleepy Posted at: 2019-05-05T10:59:48.096Z Reads: 98

```
So I changed motor from flipsky 6374 to a turnigy sk8 6374 (I'm running 12s lipo) and my drv fried on my focbox. Was working perfectly for over 800km with the flipsky. I set the new motor and did the detection etc. 

Anyways

Before I removed the blown drv I would get the focbox to power up and light on. Now I have changed the drv with a new one and ive somehow got a short somewhere. I'm 99.999 % sure all the legs on the new drv have no Bridges and obviously I've checked a million times. 
Curiously when I put a 1s battery to power it up it's getting warm on one of the mosfets.
Anyone got any ideas? I've had literally over a hundred good looks over the board and every solder joint looks perfect.
```

---
## \#2 Posted by: dareno Posted at: 2019-05-05T11:14:38.422Z Reads: 92

```
reckon a mosfet has gone too.  pictures would help though.
```

---
## \#3 Posted by: samuelsleepy Posted at: 2019-05-05T21:56:13.393Z Reads: 78

```
If it was one of the mosfets gone, and I took it off the board, then the short should go right?
```

---
## \#4 Posted by: b264 Posted at: 2019-05-05T22:28:32.555Z Reads: 75

```
Can you measure each motor phase to each power rail?  Maybe give you a good hint as to which one to suspect
```

---
## \#5 Posted by: dareno Posted at: 2019-05-05T23:32:32.013Z Reads: 67

```
I'll summon the wizard.  Great guy and a proper expert on all things focbox.
@JohnnyMeduse
```

---
## \#6 Posted by: JohnnyMeduse Posted at: 2019-05-06T02:43:36.024Z Reads: 62

```
Does the power light (blue one) light up?

Check if your have 5.18V (or around) on the 5V rail, If you have around 8V the ground pad under the drv is not properly solder. 

Also check resistor r48 to r51 to see if they are 100Ohms
```

---
## \#7 Posted by: samuelsleepy Posted at: 2019-05-06T05:41:18.169Z Reads: 56

```
I can't power it up, it is dead short across the main power in terminals. One of the mosfets heats up when I let it short for 2-3 seconds on a very flat 1s battery. Everything is brand new condition apart from the drv being changed (nothing visual wrong anywhere). It blew the drv when testing a new motor I had just fitted to my board after going full throttle to break on the bench. I always did it with my flipsky 6374 and never had an issue but doing it with the turning 6374 blew it almost straight away. I'm an auto electrician and have experience with circuit boards but I just don't understand how there could now be a short there now. It has to be something I've done because straight after it blew I still had a blue light and no motor outputs. Now I've got dead short.
```

---
## \#8 Posted by: JohnnyMeduse Posted at: 2019-05-06T12:41:55.676Z Reads: 52

```
[quote="samuelsleepy, post:7, topic:92833"]
dead short across the main power
[/quote]

Basically, you probably have 2 mosfets that are short. Best way to find out which line is short is to use a multimeter, put the positive lead on the negative (GND) pad then check the continuity with each phase. After you can swap the multimeter lead and put the negative lead on the positive pad of the focbox, then check the continuity with each phase. 

![image|690x431](upload://qTdTV1BF0HRdCbFHMWdZ92HM7cx.png)

H*_low are equivalent to the gnd (there a only a small resistance between de GND and H*_low)
```

---
## \#9 Posted by: samuelsleepy Posted at: 2019-05-07T02:40:58.382Z Reads: 39

```
So if I measure earth to each phase they are all 0 Ohms. 
Posetive to each phase are all the same too, but they are 1.7 Ohms.

Is this correct? 

Thnkyou greatly for your help btw. I really appreciate it.
```

---
## \#10 Posted by: JohnnyMeduse Posted at: 2019-05-07T02:42:27.559Z Reads: 39

```
Could you post some picture?
```

---
## \#11 Posted by: samuelsleepy Posted at: 2019-05-07T04:52:03.310Z Reads: 34

```
 ![15572046618172134971710|375x500](upload://iOuaws21CvJj5FVpY19dG2fiZwg.jpeg)
```

---
## \#12 Posted by: Blasto Posted at: 2019-05-07T05:12:32.320Z Reads: 36

```
I’m just the PR guy, but you’re missing a cap and another one half lifted off the pad (tombstoned in the pr world)

![image|335x500](upload://luq1frfdvMLpcA5ZhTzif6h69k7.jpeg)
```

---
## \#13 Posted by: b264 Posted at: 2019-05-07T05:17:23.462Z Reads: 36

```
You're missing a capacitor
```

---
## \#14 Posted by: dareno Posted at: 2019-05-07T05:32:10.394Z Reads: 35

```
What?<dwwdvwehhbdshb>
```

---
## \#15 Posted by: b264 Posted at: 2019-05-07T05:43:41.464Z Reads: 34

```
What is this?

![15572046618172134971710|375x500](upload://9JJU6ap4hMlikCwllApqykHf8Fp.jpeg) 

Also, what is this?  Is it a copper trace?  Or a piece of a leaf?

![15572046618172134971710%20(1)|375x500](upload://5niZMMqxnXTb3yNcqJqmRIHTEs8.jpeg)
```

---
## \#16 Posted by: TowerCrisis Posted at: 2019-05-07T06:05:52.947Z Reads: 35

```
Whew lord, boy you gotta clean that shit up with some alcohol. There's so much crud all over the PCB it could be a multitude of issues. Why are so many components on the right side shifted around, is that left over from the drv reflow job?
```

---
## \#17 Posted by: dareno Posted at: 2019-05-07T06:12:40.485Z Reads: 35

```
Definitely does not look like factory finish.  Looks worked on.  Give it a clean and show pics again
```

---
## \#18 Posted by: Daddyckool Posted at: 2019-07-09T10:58:19.060Z Reads: 29

```
Hey everybody, I'm looking for a reputable repair for my focbox. I had the drv changed as did one of the mosfets that blew after drv replacement.
I'm in Switzerland. I have extra mosfets and drv's if needed. 
The focbox just blinks red now.
Thanks,
Tony
```

---
## \#19 Posted by: samuelsleepy Posted at: 2019-09-26T05:06:10.645Z Reads: 18

```
So I cleaned everything up and I'm sure there are no shorts on my reflow job. But I wanted to make sure it wasn't anything I have done so I unsoldered the drv off the board again and checked - still DEAD short across main power wires. One of the Mosfets gets a little warm when I attempt to power up for the millisecond before I take battery power away. Dead mosfet too??
```

---
