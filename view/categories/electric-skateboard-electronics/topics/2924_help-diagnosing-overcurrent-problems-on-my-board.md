# Help diagnosing overcurrent problems on my board

### Replies: 45 Views: 4419

## \#1 Posted by: Jinra Posted at: 2016-05-05T17:33:21.774Z Reads: 149

```
Hey everyone, I'm a newbie to RC and e-skates and am having some troubles with the electronics on my Benchwheel C2. It rides great and seems to be built pretty sturdy, but I think the overcurrent protection keeps tripping and turning off the board. Every couple minutes of riding in fast mode the board will shut off with a blinking status light on the board and acceleration does not work, but braking does work.

My question is if this is the BMS tripping and turning it off, or the ESC. If it was the BMS wouldn't that mean there would be no power at all and I wouldn't be able to brake or have the blinking light? Would a higher rated BMS cause any problems in the setup? 

The board has a 6S4P battery @ 22v. 1800w twin motors.
```

---
## \#2 Posted by: barajabali Posted at: 2016-05-05T17:42:08.776Z Reads: 146

```
how much do you weigh
```

---
## \#3 Posted by: Jinra Posted at: 2016-05-05T17:43:17.117Z Reads: 143

```
Woops forgot that bit of info, 175lbs (~80kg)
```

---
## \#4 Posted by: barajabali Posted at: 2016-05-05T17:44:58.676Z Reads: 140

```
http://www.electric-skateboard.builders/t/e-board-for-sale/2495

Check this out.  Might be your weight. As good as they seem to be built.. theyre still cheap Chinese boards. 

Possibly changing the BMS and bypassing those electronics would fix the problem
```

---
## \#5 Posted by: Jinra Posted at: 2016-05-05T18:01:21.463Z Reads: 130

```
Yea I've read that thread and contacted the OP, but he never found out what it was exactly either. I'm 100 pounds lighter than him so I don't think it's directly weight related. I'm just trying to figure out which to replace, the BMS or the ESC.
```

---
## \#6 Posted by: barajabali Posted at: 2016-05-05T18:04:07.446Z Reads: 128

```
do you know how many amps the ESC is rated for? constant and peak and for long peak. 

My guess is the bms tho. I would just bypass it and only use it for charging if you have the tools and know-how to make the operation lol
```

---
## \#7 Posted by: Jinra Posted at: 2016-05-05T18:07:35.760Z Reads: 124

```
Unfortunately I don't know how much is rated for and haven't received word from the company about it yet. Your method is an option though it's ridiculously hard to get to the electronics as the trucks have to be taken off to access the internals.
```

---
## \#8 Posted by: barajabali Posted at: 2016-05-05T18:15:24.006Z Reads: 122

```
Yea i dont know how those things are put together. did it ever work fine for you? 

You could just swap the electronics out for any other esc and try it and see if it works.  seems like youre gonna have to do some work on it
```

---
## \#9 Posted by: Jinra Posted at: 2016-05-05T18:47:35.463Z Reads: 120

```
I just recently got it 2nd hand from someone else and had the problem from the start. The previous owner said he didn't experience any issues, but he lives in Florida and I live in San Francisco, so imagine having a bunch of hills doesn't help the situation.

I may end up trying to solder a new BMS for the pack, any recommendations as to which?
```

---
## \#10 Posted by: barajabali Posted at: 2016-05-05T18:51:04.018Z Reads: 117

```
http://www.batterysupports.com/lion-lipo-nbsp-22v-nbsp-6s-c-32_67.html

you have a choice between 30A 45A or 60A 

to be safe id go with a 60A
```

---
## \#11 Posted by: Jinra Posted at: 2016-05-05T20:53:40.427Z Reads: 109

```
Thanks a lot! Do you think 60A is a high enough limit? Or could I be hitting that as well?
```

---
## \#12 Posted by: barajabali Posted at: 2016-05-05T21:27:54.151Z Reads: 104

```
I think you'll be fine with 60a your normal operating amps shouldn't even be 1/3 of that
```

---
## \#13 Posted by: Jinra Posted at: 2016-05-05T22:28:38.964Z Reads: 103

```
Awesome, thanks a lot. I picked up the 60A BMS you recommended. Hopefully my soldering skills aren't too crap.
```

---
## \#14 Posted by: barajabali Posted at: 2016-05-05T22:43:08.695Z Reads: 98

```
Any time buddy update this thread with progress !
```

---
## \#15 Posted by: Jinra Posted at: 2016-05-06T16:27:16.311Z Reads: 92

```
UPDATE: Opened up my board and a snapped capacitor fell right out. Will try re-soldering on tonight in hopes that was the problem.

<img src="/uploads/db1493/original/2X/7/7422ea8e9cd6333894ad8e0117b933ac2e46d2f1.jpg" width="668" height="500">
<img src="/uploads/db1493/original/2X/d/d15355c52da7ce1ae01f63ca1a40236cb32232b0.jpg" width="668" height="500">
<img src="/uploads/db1493/original/2X/d/d084c75e368ee0e14b0ee2f9c2d7c2fcaf133985.jpg" width="668" height="500">
```

---
## \#16 Posted by: barajabali Posted at: 2016-05-06T17:18:36.794Z Reads: 87

```
Sick! 

20 characters now
```

---
## \#17 Posted by: Jinra Posted at: 2016-05-07T05:16:14.695Z Reads: 85

```
...aaand the capacitor did nothing. I soldered it back on but no change in performance. Still cuts off often with restart needed. Damn.
```

---
## \#18 Posted by: Sk8M8 Posted at: 2016-05-08T01:40:24.502Z Reads: 81

```
Hi! I actually bought the board from the benchwheel from the thread that was mentioned. I am experiencing the same issue, however it doesn't seem to occur on flat ground for me. I also noticed that it seems to get worse as the battery is depleted. I'm also 120 lbs so weight doesn't seem like a huge factor. Let's look into solutions together!
```

---
## \#19 Posted by: Jinra Posted at: 2016-05-08T04:17:14.989Z Reads: 80

```
Hey man, let me know if you're able to find anything. Just FYI the official word I got from Benchwheel is that the "software needs to be updated, and battery needs to be replaced" then told me to "wait until we come to America" which is pretty unhelpful.
```

---
## \#20 Posted by: Sk8M8 Posted at: 2016-05-08T07:36:44.849Z Reads: 80

```
Yeah. I wouldn't expect much help from these Chinese companies, especially because we bought these used. I'm thinking about dropping some cash on dual VESCs, but I want to see if your BMS solution works.
```

---
## \#21 Posted by: Jinra Posted at: 2016-05-08T07:41:56.240Z Reads: 75

```
I actually canceled my order. Examining the circuit boards, it looks like the BMS and ESC are integrated and it wont' be easy (if possible) to use a different BMS on this ESC. I was thinking about using dual VESCs and a BMS in there, but I'd want it to run at 37 volts which won't be possible with the current spacing for the battery. Another option is to buy the Enertion enclosure and forgoing the aluminum enclosure that came with the benchwheel. Another potential issue is the motor not being compatible with a 37v setup.
```

---
## \#22 Posted by: Sk8M8 Posted at: 2016-05-11T05:39:19.236Z Reads: 74

```
Sounds like a pain. I got the board for 300 and I think it's pretty good for getting around town. Maybe I can sell it and buy a better one.
```

---
## \#23 Posted by: Sk8M8 Posted at: 2016-05-12T02:12:58.809Z Reads: 72

```
I'm new to the ESkate world. Is there a specific reason you want a 37v setup? Is there something stopping me from performing these upgrades besides need a new BMS?
```

---
## \#24 Posted by: Jinra Posted at: 2016-05-12T02:48:41.288Z Reads: 72

```
I like 10s (37v) for the lower current draw, meaning less heat on the cables and parts. The benchwheel BMS is integrated on the ESC so you would need to get 2 ESCS (one for each motor) and a BMS for the upgrade. If you use the current battery you can run it at 6s, though if you wanted 10s you'll probably need to mount the battery external or get a new enclosure.
```

---
## \#25 Posted by: Jinra Posted at: 2016-05-15T00:14:36.906Z Reads: 72

```
UPDATE: been playing around with it a bit more and found out that, when I unplug one of the motors, it runs fine whether on fast or slow mode! Still unsure as to what is causing the shutdown when running dual motors, but I'm still guessing it's overcurrent from the dual 1800w motors.
```

---
## \#26 Posted by: barajabali Posted at: 2016-05-15T00:55:01.081Z Reads: 67

```
That's gotta be that both motors pull too many amps together
```

---
## \#27 Posted by: Jinra Posted at: 2016-05-15T02:12:16.104Z Reads: 66

```
Spoke too soon, still cutting off. Though it took a lot longer than before to start doing it.
```

---
## \#28 Posted by: rhinoinflight Posted at: 2016-06-09T06:52:00.102Z Reads: 64

```
If anyone is still following this thread i figured out how to bypass the over current cutout. There are two small wires,  black and white, that come from the battery and into the mother board. Cut the black one and no more resetting. Kind of a pain in the ass to gut the board but it's well worth it. Have pictures of the wires if needed.
```

---
## \#29 Posted by: Jinra Posted at: 2016-06-09T07:06:39.674Z Reads: 63

```
are you talking about the balance wire? There are no other wires that come from the battery other than the positive/negative and balance cables. See picture above
```

---
## \#30 Posted by: rhinoinflight Posted at: 2016-06-10T03:29:51.599Z Reads: 63

```
There should be a ribbon of orange, red, brown, black and white coming from the board the batteries are attached to. Next to those are two wires. Black and white. I assume it's part of the feedback current limiter logic. I just detached the white one and left the black. If you don't see those two wires I'll send you my pics. Yours and mine might be a little different.
```

---
## \#31 Posted by: Jinra Posted at: 2016-06-10T03:41:27.594Z Reads: 59

```
sounds like you're talking about the balance wires, definitely don't want to cut those
```

---
## \#32 Posted by: Sk8M8 Posted at: 2016-06-14T04:09:15.720Z Reads: 59

```
Very much interested in this could you send pictures? I have a malfunctioning Benchwheel as well
```

---
## \#33 Posted by: Ulfberht Posted at: 2016-06-14T04:13:45.048Z Reads: 62

```
@rhinoinflight PIcs please, homie!!
```

---
## \#34 Posted by: whitepony Posted at: 2016-06-14T04:32:34.177Z Reads: 64

```
he probably lost home and board in a mysterious battery fire :sweat_smile:
```

---
## \#35 Posted by: torqueboards Posted at: 2016-06-14T05:28:08.127Z Reads: 61

```
I think your issue is your amps. It's probably pulling 30amps max. Those boards aren't necessarily made to go uphill especially SF hills.
```

---
## \#36 Posted by: Sk8M8 Posted at: 2016-06-15T04:08:32.528Z Reads: 58

```
I found a fix (I think)!
 https://endless-sphere.com/forums/viewtopic.php?f=35&t=80073&p=1180736&hilit=+benchwheel+fix#p1180736

Apparently replacing the fuse fixed it!
```

---
## \#37 Posted by: Jinra Posted at: 2016-06-15T04:54:52.831Z Reads: 57

```
my fuse is intact, so probably not the issue here
```

---
## \#38 Posted by: Sk8M8 Posted at: 2016-06-15T04:56:23.854Z Reads: 56

```
That's unfortunate. Gonna open mine up tomorrow to see if the fuse is alright
```

---
## \#39 Posted by: TapBro Posted at: 2016-07-05T00:34:00.603Z Reads: 54

```
Any luck? I've been following the form as I am having similar issues, any luck?
```

---
## \#40 Posted by: Jinra Posted at: 2016-07-05T00:39:02.111Z Reads: 53

```
I gave up and am parting it out for a new build. The quality of the other parts is actually fairly decent. If you want to give it a go the motors are 280kv 6s 5065 motors.
```

---
## \#41 Posted by: LondonLongboarder Posted at: 2016-07-05T09:38:36.205Z Reads: 48

```
Hey Guys..

I own one of these boards i was having cutting out problems after much time this is what fixed the problem for me.

Remove the cap at the top of the board and pull out the fuse you will probaly see small black burn marks on the fuse you can buy a new fuse ( best option ) or sand of the black marks on the fuse.

The fuse gets burned abit not sure why it kept doing it over and over i then put some sponge under the fuse holder to stop it jiggling/ratling around when riding this... Fixed the problem.. Enjoy
```

---
## \#42 Posted by: TapBro Posted at: 2016-07-06T20:56:46.741Z Reads: 47

```
Thanks @LondonLongboarder, is there a fuse that would fit well, if so, could you send me a link? I really appreciate the help
```

---
## \#43 Posted by: LondonLongboarder Posted at: 2016-07-07T08:55:02.421Z Reads: 45

```
80Amp car fuse any car shop
```

---
## \#44 Posted by: hjhjh99 Posted at: 2016-07-27T18:17:42.609Z Reads: 38

```
I'm planning to buy BenchWheel B2 or C2. Is the disconnection a serious problem? Should I but another electronic skateboard instead?
```

---
## \#45 Posted by: Jinra Posted at: 2016-07-27T18:18:46.471Z Reads: 38

```
I'd avoid it myself. The older batches have the wrong firmware and it causes overcurrent issues all the time. Unless you are 100% sure you have a new batch.
```

---
