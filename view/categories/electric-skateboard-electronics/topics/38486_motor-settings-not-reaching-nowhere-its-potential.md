# Motor settings not reaching nowhere its potential?

### Replies: 32 Views: 1558

## \#1 Posted by: thisguyhere Posted at: 2017-11-16T06:14:45.475Z Reads: 156

```
wanted to run my setting by, see if i'm doing something wrong.

this is coming from what used to be a 6374 dual drive, 12s4p setup.  had to take one of the motors off for inspection / replacement so will be running it mono until it's replaced.

here's motor settings for mono drive:

<img src="/uploads/db1493/original/3X/2/d/2d0ea65d8544ca5b528a9e72a754b9ee2a4f2bf5.png" width="483" height="223">

here's what i'm getting at max power draw:

<img src="/uploads/db1493/original/3X/6/5/652c5616fd239e915f025be0282565de2e5504e3.png" width="376" height="500">

i have batt max set at 70a but going up hill under hard acceleration it's only drawing 28amps from the battery.

is there some setting i'm missing?

in dual drive, i've hit max batt 80amp draw.
```

---
## \#2 Posted by: E1Allen Posted at: 2017-11-16T06:51:26.969Z Reads: 136

```
Does it also feel like only 28 amps going up hill. Or does it feel like more
```

---
## \#3 Posted by: Youssless Posted at: 2017-11-16T07:03:48.443Z Reads: 132

```
Would voltage sag be a culprit here?
```

---
## \#4 Posted by: thisguyhere Posted at: 2017-11-16T17:12:40.950Z Reads: 116

```
[quote="E1Allen, post:2, topic:38486, full:true"]
Does it also feel like only 28 amps going up hill. Or does it feel like more
[/quote]

definitely feels underpowered

[quote="Youssless, post:3, topic:38486, full:true"]
Would voltage sag be a culprit here?
[/quote]

I was seeing about 3v sag, but amp delivery should be unchanged. my understanding is voltage and amp draw should be inversely proportional?
```

---
## \#5 Posted by: jmasta Posted at: 2017-11-16T17:24:53.278Z Reads: 111

```
It's probably your drivetrain. That might be the maximum amount of torque your system can actually transmit with one belt/pulley.  What belt width and motor pulley size are you using?
```

---
## \#6 Posted by: evoheyax Posted at: 2017-11-16T17:24:59.861Z Reads: 111

```
[quote="thisguyhere, post:4, topic:38486"]
my understanding is voltage and amp draw should be inversely proportional?
[/quote]

It's not a 1:1 ratio, but more voltage, less amps. less voltage, more amps, yes.

But that's not your problem here.

Could be a couple of things. Since I don't know what your settings were before, it's not clear if this is the problem or not.

But the VESC limits work by using which ever limit is lower: motor or battery. Devin had formulas that he claims worked, @Ackmaniac disagrees with these formulas (i'm somewheres in the middle), but has not provided any formulas either so that you can tell which one is hit first. Put the motor amps up to 100 and see if you get more battery amps. I would suspect this is your problem.
```

---
## \#7 Posted by: egzplicit Posted at: 2017-11-16T17:29:22.167Z Reads: 99

```
Is this on the same battery pack? Could it be batteries can’t deliver so many amps?

At low speeds and hard acceleration I would expect the vesc to hit motor max limit while at higher speeds the bat max should be the limit factor.

I run foc on focboxes and I never hit my battery max but it’s not far off, at most 2-3 amps lower...

If you run ackmaniac firmware could it be you have W limit on?
```

---
## \#8 Posted by: thisguyhere Posted at: 2017-11-16T18:00:54.925Z Reads: 98

```
[quote="jmasta, post:5, topic:38486"]
What belt width and motor pulley size are you using?
[/quote]

15mm width, 15/40 tooth

[quote="egzplicit, post:7, topic:38486"]
Is this on the same battery pack?
[/quote]

yea, LG HG2 12s4p. checked connections and everything looks good and all P packs are balanced

[quote="evoheyax, post:6, topic:38486"]
Put the motor amps up to 100 and see if you get more battery amps. I would suspect this is your problem.
[/quote]

sure, ill give it a go later
```

---
## \#9 Posted by: Deckoz Posted at: 2017-11-16T18:13:08.272Z Reads: 91

```
Heat is probably your issue here...not your settings. I bet your hitting vesc thermal throttling(FETs) going uphill with one motor
```

---
## \#10 Posted by: Ackmaniac Posted at: 2017-11-16T18:30:05.660Z Reads: 87

```
Just do us all a favour and make a video with the app while you go uphill. Then I can explain you what is happening in detail. Guess battery cutoff or temperature is the limiting factor here. But with a video I think I can tell you exactly.
```

---
## \#11 Posted by: Deckoz Posted at: 2017-11-16T19:12:41.536Z Reads: 83

```
What the meistro said ^^^ video log ;)
```

---
## \#12 Posted by: Hummie Posted at: 2017-11-16T19:42:47.318Z Reads: 80

```
you won't hit your battery max amps unless you're at 100% duty cycle I'm pretty sure.  maybe you need to up your motor amps so you have the amps to even get to the higher speeds, and therefore higher duty cycle, to fully get to your battery amp limit.  what's your motor amp setting?  I like 120 motor amps.  
with the pic you posted you're only at 60% duty cycle.
```

---
## \#13 Posted by: jmasta Posted at: 2017-11-16T19:44:02.198Z Reads: 76

```
Based on the calculations I just did, you are only capable of transmitting about 1200 to 1350 W (depending on belt length) for a single drive with 15T motor pulley and 15mm HTD belt

This is right inline with the 1244W you recorded
```

---
## \#14 Posted by: Eboosted Posted at: 2017-11-16T20:00:28.860Z Reads: 75

```
Would you mind sharing the formula you used considering belt length as a factor?
```

---
## \#15 Posted by: thisguyhere Posted at: 2017-11-16T21:05:02.186Z Reads: 74

```
[quote="Hummie, post:12, topic:38486"]
I like 120 motor amps.
[/quote]

its at 80a now, will give this a go later

[quote="Deckoz, post:9, topic:38486"]
hitting vesc thermal throttling
[/quote]

max temp is below 60c at top of the hill climb.  where does it start throttling?

[quote="Ackmaniac, post:10, topic:38486"]
Just do us all a favour and make a video with the app while you go uphill.
[/quote]

pardon the shitty quality, the glass covering the camera is shattered right now

https://youtu.be/b03f7LEUcL4
```

---
## \#16 Posted by: egzplicit Posted at: 2017-11-16T21:15:18.736Z Reads: 71

```
Maybe double check ppm value and see if it goes all the way up to 100%
```

---
## \#17 Posted by: Deckoz Posted at: 2017-11-16T21:18:20.548Z Reads: 71

```
That's 140f. Throttling default is 135F if im not mistaken.

Sounds like it is for sure thermal throttling if your getting up in the 140s
```

---
## \#18 Posted by: Ackmaniac Posted at: 2017-11-16T22:54:25.303Z Reads: 71

```
That is a really strange case. It's not limited by the the battery voltage and also not by the temperature.
Please post screenshots of your settings. Maybe something is wrong there.

Do you have a BMS between the Battery and the FOCBOX?
```

---
## \#19 Posted by: thisguyhere Posted at: 2017-11-16T23:04:42.465Z Reads: 70

```
yes, 80a bestech bms, using it for discharge.

i don't think it's the bms because in dual drive it gets up to 80a batt discharge.

i'll take a screenshot of settings later tonight, need to make some adjustments anyway.
```

---
## \#20 Posted by: Ackmaniac Posted at: 2017-11-16T23:10:04.377Z Reads: 70

```
Could be that one of your series packs is too far off from the other cells so that the BMS reduces the power. If you have the chance try it without the BMS and let us know if it makes a difference. 

I wouldn't include a BMS in the discharge cycle because you never know what they do in detail. Would only use it for charging with charger. On 3 of my boards i don't even use a balancer at all and check each series pack from time to time. Max difference so far was 0.01V (Li-Ion). With a Li-Po i think it is necessary to balance but with Li-ion and a adjustable charger i would set it to 4.15V for each cell and then you should have enough wiggle room if the cells start to drift.
```

---
## \#21 Posted by: jmasta Posted at: 2017-11-16T23:13:39.606Z Reads: 66

```
[quote="Ackmaniac, post:18, topic:38486, full:true"]
That is a really strange case. It's not limited by the the battery voltage and also not by the temperature.
Please post screenshots of your settings.
[/quote]

It's limited by the drivetrain design, like most belt/pulley setups.  Changing the VESC settings isn't going to change physics :wink:
```

---
## \#22 Posted by: Ackmaniac Posted at: 2017-11-16T23:17:10.646Z Reads: 66

```
Sorry, doesn't make sense to me. The belt doesn't slip in the video.
```

---
## \#23 Posted by: thisguyhere Posted at: 2017-11-17T06:52:17.100Z Reads: 60

```
so upped the motor max to 120a and it's definitely punchier than before.

hit batt max of 40a.

i'm ok with these results for now, especially because this board isn't going to stay in this configuration for too long.

settings

**BEFORE**

<img src="/uploads/db1493/original/3X/9/9/99c666ae2c8fdda8e5399f41016efa7de5f00e9d.png" width="690" height="345">

<img src="/uploads/db1493/original/3X/5/b/5be446335b2d9a816473c26f471bf4c102a7324f.png" width="690" height="345">

**AFTER**

<img src="/uploads/db1493/original/3X/c/8/c882252d57d943df2834847a48e877081fb4d4db.png" width="690" height="345">

https://www.youtube.com/watch?v=qKEjiGwnihU
```

---
## \#24 Posted by: Ackmaniac Posted at: 2017-11-17T07:29:41.788Z Reads: 47

```
You are using sensors. Please disable them and give it a try. Reason is that in BLDC mode you can get trouble when their position isn't perfect.
```

---
## \#25 Posted by: thisguyhere Posted at: 2017-11-17T07:44:54.019Z Reads: 52

```
but it's hybrid mode so should the sensors not get disabled once it's above a certain erpm?

not sure if this is worth pursuing further though, just went on a 20+ mile ride today and it's ok for the time being.
```

---
## \#26 Posted by: Ackmaniac Posted at: 2017-11-17T10:10:56.978Z Reads: 51

```
Depends on you.
Something is wrong and i guess if you add a second motor to this one then this motor will output less power than the other one. Problem is that you won't recognize because the brain adopts really fast when the board always pulls a little bit  to one side during acceleration. Like with a single drive where you mostly one feel the big difference to a dual when you switch boards without a big brake in between.
```

---
## \#27 Posted by: PXSS Posted at: 2017-11-17T11:26:01.721Z Reads: 49

```
I agree with @Ackmaniac. You want to get this fixed before it starts causing more issues. 

I would think it's your pwm. If you had the trigger all the way back it should have been trying to command 100% current if you are in current mode but it's not. 

The reason increasing the max works, I think, is because you just changed the end point of the pwm. Where before the end point was 80, now it's 120. You are still only getting about 50% of that full range.
```

---
## \#28 Posted by: thisguyhere Posted at: 2017-11-17T17:30:05.672Z Reads: 41

```
[quote="PXSS, post:27, topic:38486"]
I would think it's your pwm.
[/quote]

for sure the remote is set correctly, i tested it last night.  it's at 98% full throttle.  having said that...

[quote="Ackmaniac, post:26, topic:38486"]
Something is wrong
[/quote]

so in the last clip going up hill, the throttle is NOT at a 100%.  i rarely, if ever, need 100% throttle.

this then leads to me another question.  i need the power but not full speed.  it seems i need to use all the throttle to use all the battery current.

i'm still NOT using ackmaniac's firmware.  would watt mode provide this?  where i'm using more current draw at not full speed?

edit ---

it seems like i need to use ackmaniac's firmware:

[quote="Ackmaniac, post:1, topic:12286"]
i didn't like that i can use only 50% of my throttle at higher speeds
[/quote]
```

---
## \#29 Posted by: Ackmaniac Posted at: 2017-11-17T18:21:15.627Z Reads: 37

```
Don't think that my firmware will make a change.
```

---
## \#30 Posted by: PXSS Posted at: 2017-11-17T18:21:55.302Z Reads: 38

```
You can adjust throttle curves, limit eRPM or Duty cycle. I thought you were at full throttle. 

Throttle controls current and not duty cycle in the standard firmware if I'm not mistaken, that's why you can spin at full rpm at a relatively low throttle setting under no load. 

If you weren't going full throttle on either of those videos then there is no issue with your setup. You just need to adjust throttle curves and such to match your needs and as Ackmaniac said, his firmware won't help much with this
```

---
## \#31 Posted by: thisguyhere Posted at: 2017-11-17T18:33:23.876Z Reads: 37

```
i guess that was a critical bit of info i missed in initially, that i wasn't on full throttle.

when i observed full amp draw on dual setup, it was full throttle going 35mph, which for me never really happens.

thanks for the help @Ackmaniac @PXSS
```

---
## \#32 Posted by: Titoxd10001 Posted at: 2017-11-17T22:35:18.451Z Reads: 34

```
[quote="thisguyhere, post:28, topic:38486"]
i need the power but not full speed.  it seems i need to use all the throttle to use all the battery current.
[/quote]

If I'm not mistaken if you started with two motors with vescs with the same settings and you removed one motor to make it one wheel drive then you'd have to use twice the throttle to get the same watts/amps. And if you made it AWD you would have to use half the throttle. If it was duty cycle the position of the throttle would be the same speed for all three scenarios.
```

---
