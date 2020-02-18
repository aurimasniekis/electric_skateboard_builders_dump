# Please Help &#124;&#124; BMS started smoking

### Replies: 28 Views: 400

## \#1 Posted by: Z4MSupreme Posted at: 2018-12-31T20:13:03.507Z Reads: 122

```
Hi,

I have finally started building my board. I wired up my board according to a template I found on the forum. I have used a bestech 80 amp BMS with an eswitch and connected it up to a 10s3p 30q pack that I have made. I also have a step down converter that I am using to light up the LED switch. 

Everything was wired up with no problems at all, however when I attached the 12v power of the step down converter to the switch, smoke began to arise from the BMS. 

I bought the BMS from Alien Power Systems and am thinking of contacting him to see if I can get a warranty replacement. 

Any thoughts?

Thanks in advance 🤘
```

---
## \#2 Posted by: Trdolan03 Posted at: 2018-12-31T20:21:01.513Z Reads: 115

```
Sounds like your balance wires got out of order.
```

---
## \#3 Posted by: Z4MSupreme Posted at: 2018-12-31T20:24:19.579Z Reads: 115

```
I thought that at first, but have checked with the voltmeter and it is all correct. 

Additionally, nothing happened until I connected the power for the led switch, everything else was ok...
```

---
## \#4 Posted by: legend27 Posted at: 2018-12-31T20:48:07.498Z Reads: 104

```
Pictures?
D
Skele
```

---
## \#5 Posted by: DavidBanner Posted at: 2018-12-31T20:52:38.783Z Reads: 96

```
did you connect the main + and - before connecting the balance leads?
```

---
## \#6 Posted by: Z4MSupreme Posted at: 2018-12-31T21:35:42.819Z Reads: 91

```
Yes I did. But everything was fine until I connected the switch to the 12v power
```

---
## \#7 Posted by: Z4MSupreme Posted at: 2018-12-31T21:35:55.361Z Reads: 89

```
A picture of the BMS?
```

---
## \#8 Posted by: TowerCrisis Posted at: 2018-12-31T22:04:12.709Z Reads: 87

```
Of the BMS and all wiring attached to it.
```

---
## \#9 Posted by: brenternet Posted at: 2018-12-31T22:16:25.471Z Reads: 82

```
Ask it if it has considered vaping
```

---
## \#10 Posted by: legend27 Posted at: 2018-12-31T22:28:14.154Z Reads: 84

```
Wiring, Bms, battery etc
```

---
## \#11 Posted by: J0ker3366 Posted at: 2018-12-31T22:30:21.952Z Reads: 86

```
[quote="Z4MSupreme, post:1, topic:79488"]
BMS Started Smoking
[/quote]
We should really teach our bms' better habits then. Worst habit I have.
```

---
## \#12 Posted by: Z4MSupreme Posted at: 2019-01-01T12:01:53.837Z Reads: 70

```
![IMG_20181231_194127|281x499](upload://lfnt77edi8RoPaAD8TQgPvXomrG.jpeg) 

Sorry the photo is a mess
```

---
## \#13 Posted by: Z4MSupreme Posted at: 2019-01-01T12:05:25.307Z Reads: 67

```
![Screenshot_20190101-120359|281x500](upload://fT5elokOtVA4NO6nopoAkO1lmC4.jpeg) 

I have wired up everything like this diagram. The balance leads are all in the correct order as well as I checked with the voltmeter
```

---
## \#14 Posted by: Z4MSupreme Posted at: 2019-01-01T12:06:42.567Z Reads: 65

```
![Screenshot_20190101-120406|281x500](upload://lPtVCDdHrzZwiboveGuwtIFuJfj.jpeg) 
As well as wiring the switch like this and bridging the two poles of the switch with one of the eswitch wires
```

---
## \#15 Posted by: Z4MSupreme Posted at: 2019-01-01T12:07:36.227Z Reads: 64

```
Lol. Bad habits for 2019😭
```

---
## \#16 Posted by: Z4MSupreme Posted at: 2019-01-01T12:10:31.519Z Reads: 64

```
![IMG_20190101_120922|281x499](upload://zSg9k8vtfkan4lVrI8ExtpxLcBr.jpeg) ![IMG_20190101_120835|281x499](upload://ucGtpPEUOjNJNOhIw0QB6U7eNJ3.jpeg) 

The first picture is the bottom of the BMS, looks like the fuse has burnt out?

The second is the area around the wire for the switches
```

---
## \#17 Posted by: TowerCrisis Posted at: 2019-01-01T18:26:01.891Z Reads: 45

```
Okay, are you sure that the BMS contacts can handle 12 volts? Why didn't you try just hooking up only the switch to see if the pack even worked first.

I don't think you should have a stepdown converter, the switch should JUST be driven by the eswitch wires.

Did you check what voltage the E switch wire positive was outputting?
```

---
## \#18 Posted by: TowerCrisis Posted at: 2019-01-01T18:32:48.633Z Reads: 45

```
OH I just figured it out!

That switch wiring is wrong.

Here is what it should have been:
E switch wire to **C**
E switch wire to **NO**
stepdown converter positive to **+**
 stepdown converter negative to **-**

None of those pins should be bridged to eachother.

The stepdown converter should be connected to the battery further down the chain from the BMS. The stepdown converter should only turn on once the BMS turns the board on.

The BMS eswitch should NEVER be exposed to external power.
```

---
## \#19 Posted by: Z4MSupreme Posted at: 2019-01-01T18:59:35.990Z Reads: 39

```
Thank you so much for telling me how to wire it. However the eswitch wasn't directly connected to the power. The eswitch was connected to the two contacts whilst the step down was connected for the led on the light. 

Also, for the two E switch wires which one is connected to wich terminal on the switch? 

Many thanks.
```

---
## \#20 Posted by: TowerCrisis Posted at: 2019-01-01T19:04:27.174Z Reads: 38

```
If you did wire it up like that diagram, then the C would connect to NO when the switch is activated. And C was your 12V and NO was your BMS. So it actually did directly connect them.

It doesn't matter which BMS wire goes to NO or C. They should be the only two wires that ever connect to NO, NC, or C. In your use you just want to use NO and C.
```

---
## \#21 Posted by: Z4MSupreme Posted at: 2019-01-01T19:07:56.850Z Reads: 36

```
Holy shit. Thank you sooooo much. Can I copy and paste what you said and post it on the thread that I found that diagram. I don't want the same thing happening to anyone else. More money being spent 😭.

Also, how do you know all of this?
```

---
## \#22 Posted by: Indiangummy Posted at: 2019-01-01T19:10:22.049Z Reads: 34

```
He already stated in the thread which wiring is correct and which is incorrect.
```

---
## \#23 Posted by: Z4MSupreme Posted at: 2019-01-01T19:12:14.173Z Reads: 35

```
I found the diagram on another thread. And I just took a screenshot and put it on this thread.
```

---
## \#24 Posted by: Indiangummy Posted at: 2019-01-01T19:14:09.930Z Reads: 31

```
Yeah look on that thread. He cleared it up.
```

---
## \#25 Posted by: Migro Posted at: 2019-01-01T19:14:14.761Z Reads: 32

```
I put the right diagram as the solution on my old thread now.
```

---
## \#26 Posted by: Z4MSupreme Posted at: 2019-01-01T19:21:32.452Z Reads: 31

```
Cheers dude, I've just seen. Glad it's all sorted. 👍🤘
```

---
## \#27 Posted by: TowerCrisis Posted at: 2019-01-01T19:27:21.468Z Reads: 34

```
Just to clear some things up:

C stands for contact, or charge. It's what you normally what you put the "positive" side of whatever you are switching.

NO stands for "normally open". When the switch is not activated, the circuit passing through NO through C is "open" meaning it is disconnected. When you push the button, it is connected.

NC stands for "normally closed". When the switch is not activated, the circuit passing through NC through C is "closed" meaning it is connected. When you push the button, it is disconnected. This is useful for when you want something to always be on except when you push the button.

NC and NO will never connect to eachother, so you can drive two seperate circuits off of the one switch (assuming they take the same voltage at C). When one is on the other will always be off.

"+" Goes to the LED through a current limiting resistor (and drops voltage from 12V to something lower)
"-" Goes to the LED negative.

These LED switches all normally operate on 12V because they are made to be installed in cars or other kinds of vehicles. They all use 12V lead acid batteries and most analog circuitry also runs off of 12V in cars, especially older models.
```

---
## \#28 Posted by: Z4MSupreme Posted at: 2019-01-01T19:37:30.120Z Reads: 30

```
Thank you so much for clearing that up. You are a saviour 😂. I had no idea what I did wrong and I didnt want to buy another BMS and do the same thing wrong again. Thanks again 😀
```

---
