# Wheel lock up on Build

### Replies: 18 Views: 299

## \#1 Posted by: RadCat Posted at: 2019-10-26T22:27:18.977Z Reads: 99

```
Hey all I have a build that I have been having issues with. I built a street board with the Unity ,10S5P battery, 200kv motors and 100mm boa wheels, 2.1 gear ratio. Recently I've had 2 buddies fall on my board doing speed runs at full throttle and both got seriosly injured. Both times it happened they said it felt like the breaks locked up but weren't 100% certain if they didnt accidentally hit the breaks themselves. So I wasnt sure what to think. Last night I went on a ride on my regular path and noticed a long incline so I wanted to test my board up this hill at full throttle....i was going about 26mph uphill and all of a sudden my board instantly stopped into a full on break and violently threw me forward, luckily I was about to run it off. Almost felt like it rebooted or something but it engaged breaks no doubt!  Now I feel horrible I dont know if it's a setting  I didnt properly input or if its a faulty Unity esc?... Anyone else had this issue?
```

---
## \#2 Posted by: Flasher Posted at: 2019-10-26T22:35:07.537Z Reads: 98

```
Sounds to me like a simple cutoff. Is your bms bypassed?
```

---
## \#3 Posted by: RadCat Posted at: 2019-10-26T23:02:04.157Z Reads: 93

```
I'm using a Psychotiller built battery charge only bms connected directly to unity.
```

---
## \#4 Posted by: RadCat Posted at: 2019-10-26T23:33:16.056Z Reads: 85

```
![20191026_163227|375x500](upload://wzNlopgqqdAK2r4wSI4AMmRTdDe.jpeg)
```

---
## \#5 Posted by: RadCat Posted at: 2019-10-26T23:33:52.523Z Reads: 83

```
![20191026_163237|375x500](upload://8SitQcJxrhCWKktzd47Dl8vjnN0.jpeg)
```

---
## \#6 Posted by: RadCat Posted at: 2019-10-26T23:37:07.393Z Reads: 83

```
Does a cutoff mean the breaks might engage?...I was going up a steep hill full throttle & the board instantly stopped it actually skidded from the wheels locking up.
```

---
## \#7 Posted by: banjaxxed Posted at: 2019-10-26T23:55:31.267Z Reads: 82

```
Sorry to hear this, you need to stop letting people test pilot this and be very careful until this issue is eliminated.

Have you considered for a start -

Bypassing the bms, it is a relatively simple operation & eliminates a possibility that the bms is stuttering power delivery & petgaa asoectesetting the Unity due to a problem that is not apparent under a specific load

Get a Metr or DaveGA for data logging 

What unity firmware version are you running?

What remote?
```

---
## \#8 Posted by: RadCat Posted at: 2019-10-27T00:20:12.520Z Reads: 77

```
Hey its unity Version 2.43 and I'm using a  2.4ghz rc remote . I have not considered bypassing the bms but I am now.
```

---
## \#9 Posted by: FranciscoV Posted at: 2019-10-27T02:55:33.701Z Reads: 73

```
Wasn’t 2.43 fw the one that was having nasty cut outs under load!?   You need to upgrade to 23.44 or 23.46
```

---
## \#10 Posted by: Eboosted Posted at: 2019-10-27T06:25:21.432Z Reads: 69

```
Connect your unity to the Android app, check if it says firmware is too old
```

---
## \#11 Posted by: banjaxxed Posted at: 2019-10-27T07:00:14.000Z Reads: 70

```
No that was the fix version. Makes sense to go to latest tho
```

---
## \#12 Posted by: FranciscoV Posted at: 2019-10-27T07:23:48.753Z Reads: 69

```
Latest have been working good so far.   Even with metr pro 🤞🏼
```

---
## \#13 Posted by: bigben Posted at: 2019-10-27T07:58:13.726Z Reads: 65

```
In your photo it shows that your motor phase leads are not shrink wrapped at the joint. Possibly they could have shorted and they would cause the motor to brake. Even if it is not your problem it's something to look at.
```

---
## \#14 Posted by: banjaxxed Posted at: 2019-10-27T08:22:36.780Z Reads: 65

```
That’s well spotted, definitely a candidate for this problem![image|562x500](upload://Agltz2G2PMsr3ijqgTrAgck6a9T.jpeg)
```

---
## \#15 Posted by: Mobutusan Posted at: 2019-10-27T08:46:28.199Z Reads: 62

```
The exposed phase wire connections were my first guess too. High speed + lots of vibrations + one split second of phase lead contact = shorted motor, instant brakes, ride over.
```

---
## \#16 Posted by: RadCat Posted at: 2019-10-27T13:28:01.215Z Reads: 47

```
Thanks for noticing that I will make sure I fix that and will check firmware to makensure its up to date. I use the UI app almost every ride and I dont ever remember it saying to upgrade.
```

---
## \#17 Posted by: Eboosted Posted at: 2019-10-27T20:50:18.441Z Reads: 37

```
What FW are you currently running? This is not a common issue, you should update the title if this post as it's deceiving and could cause people to be afraid to run their Unities
```

---
## \#18 Posted by: RadCat Posted at: 2019-10-27T22:16:04.106Z Reads: 31

```
FW 2.43 ..I would change title but from previous comments seems as this has been an issue in the past.

"Wasn’t 2.43 fw the one that was having nasty cut outs under load!? You need to upgrade to 23.44 or 23.46

I will update fw if possible run setup and fix exposed wires to see if this resolves issue....its easy enough to test on another hill.
```

---
