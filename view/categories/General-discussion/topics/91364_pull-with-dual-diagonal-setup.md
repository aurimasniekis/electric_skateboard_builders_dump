# Pull with Dual Diagonal Setup

### Replies: 28 Views: 427

## \#1 Posted by: wjmoody Posted at: 2019-04-22T00:02:46.436Z Reads: 145

```
Hey everyone. So I just finished my first dual diagonal build, two 6374 149 kv motors, dual FOCBOX, landyachtz Evo falcon deck, 107 mm abecs. But, when speeding up or breaking, I'm getting a significant amount of pull. Do any of you have any tips to correct for this?  I'm goofy footed with one motor back left, the other front right. Please and thank you.
```

---
## \#2 Posted by: Jinra Posted at: 2019-04-22T00:03:28.054Z Reads: 145

```
what control mode are you using?
```

---
## \#3 Posted by: wjmoody Posted at: 2019-04-22T00:12:59.184Z Reads: 143

```
I'm not sure I understand.  I've got dual FOCBOXes without CANBUS if that's what you're asking.
```

---
## \#4 Posted by: Jinra Posted at: 2019-04-22T00:15:35.878Z Reads: 137

```
You had to have programmed it at some point, are you using current, PID, duty cycle?..
```

---
## \#5 Posted by: wjmoody Posted at: 2019-04-22T00:18:10.942Z Reads: 130

```
I'm using the new VESC tool software, programmed everything through current, didn't tinker with PID or duty cycle I believe.
```

---
## \#6 Posted by: Jinra Posted at: 2019-04-22T00:19:01.810Z Reads: 126

```
Sounds like maybe your belts are too tight then, a video of a bench test from full throttle to neutral would be helpful.
```

---
## \#7 Posted by: wjmoody Posted at: 2019-04-22T00:20:34.304Z Reads: 125

```
I can upload that in a bit.  When flipped over on the bench, I did notice one motor spinning up before the other, but the belts felt even.
```

---
## \#8 Posted by: Jinra Posted at: 2019-04-22T00:23:02.402Z Reads: 118

```
They should be as loose as possible without skipping. If they're completely stiff, they're too tight.
```

---
## \#9 Posted by: wjmoody Posted at: 2019-04-22T00:25:19.342Z Reads: 113

```
Right on, i'll make that adjustment and give it a try.  Could truck tightness effect the pull with the DD setup as well?  And what was the setting you were mentioning in VESC tool to program for the DD configuration?
```

---
## \#10 Posted by: Colson003 Posted at: 2019-04-22T04:24:04.686Z Reads: 102

```
Pull as in it wants to turn right when braking? What trucks are you using?
```

---
## \#11 Posted by: b264 Posted at: 2019-04-22T04:27:09.184Z Reads: 103

```
I have a dual diagonal and it has bad torquesteer, but that's probably because I'm running split truck angles.

Overall, I deal with the torquesteer and got used to it, because it makes up for that in the sheer amount of traction you have.  Dual diagonal is second to none in wet or snowy conditions.  Both drive wheels can be skidding or sliding, and each truck still has one wheel steering.
```

---
## \#12 Posted by: wjmoody Posted at: 2019-04-22T04:29:36.908Z Reads: 100

```
Have you found any means of lessening the amount of torque steer?  i.e. tightening the trucks, loosening the belts, etc?  I'm coming from a dual rear setup, so the feeling is completely new and obvious to me.
```

---
## \#13 Posted by: b264 Posted at: 2019-04-22T04:31:12.243Z Reads: 97

```
It had far less before I started running split truck angles.  That affected it A LOT.
```

---
## \#14 Posted by: mmaner Posted at: 2019-04-22T04:31:46.199Z Reads: 97

```
Torque steer, is that what you mean? 

You want rear heal side, front toe side. I wasn't sure what you meant in the description.
```

---
## \#15 Posted by: wjmoody Posted at: 2019-04-22T04:33:37.347Z Reads: 95

```
Ahhh, I was hoping that wasn't a possible solution, lol, another hour of swapping motors, but thanks man, hopefully it helps, i'll let you know.
```

---
## \#16 Posted by: Colson003 Posted at: 2019-04-22T04:33:37.657Z Reads: 93

```
Narrower trucks reduce it as well
```

---
## \#17 Posted by: wjmoody Posted at: 2019-04-22T06:37:21.686Z Reads: 87

```
So tried that, switched the front motor to toeside, rear motor to healside, still a lot of torque steer.  I'm considering trying to go back to dual rear, but the 6374s are so wide, I can't mount them next to each other.  Do you guys know of motor mounts or way to get dual 6374s to both fit on the back truck without staggering them.
```

---
## \#18 Posted by: Bobby Posted at: 2019-04-22T06:39:59.480Z Reads: 86

```
Are you running bldc or foc?
```

---
## \#19 Posted by: wjmoody Posted at: 2019-04-22T06:41:46.291Z Reads: 84

```
I'm running FOC.  Earlier I was having stuttering issues, but I updated the firmware on my FOCBOXes and it corrected it all.  I switched the position of the motors for dual diagonal, but the torque steer is still fierce.  Looking for options for mounting both in the back without mounting one facing out and one facing in, but that would probably require getting new mounts and/or trucks.
```

---
## \#20 Posted by: Bobby Posted at: 2019-04-22T07:56:32.623Z Reads: 75

```
I had the same issue and the only fixed seemed to be to get used to it.... i also went back to dual rear
```

---
## \#21 Posted by: Colson003 Posted at: 2019-04-23T15:16:33.284Z Reads: 64

```
@wjmoody what trucks are you using?
```

---
## \#23 Posted by: Surfer Posted at: 2019-04-23T16:06:47.963Z Reads: 60

```
Change your trucks for cast Ronin with Queen pin and your problem is solved and you got also nice riding upgrade.
100%
```

---
## \#24 Posted by: wjmoody Posted at: 2019-04-26T02:00:34.782Z Reads: 41

```
Torque Board 218 mm
```

---
## \#25 Posted by: Colson003 Posted at: 2019-04-26T02:02:06.362Z Reads: 41

```
Yeah that makes sense. Wider trucks = more leverage on the kingpin.
```

---
## \#26 Posted by: Frenchy Posted at: 2019-04-26T04:08:19.193Z Reads: 35

```
[quote="wjmoody, post:24, topic:91364, full:true"]
Torque Board 218 mm
[/quote]
Totally the problem
 get some 160 caliber 2 ... katanas work extremely well for diagonal set ups
```

---
## \#27 Posted by: wjmoody Posted at: 2019-04-26T04:15:24.851Z Reads: 34

```
I'll check that out.  Any chance you have a link to where they're sold?
```

---
## \#28 Posted by: Frenchy Posted at: 2019-04-26T04:17:57.556Z Reads: 36

```
Just look up 9inch caliber 2 for sale at your local skate shop..fuck Amazon.. go give your local skaters some weed and beer money
```

---
## \#29 Posted by: Paulycnotes Posted at: 2019-11-15T17:22:05.773Z Reads: 15

```
Belt Drive...??  YES... Do you have Dual or even a Single Idler as part of your Motor Mounts??
```

---
