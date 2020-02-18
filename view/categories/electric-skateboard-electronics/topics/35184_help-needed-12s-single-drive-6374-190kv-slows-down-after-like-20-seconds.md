# Help Needed **** 12s single drive 6374 190kv slows down after like 20 seconds

### Replies: 44 Views: 1294

## \#1 Posted by: Mattmccrary8 Posted at: 2017-10-09T16:27:11.911Z Reads: 183

```
Ok so I have all Torque board parts vesc single drive 6374 190 kv motor and a 12s4p battery. My vesc settings are pretty much based off the threads so erpm limit is 60k even though I know this setup is over. I running a 16/36 gearing on 97 abecs 

Ok the problem is my board rides amazing in the first minute and hauls ass. The out of no where the board limits to 21 mph and loses all Torque and braking. Is this a vesc setting or just to much strain on the setup. I weigh 195lbs and the motor had no problems with my 10s lipo setup 


Negative torque limiter is off. 

Motor max is 80 
Motor min -60
Max amp 50
I know the other numbers are -12 and 130 but forget what is what. 

Temp and everything else is what it came with.
```

---
## \#2 Posted by: twan Posted at: 2017-10-09T16:38:02.583Z Reads: 177

```
I think your vesc is overheating . With a 16/36 gearing and 97 wheels . Might put some strain on the vesc. Also note that the torque board vesc don't have a heatsink on them .
```

---
## \#3 Posted by: Mattmccrary8 Posted at: 2017-10-09T16:56:07.693Z Reads: 170

```
Would you say run 83’s? So overheating is def the problem
```

---
## \#4 Posted by: Mattmccrary8 Posted at: 2017-10-09T16:58:59.766Z Reads: 165

```
This is why I’m confused though. My motor and vesc ripped me with 97’s and the same gearing setup all day when I had a 10s lipo setup. Is it just to much power with 12s.. Can I limit a 12s battery to 10s power?
```

---
## \#5 Posted by: MysticalDork Posted at: 2017-10-09T17:10:30.313Z Reads: 159

```
Check the real-time monitoring, see what the temperature readings say. I've had a couple vescs with faulty temperature sensors that would cause the vesc to go into thermal limiting before it was actually hot.
```

---
## \#6 Posted by: NickTheDude Posted at: 2017-10-09T17:19:26.891Z Reads: 152

```
What are your voltage cutoffs set at?
```

---
## \#7 Posted by: ugothakd Posted at: 2017-10-09T17:53:55.271Z Reads: 145

```
I had a similar issue, my board would be quick for a few seconds, then eventually power would come to a minimum. I couldn't even get up the hill it just took me up. Wouldn't go past 5mph. Replaced my batteries and solved the problem
```

---
## \#8 Posted by: Mattmccrary8 Posted at: 2017-10-09T18:08:55.935Z Reads: 141

```
How do I check that?
```

---
## \#9 Posted by: Mattmccrary8 Posted at: 2017-10-09T18:09:53.273Z Reads: 139

```
They are set @ 34v start and like 30 or 29v end
```

---
## \#10 Posted by: Mattmccrary8 Posted at: 2017-10-09T18:10:33.255Z Reads: 137

```
It’s a brand new battery so I doubt that could be the issue. I really don’t have a way of testing that from me understanding
```

---
## \#11 Posted by: NickTheDude Posted at: 2017-10-09T18:15:25.108Z Reads: 132

```
Well there's your problem. Those settings are waaaaaay to low. You probably overdrained your cells and killed your battery. You need to use a multimeter to check the voltage of you cells.
```

---
## \#12 Posted by: Mattmccrary8 Posted at: 2017-10-09T18:26:01.157Z Reads: 127

```
@namasaki has posted on threads that lion packs can’t be set that low. That wouldn’t have anything to do with my torque and speed would it? I thought that is more so for range and to protect batteries from damaging
```

---
## \#13 Posted by: Mattmccrary8 Posted at: 2017-10-09T18:27:26.553Z Reads: 124

```
The pack is also 532 WH so I shouldn’t see any drop in speed for a pretty good awhile if it was all working correctly. This is so frustrating because I can’t figure out while it limits within a minute
```

---
## \#14 Posted by: NickTheDude Posted at: 2017-10-09T18:40:05.411Z Reads: 128

```
Fair enough, from what I understand 2.5V per cell is still super low. If your cells are damaged they could sag significantly and throw errors. Go to the terminal in BLDC tool and enter "FAULTS" and see if anything comes up.

Also take screenshots of your config and post them here.
```

---
## \#15 Posted by: Mattmccrary8 Posted at: 2017-10-09T18:54:09.481Z Reads: 126

```
I will when I get home in like 3 hours. I’m kicking myself for not taking pictures yesterday. I’m really hoping I didn’t screw myself
```

---
## \#16 Posted by: NickTheDude Posted at: 2017-10-09T18:57:53.989Z Reads: 125

```
Haha welcome to DIY, I've fucked up my fair share of batteries too :sweat_smile: That being said it could be a bunch of stuff so seeing all your settings will definitly help track it down.
```

---
## \#17 Posted by: cwazy1 Posted at: 2017-10-09T19:22:34.139Z Reads: 117

```
yeah my battery limiter and cutoffs are 40 and 37.
```

---
## \#18 Posted by: Mattmccrary8 Posted at: 2017-10-09T20:26:32.888Z Reads: 110

```
How much speed do you get on your setup because we have indetocal ones correct?
```

---
## \#19 Posted by: MysticalDork Posted at: 2017-10-09T20:26:56.606Z Reads: 110

```
Go into the monitoring tab in BLDC tool, it's the one with graphs. Look for the temperature readings.
```

---
## \#20 Posted by: cwazy1 Posted at: 2017-10-09T20:28:33.742Z Reads: 110

```
I'm running a 13/36 gearing with shaven 100mm MBS. Mine is close to 31mph loaded max speed.

Without a doubt something is going stray with your setup. You should have a faster top speed. 

Check your motor mount screws to make sure they don't protrude into the motor and touch any magnet wire.
```

---
## \#21 Posted by: GrecoMan Posted at: 2017-10-09T20:40:52.427Z Reads: 106

```
his motor just wouldn't spin if that was the case.  I know from experience :wink:
```

---
## \#22 Posted by: cwazy1 Posted at: 2017-10-09T20:41:41.180Z Reads: 102

```
Mine were touching yesterday, they spun, just not as fast as they were constantly braking. Motor also ran hot. I cut about 1/2cm off each of the touching bolts. Now they don't brake.
```

---
## \#23 Posted by: GrecoMan Posted at: 2017-10-09T20:42:26.516Z Reads: 101

```
I guess that does make sense...
Mine were embedded in the windings of my motor :grin:
```

---
## \#24 Posted by: Mattmccrary8 Posted at: 2017-10-09T21:25:10.019Z Reads: 93

```
Wait what are you guys talking about because my motor did spin in place yesterday as well once but I wasn’t moving. It sounded like it was winding up but nothing was happening
```

---
## \#25 Posted by: Mattmccrary8 Posted at: 2017-10-09T21:25:43.217Z Reads: 89

```
Can you show me a picture of what your talking about. I’m about off work to provide pics of my vesc settings
```

---
## \#26 Posted by: twan Posted at: 2017-10-09T21:56:22.355Z Reads: 83

```
post your vesc settings, its either the vesc heating up too much or your voltage cuttoff limiting the power.
```

---
## \#27 Posted by: Mattmccrary8 Posted at: 2017-10-09T22:02:03.030Z Reads: 82

```
On my way home now will be the next thing I post
```

---
## \#28 Posted by: cwazy1 Posted at: 2017-10-09T22:36:28.070Z Reads: 84

```
I can take one later, but we are talking about the 4, M4 Hex bolts that hold the motor to the motor mount. Those bolts are way too long. You can look into the motor through the little cutouts on the pulley side of the motor and see how far the bolts stick into the motor. 

If you see that any of the 4 bolts are touching the wires inside, you've got a problem. You'll need to file down the bolts so they don't touch. 

You can test this by taking a look inside, if there are one or two bolts that touch, just back them out a little bit and retest on the bench.
```

---
## \#29 Posted by: Mattmccrary8 Posted at: 2017-10-09T22:40:11.941Z Reads: 84

```
<img src="/uploads/db1493/original/3X/3/4/347a3bc4b7d6673aaecb57370054e9d7cd0fc2b8.jpeg" width="666" height="500"><img src="/uploads/db1493/original/3X/d/4/d4b14140373cc0dbea91ea3dce67ec0d48fdc0aa.jpeg" width="666" height="500"><img src="/uploads/db1493/original/3X/4/9/498b5a5f8bd0133857e2efa28134613a6542724c.jpeg" width="666" height="500">
```

---
## \#30 Posted by: Mattmccrary8 Posted at: 2017-10-09T22:41:07.917Z Reads: 81

```
Did the temp reading and everything was fine
```

---
## \#31 Posted by: Mattmccrary8 Posted at: 2017-10-09T23:14:25.684Z Reads: 82

```
Just rode again and for the first mile it would top out at 28-29mph then after that it wouldn’t go past 20mph and loss all Torque! WTF
```

---
## \#32 Posted by: cwazy1 Posted at: 2017-10-09T23:18:11.554Z Reads: 78

```
wtf... your integrator limit is 11 when your detection shows 113. Thats 100% your issue.
```

---
## \#33 Posted by: Mattmccrary8 Posted at: 2017-10-09T23:20:23.440Z Reads: 76

```
No that was a mistake. It’s set at 110 because the benchmark was 113
```

---
## \#34 Posted by: cwazy1 Posted at: 2017-10-09T23:22:34.226Z Reads: 75

```
you might be hitting the max erpm?
```

---
## \#35 Posted by: Mattmccrary8 Posted at: 2017-10-09T23:36:06.085Z Reads: 75

```
How would I know if I’m doing that? If there a way to benchmark it? I thought with this setup I’d be able to coast at 30mph
```

---
## \#36 Posted by: Mattmccrary8 Posted at: 2017-10-10T00:29:45.502Z Reads: 72

```
Could I limit the erpm to 50,000 and then it wouldn’t be hitting it? I’m just wanting this thing to get 10-12 miles at 30mph if that’s possible
```

---
## \#37 Posted by: Mattmccrary8 Posted at: 2017-10-10T00:34:55.592Z Reads: 74

```
@torqueboards any help with the setting you can think of? Or am I trying to run a single motor to high for a 195lb guy
```

---
## \#38 Posted by: twan Posted at: 2017-10-10T16:56:03.989Z Reads: 72

```
try lowering your battery cutoff start and end to like 7 and 8 volts thats what I have mine at, but then again I don't think that would do much since your battery pack is so huge at 500Wh there shouldn't be much voltage sag. Power is usually attributed to the mosfet temps from what I have experienced because I run 10s single drive and weigh 190 and after climbing a hill all my power is gone due to mosfet reaching 80 degrees.
```

---
## \#39 Posted by: GrecoMan Posted at: 2017-10-11T00:34:46.260Z Reads: 70

```
why the hell are your cutoffs so low
```

---
## \#40 Posted by: twan Posted at: 2017-10-11T02:32:03.004Z Reads: 65

```
Idk works for me . Not like I need those cut offs. got voltage monitors on board and on phone
```

---
## \#41 Posted by: i2oadsweepei2 Posted at: 2017-10-11T16:23:57.010Z Reads: 59

```
Wondering where you ended up with this? Not sure if you are going to hop back on and try again. If you do don't gun it straight till it cuts out. Try just a normal 15mph cruise. Control the throttle. See how far it goes. Be patient with it. There is already an issue pointed out many times that you are over the erpm limit. You are at 57456 erpm already at nominal voltage of 43.2v. When the pack is fully charged it is 50.4v. It does sound like the safety mechanisms are cutting power. If you keep pushing it something will fail and you may get hurt. That would suck. Also normal cutoffs are 36 start and 33.6 end.

Be safe
```

---
## \#42 Posted by: Mattmccrary8 Posted at: 2017-10-12T16:05:04.407Z Reads: 58

```
Ok everyone! I did solve the problem. I ended up adding a few holes. Then also cut some shrink off the mosfets. It was the 97mm wheels adding to much stress to the motor. I put 90mm wheels on and ripped around 31mph stopping, starting for 7 miles and nothing was overheated or sagging. But since I’m addicted to going 30mph....

All the high speed runs got me to go dual now. So another 6374 190kv motor. Vesc and big trucks are on the way. The single motor braking isn’t enough for a 200lb man who likes to go fast! I know I could change up the hearing but I figured I was going to make the move regardless! Will post some pics off my final build soon!
```

---
## \#43 Posted by: i2oadsweepei2 Posted at: 2017-10-12T16:29:20.165Z Reads: 52

```
You are absolutely gonna love dual!!! I'm 220lb and can attest :slight_smile:
```

---
## \#44 Posted by: ATLesk8 Posted at: 2017-10-12T19:45:07.507Z Reads: 47

```
I just upgraded to dual 6355s with 9mm belts/pulleys from a single 190kv 6374 with a 15mm belt/pulley and the difference in on demand power is significant...it also seems to run more efficiently somehow. Oh and I'm using a torqueboards 10s3p battery and vesc
```

---
