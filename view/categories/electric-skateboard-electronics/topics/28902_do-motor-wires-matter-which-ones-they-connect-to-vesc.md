# Do motor wires matter which ones they connect to VESC?

### Replies: 48 Views: 3091

## \#1 Posted by: thetechtrader Posted at: 2017-07-28T14:02:11.752Z Reads: 252

```
Im getting ready to plug in my first vesc and motor but I dont know what wires go where. Both the motor and vest have three wires.

Do I just plug them in so the middle wire on motor goes to middle wire on vesc, then flip the two outside wires to change direction of motor if needed?
```

---
## \#2 Posted by: JLabs Posted at: 2017-07-28T14:03:38.159Z Reads: 250

```
[quote="thetechtrader, post:1, topic:28902"]
Do I just plug them in so the middle wire on motor goes to middle wire on vesc, then flip the two outside wires to change direction of motor if needed?
[/quote]

Kind of, you can use any combination of wires with the VESC, and if you need to change direction swap any two wires.
```

---
## \#3 Posted by: gliz5714 Posted at: 2017-07-28T14:27:27.331Z Reads: 237

```
Thanks for asking this question... I will be assembling sometime next week and I also was wondering this!
```

---
## \#4 Posted by: thetechtrader Posted at: 2017-07-29T04:34:16.837Z Reads: 220

```
Im a first time VESC user, got everything all soldered up and ready, but now I need the final steps on how to set all the VESC settings for my particular setup and would really appreciate a step by step/screen share for variables/settings everything you think I would need to set:slight_smile: 

Keep in mind, this is NOT for a skateboard, rather a type of boat.

- Im running 2x 6S (22.2v each) in series providing 12S, any settings for this power?
- I have inline 60A fuse, and would like to set the VESC to liimit max Amps to 50A ??
- I do not want reverse
- I do not want regenerative braking
- Im running 500kv, 6 POLE inrunner. how do I limit RPM to 20,000

Im running VESC:
Hardware version:4.12   
Firmware version:2.18
```

---
## \#5 Posted by: Namasaki Posted at: 2017-07-29T04:42:57.560Z Reads: 201

```
500kv is much too high.
For 12s you should be using 170kv  motor
```

---
## \#6 Posted by: Jinra Posted at: 2017-07-29T04:44:30.087Z Reads: 196

```
Current limits are in BLDC tool. Battery max is current going into the VESC, Motor max is current in the motor. A 6 pole motor should translate to 3 erpm = 1 rpm. Which means 60,000 eRPM = 20,000rpm which is perfect since 60k is about what the VESC4 can take. You can set that limit in the same page as currents.

For setup, you just need to configure the current limits, then run motor detection in the BLDC tab. Then setup your controller in the App Config tab and you're pretty much set.

@Namasaki this is a boat not esk8
```

---
## \#7 Posted by: Namasaki Posted at: 2017-07-29T04:45:46.458Z Reads: 188

```
[quote="Jinra, post:6, topic:28902"]
@Namasaki this is a boat not esk8
[/quote]


Oh, LoL......
So much for my fast reading skills, skipped right over that.
```

---
## \#8 Posted by: evoheyax Posted at: 2017-07-29T05:02:53.892Z Reads: 181

```
[quote="thetechtrader, post:4, topic:28902"]
Im running 500kv, 6 POLE inrunner. how do I limit RPM to 20,000
[/quote]

You need to calculate the erpm. To calculate erpm, take the number of poles, divide by 2, and multiple by the rpm.

So if you have typical 14 pole pair, 20000*7 = 140000 erpm.

This is your max erpm setting, which is found on the right side of the main page of the BLDC tool!
```

---
## \#9 Posted by: thetechtrader Posted at: 2017-07-29T13:08:28.907Z Reads: 160

```
Thanks everyone!
how about making sure REVERSE is turned off? is there a box to check or something?
```

---
## \#10 Posted by: Alanhunt123 Posted at: 2017-07-29T13:13:04.363Z Reads: 151

```
Yes, on the "App Configuration" tab, there should be a tab on the left called "PPM". Within that tab there should be a number of different settings to choose frop at the top, I would choose "current no reverse".
```

---
## \#12 Posted by: thetechtrader Posted at: 2017-07-29T13:44:02.560Z Reads: 135

```
I got it to connect ignore this, sorry guys
```

---
## \#13 Posted by: thetechtrader Posted at: 2017-07-29T13:44:27.924Z Reads: 130

```
This is what I need to figure out:
<img src="/uploads/db1493/original/3X/b/d/bd24a8ce86859a36d05617d0f1803bd4dde89112.png" width="574" height="339">
```

---
## \#14 Posted by: JLabs Posted at: 2017-07-29T14:05:46.569Z Reads: 114

```
You would do 4.2 x 12 = 50.4 for max and 3 x 12 = 36 for min
```

---
## \#15 Posted by: thetechtrader Posted at: 2017-07-29T14:31:07.608Z Reads: 109

```
Are you talking about the TOP TWO? "Min Input Voltage" and Max input voltage"?

Or the battery cuttof start and stop.

Can you tell me a safe range for all four please :slight_smile:
```

---
## \#16 Posted by: JLabs Posted at: 2017-07-29T14:44:11.785Z Reads: 103

```
Oh sorry my bad, I was thinking something different. 

36v is you batt cutoff end and you can use 39.6v as the batt cutoff start. Do not change the first two values.
```

---
## \#17 Posted by: thetechtrader Posted at: 2017-07-29T15:04:48.575Z Reads: 99

```
Thank you,

Also, my alien power system remote seems to only be one speed, all of nothing. Is there a setting in BLDC tool to set the remote to have varial speed in the trigger?
```

---
## \#18 Posted by: JLabs Posted at: 2017-07-29T15:45:19.833Z Reads: 95

```
Not exactly sure what you mean, but did you set the min and max pulse width values in the PPM tab if the VESC?
```

---
## \#19 Posted by: thetechtrader Posted at: 2017-07-29T15:58:00.102Z Reads: 91

```
just have default min max pulse being min 1.50, and max 2.0
PID mad ERPM 15000 (not sure what PID ERPM is)?
```

---
## \#20 Posted by: JLabs Posted at: 2017-07-29T16:11:43.071Z Reads: 90

```
Check the little “display” box and a green bar will appear.  Then push the trigger all the way forward for break and look at the value inside the changing box, then input that value in the min pulse width. Then pull the trigger on the way back for throttle and enter the value you see in the max pulse width box.

Should be somewhere around 1 for min and 2 for max
```

---
## \#21 Posted by: thetechtrader Posted at: 2017-07-29T16:25:55.110Z Reads: 78

```
interesting, when my trigger is fully pulled its reading 2.85 much higher than the max 2 that you stated?
```

---
## \#22 Posted by: JLabs Posted at: 2017-07-29T16:57:24.758Z Reads: 73

```
That’s fine, just input that value in the max box
```

---
## \#23 Posted by: thetechtrader Posted at: 2017-07-29T16:59:09.180Z Reads: 70

```
Thanks JLabs.. 
I just cant get the throttle to have any control still. its full out, or nothing, frustrating
```

---
## \#24 Posted by: JLabs Posted at: 2017-07-29T17:03:17.233Z Reads: 69

```
Interesting... Post some full screenshots of your PPM and App Config Tab please.

Also, can you post a video of you pulling the remote? With no load it may seem that it uses very little throttle range but when you ride it should be fine.
```

---
## \#25 Posted by: thetechtrader Posted at: 2017-07-29T17:05:19.474Z Reads: 72

```
<img src="/uploads/db1493/original/3X/1/4/14f69958ffbdd58d75bcd6946148ad4022ce632b.png" width="690" height="358">
<img src="/uploads/db1493/original/3X/f/7/f7df77dd1d1167f2c1b4b17b2ae699f4b1502716.png" width="690" height="357">
```

---
## \#26 Posted by: JLabs Posted at: 2017-07-29T17:09:24.439Z Reads: 62

```
Download @Ackmaniac’s modded VESC tool. It has an auto wizard for calculating the correct PPM values and a bunch of other stuff. (When not touching the throttle you want the green bar in the middle)

http://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286
```

---
## \#27 Posted by: thetechtrader Posted at: 2017-07-29T17:17:27.455Z Reads: 57

```
Ill check that out. do you think its my controller is the issue or do all controllers with VESC go all or nothing?

I also dont get the RPM's/ERPM I have changed them drastically and tested and motor speed is aways the same in VESC  BLDC tool 34,000 RPM, why do the limitors not work?

Could we do a screen share on skype or something quickly?
```

---
## \#28 Posted by: JLabs Posted at: 2017-07-29T17:33:02.608Z Reads: 56

```
I’m in the car atm so Skype would not be so mobile data friendly. I’m not sure if it’s a controller issue or not but definitely download the other BLDC tool and try that out.
```

---
## \#29 Posted by: pjotr47 Posted at: 2017-07-29T17:35:56.822Z Reads: 49

```
the full or nothing is on the testbench go test it outside with you on the board. Than you go see that it works correct
```

---
## \#30 Posted by: Jinra Posted at: 2017-07-29T17:44:49.227Z Reads: 52

```
The full throttle is because you're using current control. For boat use duty cycle or pid speed control and set max pid erpm to 60k
```

---
## \#31 Posted by: thetechtrader Posted at: 2017-07-29T19:01:30.321Z Reads: 53

```
Thanks, but on those settings the motor starts, then just keep running and there is still now throttle control to vary the speed? not sure why this is being so difficult on me.. lol
```

---
## \#32 Posted by: Jinra Posted at: 2017-07-29T19:03:23.668Z Reads: 52

```
are you using "Duty Cycle no reverse"? If you do it's assuming you're starting from minimum PPM (as if you're throttle was all the way down) meaning neutral on a normal controller will act as 50% speed. You might want to use PID speed control instead.
```

---
## \#33 Posted by: thetechtrader Posted at: 2017-07-29T19:05:54.279Z Reads: 50

```
I tried both. they just start up, then go full out and nothing I do turns the motor off, so I just select a different type of control mode and configure to shut that down.
```

---
## \#34 Posted by: Jinra Posted at: 2017-07-29T19:08:49.495Z Reads: 47

```
so full brake doesn't stop the motor?
```

---
## \#35 Posted by: thetechtrader Posted at: 2017-07-29T19:09:47.632Z Reads: 45

```
no it does not.
```

---
## \#36 Posted by: Jinra Posted at: 2017-07-29T19:10:38.676Z Reads: 46

```
Sounds like something isn't configured correctly then, but for boat I'd definitely say pid/duty is the way to go.
```

---
## \#37 Posted by: thetechtrader Posted at: 2017-07-29T19:17:56.067Z Reads: 48

```
<img src="/uploads/db1493/original/3X/2/7/2701d59bf81240d507c03aeb0c2d3f318640ecca.png" width="690" height="364">
```

---
## \#38 Posted by: Jinra Posted at: 2017-07-29T19:18:46.907Z Reads: 47

```
Looks like you didn't apply your motor detection settings. Make sure to hit "apply" and "write config" after detection.
```

---
## \#39 Posted by: thetechtrader Posted at: 2017-07-29T19:22:34.863Z Reads: 46

```
ok made some changes and it varial speed now.. cool! Thanks we almost have it!

But how to get take off brake so when I push trigger forward it diest not stop DEAD?
```

---
## \#40 Posted by: Jinra Posted at: 2017-07-29T19:28:08.333Z Reads: 45

```
Why would that matter on a boat? Wouldn't it not really affect it anyway? You can try using motor min and battery min at 0A, though not sure if that works.
```

---
## \#41 Posted by: thetechtrader Posted at: 2017-07-29T19:31:14.454Z Reads: 45

```
Well its a mor complicated system with gear reduction drive, if the input RPM are too high it will kill the drive. so Im trying to set the ERPM to 18,000 for my 6 pole motor but it either goes 34,000 or 60,000 on the realtime data window, I cant knock it down to 18,000??
```

---
## \#42 Posted by: Jinra Posted at: 2017-07-29T19:32:26.046Z Reads: 45

```
set the erpm limits here

<img src="/uploads/db1493/original/3X/d/4/d4a8d542333b968ccac1ec7d21730dc9dea2eea2.png" width="690" height="408">
```

---
## \#43 Posted by: thetechtrader Posted at: 2017-07-29T19:44:19.079Z Reads: 43

```
Thanks, 
last question for now :) I really do appreciate all your help here Jinra!

When my motor gets up to the ERPM setting it shuts down and turns off. I then need to put trigger back to start position and pull it again and has full control perfeclty.. but one mat ERP is it the shuts down again?? any ideas?
```

---
## \#44 Posted by: Jinra Posted at: 2017-07-29T20:06:12.725Z Reads: 44

```
Is it hitting the "end" limit? Try making your start limit your goal, and have end eRPM be higher.
```

---
## \#45 Posted by: thetechtrader Posted at: 2017-07-29T23:11:58.037Z Reads: 40

```
Jinra, Your help today has been incredible and I thank you BIG TIME! 

The VESC or Trigger remote are super finicky, I change one thing a little and it does not work, If I was an electronics guy im sure the little changes im doing are likey BIG in the world of electronics.. LOL

Anyways, I seemed to have found a sweet spot there things work, and I have to adjust APP CONFIGURATIONS to make the trigger pickup and max out at certain levels before hitting a target ERPM and then machine shuts off. but I got it.

Only issue now maybe you could shed more light on, is if I touch the trigger a hair, the motor kicks, and stops before ever moving, then it seems it waits a second or two before I can get it to go again with a fresh new trigger pull. can I eliminate this twitch and pause in the motor?
```

---
## \#46 Posted by: DavidBanner Posted at: 2017-07-29T23:18:29.226Z Reads: 42

```
>Keep in mind, this is NOT for a skateboard, rather a type of boat.

@thetechtrader what sort of boat? any chance of photos? I am curious now :)
```

---
## \#47 Posted by: thetechtrader Posted at: 2017-07-31T00:47:50.930Z Reads: 41

```
It is not actually boat, it's a high-performance propulsion system I'm building for my new toy (efoil, jetfoiler, pacificmeister) [**DIY Electric Hydrofoil**](http://www.diy-electric-hydrofoil.com/) board which also has a quick connect/disconnect for easy attachment  of motor and battery systems, so I can have an electric surfboard, and electric hydrofoil SUP for riding different water conditions.

I'm about to start sharing videos of my build every few days as I progress, I almost have everything I need now to hit the water full speed!

<img src="/uploads/db1493/original/3X/4/5/45352871a0494e843df44e0015d49b72df65ed97.JPG" width="666" height="500">

<img src="/uploads/db1493/original/3X/f/b/fbfb98ed38184e1de7a4dbc0f5eff6dda6e6dffe.JPG" width="666" height="500">
```

---
## \#48 Posted by: DavidBanner Posted at: 2017-07-31T09:11:17.462Z Reads: 40

```
very cool project!
```

---
## \#49 Posted by: thetechtrader Posted at: 2017-10-14T12:31:39.065Z Reads: 29

```
Question Regarding low rpm raw torque per rotation.

Two setups, which one would have more turning power at low rpm given same volts?

1: 500kv, 7Y (56104 can)
2. 290kv, 10Y (58122 can)

Anyone have a good article talking about the "Y" in brushless motors?
```

---
