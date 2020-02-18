# GT2B constantly dropping signal and motor detection stopped working after connecting sensor wires \[RESOLVED\]

### Replies: 58 Views: 2220

## \#1 Posted by: FlashNova Posted at: 2016-11-01T17:26:59.621Z Reads: 173

```
I broke my previous GT2B trying to install the Master Cho enclosure (antenna broke off while I was handleing the circuit board). My old GT2B worked perfectly, never had any drop outs, and always rode smoothly, I bought a new GT2B, and it's the exact opposite, constantly dropping signal, and acceleration feels really jerky when i hold down the trigger. Doesn anybody have any idea how to fix this? Or did I just happen to get a faulty GT2B?
```

---
## \#2 Posted by: Pimousse Posted at: 2016-11-01T17:36:33.565Z Reads: 166

```
Hi !
I also broke my antenna mounting the Mad Munkey enclosure from @FLATLINEcustoms.
It's a pain to repair but it's doable ! :slight_smile:

Otherwise, it's the first time I hear about GT2B signal drops ! :neutral_face:
Maybe a faulty one...
Try to add a ferrite ring on the wire between receiver and (V)ESC.
It could help sometimes.
```

---
## \#3 Posted by: mattdig Posted at: 2016-11-01T17:51:10.792Z Reads: 160

```
My GT2B was cutting out, and it was the connector from the ESC into the receiver wiggling around. Add some tape or glue and see if the signal still drops.
```

---
## \#4 Posted by: FlashNova Posted at: 2016-11-01T18:28:49.813Z Reads: 148

```
Now the motor detection doesnt work on any of my vescs. It says bad detection or detection failed. Now i cant figure out if its my vescs that are broken or my motors. All these problems started when i tried to connect my sensor wires. I only did a quick test run with the sensor wires connected, when my GT2B started dropping out, I disconnected my sensor wires to see if that would fix the problem. The motor detection still worked when i disconnected the sensor wires. Now it doesnt work at all with either of my vescs. Does anybody know what is going on with my board? This is so frustrating, ive tried everything to fix it, my board was running perfectly last week. PLEASE HELP!!!
```

---
## \#5 Posted by: JohnnyMeduse Posted at: 2016-11-01T18:34:24.902Z Reads: 142

```
Are you still in sensor or hybrid mode in the bldc, also if the 5v on your sensor motor is short it might have broke the drv or the receiver. Could you take some picture of your sensor wire right at the end of your motor and some of the sensor connector and resistor on the vesc
```

---
## \#6 Posted by: Pimousse Posted at: 2016-11-01T18:58:59.834Z Reads: 141

```
I had some mysterious issues with my VESC. Nothing worked.
I re-flashed the firmware and all came back normally.
Try it, it could fix your problem.
```

---
## \#7 Posted by: FlashNova Posted at: 2016-11-01T19:03:29.678Z Reads: 138

```
I don't know which chip is the DRV, here are some pictures i took.
<img src="/uploads/db1493/original/3X/6/a/6ae8c161eb2d496b23830f32310aaf202ccbab02.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/b/4/b46173b51dc00ddfa56bffef3b0bb0c446fd9bcc.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/3/6/3656aaad0571b6cece59df216244efdcfa1a4da5.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/3/5/350fad93ea20ca853c1a95c8936fe3ed183d4946.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/6/9/69a307764f70fa1e3d59ae8feca540440ba30345.JPG" width="666" height="500">
```

---
## \#8 Posted by: FlashNova Posted at: 2016-11-01T19:07:31.191Z Reads: 130

```
I guess I can give that a shot. Is it hard to do?
```

---
## \#9 Posted by: FlashNova Posted at: 2016-11-01T19:08:15.855Z Reads: 129

```
here is some video of how my board responds after I plug everything back in. The motor spins really slow.

https://youtu.be/YH_YPf7iiq4
```

---
## \#10 Posted by: Pimousse Posted at: 2016-11-01T19:10:18.188Z Reads: 126

```
Not at all, but double-check the firmware version matches to the Hardware version.
There is a tutorial somewhere on the forum I guess.

The behaviour of your motor makes me feel that there is q problem with sensors.
Are you in sensorless mode ?
```

---
## \#11 Posted by: FlashNova Posted at: 2016-11-01T19:11:21.294Z Reads: 126

```
Yes I am back in sensorless mode. And I have disconnected the sensor wires.
```

---
## \#12 Posted by: Pimousse Posted at: 2016-11-01T19:16:35.229Z Reads: 126

```
Ok.
Try reflashing.
DRV seems ok since you can spin the motor.
```

---
## \#13 Posted by: FlashNova Posted at: 2016-11-01T19:20:51.888Z Reads: 121

```
do i need a VESC USB Programmer STLinkv2 like this one to flash the firmware?

diy-electric-skateboard-kits-parts/vesc-usb-programmer-stlinkv2/
```

---
## \#14 Posted by: JohnnyMeduse Posted at: 2016-11-01T19:35:45.941Z Reads: 119

```
I don't think it's a firware issue, I think it's a issue with, the servo cable or the sensor lead. but it look like de 5v short and broke the drv
```

---
## \#15 Posted by: FlashNova Posted at: 2016-11-01T19:37:54.930Z Reads: 118

```
When I type fault in the BLDC terminal i dont return any fault codes. It says FAULT_CODE_NONE

Could it be my motors that are broken?
```

---
## \#16 Posted by: JohnnyMeduse Posted at: 2016-11-01T19:45:02.525Z Reads: 114

```
It' s not because you don't see any faults that there not any problem with the drv. 

But does it work in sensorless mode ?
```

---
## \#17 Posted by: FlashNova Posted at: 2016-11-01T19:50:03.341Z Reads: 116

```
No it doesnt work in sensorless mode. I only ran hybrid mode for a test run, and then switched back to sensorless. Motor detection was working for awhile when I switched back to sensorless, but then for some reason motor detection stopped working all together on both of my VESCs.
```

---
## \#18 Posted by: FlashNova Posted at: 2016-11-01T19:52:28.696Z Reads: 118

```
@torqueboards Hey dude, I bought my motors, VESC's, and sensor wires from you. Any idea what is going on with my board? I just want to know what is broken so I can purchase the correct replacement parts.
```

---
## \#19 Posted by: Pimousse Posted at: 2016-11-01T20:00:38.428Z Reads: 115

```
No, you don't.
You just need the usual USB cable.

Like the FOC/BLDC switch issue, some parameters can stay "ghosts" and create issues on the VESC.
That's why often a reflash solve some troubles (I thought my VESC was died and reflash bringing it back to life ;) )
```

---
## \#20 Posted by: JohnnyMeduse Posted at: 2016-11-01T20:14:43.708Z Reads: 108

```
Well I had a few issue with my old motor and sensor setup, the sensor cable was stretching up and make bad contact or even short with the ground
```

---
## \#21 Posted by: FlashNova Posted at: 2016-11-01T20:22:26.390Z Reads: 101

```
I'm not sure which one is the correct firmware.

<img src="/uploads/db1493/original/3X/4/a/4a98292512af7b44971ec3e232255baefdf0b541.png" width="690" height="233">

Is it the one that says VESC_default.bin

Sorry for all the questions, I cant find a tutorial on here on how to flash the firmware without the STLink.
```

---
## \#22 Posted by: FlashNova Posted at: 2016-11-01T20:44:02.380Z Reads: 93

```
Well I updated the firmware. Motor detection still doesn't work.

I really hope @torqueboards gets back to me, cause I really have no idea what part to replace on my board.
```

---
## \#23 Posted by: Pimousse Posted at: 2016-11-01T20:47:32.860Z Reads: 89

```
Ok. So if it doen't work, I don't know.
I hope you'll find the answer.
```

---
## \#24 Posted by: flatsp0t Posted at: 2016-11-01T20:59:41.370Z Reads: 88

```
What happens if you try to spin your motors from the bldc tool instead of with the remote?
```

---
## \#25 Posted by: FlashNova Posted at: 2016-11-01T21:02:18.637Z Reads: 86

```
The motors spin in both directions when i control them in BLDC tool.
```

---
## \#26 Posted by: flatsp0t Posted at: 2016-11-01T21:23:39.621Z Reads: 85

```
So the problem seems to be somewhere in the remote section.
There might be problems with the binding, coud you try to rebind the remote to the receiver using this guide: http://www.rchobbyspares.com/storepage3216603.aspx
```

---
## \#27 Posted by: FlashNova Posted at: 2016-11-01T21:30:13.154Z Reads: 82

```
I'm not really concerned with the remote issue at the moment, cause right now i cant get the motor detection to work at all, even with the reciever disconnected. If you look at the video I posted, the motors spin really slow when everything is all hooked up
```

---
## \#28 Posted by: flatsp0t Posted at: 2016-11-01T21:31:36.988Z Reads: 81

```
can you give me some screen shots from you bldc-tool config then?
```

---
## \#29 Posted by: JohnnyMeduse Posted at: 2016-11-01T21:45:52.742Z Reads: 82

```
Are your motor wire using the can port or a y servo cable over the receiver
```

---
## \#30 Posted by: FlashNova Posted at: 2016-11-01T21:49:31.072Z Reads: 83

```
@flatsp0t @Pimousse @JohnnyMeduse

Okay, so i have no idea what I did but the motor detection started working again. Maybe it was the firmware flash. I'll  keep you guys updated on my progress. Thank you guys so much for all your help!! Words cannot express how much I appreciate the support.
```

---
## \#31 Posted by: flatsp0t Posted at: 2016-11-01T21:50:55.512Z Reads: 83

```
Nice to hear.
Phantom problems are sometimes the funniest to troubleshoot as nobody knows wtf it is doing^^
```

---
## \#32 Posted by: FlashNova Posted at: 2016-11-01T23:38:23.319Z Reads: 81

```
So good news, just as I was about to give up, I got my vescs and motors working again! But my new GT2B is still dropping signal like crazy. I'm gonna try to rebind the remote to the receiver, or repair my old GT2B if that doesn't work. Worse case scenario I will just buy another GT2B, since they are only $30. That's a lot better than spending $400 on new motors and vescs, I was ready to cry myself to sleep.
```

---
## \#33 Posted by: FlashNova Posted at: 2016-11-02T03:51:54.985Z Reads: 75

```
Okay, so i replaced my new receiver with the receiver from my old GT2B, binded them together, and now everything is back to normal. No more dropouts. Must have been a faulty receiver. What a relief. 

However I'm really scared to reconnect my sensor wires. Not sure it's worth all the trouble. Just happy that my board is working again.
```

---
## \#34 Posted by: flatsp0t Posted at: 2016-11-02T04:41:55.560Z Reads: 73

```
If you do, do backups from all your VESC config(Export XML), so you can revert to that working settings.
```

---
## \#35 Posted by: FlashNova Posted at: 2016-11-02T04:46:37.447Z Reads: 73

```
I'm so glad you bring that up, cause I don't remember my VESC settings cause I set them so long ago. Does this look okay? I'm not sure if I had motor max set to 40a or 60a. I have 50mm motors and 6s battery if that matters.

<img src="/uploads/db1493/original/3X/5/0/5095931a7337b78d7c0314b4a50c9dde7441330c.png" width="690" height="344">
```

---
## \#36 Posted by: flatsp0t Posted at: 2016-11-02T04:52:47.380Z Reads: 70

```
Seems Good. 40 Amps are okay, you need to feel if it fits, as with VESCS and Current control, the max Amps influence the Throttle range.
So, just get a nice Hill, bomb it up, and if there is less torque than expected, up the amps by 5.
Repeat and check motor and VESC Temps(They are allowed to be warm to the touch, but not hot.)
```

---
## \#37 Posted by: FlashNova Posted at: 2016-11-02T04:58:05.309Z Reads: 72

```
Thank you sir! I will give that a shot.

I was checking the TorqueBoards website, and it says max amps is 60 amps. does that mean the highest I can set the motor max to is 60a? or is that for something else?

<img src="/uploads/db1493/original/3X/2/3/23dbc3e2445ee5c7b798cdb60c03ed69c3379589.png" width="601" height="200">
```

---
## \#38 Posted by: flatsp0t Posted at: 2016-11-02T05:00:31.615Z Reads: 68

```
Well, maybe 65, but you will not need that, especially not with a dual setup.
```

---
## \#39 Posted by: Pimousse Posted at: 2016-11-02T05:07:48.392Z Reads: 65

```
It's the worst thing you can do.
Some guys fried their VESC after loading .xml config.
It's better to start from scratch or write parameters by hand on a notepad file or something.
```

---
## \#40 Posted by: flatsp0t Posted at: 2016-11-02T05:10:17.565Z Reads: 65

```
Did they?
Well, maybe i was lucky, i do this every time i tinker with some settings, and never had problems with any of my VESCs.
```

---
## \#41 Posted by: flatsp0t Posted at: 2016-11-02T05:38:14.336Z Reads: 61

```
Do you know if they used it on the same VESCS or to transfer the settings to another?
```

---
## \#42 Posted by: FlashNova Posted at: 2016-11-02T05:41:17.986Z Reads: 60

```
I just connected my sensor wires again, and I can't get them to work. I give up, and moving on with my life. Sensor wires are overrated lol. Definitely not worth the trouble.
```

---
## \#43 Posted by: FlashNova Posted at: 2016-11-02T06:00:04.415Z Reads: 59

```
And motor detection stopped working on one of vescs again. Let's hope I can fix it, again. #NeverAgain
```

---
## \#44 Posted by: FlashNova Posted at: 2016-11-02T07:26:00.637Z Reads: 58

```
And it's fixed, again. f sensor wires.
```

---
## \#45 Posted by: flatsp0t Posted at: 2016-11-02T08:07:40.253Z Reads: 60

```
So, it is time to let the Sensors be Sensors and go on without(nobody really needs sensors tbh).
```

---
## \#46 Posted by: Pimousse Posted at: 2016-11-02T11:02:03.446Z Reads: 57

```
I know a guy who just update the firmware then load xml config file.
2 throttles push and pshiiit...

And others guys on this forum as well, some say the same as me.

@FlashNova : I also trusted in sensors system but I forgave at the first try (I had some troubles like you).
Vedder himself says that it's not worth using sensors on eskate.
```

---
## \#47 Posted by: Bender Posted at: 2016-11-02T12:02:04.285Z Reads: 53

```
If your using the sensor wires the motor phase wires have to be In a specific order when connected to the vesc otherwise it won't function properly and could fry your vesc. I'd ask Dexter at @torqueboards for the correct layout

I love the sensored startup personally :grinning:
```

---
## \#48 Posted by: flatsp0t Posted at: 2016-11-02T12:06:41.443Z Reads: 51

```
Well, i do it only on same hardware and same firmware, maybe this saved me.
I should maybe reconsider using this feature.
```

---
## \#49 Posted by: FlashNova Posted at: 2016-11-02T12:09:11.803Z Reads: 49

```
Well considering how he never responded to me, I'm not sure how much help he would be.
```

---
## \#50 Posted by: flatsp0t Posted at: 2016-11-02T12:10:57.831Z Reads: 52

```
He sometimes seems to only be reachable through the live chat on his page, did you try that?
```

---
## \#51 Posted by: flatsp0t Posted at: 2016-11-02T12:15:26.681Z Reads: 53

```
[quote="Bender, post:47, topic:12265"]
motor phase wires have to be In a specific order
[/quote]

Doesn't this only apply to RC ESCs?
The VESC detects the order they are plugged in and it works in every direction.

That said:
This is the correct behaviour, but we never know, so I would try that anyways.
```

---
## \#52 Posted by: FlashNova Posted at: 2016-11-02T12:18:15.923Z Reads: 51

```
It's all good. I resolved the issue myself and my board works, that's all that matters. Like I said, I'm moving on with my life lol.
```

---
## \#53 Posted by: Bender Posted at: 2016-11-02T12:18:59.293Z Reads: 51

```
@FlashNova  Yes in unsensored mode the vesc auto detects but the sensors need to match up with the corresponding phase that they are monitoring, hence they have to be in the correct order. At least that's my understanding.
```

---
## \#54 Posted by: flatsp0t Posted at: 2016-11-02T12:29:34.073Z Reads: 52

```
@Bender http://vedder.se/forums/viewtopic.php?f=6&t=73#p369
Third part. It should not matter if everything works correctly.

@FlashNova You may be done, but I am a guy that wants to have a problem completely solved, so I will add some thoughts here, sorry for that.
```

---
## \#55 Posted by: Pimousse Posted at: 2016-11-02T12:31:25.722Z Reads: 52

```
Yes, @Bender I experienced this as well !
The Hall sensors table shall match the wiring order.
If you reconnect in a wrong order, the motor try to spin but only stuttering.

Sensors are interesting for stand startup but personally I always give one push thus making sensors useless.
```

---
## \#56 Posted by: FLATLINEcustoms Posted at: 2016-11-02T14:15:55.487Z Reads: 52

```
Always check the antenna where it is soldered to the board. I have opened a few brand new GT2b's in my time and I have had one antenna fall off straight out of the box. Just check to see if it is possible wiggling on the board.
```

---
## \#57 Posted by: Russell23 Posted at: 2017-01-21T22:20:41.624Z Reads: 37

```
I have a problem with my mod, when i turn my gt2b on the green light flashes viciously and only when i charge it it goes back to normal and im able to bind it with the receiver but a couple of minutes later it will go back to fast flashing green light
```

---
## \#58 Posted by: Russell23 Posted at: 2017-01-21T22:21:16.427Z Reads: 35

```
Heres a video of it https://youtu.be/8XANd_NZGDc
```

---
