# 2 x VESCs over can bus, one motor spinning only sometimes

### Replies: 28 Views: 406

## \#1 Posted by: Pantata Posted at: 2018-09-09T18:43:44.281Z Reads: 82

```
Hey guys, I couldn't find anyone with this problem. One of my motors only spins sometimes... Usually after I start gaining speed usually the second motor kicks in... SOmetimes it doesn't kick in, sometimes it does... Seems once it starts spinning it will keep working unless I stop or slow down to a walk paste. Any help would be much appreciated. I am using the Torque VESCs...
```

---
## \#2 Posted by: L3chef Posted at: 2018-09-09T18:45:23.956Z Reads: 81

```
You have done detection on both motors right?
Are they sensored or sensorless?
Any faults in terminal?
More info would be great. Screen shots of your settings
```

---
## \#3 Posted by: linsus Posted at: 2018-09-09T18:53:30.863Z Reads: 80

```
Hard to evaluate without a video or something but prob diffrent dragforce on the motors. Enable traction control and they should spin evenly.
```

---
## \#4 Posted by: Pantata Posted at: 2018-09-09T18:57:40.460Z Reads: 78

```
HI, thanks for the reply... Well I was having problems with detection on that faulty motor but then it went through... I redone it today to make sure everything is as it should and it went through detection with no problmes, I am using BLDC mode, sensorless. ERPM -+60 000, 2500w (for 2500w motors). I have no faults when streaming real time data. How do you enable traction control? 

![image|690x454](upload://vrqYcXbAbHoHFbRabitnpSxLC5D.png)
```

---
## \#5 Posted by: Pantata Posted at: 2018-09-09T19:03:15.761Z Reads: 66

```
I see the traction control. Is it supposed to be on only for master or slave or both?
```

---
## \#6 Posted by: linsus Posted at: 2018-09-09T19:06:14.667Z Reads: 64

```
Think master is enough, wont hurt to do both tho :slight_smile:
```

---
## \#7 Posted by: Pantata Posted at: 2018-09-09T19:09:54.820Z Reads: 61

```
Ok now the normally working motor stutters and then all of a sudden they both start spinning.. .Obviously for some reason that other motor doesn't want to start spinning right away... But the both work no problem, both vescs work no problem...
```

---
## \#8 Posted by: linsus Posted at: 2018-09-09T19:12:39.666Z Reads: 61

```
are you running hallsensors? Cause if theres too much drag they might be litle upset just starting from standstill. They should both be running without any problem if they are already spinning tho (i.e you got some speed with your foot first), no matter traction control, hall sensored or not
```

---
## \#9 Posted by: Pantata Posted at: 2018-09-09T19:12:52.713Z Reads: 59

```
N sensors, BLDC only sensorless
```

---
## \#10 Posted by: Pantata Posted at: 2018-09-09T19:26:12.233Z Reads: 58

```
OK, I switched the wires and now the before flawlessly working motor won't go through detection (As I had problems with the other motor before) So I can assume my VESC is screwed and get a new one right? Also it happened to me twice today when riding, that even without using power, just pushing that the motor on the weird vesc would start braking all of a sudden... dangerous as hack...
```

---
## \#11 Posted by: Pantata Posted at: 2018-09-09T19:31:56.422Z Reads: 56

```
Thanks for the time guys... sorry to bother, I should have tried that straight away
```

---
## \#12 Posted by: linsus Posted at: 2018-09-09T19:38:03.084Z Reads: 57

```
is it flashing red? then you have something wrong, type "faults" into the terminal in vesctool to see error report
```

---
## \#13 Posted by: Pantata Posted at: 2018-09-09T19:50:37.271Z Reads: 54

```
True I should have looked... I have it on charging in my other room now... But I am going to buy a new VESC, I am not gonna risk my life with it. This is not just some bad setting, that motor randomly starts spinning, it randomly starts braking, it won't go through motor detection most of the time... I am not using that suicidal VESC :)
```

---
## \#14 Posted by: L3chef Posted at: 2018-09-09T19:52:41.451Z Reads: 49

```
What battery do you have? Your battery max is higher than @skunk is
```

---
## \#15 Posted by: Pantata Posted at: 2018-09-09T19:53:07.544Z Reads: 47

```
I have 12s4p samsung 30q 15amps discharge (*4)
```

---
## \#16 Posted by: L3chef Posted at: 2018-09-09T19:53:43.880Z Reads: 44

```
Dual motors. You need to split your max battery in 2.
Same with regen
```

---
## \#17 Posted by: L3chef Posted at: 2018-09-09T19:56:19.567Z Reads: 47

```
[quote="Pantata, post:9, topic:67529"]
BLDC only sensorless
[/quote]

Since there's no sensors. You need to spinn your motors before they will move by remote
```

---
## \#18 Posted by: Pantata Posted at: 2018-09-09T19:56:24.638Z Reads: 44

```
Wow, you are right, how did that go pass me... thanks for the heads up... But still that VESC doesn't even work by itself with the good motor... But thanks for telling me, I would be draining 2 times as much from the battery
```

---
## \#19 Posted by: Pantata Posted at: 2018-09-09T19:57:33.602Z Reads: 44

```
They spin ok with that one VESC, not with the other... As I said it is doing crazy stuff and when I switch motors the other one is scrwewed so it has to be the vesc
```

---
## \#20 Posted by: L3chef Posted at: 2018-09-09T19:57:44.548Z Reads: 43

```
It's more that you will damage your battery with trying to pull more amps than it can handle
```

---
## \#21 Posted by: L3chef Posted at: 2018-09-09T19:59:11.854Z Reads: 42

```
Are you sure you flashed/wrote the detection to the vesc after the detection was done?.
```

---
## \#22 Posted by: Pantata Posted at: 2018-09-09T20:00:03.493Z Reads: 41

```
Yeah I spent 6 hours with it and finally at last managed to get through detection. I have done it like 30 times that night. But that's the thing, just get it through detection was a great pain in the ass... ( ANd I redid it today again)
```

---
## \#23 Posted by: L3chef Posted at: 2018-09-09T20:01:06.918Z Reads: 40

```
Hehe okey. Hmm. Check if you have something called "send status over can" activated on master vesc
```

---
## \#24 Posted by: L3chef Posted at: 2018-09-09T20:02:10.123Z Reads: 39

```
When you say it's a pain. What happen when you try to detect it? Errors or any faults?
```

---
## \#25 Posted by: Pantata Posted at: 2018-09-09T20:02:16.882Z Reads: 38

```
yeah I had that for set for slave, it automatically does these settings when I go through input wizard.
```

---
## \#26 Posted by: Pantata Posted at: 2018-09-09T20:04:10.662Z Reads: 36

```
I haven't looked in the log, I didn't know about it then...  ALways the same error, could not detect or something like that and the VESC just blincks 3 times red...  Since that VESC tried to kill me today several times, I am done with her... Beauty she is but time for a new one... Thank you for your time.
```

---
## \#27 Posted by: Silverline Posted at: 2018-09-09T20:06:11.102Z Reads: 36

```
It could be a bad phase Wire between motor and vesc. Check you bullets and the soldering.
```

---
## \#28 Posted by: L3chef Posted at: 2018-09-09T20:12:12.152Z Reads: 32

```
Could be the drv chip is fryed. Sounds like it. 
If you're willing to try something still. Go into the vesc tool. Try to spinn the faulty motor upp and go tl terminal and type in "fault"
```

---
