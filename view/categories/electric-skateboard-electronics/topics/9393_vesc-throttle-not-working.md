# VESC throttle not working

### Replies: 61 Views: 2773

## \#1 Posted by: michaeld33 Posted at: 2016-09-11T15:35:20.155Z Reads: 143

```
So I'm having an issue setting up my VESC, where starting up the throttle (just ever so slightly) will make the motors go full speed and pulling the throttle, even more, will just result in no speed change. I have added a video with the issues. Does anyone know why this is happening? I believe I already did the throttle range calibration, at least the display reads the throttle correctly, but it's not functioning properly.

http://www.youtube.com/watch?v=bn4r2Zi_jSE
```

---
## \#2 Posted by: JohnnyMeduse Posted at: 2016-09-11T15:43:44.219Z Reads: 138

```
With no load, you won't be able to see any speed change... The rpm will go at their max in a instant... Also to protect your vesc put the max erpm at 70000 max
```

---
## \#3 Posted by: Blasto Posted at: 2016-09-11T15:53:14.040Z Reads: 136

```
No issue there, in current control, you will ramp the current from 0A to your motor max.

But with no load, you motor will hit it's max rpm at 5-6A (could even be lower)

Put a load on in it, whole different story.
```

---
## \#4 Posted by: Ackmaniac Posted at: 2016-09-11T16:49:09.170Z Reads: 127

```
But the motor steps in to hard. please make a Screenshot of your PPM settings. I think we can find the issue there. Just set it in the PPM window to disabled and then switch on the Display checkbox. Then you should see that the value changes with the throttle. Once that is working and adjusted correctly you can switch it back on and have fun.
```

---
## \#5 Posted by: Blasto Posted at: 2016-09-11T17:11:40.297Z Reads: 121

```
With no load it would propably take 5-10% throttle to hit the max rpm.

But yes, calibrate your ppm setting like @Ackmaniac suggested
```

---
## \#6 Posted by: michaeld33 Posted at: 2016-09-11T20:11:37.992Z Reads: 112

```
Yeah, I calibrated my PPM settings... Is that the same as the throttle range calibration? Anyway, I put a load on it (both standing on it and putting it on the ground without standing on it)
I took a couple videos which I linked below.
When it was just on the ground, it moved, but it still went full throttle after a bit of "jiggling"
When I stood on it, it would not move, instead, the motors just moved back and forth very quickly (ie - jiggling) it was kind of moving/rolling backwards though?
I'm not sure.
Any ideas?


https://youtu.be/hAseQ--MqtE


https://youtu.be/uzgtJS5QQ8c


https://youtu.be/6jQ9AIYLx4A
```

---
## \#7 Posted by: JohnnyMeduse Posted at: 2016-09-11T20:21:36.540Z Reads: 99

```
can you post a screen shoot of your parameter ? I think you might need a little push to make this board move (you should test it outside, a try to take on more speed)
```

---
## \#8 Posted by: Blasto Posted at: 2016-09-11T20:32:25.293Z Reads: 103

```
Give your hubs a chance, just a push start is all you need.

You can also slightly increase your startup boost in the advanced tab
```

---
## \#9 Posted by: michaeld33 Posted at: 2016-09-11T20:35:18.630Z Reads: 102

```
I believe the start-up boost is 0.09
^^ but that's only on one VESC
```

---
## \#10 Posted by: JohnnyMeduse Posted at: 2016-09-11T20:40:59.143Z Reads: 102

```
Is the traction control enable ?
```

---
## \#11 Posted by: michaeld33 Posted at: 2016-09-11T20:41:45.853Z Reads: 96

```
VESC is not over CAN. Y servo connector
```

---
## \#12 Posted by: JohnnyMeduse Posted at: 2016-09-11T20:49:03.666Z Reads: 92

```
Can you post screenshot of your parameter ?
```

---
## \#13 Posted by: cmatson Posted at: 2016-09-11T21:14:58.321Z Reads: 89

```
hubs definitely won't start from a stop, especially on what looks like carpet. 

on my dual hummie board I literally cannot move if the board doesn't have a push.. and that's 10s 40amps a piece to the two hubz.
```

---
## \#14 Posted by: michaeld33 Posted at: 2016-09-11T21:16:00.164Z Reads: 90

```
hmm, yeah I tested it on the street just now... much better
```

---
## \#15 Posted by: michaeld33 Posted at: 2016-09-11T21:56:57.360Z Reads: 91

```
<img src="/uploads/db1493/original/3X/1/0/10b2e07d2684edcf0536764564b039a6346fe96b.png" width="690" height="431"><img src="/uploads/db1493/original/3X/0/e/0e2f52f0dbde89af48bc3007935f46d4f1a1cf74.png" width="690" height="431"><img src="/uploads/db1493/original/3X/e/b/eb9be04ae40166887a12d60a467a24f83ccd122a.png" width="690" height="431"><img src="/uploads/db1493/original/3X/c/9/c910acb14e6b429a79dd1890205b8d46712164fe.png" width="690" height="431"><img src="/uploads/db1493/original/3X/c/8/c80fb2c3524c37378e90ad9c046fc83faf571736.png" width="690" height="431"><img src="/uploads/db1493/original/3X/3/0/30f1b8a0cdb56fe36ba501d783d5bffa32c60070.png" width="690" height="431">
```

---
## \#16 Posted by: JohnnyMeduse Posted at: 2016-09-11T21:58:39.414Z Reads: 79

```
Is your firmware 2.16 ?
```

---
## \#17 Posted by: michaeld33 Posted at: 2016-09-11T21:59:12.497Z Reads: 82

```
My VESC is 4.12
```

---
## \#18 Posted by: JohnnyMeduse Posted at: 2016-09-11T22:01:04.024Z Reads: 82

```
Firmware... Not hardware... Or What is your BLDC tool Version?
```

---
## \#19 Posted by: michaeld33 Posted at: 2016-09-11T22:02:16.735Z Reads: 83

```
Not sure... BLDC tool was just downloaded like 2 days ago from Jacobs site.
```

---
## \#20 Posted by: JohnnyMeduse Posted at: 2016-09-11T22:05:41.243Z Reads: 85

```
OK... It weird because the MAX CURRENT RAMP STEP is suppose to be at 0.0400 in the 2.18 default parameter. But in the 2.16 Firmware it is at 50.... 

Can you go in the Firmware part of the BLDC tool and make a read.
```

---
## \#21 Posted by: michaeld33 Posted at: 2016-09-11T22:07:53.414Z Reads: 86

```
I will in a second, but the supported versions are 2.17 or 2.18
```

---
## \#22 Posted by: Ackmaniac Posted at: 2016-09-11T22:15:40.076Z Reads: 83

```
You need to update your firmware. That is a known bug which can kill your VESC. After the update make sure that the MAX CURRENT RAMP STEP is at 0.0400. And then write the values and read it again. Make sure that the value is still at 0.0400 after the read and not at 0.4000

And then reduce the startup boost and set it to 0.000 in the BLDC advanced screen and give it a try.

And if everything still doesn't help then please make a video of the PPM Screen while you have the Display checkbox enabled. When you start to pull the trigger you should see that the % inreases and when the trigger is pulled fully then it should be at 100 %. If you pull it half it should be at 75 % and when you relese it it should be at 50%. If that's not the case then adjust the values for minimum and maximum until it fits.
```

---
## \#23 Posted by: michaeld33 Posted at: 2016-09-11T22:17:46.446Z Reads: 82

```
Sorry, but where is the MAX CURRENT RAMP STEP? In which tab?
```

---
## \#24 Posted by: JohnnyMeduse Posted at: 2016-09-11T22:18:41.281Z Reads: 80

```
TAB motor configuration and advance
```

---
## \#25 Posted by: JohnnyMeduse Posted at: 2016-09-11T22:20:40.761Z Reads: 76

```
but don't write down 0.04000... without knowing witch firmware you have... or juste in case you can re-flash the firmware usine the file: VESC_default.bin... in the folder for the hardware 4_10 4_12
```

---
## \#26 Posted by: michaeld33 Posted at: 2016-09-11T22:38:18.203Z Reads: 72

```
Firmware is 2.18
```

---
## \#27 Posted by: michaeld33 Posted at: 2016-09-11T22:39:10.159Z Reads: 71

```
So for 2.18 it needs to be 0.04?
```

---
## \#28 Posted by: JohnnyMeduse Posted at: 2016-09-11T22:41:51.040Z Reads: 70

```
yes so maybe try to reprogram your vesc
```

---
## \#29 Posted by: michaeld33 Posted at: 2016-09-11T22:42:25.445Z Reads: 68

```
Do I need to reprogram it or just set it to 0.04?
```

---
## \#30 Posted by: JohnnyMeduse Posted at: 2016-09-11T22:44:47.872Z Reads: 69

```
Try to reprogram it first, to see what it does... (I will do the same on my side just to be sure)
```

---
## \#31 Posted by: michaeld33 Posted at: 2016-09-11T22:45:18.319Z Reads: 67

```
Ok, when I tried to set it to 0.04 it wouldn't let me, kept going to 0.4
```

---
## \#32 Posted by: JohnnyMeduse Posted at: 2016-09-11T22:46:11.936Z Reads: 63

```
set it to 0.004
```

---
## \#33 Posted by: JohnnyMeduse Posted at: 2016-09-11T22:53:44.760Z Reads: 63

```
[quote="michaeld33, post:31, topic:9393, full:true"]
Ok, when I tried to set it to 0.04 it wouldn't let me, kept going to 0.4
[/quote]


it sound like the same problem people got with the early release of the firmware 2.18 and by setting it to 0.004 it will go to 0.04
```

---
## \#34 Posted by: michaeld33 Posted at: 2016-09-11T22:59:51.274Z Reads: 64

```
Ok. Got it.
```

---
## \#35 Posted by: michaeld33 Posted at: 2016-09-11T23:01:28.425Z Reads: 62

```
Alright, yeah that was it, its now at 0.04.
```

---
## \#36 Posted by: michaeld33 Posted at: 2016-09-11T23:07:14.646Z Reads: 62

```
Alright, so I switched it... and nothing's different. It feels the exact same, and the same issue is still there, although the board moves me once I push, I still have the same issue where most of the throttle isn't used, as in 75% throttle is the same as 100%
```

---
## \#37 Posted by: cmatson Posted at: 2016-09-11T23:13:34.551Z Reads: 65

```
I have that throttle issue too, but it is common. 

This is because the vesc determines throttle by amps, not rpm.

So if you only need 10 amps to go max speed, but you set your vesc to a max of 30 amps, than it can get up to speed at 1/3 throttle. Likewise if you set a bunch of amps and punch it, the board will accelerate crazy fast and then flatten out really quickly at a lower throttle position.

On my hummie board with 40 amps 10s per motor, I can slam the throttle right to 1/2 and get up to full speed in a few seconds. Then, the second 1/2 of the throttle does nothing
```

---
## \#38 Posted by: michaeld33 Posted at: 2016-09-11T23:15:14.389Z Reads: 66

```
Hmm interesting, I figured there must be some kind of issue though, because when I go to calculate the speed, it should have a theoretical max of 30mph with a weighted of around 24. (but I'm really light so it should be around 27/28)

When I was riding, at top speed it was more like 12mph
```

---
## \#39 Posted by: Ackmaniac Posted at: 2016-09-11T23:15:23.219Z Reads: 69

```
Then check the ppm settings. Connect to the vesc in the BLDC-Tool. Go to the PPM tab. Switch on the Display Checkbox. When you release the throttle then it should be at 50%. When you pull it half it should be at 75%, when you pull it full then it should be at 100%. If that is not the case then adjust it with the minimum pulsewidth and maximum pulsewith values. 

<img src="/uploads/db1493/original/3X/0/1/01ad2ff4851c6c33b3282e829044020a7e4d6abb.jpg" width="690" height="418">
```

---
## \#40 Posted by: michaeld33 Posted at: 2016-09-11T23:16:34.623Z Reads: 66

```
Yep, everything is right, when released at 50%, when pulled at 100%, and in the middle is 75%...
```

---
## \#41 Posted by: Ackmaniac Posted at: 2016-09-11T23:17:18.412Z Reads: 64

```
And also set your startup boost in the advanced motor configation tab to 0. Actually it is at 0.090.
```

---
## \#42 Posted by: michaeld33 Posted at: 2016-09-11T23:18:21.684Z Reads: 61

```
Really 0? Doesn't that assist the motors when throttle is applied, so that it doesn't jitter?
```

---
## \#43 Posted by: Ackmaniac Posted at: 2016-09-11T23:20:30.292Z Reads: 62

```
Try it, And it seems that you have 2 vescs. Is the receiver connected to the vesc which drives the motor with that you test.

Another question. Do you want to run 2 motors later on or only one. Because if you want to run 2 then set the Motor max current to 30 and the battery max current to 20. (Only half when you use 2)
```

---
## \#44 Posted by: michaeld33 Posted at: 2016-09-11T23:23:10.144Z Reads: 63

```
Both VESCs receive the signal from the controller receiver, no CAN. And yea, I plan on using dual hubs later on unless I hate it, in which case I'll go single VESC with a belt driven motor. I will correct the motor max and battery current. :slight_smile:
```

---
## \#45 Posted by: Ackmaniac Posted at: 2016-09-11T23:25:38.655Z Reads: 62

```
First of all unplug the receiver cable of the second vesc and try only with one. If that works then you can connect the 2 VESC via CAN so that only one vesc receives the signal.
```

---
## \#46 Posted by: michaeld33 Posted at: 2016-09-11T23:26:45.504Z Reads: 58

```
Tried it with one yesterday. Doesn't seem any different... Should I still do it with a load?
```

---
## \#47 Posted by: Ackmaniac Posted at: 2016-09-11T23:29:13.101Z Reads: 53

```
So you also disconnected one vesc from the receiver and set Motor max curent to 30 and batterie max to 20?
When the answer is yes then give it a go.
```

---
## \#48 Posted by: michaeld33 Posted at: 2016-09-11T23:29:59.544Z Reads: 56

```
No, I had just tested it as one VESC, will set to 30a motor max and 20a battery max
```

---
## \#49 Posted by: Ackmaniac Posted at: 2016-09-11T23:32:17.799Z Reads: 56

```
And don't forget the startup boost.
```

---
## \#50 Posted by: michaeld33 Posted at: 2016-09-11T23:46:54.407Z Reads: 54

```
With just one motors it's got virtually no power, with two motors it's the same as before.
```

---
## \#51 Posted by: JohnnyMeduse Posted at: 2016-09-11T23:55:18.547Z Reads: 51

```
what kind of battery are you using?
```

---
## \#52 Posted by: michaeld33 Posted at: 2016-09-11T23:56:31.917Z Reads: 55

```
10S3P li-ion custom pack. But it's not charged so it's at 3.4V right now.
```

---
## \#53 Posted by: Ackmaniac Posted at: 2016-09-11T23:57:00.841Z Reads: 55

```
Did you apply the settings to both Vesc's. Otherwise it seems to be a problem with the spillted receiver cable. Test both Vescs individually with the 30A motor and 20 A Battery. They should both react the same when they run individually. Then connect them again. When they go creazy again then it is the splitted receiver cable. This can be solved with a CAN cable.

BTW, the PPM settings also have to be adjusted at both vesc's.
```

---
## \#54 Posted by: JohnnyMeduse Posted at: 2016-09-11T23:59:08.657Z Reads: 56

```
you are near the cutoff voltage of the VESC, so maybe try charging your battery before... to eliminate this possibility
```

---
## \#55 Posted by: michaeld33 Posted at: 2016-09-11T23:59:12.829Z Reads: 58

```
I adjusted on both. May have to do with the receiver, but I'm not sure... The motors react the same if just one is running or two is running. But with on, it doesn't push me as well since it's much less torque.
```

---
## \#56 Posted by: michaeld33 Posted at: 2016-09-12T00:01:05.729Z Reads: 57

```
I need to hook up BMS and get the charger first. I know, bad idea.
```

---
## \#57 Posted by: JohnnyMeduse Posted at: 2016-09-12T00:05:12.331Z Reads: 60

```
Well, you can still push your battery, but because cutoff setting on the VESC is at 33, when you put load it can draw enough current to pull down the voltage under 33V so you will lost all power from the VESC
```

---
## \#58 Posted by: michaeld33 Posted at: 2016-09-14T01:01:25.383Z Reads: 60

```
Is there a way to adjust the throttle more accurately? I don't want half my remote to be useless
```

---
## \#59 Posted by: Ackmaniac Posted at: 2016-09-14T05:08:08.441Z Reads: 57

```
Try lowering the deadband in the ppm settings. That reduces or increases the offset. Did you manage to get your motors running correctly. Just curious what the issue was.
```

---
## \#60 Posted by: michaeld33 Posted at: 2016-09-14T12:02:44.307Z Reads: 54

```
It has some speed "range" now, but due to the small throttle it's really hard to tell, also, it's speed is much less than it feels like it should be.
```

---
## \#61 Posted by: cmatson Posted at: 2016-09-14T16:00:28.583Z Reads: 53

```
It's all about balancing rider weight, motor max, and max amps. If you get them tuned right, you'll have softer acceleration, but I fully utilized throttle range. 

If you boost the amps for example the throttle range will be smaller, but your board can also physically accelerate faster. 

Settings for me (60kg) wouldn't be so hot for my someone who is 100kg. The board would probably feel slow and sluggish
```

---
