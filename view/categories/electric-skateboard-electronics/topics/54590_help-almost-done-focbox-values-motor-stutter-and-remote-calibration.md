# Help, almost done. Focbox values, motor stutter and remote calibration

### Replies: 9 Views: 466

## \#1 Posted by: accrobrandon Posted at: 2018-05-06T19:24:54.439Z Reads: 116

```
I made a video cuz its way more inclusive but can someone give things a one over and ideas? Winning remote doesnt get 100% brake value in.configuration... Only once on tb vesc as was in.bldc mode (not sure if thats relevant) and mild motor stutter as you'll see. Thanks.... Trying to take my maiden voyage today if.possible.
https://youtu.be/rdbG6juEVyQ
```

---
## \#2 Posted by: Blasto Posted at: 2018-05-06T19:29:29.641Z Reads: 104

```
For the stuttering,You need to config the hall table, check it out on the bottom of the foc page
```

---
## \#3 Posted by: Jinra Posted at: 2018-05-06T19:29:52.275Z Reads: 102

```
you need to input the correct minimum PPM value. It looks like 1.11, but it's hard to see as it's white on grey. Put then in and write config and it should go to 0 when you full brake.
```

---
## \#4 Posted by: Jinra Posted at: 2018-05-06T19:31:15.906Z Reads: 96

```
First thing I recommend is to upgrade to 3.xx f/w. FOC doesn't run as well on 2.xx firmware.
```

---
## \#5 Posted by: accrobrandon Posted at: 2018-05-06T20:07:45.029Z Reads: 93

```
[quote="Blasto, post:2, topic:54590, full:true"]
For the stuttering,You need to config the hall table, check it out on the bottom of the foc page
[/quote]

thanks great...smooth as butter now...


[quote="Jinra, post:3, topic:54590, full:true"]
you need to input the correct minimum PPM value. It looks like 1.11, but it’s hard to see as it’s white on grey. Put then in and write config and it should go to 0 when you full brake.
[/quote]


perfect now... will do firmware in a bit...

how does my belt alignment look? looked decent as i ran the motor and wasnt drifting... the wheel pulley sit slighty under the wheel wall so i offset the mount a hair to make sure the belt wouldnt rub the sidewall

![0506181604_HDR|690x388](upload://mRCJQdJNXqcSMGomAyqCG17x2vu.jpg)
```

---
## \#6 Posted by: MannyM0E Posted at: 2018-05-06T21:37:57.471Z Reads: 71

```
You could put washers in the idle to make it line up better with your belt
```

---
## \#7 Posted by: accrobrandon Posted at: 2018-05-06T21:45:08.757Z Reads: 70

```
yeah...i also think i saw a pic recently where someone used fender washers as well on the outside to keep the belt inline like the motor pulleys lip...
```

---
## \#8 Posted by: Aleks Posted at: 2018-05-07T01:20:27.749Z Reads: 65

```
This was my last build (now sold) but i put some fender washers on either end to make sure the belt doesnt slip off.

![image|374x500](upload://cCmmPYuqvnRHaD6ZjwkyDKAOlDX.jpg)
```

---
## \#9 Posted by: accrobrandon Posted at: 2018-05-07T01:47:22.384Z Reads: 60

```
yeah nice... this mighta been what i saw.

gave the board its first test ride... based on only having a meepo the start up was kinda remiscent of starting in intermediate mode... not super jerky and once in the mid to high rpm band really started taking off... braking wasnt good enough so ive bumped numbers up to 50/-50 for tomorrow test to see how that changes things =)

probably will add the fender washers as well to keep it all nicely contained!
```

---
