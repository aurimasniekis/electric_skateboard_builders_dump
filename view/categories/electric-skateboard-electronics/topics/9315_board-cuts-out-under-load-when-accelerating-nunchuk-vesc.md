# Board cuts out under load / when accelerating (Nunchuk &amp; VESC)

### Replies: 36 Views: 3401

## \#1 Posted by: Charlie_H Posted at: 2016-09-10T07:16:20.928Z Reads: 190

```
Although there is already some information out there on how to stop the nyko nunchuk remotes from cutting out, i am still having problems with mine. 

Upon acceleration (even on flat ground) when the throttle is around 90% the board will momentarily cut out and then keep going, it also does this when going up hills

-I have checked all my solder joint and have only one wire for each connection going directly from the receiver to the VESC (previously i had a JST connector.)
-Shaking the board and pulling on wires does not make the board cut out, it's only under load.
-The board runs off of two 4s lipos in series. although i have tested it on a 6s and it still happens
-cut outs still occur even when not cased in aluminium  housing.
-I have changed my low voltage cutt off to well below the necessary level to check that the vesc wasn't getting confused and thinking the LiPos were flat.

The only other thing i can think of that i have done wrong is set my settings wrong in the BLDC Tool.

Please if anyone has any other potential solutions,  ideas on how to fix it, or the very least ways to rule out certain things it would be greatly appreciated! 

Thanks!
```

---
## \#2 Posted by: flatsp0t Posted at: 2016-09-10T10:46:04.692Z Reads: 171

```
Sounds like you trigger the over-current cutoff.
Could you please do some screenshots of your BLDC tool configuration tab?
Or could you tell me Motor-/Battery Max values and your battery ratings?
```

---
## \#3 Posted by: Charlie_H Posted at: 2016-09-10T11:15:42.172Z Reads: 167

```
Admittedly, I Iack knowledge about the BLDC Tool so hopefully it's a simple fix.

NOTE: the voltage cut off has intentionally been set super low as to check that was not not the problem. 

<img src="/uploads/db1493/original/3X/6/d/6d9e9ae7b877ad1be25d196f826899e862201e8a.png" width="690" height="344"><img src="/uploads/db1493/original/3X/c/b/cbe6946708464a4a36f0d7720389c699e137940d.png" width="690" height="348">
```

---
## \#4 Posted by: elkick Posted at: 2016-09-10T11:25:14.256Z Reads: 148

```
Better set max input voltage back to default 57V.

There are too many tutorials out there giving the wrong advice to lower that value and it always leads to those problems and questions.
```

---
## \#5 Posted by: flatsp0t Posted at: 2016-09-10T11:26:27.008Z Reads: 147

```
You battery max input voltage seems too low, voltage spikes can cause a shutoff.
```

---
## \#6 Posted by: Charlie_H Posted at: 2016-09-10T11:30:36.016Z Reads: 146

```
I'm running the board off of 30 volts. Do you think 40 volts is high enough? 

Also what is the purpose of this function?
```

---
## \#7 Posted by: elkick Posted at: 2016-09-10T11:32:18.617Z Reads: 143

```
It prevents the VESC of taking a higher voltage than it can handle. And that's 60V, so it's safe to leave that value at 57V.
```

---
## \#8 Posted by: Charlie_H Posted at: 2016-09-10T11:34:32.507Z Reads: 142

```
I see, Thank you for your help! I will adjust my settings accordingly and see what happens. Fingers crossed.
```

---
## \#9 Posted by: Charlie_H Posted at: 2016-09-11T00:23:14.853Z Reads: 133

```
Problem is still occurring :( , Please if anyone has any other suggestions please let me know.
```

---
## \#10 Posted by: Ackmaniac Posted at: 2016-09-11T01:51:02.660Z Reads: 128

```
Please show us pictures again of your current settings. And also add a screenshot of the advanced screen in motor config.
```

---
## \#11 Posted by: Bender Posted at: 2016-09-11T01:56:31.050Z Reads: 126

```
I had very similar problems in FOC (but not in BLDC)

I did some research and you can set the vesc to a absolute max of 240 which prevents abs over current spikes when breaking or accelerating hard
Default is 130
```

---
## \#12 Posted by: boards Posted at: 2016-09-11T02:12:14.845Z Reads: 122

```
Try adding a (4-20)uf cap between 3.3 and on the vesc side. I think the 3.3 line just sucks.
```

---
## \#13 Posted by: Charlie_H Posted at: 2016-09-11T02:22:39.911Z Reads: 126

```
<img src="/uploads/db1493/original/3X/7/1/71c0266712270c6590b336aeb793da11c8a6094c.png" width="690" height="343"><img src="/uploads/db1493/original/3X/6/0/604c771e53fb1ee56c8765c52a05f33e755bb3a8.png" width="690" height="342"><img src="/uploads/db1493/original/3X/d/c/dc8cf123289e32c5ac5f61ee7fd17aa0e91421dc.png" width="690" height="346">
```

---
## \#14 Posted by: Namasaki Posted at: 2016-09-11T03:59:53.645Z Reads: 119

```
your battery max current seems too low.
Your Lipo batteries  should be able to handle more than 25amps.  AH x C = discharge capability
example: 5000mah = 5ah x 20C = 100 amps continuous discharge capability.
If your batteries are 5000mah with a 20C rating you could set your single or even dual vesc much higher on the batt max amp. 
I think your cutting out because your not feeding the vesc enough current from the battery
It's like your running out of gas as you accelerate.
Funny, I had a similar problem on my Jet Boat. 350 chevy with a 4 barrel carb and a stock mechanical fuel pump
The motor would start and idle but as soon as I punched it, it would die. 
It would start back up and idle no problem, but every time I hit the throttle it would die.
The solution was a high volume electric fuel pump. After I installed the new fuel pump, it ran great!
The mechanical fuel pump just couldn't supply enough gas.
```

---
## \#15 Posted by: Charlie_H Posted at: 2016-09-11T05:44:28.890Z Reads: 119

```
I'm running the board on two 10ah 4s lipos in series, each rated up to 10c.  is 100 amps a safe number though? i left that value as the default 25 because i was paranoid about damaging something. I'm a bit nervous to increase that value by more than 4 x without fully understanding the implications of doing so.  

I will look more into it! thanks for the tip!!
```

---
## \#16 Posted by: Namasaki Posted at: 2016-09-11T06:02:37.038Z Reads: 116

```
Those batteries can deliver 100amps continuously.
If your running a single vesc, try raising the max batt current to 50a and see if that fixes the problem.
The battery max current setting is for protecting the battery.
So even at 50a your way under what the battery can handle.
while your at it, you might want to turn the motor max current down to 50a.  The Vesc is rated for 50a cont output
```

---
## \#17 Posted by: Charlie_H Posted at: 2016-09-11T06:52:07.761Z Reads: 114

```
I will give it a shot! assuming that problems still occur after i test 50amps, is it safe to continue to increase the batt max by + 10 too see if it stops? all the way up to 100 amps? thanks again for taking the time to help me :slight_smile:
```

---
## \#18 Posted by: chris.hunt Posted at: 2016-09-11T07:07:52.071Z Reads: 116

```
Hey how do you like you nunchuk remote I am looking and remotes and this one popped up on my radar.
```

---
## \#19 Posted by: Ackmaniac Posted at: 2016-09-11T08:57:44.421Z Reads: 114

```
You have the Firmware with the bug in Min current ramp step. It always increasdes by the factor of 10 when you read and write the settings. Get the latest firmware or always check that value before you write your settings. By default it is at 0,0400. This can damage your vesc. Maybe that is also the reasen for your issues,

<img src="/uploads/db1493/original/3X/4/c/4cc3f332a5dd3ab68e36fb3824de85c9589b1986.jpg" width="690" height="344">
```

---
## \#20 Posted by: Pyrax Posted at: 2016-09-11T09:10:00.889Z Reads: 110

```
I had a similar problem with my board. Whenever accelerating or braking, about 2 seconds later the board would just stop responding until about 1 second later. It was due to there being a poor connection between the remote (winning remote) and the receiver. I moved the receiver to a better location and it worked fine. Maybe try your board with the receiver on the outside? (btw this also did only happen whilst the board was under load)
```

---
## \#21 Posted by: Charlie_H Posted at: 2016-09-11T09:23:04.260Z Reads: 106

```
I received my vesc after the date in which the bug was supposed to be an issue. I will try updating the firmware just to be sure. thanks!
```

---
## \#22 Posted by: Charlie_H Posted at: 2016-09-11T09:57:56.139Z Reads: 105

```
My receiver hasn't been housed in anything while testing. :/ i'm thinking maybe interference from the battery leads may be causing some issues even though they're not touching.
```

---
## \#23 Posted by: Charlie_H Posted at: 2016-09-11T10:01:43.200Z Reads: 104

```
I can not comment on that yet haha, i'm still having problems with my board and until i can confirm that it is not an issue with the nunhcuk i wont be recommending it.
```

---
## \#24 Posted by: Namasaki Posted at: 2016-09-11T12:36:05.910Z Reads: 100

```
Good catch @Ackmaniac 
However, the firmware bug would multiply the default .04 by 10 making it .4 not 50.0
Something else happened here. Someone may have adjusted that setting incorrectly. 
@Charlie_H 
Set the ramp step at .004 and write config to the Vesc. 
Then read config and check to see if it multiplied. 
If yes, update firmware
If no, reset value to .04 and write config.
```

---
## \#25 Posted by: Ackmaniac Posted at: 2016-09-11T12:42:18.583Z Reads: 95

```
When you read and write again then it multiplys each time.
First time write at 0.04 read 0.4
Second time write 0.4 read 4
Third time write 4 read 40
fourth time write 40 read 50 (50 is max).

Same discussion here
http://www.electric-skateboard.builders/t/lifepo4-battery-getting-drained-too-quickly/9249/9
```

---
## \#26 Posted by: Charlie_H Posted at: 2016-09-11T12:49:30.516Z Reads: 89

```
I updated the firmware. Board still cuts out, i'm going to continue to increase my batt max value tomorrow to see what happens. 

I have also ordered a cheap standard 2.4ghz 3 ch remote to see if that makes a difference
```

---
## \#27 Posted by: Namasaki Posted at: 2016-09-11T13:22:29.244Z Reads: 87

```
Didn't know that. Thanks for sharing!
```

---
## \#28 Posted by: Namasaki Posted at: 2016-09-11T13:23:55.488Z Reads: 89

```
If it's still cutting out at 50a, then something else is the problem. Likely the Kama remote
These are really good:
http://www.electric-skateboard.builders/t/33-bucks-small-group-buy-2-4ghz-mini-remote-trigger-style/7402
```

---
## \#29 Posted by: treenutter Posted at: 2016-09-11T13:48:18.128Z Reads: 92

```
@Ackmaniac @Namasaki Was this bug only present in BLDC Tool ports to OSX and Windows, or was it a part of the Linux rollout as well? I use Linux and I haven't noticed this problem w 2.18.

@Charlie_H I started out using nunchuck and VESC. I eventually stopped using the nunchuck because of two main problems:

1) the issue you're noting here. I couldn't seem to get a smooth throttle curve using nunchuck. For some unknown reason (unknown to me, anyway) the nunchuck paired with the native VESC app only interpreted a few throttle strengths (it seemed like 0%, 50%, 100%). This meant that I would hit a voltage cutoff too often because the throttle would register at 100% unintentionally. Maybe I had a dud nunchuck, maybe something wasn't set correctly, but I couldn't get it completely resolved.

2) The other issue was random dropouts, presumably due to signal interference. I tried two different nunchuck\receiver combinations. They would work great 80% of the time but then once in a while the remote would lose signal. This is OK if you're just riding in a driveway. For commuting it's totally unacceptable. 

I hope you can resolve your issues w nunchuk, but I couldn't, so I moved on to a modded GT2B and it is rock solid after about 400 miles of riding. Not a single dropout, control is highly responsive, and the case mod even makes it look cool!
```

---
## \#30 Posted by: Bender Posted at: 2016-09-11T14:14:39.539Z Reads: 88

```
The best way to find out if its is the remote or the vesc is to NOT turn off your board after it happens plug in the vesc to BLDC tool and type "faults" at the bottom of the terminal tab and you can see if there are any errors with the vesc. Also the red light on the Kama blinks for a few seconds when it about to or does disconnect. Though that is tough to see while your riding.
```

---
## \#31 Posted by: elkick Posted at: 2016-09-11T14:41:36.594Z Reads: 85

```
[quote="treenutter, post:29, topic:9315"]
Was this bug only present in BLDC Tool ports to OSX and Windows, or was it a part of the Linux rollout as well? I use Linux and I haven't noticed this problem w 2.1
[/quote]

It was fixed in the Linux version already end of June.
```

---
## \#33 Posted by: Bender Posted at: 2016-09-11T15:43:31.127Z Reads: 88

```
Please remember this was actually a firmware bug so I believe it was present in all iterations for a few weeks but unless you updated the firmware it doesn't mater which BLDC tool you use it will still be there.
So in short get any current BLDC tool then update (or re flash) the firmware. It might be the same name and number. And you should be all set.
```

---
## \#34 Posted by: Namasaki Posted at: 2016-09-11T21:08:42.273Z Reads: 87

```
When this bug was first discovered, it was reported that the issue did not occur when using linux bldc tool.
```

---
## \#35 Posted by: Charlie_H Posted at: 2016-09-12T13:09:33.684Z Reads: 80

```
I will give it a shot! i'm bust at the moment, but i was also considering putting a raspberry pi with bldc tool on it on the board to i can log the data from the ride and see what's happening when it cuts out
```

---
## \#36 Posted by: whitepony Posted at: 2016-09-12T13:54:02.608Z Reads: 84

```
I had these issues with nunchuck and other remote/receiver pairs, when the large currents ran too close to the receiver / receiver antenna!

to know for sure whats going on, provoke the cutout, then connect with your laptop without switching off the vesc, then type "faults" in the console input of the bldc gui and check if there have been any drv errors ... and if so, which ones!
```

---
## \#37 Posted by: Spencermiller Posted at: 2017-05-21T01:10:50.177Z Reads: 47

```
I had the exact same problem as you did, but I'm using 18650 cells in a 10S3P setup.  Did you ever resolve this issue?  If so, could you share your solution?  Thanks.
```

---
