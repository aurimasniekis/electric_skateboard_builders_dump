# Help! Why is this happening?

### Replies: 36 Views: 880

## \#1 Posted by: Caydenfish Posted at: 2018-06-22T03:47:01.876Z Reads: 226

```
My motor is just twitching, im not sure why!! I will plug it in one way and it will spin but seemingly slow, then ill plug it in again it and will just squeak and twitch... Is this due to bad connections? Reading at 38.7v
```

---
## \#2 Posted by: PatRocks Posted at: 2018-06-22T03:51:55.658Z Reads: 227

```
Nobody knows what you're talking about. USE SEARCH FUNCTION before creating a thread, especially one that provides no useful information for anybody to help you

Edit: I didn't mean to lash out like that, but these kind of posts are frustrating
```

---
## \#3 Posted by: Caydenfish Posted at: 2018-06-22T04:22:59.940Z Reads: 208

```
Sorry, I have looked the subject up, but found nothing describing what is happening with mine. I tried to post a video but I have to convert the file type. Would it be helpful to post that? Or is there a more effective way to search to get the results I need?
```

---
## \#4 Posted by: trancejunkiexxl Posted at: 2018-06-22T04:30:13.338Z Reads: 189

```
hey man, pics of your settings in bldc.. have you tried changing phase cable combination, ppm adjustment?
```

---
## \#5 Posted by: PatRocks Posted at: 2018-06-22T04:31:19.985Z Reads: 178

```
What you would need to include in your post/search to get the help you need is details. Quality in, quality out! What esc, motor, batteries, etc. The more information you provide the more likely you'll find the answer that you're looking for
```

---
## \#6 Posted by: Eboosted Posted at: 2018-06-22T04:45:24.761Z Reads: 171

```
Have you performed motor detection?
```

---
## \#7 Posted by: Caydenfish Posted at: 2018-06-22T05:07:59.391Z Reads: 156

```
Using, Turnigy sk3 6374 192kv, diy electric skateboard VESC, and 5x 2s 5200mah zippy 30c series batteries. Update- I resoltered my vesc leads (to motor) and gained a lot of speed on the motors rpm, but still have the twitching. It is as if it does not have enough power to get the motor going. I will be redoing my motor wires tomorrow. Im guessing it was due to cold soldering joints.
```

---
## \#8 Posted by: Caydenfish Posted at: 2018-06-22T05:08:11.809Z Reads: 149

```
No... what exactly is this?
```

---
## \#9 Posted by: Caydenfish Posted at: 2018-06-22T05:09:04.058Z Reads: 146

```
Ive messed with the cable combination, doesnt seem to do much. I still need to program via BLDC, where can I find ideal setting for certain battery setups?
```

---
## \#10 Posted by: Eboosted Posted at: 2018-06-22T05:13:13.620Z Reads: 135

```
When connecting a new motor you need to follow a
Procedure called motor detection. There are a lot of threads explaining how to do it, do not even think about trying to spin your motor without doing that or you will fry the vesc.
```

---
## \#11 Posted by: Caydenfish Posted at: 2018-06-22T05:15:53.883Z Reads: 133

```
Will do this right now! Thanks for the heads up!
```

---
## \#12 Posted by: PatRocks Posted at: 2018-06-22T05:28:09.986Z Reads: 125

```
What @Eboosted said. In order to avoid destroying your ESC, I would recommend a significant amount of research on proper setup for the vesc programming. Take your time, check and double-check that everything is ready before you start your motor detection. It is very important that all of your data is put in correctly, and that your motor is mounted with nothing attached and can spin freely. I ruined my first FOCBOX in this process because I did not know at the little circlip at the base of the motor shaft was contacting the motor mount. Ran detection, and instantly "drv overcurrent fault " $150 out the window. Live and learn lol
```

---
## \#13 Posted by: Caydenfish Posted at: 2018-06-22T05:31:33.669Z Reads: 122

```
For sure XD. Thanks for the patience. My VESC says v4.12, however BLDC is saying the firmware is "too old", where to I go to update?
```

---
## \#14 Posted by: PatRocks Posted at: 2018-06-22T05:33:44.008Z Reads: 119

```
YouTube!!!

Good luck!
```

---
## \#15 Posted by: Eboosted Posted at: 2018-06-22T05:37:11.856Z Reads: 116

```
These at very basic questions, you need to read the forum more time, I'd suggest you stop doing what you are doing right now and start over when you have no more questions or doubts
```

---
## \#16 Posted by: Acido Posted at: 2018-06-22T05:45:50.025Z Reads: 107

```
does it move normally when you are rolling and press the throttle?
```

---
## \#17 Posted by: Caydenfish Posted at: 2018-06-22T05:59:46.272Z Reads: 108

```
Have not used it under load because I don't want to risk damaging anything, however if I spin it slightly then give it throttle without load it will spin as normal.
```

---
## \#18 Posted by: Acido Posted at: 2018-06-22T06:00:39.498Z Reads: 108

```
and you are running sensorless?

if so thats normal
```

---
## \#19 Posted by: Caydenfish Posted at: 2018-06-22T06:16:49.219Z Reads: 109

```
https://youtu.be/9vbpLJVgN_s
```

---
## \#20 Posted by: Caydenfish Posted at: 2018-06-26T19:49:27.235Z Reads: 89

```
Hey man, I appreciate you being blunt with me, I have stopped everything I am doing and have just been researching a lot, but still am having trouble figuring a few things out. Do you have any good links to videos/pages that explain a pretty much step by step? My main issue is that all the videos I have seen have been on the BLDC tool, which supports firmware 2.17 and 2.18 (at least the versions I have found). My VESC is saying it has firmware 3.38 on thr VESC tool? Apparently the VESC has a bootloader, but when I try to upload the "VESC_default" file, I get a buffer erase timeout. At this point I am pretty stuck.
```

---
## \#21 Posted by: Eboosted Posted at: 2018-06-26T19:53:28.985Z Reads: 87

```
Of course. 

Please tell me:

what vesc do you have
Are you runing sensor less or sensores motors? 

Get this version of firmware and ESC tool software:

http://www.electric-skateboard.builders/t/extended-ackmaniac-esc-tool-based-on-vesc-tool/35116

On the link you will find the software, when you connect to the vesc via USB to your computer go to firmware and upload the c I rresoi fing firmware, they are built in the software
```

---
## \#22 Posted by: Benjamin899 Posted at: 2018-06-26T20:03:34.774Z Reads: 78

```
This is normal behaviour for a motor starting from standstill going full throttle without sensors.
```

---
## \#23 Posted by: briman05 Posted at: 2018-06-26T20:05:31.631Z Reads: 77

```
[Watch this video](https://www.youtube.com/watch?v=5HLZaMcYRuY)

The firmware that you now have on your vesc is for the vesc tool.  Which is basically the bldc tool but with alot more features.
```

---
## \#24 Posted by: Caydenfish Posted at: 2018-06-26T20:07:59.115Z Reads: 77

```
I am used a Torqueboards VESC 4.12, and a Turnigy Sk3 6374 sensorless.
```

---
## \#25 Posted by: Caydenfish Posted at: 2018-06-26T20:12:42.086Z Reads: 77

```
I understand that since the motor is sensorless it causes for unsmooth startups, but the issue it is never reaches full speed
```

---
## \#26 Posted by: Benjamin899 Posted at: 2018-06-26T20:17:46.704Z Reads: 76

```
at no point did you mention speed beeing an issue. So what is your real question then?
```

---
## \#27 Posted by: Eboosted Posted at: 2018-06-26T22:48:48.539Z Reads: 69

```
Did you download the ESC from the link I gave you?, did you write the corresponding firmware?
```

---
## \#28 Posted by: Caydenfish Posted at: 2018-06-26T23:06:30.358Z Reads: 65

```
Trying it right now, I have the program open, but when I navigate to the firmware tab I don't see the file you mentioned. Under hardware version I see "410 & 411 & 412", but only see the VESC_Default firmware. I also tried to show non-default options and didn't see it.
```

---
## \#29 Posted by: briman05 Posted at: 2018-06-27T00:20:12.664Z Reads: 63

```
Flash the firmware to the 4.12 default firmware.
```

---
## \#30 Posted by: Eboosted Posted at: 2018-06-27T00:35:07.409Z Reads: 61

```
Correct, flash 4.12.
```

---
## \#31 Posted by: Caydenfish Posted at: 2018-06-27T05:19:45.310Z Reads: 54

```
Alright, Unfortunately I am getting three blinking red lights from the VESC with any movement of my throttle, which I understand based on my reading means that the DRV chip is done for do to my lack of knowledge of doing motor detection prior to spinning the motor up. So unless I hear otherwise I will most likely be getting a new VESC. Do you all think it is possible that this could also be the cause of the twitching in the motor? Thanks so much for you help though!! I think I will get a FOCBOX to run FOC mode through the BDLC tool.
```

---
## \#32 Posted by: telnoi Posted at: 2018-06-27T06:05:35.452Z Reads: 50

```
[quote="Caydenfish, post:31, topic:59695"]
Do you all think it is possible that this could also be the cause of the twitching in the motor?
[/quote]

No...has already been explained by Benjamin. If you read things like ''smooth sensorless startup'' in marketing text, it's just that..marketing.

Read up on things like:

* Sensored.
* Sensorless
* BLDC
* FOC (and why you should NOT use it with torqueboards VESC)
* Motor max/min, bat max/min

The VESC-Tool is almost self-explanatory except for some of the terminology mentioned above. Steps to be taken:

1. Upgrade firmware.
2. Motor setup wizard.
3. Input setup wizard.
4. Adjust safety features (read up on failsafe!)

Any other order will result in your board misbehaving, not performing according to standards, the board killing you,  you killing the board, a car killing you, your board shooting off into the distance without you on it, brakes not working or working poorly, your power supply blowing up or shortening the life span, etc.

There is no plug & play.
```

---
## \#33 Posted by: Caydenfish Posted at: 2018-06-27T06:21:01.188Z Reads: 44

```
Okay, I mentioned that I would get a FOCBOX, I assume based on the name that FOC mode is good to go with this VESC? XD
```

---
## \#34 Posted by: briman05 Posted at: 2018-06-27T13:04:49.041Z Reads: 37

```
I am currently running dual focbox running in sensored foc mode.  If you get a focbox you will still need to update the firmware if you are going to use the vesc tool software.  Are you running this on windows or Mac?  Before you start messing around with any vesc watch the video I had posted the link to as well as this one https://www.youtube.com/watch?v=1N024tVWpmg  They are pretty good over views of how to set up the vesc.  I did a lot of research before I even attempted to do the vesc set up.  I had some issues but where more on sensor detection but since you are running sensorless you wont have them.  Sensorless you will need to do a push start to get your board going once it is configured and under load.
```

---
## \#35 Posted by: rey8801 Posted at: 2018-06-27T13:12:10.241Z Reads: 37

```
Also in this video is really simple explained https://www.youtube.com/watch?v=v1glLDO-EjA&t=1128s. Of course you need to do it only once since you are running single drive
```

---
## \#36 Posted by: Caydenfish Posted at: 2018-06-27T19:57:16.705Z Reads: 25

```
Cool thanks for the info! Also I am using windows.
```

---
