# LifePO4 battery getting drained too quickly

### Replies: 11 Views: 1642

## \#1 Posted by: Chigzy Posted at: 2016-09-09T07:08:05.580Z Reads: 129

```
Hi Guys, Just an introduction of my self before I start. Ok, well I've been lurking these forums for a while now, and my passion for E-boarding started from my Metroboard Stealth. This thing is actually quite good, but now it has been stripped apart due to coming across this Forum and getting hooked lol. I have recently built a board using the below, and I am a little confused on what settings I should use to prevent my battery draining so quickly.

Parts used on Build:

36v LifePO4 8ah battery (This was ripped out from the Metroboard)
6374 Outrunner Motor  from the Metroboard

Globe The Maiden Deck  (Awesome board i tell ya :) )
The good ole VESC from chaka  :)
Enertion Steez remote :)
Caliber 50deg trucks
97mm wheels
17t motor pulley
37t wheel pulley

Ok, so when the battery was in the Metroboard, I used to get around 16-18 miles range   as it was the 20 mile option I bought.

Now I probably dont even get like 6. So Im not sure what to do. I am a newb to this, so I appologize for any stupidity at the moment. I'm hoping someone can help with the below questions. I will be posting pictures soon, but can't at the moment because I don't have internet at home, so this is being written at work   (Shhhhushhhh :)   )

What is the best Low Voltage cut off I can use for LifePO4?
How can I find out the best settings for the battery?
What settings should I use on VESC for the Motor, or how can I find out what KV it is to then work around it.

Like I said, Im sorry for the lack of info but I am a newbbb lol   
Just a side note, Ive enjoyed building this just as much as riding it, its a blast.
```

---
## \#2 Posted by: themegak Posted at: 2016-09-09T16:31:10.003Z Reads: 101

```
I have a metro board battery as well 36volt 5ah LifePo4 Chemistry same as you.  I'm planning on using this for a hub setup but am waiting for CarveOn V3.  In the interim if you search the forum you should be able to find @RunPlayBack vesc settings that he uses with his LifePO4 pack.  I have squirreled those settings away as I believe he has had success for some time using LifePO4 battery packs.  In case you can't find them, below is a snapshot (keep in mind his motor and battery settings are tuned for Carveon hubs motors) of what his settings are (you may want to bring batt max down to 25 - 30 amps and change your motor min motor max settings as per your set up) according to a post he put up on this forum some time ago.  Hopefully he sees this post and can chime in.  Best of luck and do post your current VESC settings as that should help others help you troubleshoot.  Here is the screenshot :   <img src="/uploads/db1493/original/3X/e/d/ed1a22d57f204e2ae5c73f9aa85bd183a65ab5dc.JPG" width="690" height="296">
```

---
## \#3 Posted by: Chigzy Posted at: 2016-09-10T09:59:59.662Z Reads: 82

```
Hi, thanks for the help. These are my settings I have set currently:

<img src="/uploads/db1493/original/3X/6/8/68db5a061d65d30987db32fa7d242eb96b7dddd3.png" width="690" height="373">

<img src="/uploads/db1493/original/3X/8/d/8d4f8d83fa2821ba37c7bf262dda3b5e3dbe4ea7.png" width="690" height="373">

<img src="/uploads/db1493/original/3X/f/e/febb219cd5da287e8a07fa9ff7b8d2c4ddb7c8e0.png" width="690" height="373">

<img src="/uploads/db1493/original/3X/3/9/3938ac057a8565d2e0c54ac4c317cc6be2ff683f.png" width="690" height="373">

Did you copy and paste all of that or is there a way in BLDC i can run a report or something to capture all my settings.
Also, im confused as to why realtime data is not showing my voltage and such. Im sure Im missing sections off the bottom. Have a look and tell me what you think. Thanks aswell, really appreciated.

<img src="/uploads/db1493/original/3X/b/0/b0848c23e4bfb5ab84dfd970eef450bbd6d8b6d5.png" width="690" height="373">


Last but not least, heres the board in testing stage :slight_smile:
 
<img src="/uploads/db1493/original/3X/1/c/1ce66788b845d7a5c9990a5472da48162a22e796.jpg" width="282" height="500"><img src="/uploads/db1493/original/3X/d/b/dbecfbcaafedef0e0649d8d94458c5527e9483b3.jpg" width="689" height="390">

Not gonna lie, I love this deck. Just looks futureristic.

I have a pair of Jacobs Hub Motors, but only have 1 vesc. I tried it on 1 , but it seemed to get too hot, so may have to wait until Ive got a dual vesc in future.
```

---
## \#4 Posted by: Ackmaniac Posted at: 2016-09-10T23:58:34.497Z Reads: 69

```
A couple of things.
First, you have the Vesc Firmware bug. Your Max current ramp step is at 50.000.
By default this is at 0.04. So please correct this and update your firmware or check this every time you write the settings. Otherwise it is very likely that it will damage your vesc.

Second it seems that you haven't done a motor detection. Because the settings seem to be the default settings. So please press start detection in the BLDC tab and then Apply if it was sucessful.

Third, i don't know what kv this motor has but if it has for example 192kv as mine then your 17teeth motor pulley would be far too big. If it is like 150 kv then it would be ok.
```

---
## \#5 Posted by: Chigzy Posted at: 2016-09-11T10:08:54.744Z Reads: 57

```
Ok, so I have done a motor detection and now I have set the Intergrator limit as 185 and BMF coupling to 550. I done a few detections and clicked apply a few times, this is what it sticks around.

Also. Changed the Max current ramp step to 0.40 the default. What does this actually do as I'm new to this. What can I change it to. As in the Max and what would it do in regards to performance. So many settings in the Vesc and I really don't have a clue yet lol 

Thanks for all the input. I've already thought about making a carbon fibre deck lol. Am I jumping ahead of myself :)
```

---
## \#6 Posted by: Jinra Posted at: 2016-09-11T11:07:11.058Z Reads: 53

```
.04 is the default, not .4. Also you'll want to change it to .004 and write since the bug multiplies the value by 10 when you write.

From my understanding the setting controls how fast the current ramps up from load. I'm not sure what the actual numerical value represents though.
```

---
## \#7 Posted by: Ackmaniac Posted at: 2016-09-11T12:25:23.665Z Reads: 50

```
Set it to 0,04. The error happened when the calue was read by the BLDC-Tool. Not when it was written. So when you set it to 0,04 then you vesc will handle it with 0,04.

To be a bit more precise what it means. It is only allowed for the VESC to increase or decrease the current settings by this value for every step. And there are 1000 steps each second (1000 Hz = 1 kHz). 

So to go from 0 to 50 Amps it needs 1250 Steps (50 / 0,04 = 1250 Steps / 1000 per second = 1,25 seconds).
With the wrong settings it would do it in a milli second.  (50 / 50 = 1 Steps / 1000 per second = 0.001 second).
```

---
## \#8 Posted by: Jinra Posted at: 2016-09-11T12:30:18.714Z Reads: 44

```
Thanks for the explanation, but I'm pretty sure the bug happens when it's written given that the big is firmware based and not on bldc tool side.
```

---
## \#9 Posted by: Ackmaniac Posted at: 2016-09-11T12:32:36.804Z Reads: 45

```
Yes it is firmware based. Because you send a request to the firmware to send the BLDC-Tool the actual settings. And there the firmware reads it wrong.

Here you can see the bug fix
https://github.com/vedderb/bldc/commit/fbfc442b432e88825d1c1999cf726256303c81aa
```

---
## \#10 Posted by: Jinra Posted at: 2016-09-11T12:36:01.561Z Reads: 42

```
I'll take your word for it :) Good thing its been fixed, just hope people are updating their firmwares.
```

---
## \#11 Posted by: Chigzy Posted at: 2016-09-11T15:29:04.573Z Reads: 36

```
Thanks for the heads up guys. I noticed it changed by 10 times so I did as you said and set it at 0.004 which then multiplied by ten.

Not sure why but I'm only maxing out at around 18mph, was hoping to hit the 25+ Mark . Should I increase the motor pulley teeth. It has loads of torque at the moment. 

Also, battery seems to just get drained. 36v 8ah. So that's 288kwh. I'm sure I read somewhere that you get around 1km every 10kwh so that's 28 km. Is this right. What range do you think I should get and if I got an Enertion Rspec. Would that be a lot faster
```

---
