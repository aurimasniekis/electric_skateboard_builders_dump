# Upgrading from 8S to 10S with VESC and 245kv 6364 SK3

### Replies: 32 Views: 3185

## \#1 Posted by: Alanhunt123 Posted at: 2017-02-21T05:45:06.059Z Reads: 223

```
Hi, 

I have been running a 245kv SK3 on 8s for a while, and thought it did pretty ok. However, the torque really wasn't quite enough for me. Eventually, my lipos gave out, and I decided to build a 10s4p pack with Samsung 25rs to try and get a little more umph. A friend of mine helped me set it up, and was kind enough to let me borrow his spot welder.

My question is, as long as I limit my ERPM to 60K, will my vesc be ok? Or should I just get a new motor? I only realized this might be an issue after I built the pack. Doh!

I have my eyes on a 6374 sk3, would be a blast! But, if it is unnecessary to upgrade, I'd like to keep my current motor. What do you guys think?
```

---
## \#2 Posted by: Alanhunt123 Posted at: 2017-02-21T05:49:20.410Z Reads: 222

```
Forgot to mention, I'm sticking with BLDC. Haven't tread into FOC waters yet. Besides, I kind of like having the noise, lets others know I'm coming.
```

---
## \#3 Posted by: dogeatgod Posted at: 2017-02-21T11:57:36.963Z Reads: 200

```
I went from 6S Car ESC on a 245kv to 10S VESC - despite changing gearing and changing VESC settings could not get the same performance as original set up. Changed to 6374 192kv and all good.
```

---
## \#4 Posted by: LukeL Posted at: 2017-02-21T13:27:42.791Z Reads: 189

```
I'm using 10S lipo with 240kv alien motor and limited the erpm 60k, I havn't had any vesc failures,

when i first built it i hadn't read about the erpm and used it without the limit, even then i had no failures riding it around my street.

to reach the 60k erpm limit with 15T - 36T gearing and 80mm wheels you have to go over 33mph, i'm guessing most people who got failures from this were spinning the motor with no load  or had a higher gearing ratio.

but i haven't tried any other motors yet so a lower kv may be better in someway

[quote="dogeatgod, post:3, topic:18019"]
I went from 6S Car ESC on a 245kv to 10S VESC
[/quote]

What do you mean by performance? I can't see how you could get near the same amount of speed/torque out of a 6S
```

---
## \#5 Posted by: Alanhunt123 Posted at: 2017-02-21T13:33:38.543Z Reads: 189

```
[quote="dogeatgod, post:3, topic:18019"]
changing VESC settings could not get the same performance as original set up
[/quote]

Very interesting. I wonder why that is.[quote="LukeL, post:4, topic:18019"]
I'm using 10S lipo with 240kv alien motor and limited the erpm 60k, I havn't had any vesc failures,
[/quote]

Thanks for the reply, sounds like you've had some sucess. As long as I limit my ERPM I shouldn't get any no load failures, right?
```

---
## \#6 Posted by: LukeL Posted at: 2017-02-21T14:02:08.020Z Reads: 176

```
Yeah the setting should  stop any chance of the erpm causing a failure. 

I also use the soft erpm limits on the ppm tab to slow down acceleration as you approach  60k. The fastest I've gone on my board is 24.8mph so this probably isn't a concern anyway.
```

---
## \#7 Posted by: Tuomalar Posted at: 2017-02-21T14:42:36.263Z Reads: 172

```
[quote="dogeatgod, post:3, topic:18019"]
I went from 6S Car ESC on a 245kv to 10S VESC - despite changing gearing and changing VESC settings could not get the same performance as original set up. Changed to 6374 192kv and all
[/quote]

So you didn't change battery? Just esc to vesc?
```

---
## \#8 Posted by: dogeatgod Posted at: 2017-02-21T14:57:14.235Z Reads: 165

```
6S to 10S with same motor SK3 245
6S was ESC - 10S VESC
I did not get any failures - just performance was not as good as with 10S.
Power was the issue, lack of acceleration, changed to 192 kv motor and bingo. Good acceleration and good top speed.
```

---
## \#9 Posted by: dogeatgod Posted at: 2017-02-21T14:59:16.146Z Reads: 162

```
6S 245 was a good all rounder
10S 245 lacked torque
```

---
## \#10 Posted by: Alanhunt123 Posted at: 2017-02-21T15:56:44.986Z Reads: 161

```
[quote="dogeatgod, post:8, topic:18019"]
Power was the issue
[/quote]

Maybe it was your motor max amp setting (on the low side). This plays a huge role in performance in the low speed torque. Since a Car ESC (or whatever you were using) likely doesn't limit motor current, this might be why you had worse performance from the VESC.
```

---
## \#11 Posted by: dogeatgod Posted at: 2017-02-21T16:23:24.558Z Reads: 151

```
yes, that's correct - I like cake a beer, so even with increasing max amps it wasn't enough.

I like the way an ESC can take abuse without complaining and am tempted to go back to the dark side for a 12S set up but am holding off until VESC 6 has been trialled.
```

---
## \#12 Posted by: treenutter Posted at: 2017-02-21T20:52:59.124Z Reads: 156

```
@Alanhunt123 here's the best thread we have on the subject, compliments of @chaka. TLDR: Your VESC and motor will be fine as long as the 60K  RPM threshold is not exceeded. You would likely experience an increase in available torque with a lower KV motor, at the cost of a lower top speed of course. If it were me, I'd keep the motor you've got. If you upgrade in the future you might consider 192kv.

I feel that the VESC the ERPM should be programmed into VESC firmware. Maybe there are some scenarios where you'd want to exceed it, but it seems to just cause problems for folks. I had a DRV fault once during bench testing. Seems like an avoidable problem!

http://www.electric-skateboard.builders/t/choosing-the-right-motor-kv-for-the-vesc/3125?source_topic_id=4737
```

---
## \#13 Posted by: eaglo Posted at: 2017-02-21T21:27:48.909Z Reads: 149

```
I have only put about 10 miles on my build, but its 10s dual vesc sk3 6364 245kv, erpm limit 60k, and I have had good torque and no vesc issues so far.
```

---
## \#14 Posted by: Namasaki Posted at: 2017-02-22T02:40:08.496Z Reads: 140

```
[quote="Alanhunt123, post:1, topic:18019"]
I have been running a 245kv SK3 on 8s for a while, and thought it did pretty ok. However, the torque really wasn't quite enough for me.
[/quote]

It has been said that lower KV and Larger motors like the 6374 produce more torque and is usually the best choice for a single drive.
6355 190kv motors work well on 10s in a dual drive.
I have found( thanks to @Hummie who led me in this direction) that increasing your motor max amps in the bldc tool will also increase power/torque especially at lower speeds. I got noticeable improvement on my dual drive with Vescs and 6355 190kv motors by just uping the max motor amps from 60 to 80, with no ill side affects caused to the Vescs or motors.
```

---
## \#15 Posted by: Namasaki Posted at: 2017-02-22T02:42:10.512Z Reads: 123

```
[quote="eaglo, post:13, topic:18019, full:true"]
I have only put about 10 miles on my build, but its 10s dual vesc sk3 6364 245kv, erpm limit 60k, and I have had good torque and no vesc issues so far.
[/quote]
Thanks for sharing that.
Good to know that the Erpm limit in the bldc tool really works.
```

---
## \#16 Posted by: Alanhunt123 Posted at: 2017-02-22T02:59:39.464Z Reads: 120

```
[quote="Namasaki, post:15, topic:18019"]
Thanks for sharing that.Good to know that the Erpm limit in the bldc tool really works
[/quote]

I've tried using really low ERPM limits, and it seems to work well. For example, I limit my reverse ERPM to 5000 to avoid backing up too fast. It never gets jittery around the limit, so I may end up limiting my forward ERPM to something like 50k-55k, since I don't want to go faster than that anyways. In fact, when I first tested my VESC on 8S, I limited to 40K, and never experienced any issues, the soft cutoff worked like magic!
```

---
## \#17 Posted by: Alanhunt123 Posted at: 2017-02-22T03:01:38.431Z Reads: 114

```
[quote="Namasaki, post:14, topic:18019"]
I got noticeable improvement on my dual drive with Vescs and 6355 190kv motors by just uping the max motor amps from 60 to 80, with no ill side affects caused to the Vescs or motors.
[/quote]

I have my motor max set to 70, the recommended max amp stated on Hobbyking, but my motor stays pretty cool. I'll try bumping up to 80, should give a nice boost! We'll see if my belt can hold out... just upgraded to a steel pulley.
```

---
## \#18 Posted by: Namasaki Posted at: 2017-02-22T04:40:41.575Z Reads: 111

```
The information your sharing about the erpm limit is very good. Maybe I've missed something along the way but this thread is the first I've seen where someone actually ran tests with erpm limiting and was able to offer conclusive results. This kind of knowledge is a real game changer. 
As for the motor max amps, my motors are rated for 80 amps. I have run the motor max as high as 100a
With just a little warming while driving hard uphill. 
At 80a motor max, they barely even get warm. 
The person who got me to experiment with this setting is running his at 200a in FOC mode!
100a felt like more power than I needed so I backed it down to 80a
```

---
## \#19 Posted by: Alanhunt123 Posted at: 2017-02-22T05:01:23.365Z Reads: 115

```
[quote="Namasaki, post:18, topic:18019"]
The information your sharing about the erpm limit is very good.
[/quote]

Great to hear! I'm always trying to get more involved in the E-Sk8 community.

[quote="Namasaki, post:18, topic:18019"]
The person who got me to experiment with this setting is running his at 200a in FOC mode!
[/quote]

That's insane! Must be a beast with tons of startup torque! This type of setup must really benefit from having a sensored motor. I have yet to venture into the sensored territory, but will likely pick one up if/when my current motor dies.
```

---
## \#20 Posted by: Namasaki Posted at: 2017-02-22T05:09:08.825Z Reads: 109

```
I don't think he's running sensor motors. Just FOC mode in the Vesc. 
And you hit the nail right on the head. 
He said it gave him lots of startup torque
```

---
## \#21 Posted by: Alanhunt123 Posted at: 2017-02-22T05:13:15.161Z Reads: 102

```
Interesting. I am hesitant to try FOC on my VESC, since it is an Enertion board, which is already known to be finicky. Plus, I kind of enjoy the sound BLDC gives me. Is startup torque better in FOC, even with sensorless?
```

---
## \#22 Posted by: Hummie Posted at: 2017-02-22T06:00:08.383Z Reads: 105

```
@devin, who is now just over his banning period...haha, got me on the 200 motor amp limit.  they are 200 amps for a fraction of the commutation time, the "duty cycle" and the inductance of the motor coils smoothes out the pulses out to an average amperage much lower.  
a stated motor amp limit is suspect besides.
200 motor amps feels much smoother, much better early acceleration, and has less cogging and I can start from a dead stop with the slightest rocking.
```

---
## \#23 Posted by: Alanhunt123 Posted at: 2017-02-22T06:10:05.858Z Reads: 121

```
Should I try this with BLDC? Maybe something like 150A? I have more than adequate cooling on my mosfets, as I custom CNC milled an aluminum  VESC enclosure that doubles as a massive heatsink. Will post pictures if anyone is interested
```

---
## \#24 Posted by: Namasaki Posted at: 2017-02-22T07:03:25.633Z Reads: 145

```
Oh ya, I'll bet CNC heat sink Vesc enclosures would sell like hotcakes here!
Post some pics please!
```

---
## \#25 Posted by: Alanhunt123 Posted at: 2017-02-22T14:43:04.842Z Reads: 145

```
<img src="/uploads/db1493/original/3X/a/1/a119e98c6a1b54bb75d26f618fc6f6a5901b0dad.PNG" width="690" height="466">

<img src="/uploads/db1493/original/3X/d/6/d69e560c60c42fc00ef0f4dc6b3f1fe2cd08c5e9.jpg" width="666" height="500">

<img src="/uploads/db1493/original/3X/0/5/05535e2e9efa0dd712d3144dc1eabb156ade90d1.jpg" width="666" height="500">

This enclosure has a raised surface inside it that the MOSFETs sit on. I used some thermal paste to transfer heat between the MOSFETs and the enclosure. The top MOSFETs have a "Bridge" that makes contact with them and transfers heat to the case through the mounting screws (which are also coated with thermal paste).

Since I switched from heat shrink to this enclosure, I went from having power loss after 20 seconds of going uphill to no power loss on any hills at all. The enclosure really does an overkill job of keeping those MOSFETs cool, as well as looking beautiful under the board.

Here is the one caveat preventing me from manufacturing more to sell. Since the enclosure was designed using WPI licensed software (Solidworks) and machined using WPI owned machinery (Haas VM2), I would run into legal issues very quickly with WPI.

This summer, however, I am working for a professor that owns a custom CNC shop oriented towards small production sizes, mainly for hobbyists or educational teams, such as a robotics team. So, we may be able to strike a deal making some of these. For now, the VESC enclosure remains off the market. :disappointed:
```

---
## \#26 Posted by: Hummie Posted at: 2017-02-22T15:08:32.791Z Reads: 135

```
I've never hit an overheat shut down running even one large hub motor and 200 motor amp limit.  before i was running two motors at 70 battery and 70 motor each and never had a shut down either.  no heat sink or special cooling.
```

---
## \#27 Posted by: Alanhunt123 Posted at: 2017-02-22T15:16:19.133Z Reads: 132

```
Yeah, I was a bit perplexed why I was getting this overheating issue, perhaps it was the heat shrink supplied with the VESC that was the issue (was a board that a guy from Enertion had sitting on his desk to replace my stubborn board that kept blowing DRVs). The Vesc was sitting pretty cramped inside my battery enclosure, which may have something to do with it as well.

I never got a shutdown either, but after a few seconds of hillclimb or braking, I would notice a decrease of performance to the point that the board could no longer climb. No issues with this setup though, now that I have the enclosure. In fact, I bet it could handle crazy amounts of current now that it has a really good heatsink.
```

---
## \#28 Posted by: Alanhunt123 Posted at: 2017-02-27T16:32:55.921Z Reads: 117

```
Just tried out my new 10s board with this motor. It's a beast! Using 120A/45A motor/battery current, a 15:40 ratio, and 83mm wheels, it's just crazy powerful. No problems so far. Will post a build thread soon.
```

---
## \#29 Posted by: Namasaki Posted at: 2017-02-27T21:39:38.290Z Reads: 110

```
15:40 is very low gearing and with 83mm wheels and 120a motor current, your acceleration must be insane!
Keep an eye on your motor to make sure its not overheating. If you feel it's getting too hot then you can back off your motor current to bring the temp down.
```

---
## \#30 Posted by: Alanhunt123 Posted at: 2017-02-28T14:54:01.369Z Reads: 107

```
At the very most, the motor is warm to the touch, but not so hot that you can't touch it for an extended period of time. I'll try a hill climb test to see how it performs.
```

---
## \#31 Posted by: makevoid Posted at: 2017-02-28T15:12:43.135Z Reads: 108

```
wow, that enclosure is awesome! it looks like it protects and cools the vesc perfectly 

@Hummie I recently switched from single motor to dual and the vescs don't get hot anymore as my single one did but on my single (6374) old build the vesc overheated significantly. I'm quite heavvy (~105kg) and I wasn't able to climb hills at speed when the vesc overheated and I had to break softly to make breaks not to cut out. I guess with dual, with smaller motors and/or if you're 70kg or less that is less of an issue.
```

---
## \#32 Posted by: Alanhunt123 Posted at: 2017-02-28T18:18:14.315Z Reads: 104

```
Really proud of the enclosure. It looks like I may have a deal with the professor I am working with to make some eSk8 parts, this might be one of them!
```

---
