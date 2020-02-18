# Power cuts/disconnects after installing ABEC 107&rsquo;s

### Replies: 31 Views: 430

## \#1 Posted by: Celt Posted at: 2019-03-16T14:58:47.223Z Reads: 160

```
Hey guys,

So I just recently upgraded from my Torque Board's 97mm to the ABEC 107mm, nothing else has changed  and I started getting what I want to call power cuts under heavy acceleration. 

I'm running 12S4P with dual 6355's with the Focbox Unity.

When I first installed them I definitely noticed a reduction in acceleration. I thought maybe there's to much strain so I up'd the amperage from 50 to 55 and same with the brakes but no difference that I can tell other then a bit more power. I never touched the battery amps.

Any ideas?

Also separate issue is that one of the motors is noticeably a bit louder then the other, annoyingly so. I tried adjusting belt tension to be the same as the other side and swapped to a different belt but no change. It honestly sounds like one is running in FOC and the other is running in BLDC just to give an idea.

Thanks!!
```

---
## \#2 Posted by: goldrabe Posted at: 2019-03-16T15:10:40.070Z Reads: 152

```
Did you adjusted the motor amps via android app?
```

---
## \#3 Posted by: legend27 Posted at: 2019-03-16T15:10:52.435Z Reads: 151

```
Im guessing it's Samsung 30Q, right?

12S4P 30Q are able to draw a max of 60A (actually 80A).
Is it 55A on motor max or battery max?

If it's 55A battery max on each motor, then i'm guessing it's overdraw limit (if that's a thing).

Try bumping your amps down to 50A again. You won't be able to get the same acceleration again with 107mm anyway.
```

---
## \#4 Posted by: Celt Posted at: 2019-03-16T15:13:11.058Z Reads: 142

```
Hey yeah I did.
```

---
## \#5 Posted by: goldrabe Posted at: 2019-03-16T15:15:36.694Z Reads: 135

```
Are you sure that you hit read before applying the new settings?
The App is still buggy, hook the Unity to your computer and redo motor detection and settings with the Focbox tool and see if it goes away.
```

---
## \#6 Posted by: Celt Posted at: 2019-03-16T15:16:43.027Z Reads: 133

```
Yup it's 30Q. Wait so 60 or 80A? 

Atm my settings are Battery=50A, Max Braking=-8A, Motors=57A & -57A.

Well thing is it was a 50A on battery and motors before I did anything. Then I up'd them to the settings I listed. I've been having cuts on 50A & the higher settings (57A).
```

---
## \#7 Posted by: Celt Posted at: 2019-03-16T15:18:25.832Z Reads: 130

```
Yeah I definitely did hit read. Thing is this was a none issue when I had the 97mm on. I could try hooking it up and redoing I guess. So lazy I'll do it later today...lol.
```

---
## \#8 Posted by: goldrabe Posted at: 2019-03-16T15:23:01.264Z Reads: 123

```
The Bluetooth is still unreliable, I don´t use the app anymore for changing any settings. Sometimes it even does not show the HUD data correctly, I am pretty sure that this messed up your motors settings.
```

---
## \#9 Posted by: Celt Posted at: 2019-03-16T15:28:04.215Z Reads: 120

```
Alright I hear you, I'll adjust later on today and report back.

For what it's worth BT has been working ok for me for the most part.
```

---
## \#10 Posted by: legend27 Posted at: 2019-03-16T16:02:51.282Z Reads: 116

```
Rated for 15A (per cell) by Samsung but have been tested at 20A (per cell) without any issues. We are starting to hit my knowledge limit but I'm pretty sure it isn't recommend to set your battery to 80A but 70A should be okay I believe (not sure)

Anyway.

Is battery 50A for each motor or both?
```

---
## \#11 Posted by: Celt Posted at: 2019-03-16T16:06:12.995Z Reads: 107

```
What does upping the battery max do anyway?  
I think it's both since there's only one slider?
```

---
## \#12 Posted by: legend27 Posted at: 2019-03-16T19:10:42.447Z Reads: 93

```
Limits how many amps you can pull from your battery.

Sounds like you are right. 25A for each then. 

Have you got like a Metr module or something you can record your live stats? Maybe you can try to record your stats when accelerating hard?
```

---
## \#13 Posted by: Celt Posted at: 2019-03-18T18:41:22.385Z Reads: 78

```
I don't having anything to record the stats. I have the Unity and I don't know what other apps it works with besides the Unity app.
```

---
## \#14 Posted by: Celt Posted at: 2019-03-18T18:46:29.655Z Reads: 77

```
So just to update this thread.
Yesterday I hooked up the Unity via cable and did a firmware update (just to reset everything, I already have the latest firmware) and then I changed some settings up to almost 60 amps. Yesterday all seemed ok didn't have any issues what so ever. Then today I was just riding and it started happening again a lot. Accelerating and cut or braking and cut. I also checked the receiver and I have it siliconed in and it doesn't seem to be coming out or anything. I have no idea what else to do at this point. I can only assume interference, I am in Seattle but it happens in residential and down town. Sigh....
```

---
## \#15 Posted by: Celt Posted at: 2019-03-19T04:01:11.436Z Reads: 72

```
If anyone has any ideas I'd be grateful!
```

---
## \#16 Posted by: dareno Posted at: 2019-03-19T04:22:32.956Z Reads: 68

```
Could be wrong but it sounds more like a remote receiver issue than a settings problem.  Pretty conservative battery/motor settings really.  What remote are you using?
```

---
## \#17 Posted by: myreala Posted at: 2019-03-19T06:51:40.783Z Reads: 63

```
What bms are you using?
```

---
## \#18 Posted by: legend27 Posted at: 2019-03-19T06:55:56.647Z Reads: 63

```
xMatic, but it's no way near the Metr app. Just shows some overall stats for the ride and error logging. You need it to show every single little stat through the ride.
```

---
## \#19 Posted by: Celt Posted at: 2019-03-21T13:19:03.189Z Reads: 55

```
Hey! I'm using the Nano V2 from Torque Boards.
```

---
## \#20 Posted by: Celt Posted at: 2019-03-21T13:19:34.804Z Reads: 53

```
I'm using the 12S4P battery from Torque Boards so I have no idea what the BMS is.
```

---
## \#21 Posted by: Celt Posted at: 2019-03-21T13:21:52.596Z Reads: 51

```
[quote="legend27, post:18, topic:87331"]
xMatic
[/quote]

Problem is I have android :(.

If needed though I could potentially get a cheap iPhone just to error log?
```

---
## \#22 Posted by: Sn4pz Posted at: 2019-03-21T13:38:26.316Z Reads: 50

```
Metr works on Android, the hardware you have to monitor your vesc is what isn't up to the task

You have an hm 10 module, right?
```

---
## \#23 Posted by: Celt Posted at: 2019-03-21T13:54:28.657Z Reads: 50

```
I have a Focbox Unity, has bluetooth built in.
```

---
## \#24 Posted by: Sn4pz Posted at: 2019-03-21T14:01:02.564Z Reads: 52

```
Ah ok, that is not the Metr module, and although its annoying to go out and buy another thing, the Metr is the best diagnostics tool that we have out now, I would think

@CarlCollins <- this guy is magic, he can probably help you out
```

---
## \#25 Posted by: Celt Posted at: 2019-03-21T15:39:41.478Z Reads: 49

```
Thanks! I sent him a message. We'll see what he says.
```

---
## \#26 Posted by: DerelictRobot Posted at: 2019-03-21T15:40:06.366Z Reads: 48

```
This is actually almost identical to the issue that came up for me yesterday. I'm 150 miles into riding this build, it's been solid until yesterday and I experienced almost exactly what you describe. 90 motor/40 single(80) both channels on battery. I did see 'over current' error coming up while this was happening and it was isolated to my right channel in physical behavior. I lowered settings to 'babytown frolics' mode at 65/60 and still had the exact same issues. 

Haven't had time to diagnose yet but will when I get back from Bakersfield next week.
```

---
## \#27 Posted by: Celt Posted at: 2019-03-21T15:41:34.607Z Reads: 45

```
[quote="DerelictRobot, post:26, topic:87331"]
os
[/quote]

Yeah please keep me posted and I hope you get it sorted out!
```

---
## \#28 Posted by: legend27 Posted at: 2019-03-21T18:07:28.449Z Reads: 42

```
I totalt forgot about Ackmaniac! Try it! Its an app for Android only :slight_smile:
```

---
## \#29 Posted by: myreala Posted at: 2019-03-21T22:09:09.855Z Reads: 39

```
If it's an older model they only had 30A or 45A BMS at the time. That could be your problem, with 107's you are likely pulling more current for the same torque and its hitting the limit of the BMS which switch's off. If you accelerate slowly then this shouldn't happen. Anothing way to test this is to start on a hill and do full throttle, if you cut out it is more likely to be the BMS.
```

---
## \#30 Posted by: CarlCollins Posted at: 2019-03-22T08:40:16.760Z Reads: 37

```
Replied to you inbox message
```

---
## \#31 Posted by: Celt Posted at: 2019-04-01T18:16:12.217Z Reads: 27

```
Hey guys so just to update this thread. It looks like it was AGAIN my receiver/server wire connections that were coming loose. It was pretty subtle and I was surprised it was happening. It did a short test ride and no issues.

So yeah check that connection if you’re having the same issues as me!
```

---
