# Advice - more speed/torque

### Replies: 27 Views: 1712

## \#1 Posted by: ROFEN13 Posted at: 2018-01-02T02:19:44.766Z Reads: 238

```
Here is my current setup
[quote="ROFEN13, post:1, topic:36603"]
Deck: Ehler Switch Ninja
Trucks: Caliber II 44
Wheels: clone Flywheel 97mm 
Motor mount/Gears: Touqueboards 16/32t
Motor: SK3 6364 190KV
VESC: Ollin 4.12
Battery: Samsung 25R 12S4P 
[/quote]
What I want to know is what would be the cost effective was to increase speed / torque on this board?
This was my first build and I really enjoyed it. I hopefully look forward to more, wife permitting :)
```

---
## \#2 Posted by: Battosaii Posted at: 2018-01-02T02:25:07.972Z Reads: 231

```
A second motor
```

---
## \#3 Posted by: E1Allen Posted at: 2018-01-02T03:16:01.299Z Reads: 222

```
Taller gearing to go with the second motor if you want more torque and speed
```

---
## \#4 Posted by: abenny Posted at: 2018-01-02T03:23:01.323Z Reads: 219

```
bigger wheels would give you more top speed but would trade off a bit of acceleration
```

---
## \#5 Posted by: Namasaki Posted at: 2018-01-02T05:29:57.779Z Reads: 199

```
Can you post a screen shot of your Vesc settings?
```

---
## \#6 Posted by: E1Allen Posted at: 2018-01-02T05:35:33.504Z Reads: 188

```
I was thinking he should be going pretty quick on the current setup already
```

---
## \#7 Posted by: Namasaki Posted at: 2018-01-02T05:41:01.599Z Reads: 190

```
[quote="E1Allen, post:6, topic:42537, full:true"]
I was thinking he should be going pretty quick on the current setup already
[/quote]


I agree unless he doesn't have enough torque and the motor is bogging down. His gearing is a bit tall.
I'm curious what his motor max amps setting is. If he's running less than 80a, that could be the problem.
Adding a second motor would definitely help as well.
```

---
## \#8 Posted by: Hummie Posted at: 2018-01-02T05:48:55.250Z Reads: 178

```
vesc motor and battery amp settings = more low and high speed torque

higher gear ratio = more speed
```

---
## \#9 Posted by: E1Allen Posted at: 2018-01-02T06:00:57.507Z Reads: 175

```
So he has the same 2:1 ratio I have on my dual build. I noticed a huge difference between 16/36 and going to 18/36. 

What kind of speeds on flat ground are you getting? Have you hit the boards max speed yet?
```

---
## \#10 Posted by: Lumaci Posted at: 2018-01-02T10:15:42.853Z Reads: 161

```
Gearing: 13/36(Or40) and 100/110mm wheels.
```

---
## \#11 Posted by: ROFEN13 Posted at: 2018-01-02T13:22:47.460Z Reads: 151

```
I will post my Vesc settings tonight when I get home from work. I am currently topping out at about 27 mph.
```

---
## \#12 Posted by: ROFEN13 Posted at: 2018-01-03T21:54:51.676Z Reads: 131

```
Here are my settings. Please tell me what you think!
I am also planning on making it a dual setup. I am planning on getting ...
TB extended trucks
a second Ollin VESC from someone on this forum
second SK3 6364 190kv motor
mount and gears from TB
I also thought abut the 20t motor (15mm) pulley for TB

I grew up longboarding and loved DH riding so I really want to=he option for more speed.
Thanks!
<img src="/uploads/db1493/original/3X/8/9/89d8a31525393209111a54d31dd073d407812913.png" width="690" height="387"><img src="/uploads/db1493/original/3X/1/0/1057c0acafe45ae291b43b0129e3797b9cc959df.png" width="690" height="387"><img src="/uploads/db1493/original/3X/5/d/5d95f4091416253c3fd6f677940775674a52297d.png" width="690" height="387">
```

---
## \#13 Posted by: cwazy1 Posted at: 2018-01-03T22:20:13.247Z Reads: 110

```
Increase motor max to 80 and battery max to 40. That will give some kick to your board.

also uncheck the limit erpm with negative torque
```

---
## \#14 Posted by: Namasaki Posted at: 2018-01-03T22:29:16.508Z Reads: 113

```
As @cwazy1 stated,
motor max 80
batt max 40
and uncheck "Limit erpm with negative torque"

Also
Set max  erpm to 60000 and min erpm to -60000
If you run it over 60000, you might fry your Vesc.

Going from 40a to 80a motor max will make a noticeable increase in torque.

Upgrading to a dual drive would help as well and give you more even torque and improved braking.
```

---
## \#15 Posted by: ROFEN13 Posted at: 2018-01-04T00:39:23.756Z Reads: 103

```
WOAH! Thanks guys. It's cold here in Baltimore so I only took it around the block but that really really helped!
```

---
## \#16 Posted by: cwazy1 Posted at: 2018-01-04T02:30:18.789Z Reads: 101

```
if you find that now you're accelerating faster and also want stronger brakes, you can bump your motor min down to -80 and also your battery min down to -16. Don't go any lower than those numbers but feel free to go anywhere higher than those numbers.
```

---
## \#17 Posted by: Battosaii Posted at: 2018-01-04T02:30:53.258Z Reads: 99

```
I have a similar gear ratio and a 12s4p just dual motor and I top out around 45mph on 107s on flat ground and I weight a little north of 300 so you should be easily getting 30mph+ with your set up now.
```

---
## \#18 Posted by: E1Allen Posted at: 2018-01-04T06:12:46.306Z Reads: 86

```
[quote="Battosaii, post:17, topic:42537, full:true"]
I have a similar gear ratio and a 12s4p just dual motor and I top out around 45mph on 107s on flat ground and I weight a little north of 300 so you should be easily getting 30mph+ with your set up now.
[/quote]

What's your motor and battery settings?
```

---
## \#19 Posted by: Battosaii Posted at: 2018-01-04T16:58:30.052Z Reads: 76

```
Motor amps is 80 per focbox and 30amps per focbox for battery amps.
```

---
## \#20 Posted by: E1Allen Posted at: 2018-01-04T19:48:28.118Z Reads: 74

```
I may bump up the motor amps on mine.  See what that does for acceleration
```

---
## \#21 Posted by: ROFEN13 Posted at: 2018-01-04T19:49:18.132Z Reads: 69

```
What is are your settings? When I changed mine it was an incredible difference.
```

---
## \#22 Posted by: E1Allen Posted at: 2018-01-04T19:56:05.324Z Reads: 73

```
60focbox and 65 motor each focbox
```

---
## \#23 Posted by: Hummie Posted at: 2018-01-04T20:07:22.075Z Reads: 72

```
whats the max motor amps the focbox is said to be able to do?  that's the low speed torque and battery amps are the high speed torque. on the vesc I think it was 120 but may be different with different versions.  I run 120 on both 4.12 I have with no problem and the least cogging at the slowest speed, but i'm using hub motors so you might not need so much
```

---
## \#24 Posted by: E1Allen Posted at: 2018-01-04T20:10:29.886Z Reads: 70

```
Well FocBox is rated for 60 and the motors said 65
```

---
## \#25 Posted by: Hummie Posted at: 2018-01-04T20:20:23.393Z Reads: 67

```
60 battery, what about motor amps? 
 the motor ratings are empty and sure you could do more for a short period.  they should state at what amperage the magnetic field cant be further built in the stator steel, so maybe linear efficiency happens till 65 amps with such a kv, and beyond that the current is turned to mostly heat
```

---
## \#26 Posted by: E1Allen Posted at: 2018-01-04T23:04:52.189Z Reads: 66

```
<img src="/uploads/db1493/original/3X/4/e/4e67eb525fe8da8f83e60c61228e28106a3eebb4.PNG" width="281" height="500">this is what I get
```

---
## \#27 Posted by: ROFEN13 Posted at: 2018-01-17T11:34:41.723Z Reads: 60

```
So I also upgraded this to a dual setup, I see some people say half my settings, others leave them the same. I didn't see a clear answer, how are dual VESC settings different from a dual? (I'm running split ppm so the remote will be setup the same)
```

---
