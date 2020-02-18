# Another VESC Blown

### Replies: 43 Views: 854

## \#1 Posted by: erod998 Posted at: 2018-08-22T05:14:56.749Z Reads: 240

```
Hey all
Second VESC here. TorqueBoards one. First one I shorted a motor wire and blew, replaced. Got it yesterday and installed it today and was doing about 15 miles of riding. Next thing I know....

![IMG_2104|374x500](upload://vX3YJtBo388sY2SonUxiHTVo9tP.JPG)
![IMG_2105|374x500](upload://6kVjbBAHln53siopyi2GaP0sERc.JPG)
I am using a 12s4p, and their 6374. Motor limit was 80, -80 watts. ERPM limit was 60,000 and -60,000, and battery limit was 70 and -12.

So I have two questions. What the heck coulda caused this to blow? I was literally riding it and it stopped. Not pushing it hard. Also, anyone know any VESC repair services on here?
```

---
## \#2 Posted by: nuttyjeff Posted at: 2018-08-22T12:47:27.326Z Reads: 214

```
DRV blown - are you running FOC on 2.18 firmware?
```

---
## \#3 Posted by: Andy87 Posted at: 2018-08-22T12:52:31.847Z Reads: 210

```
@Martinsp repairs 4.12 HW

You run single VESC right?
70A bat max definitely too much.
Not sure what´s the limit for 4.12, but should be around 40-50A max with heat sink.
I know your battery maybe can supply that, but your VESC as you can see can´t handle it.
Do you have some logfiles from your ride?
```

---
## \#4 Posted by: BoostedBuilder Posted at: 2018-08-22T13:14:45.299Z Reads: 200

```
You want a FOCBOX so this doesn't happen anymore!?
```

---
## \#5 Posted by: Andy87 Posted at: 2018-08-22T13:15:34.227Z Reads: 198

```
Which focbox can handle 70a battery current?
```

---
## \#6 Posted by: BoostedBuilder Posted at: 2018-08-22T13:18:08.158Z Reads: 195

```
UNITY can
So can a single one if properly cooled
And motor amps aren't necessary the same as battery amps
```

---
## \#7 Posted by: Andy87 Posted at: 2018-08-22T13:23:52.269Z Reads: 189

```
Unity is a other topic...and a unity for single setup 🤔...ok 
I think only @Kug3lis got that focbox to such a high current with his special heat sink case.
But that’s also a bit a tuning of the focbox 😉
The standard focbox will not last long with that settings.
```

---
## \#8 Posted by: erod998 Posted at: 2018-08-22T14:20:04.349Z Reads: 176

```
I do not have logs.
```

---
## \#9 Posted by: linsus Posted at: 2018-08-22T14:24:25.775Z Reads: 176

```
[quote="erod998, post:1, topic:65675"]
I am using a 12s4p
[/quote]

Dont do 12S on 4.12 HW...Switch to 10S and make sure you have 4.2uF on C18.
```

---
## \#10 Posted by: threebysix Posted at: 2018-08-22T14:33:12.994Z Reads: 165

```
I run 12s on my TB vesc but my values aren't as high as op's
```

---
## \#11 Posted by: erod998 Posted at: 2018-08-22T14:49:26.957Z Reads: 159

```
I have a hot air rework station. Kinda wanna attempt to replace the DRV again. Last time I didn’t have solder paste and messed up a pin on the PCB when I tried to remove. If I can’t find a service for 40 ish bucks in the US I will try it. 

Also, I didn’t know the VESC couldn’t handle those values. Should I reduce them or heat sink the mosfets and DRV?
```

---
## \#12 Posted by: erod998 Posted at: 2018-08-22T14:50:09.738Z Reads: 151

```
I’ll add the capacitor but going to 10s is impossible now.
```

---
## \#13 Posted by: erod998 Posted at: 2018-08-22T14:51:15.982Z Reads: 150

```
If the battery amps is set to 50, isn’t the motor technically limited to 50?
```

---
## \#14 Posted by: mmaner Posted at: 2018-08-22T14:51:43.807Z Reads: 151

```
PM @JohnnyMeduse, he can fix the the VESC for you.  FYI, anything over 50/-50 on the TB VESC is dangerous.   With a focbox you can go to 60/-60 with no problems, in fact i've run 70-70 before.
```

---
## \#15 Posted by: erod998 Posted at: 2018-08-22T14:59:49.246Z Reads: 144

```
Over 50 battery amps or motor amps?
```

---
## \#16 Posted by: mmaner Posted at: 2018-08-22T15:02:46.422Z Reads: 142

```
this is what I run...
![image|583x158](upload://LgfgnDpRZVdN2DSWSgzUWlKus9.png)
```

---
## \#17 Posted by: Namasaki Posted at: 2018-08-22T15:08:46.384Z Reads: 143

```
[quote="erod998, post:13, topic:65675, full:true"]
If the battery amps is set to 50, isn’t the motor technically limited to 50?
[/quote]

No........
I run batt max 50a
Motor max 80a
On 10s
On 12s you should start with @mmaner suggested motor max and go from there checking your motor temp. 
Running motor max too high can cause the motor to overheat
```

---
## \#18 Posted by: Andy87 Posted at: 2018-08-22T16:36:25.245Z Reads: 127

```
The vesc converts your amps and voltage coming in to what is going out.
That means that the motor current can be higher than the battery current but the voltage on the motor will drop in this case.
So U*I input is U*I Output but the values of U and I is changed by the vesc according to your response on the throttle.
```

---
## \#19 Posted by: erod998 Posted at: 2018-08-22T22:29:19.484Z Reads: 116

```
Doe sit matter if I get the DRV8302DCA or DRV8302DCAR? The former is out of stock at mouser.
```

---
## \#20 Posted by: b264 Posted at: 2018-08-22T23:05:37.772Z Reads: 115

```
[quote="threebysix, post:10, topic:65675, full:true"]
I run 12s on my TB vesc but my values aren’t as high as op’s
[/quote]

I jumped off a bridge and didn't die, but I had my arms sticking out further

It must be safe for you to jump, if you stick your arms out further

/s :stuck_out_tongue:
```

---
## \#21 Posted by: Zac13 Posted at: 2018-08-22T23:23:13.475Z Reads: 107

```
Do you have a dual setup or a single?
```

---
## \#22 Posted by: Zac13 Posted at: 2018-08-22T23:36:33.422Z Reads: 108

```
I've run 40 each on TB vescs and have blown 2

I've read that they're just problematic

I just ordered focboxes myself
```

---
## \#23 Posted by: threebysix Posted at: 2018-08-22T23:41:00.840Z Reads: 103

```
I run dual 6355 at 50 and -60 for about 5ish months now. But I am a light weight tho...

I guess only time will tell when it fails
```

---
## \#24 Posted by: threebysix Posted at: 2018-08-22T23:42:06.103Z Reads: 105

```
heh

"Jumps off sidewalk curb"
```

---
## \#25 Posted by: Zac13 Posted at: 2018-08-22T23:50:01.270Z Reads: 101

```
ah nice

I'm about 180 lbs, running dual 6374.  Idk.  Maybe i'll lower it even further than 40 when i get focboxes
```

---
## \#26 Posted by: threebysix Posted at: 2018-08-23T00:09:45.190Z Reads: 94

```
I'm about 120 lbs. How did your TB vescs fail? sudden failure?

I'm considering Flipsky's esc.
```

---
## \#27 Posted by: Zac13 Posted at: 2018-08-23T01:33:35.240Z Reads: 91

```
Yup exactly
```

---
## \#28 Posted by: DougM Posted at: 2018-08-23T01:39:37.945Z Reads: 93

```
I'm in the process of retiring all of my 4.1x series.  Consider this an upgrade opportunity? :slight_smile:
```

---
## \#29 Posted by: erod998 Posted at: 2018-08-24T01:08:00.987Z Reads: 83

```
I am 180. I would like to upgrade but that’s not in the budget right now. I’m two VESCs deep on this build now.
```

---
## \#30 Posted by: threebysix Posted at: 2018-08-24T02:47:04.185Z Reads: 81

```
Won't matter. The letters only affect the way the DRV is packaged (eg: comes in plastic reel or, paper reel).
```

---
## \#31 Posted by: erod998 Posted at: 2018-08-27T21:14:44.245Z Reads: 73

```
I replaced the DRV with one I had lying around. The DRV was new but it had previously been attempted to be soldered on another VESC. The DRV does not show any signs of failure though. After I replaced it, I powered it on. Found I had a short on one of the DRV pins and fixed it. Powered on again and found that the D5 diode was hot. I replaced it and the board turned on for about 2 seconds before going dark again. I have a short between the D5 diode I think, the 5v and GND on the servo connector have continuity. I have another diode to try, but that doesn't help me if it is going to short again somehow. I believe D5 and D4 are both fried somehow since I am getting .12 volts either way I test them. UPDATE:
Turned on the VESC even though it was getting hot. D5 got so hot it unsoldered itself, but after it did, the board came on and I am connected in the VESC tool. What does D5 do, and can I run it without? And what could cause D5 to short?
```

---
## \#32 Posted by: b264 Posted at: 2018-08-27T22:01:58.255Z Reads: 69

```
[quote="erod998, post:31, topic:65675"]
What does D5 do, and can I run it without?
[/quote]

D5 clamps any overvoltage on the 5V rail before it destroys the microcontroller/CPU.  The DRV8302 provides the 5V.  It can run without it, but it's a safety device which should probably be replaced.  The servo receiver also uses the 5V supply rail for power.
```

---
## \#33 Posted by: erod998 Posted at: 2018-08-27T22:09:13.162Z Reads: 67

```
[quote="erod998, post:31, topic:65675"]
Turned on the VESC even though it was getting hot. D5 got so hot it unsoldered itself, but after it did, the board came on and I am connected in the VESC tool. What does D5 do, and can I run it without? And what could cause D5 to short?
[/quote]


Maybe the diode I pulled off another VESC was broken, but when I replaced it, it did the same thing the other one did. NO power and and gets hot. I pulled it back off and it was working. Could there something else that could cause a good diode to go bad in that case? Or did I have a bad diode.
```

---
## \#34 Posted by: b264 Posted at: 2018-08-27T23:08:32.299Z Reads: 67

```
Using a multimeter, check the voltage on the pads when the diode is removed, or the voltage on the servo power and ground pins
```

---
## \#35 Posted by: gaetjen Posted at: 2018-08-28T08:08:17.922Z Reads: 63

```
![IMG_20180812_182802|281x500](upload://i1U6FNKMldfIwLk9qVLHaN3YTkb.jpg)
Does anybody know what the reason for this could be? I have ran the same setup for 2 years. I installed a new button on my anti spark switch and after a couple of rides, this happened.
```

---
## \#36 Posted by: erod998 Posted at: 2018-08-28T13:39:54.417Z Reads: 54

```
Not sure what happened. Had the system on and tried to spin the motor up and it blew up the mosfet switch and the motor didn’t spin. If I use a lab power supply, is there a way to see if the VESC is sending power through the phase wires?
```

---
## \#37 Posted by: ARetardedPillow Posted at: 2018-08-28T13:53:45.027Z Reads: 53

```
Have you tried turning it on and off again?
```

---
## \#38 Posted by: mmaner Posted at: 2018-08-28T14:51:03.225Z Reads: 47

```
jesus christ, did you summon a demon? :slight_smile:
```

---
## \#39 Posted by: erod998 Posted at: 2018-08-28T14:58:05.782Z Reads: 46

```
Haha, it scared the crap out of me. The mosfet on the spark switch freaking exploded. Time to order a new one, but more importantly, inspect the VESC.
```

---
## \#40 Posted by: gaetjen Posted at: 2018-08-28T17:12:25.472Z Reads: 44

```
No, there´s a hole in it...:-)
```

---
## \#41 Posted by: erod998 Posted at: 2018-08-28T20:10:54.385Z Reads: 39

```
Yea I messed the VESC up. Suspected reason: I had polarity wrong. No resistance between positive and negative Vin on the VESC now. Anywhere from 0.0 to .01 ohms. How fun.
```

---
## \#42 Posted by: b264 Posted at: 2018-08-28T20:14:35.752Z Reads: 40

```
If it was operator error and not equipment failure, you should consider removing the "TB" from the title :slight_smile:
```

---
## \#43 Posted by: erod998 Posted at: 2018-08-28T20:15:30.110Z Reads: 40

```
Yes originally I suspected equipment failure, but the original failure of the VESC was supposedly from having the battery amps too high. Title changed. 
Anyways, is it possible to fix a VESC damaged by reverse polarity?
```

---
