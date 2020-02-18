# Can’t pair gt2b

### Replies: 102 Views: 984

## \#1 Posted by: dg798 Posted at: 2018-07-03T13:49:39.655Z Reads: 111

```
So I have a gt2b and this is the procedure I go through for pairing:
Plug ppm cable into vcc on receiver 
Plug bunding plug into bind channel
Power vesc
Hold bond button on remote and turn on and the receiver is solid red.
Power off vesc then remote.
Remove bind plug and then power up vesc and then remote and the receiver is back to blinking red and the remote still blinks green.

Please help
```

---
## \#2 Posted by: FLATLINEcustoms Posted at: 2018-07-03T15:10:11.526Z Reads: 96

```
Is this a stock or modified GT2b?
```

---
## \#3 Posted by: dg798 Posted at: 2018-07-03T15:49:27.357Z Reads: 88

```
Modified 
10 charc
```

---
## \#4 Posted by: clistpdx Posted at: 2018-07-03T16:34:26.721Z Reads: 79

```
In your list of steps you are missing 'plug PPM cable into channel 2 on receiver' before the 'power up vesc' step.
```

---
## \#5 Posted by: dg798 Posted at: 2018-07-03T18:08:26.013Z Reads: 74

```
I’m supposed to plug into vcc or channel 2 on receiver.
```

---
## \#6 Posted by: dg798 Posted at: 2018-07-03T18:14:58.357Z Reads: 74

```
And do I plug into channel 2 after I shut everything off and it’s already binded or instead of first plugging it into vcc
```

---
## \#7 Posted by: Sebike Posted at: 2018-07-03T19:46:30.683Z Reads: 71

```
https://www.electric-skateboard.builders/t/how-to-bind-the-gt2b-receiver-controller-a-step-by-step-guide-4-easy-steps-smile/47074
```

---
## \#8 Posted by: dg798 Posted at: 2018-07-03T20:15:48.133Z Reads: 67

```
Will try tonight and post if works
```

---
## \#9 Posted by: dg798 Posted at: 2018-07-03T21:17:25.882Z Reads: 61

```
didnt work
```

---
## \#10 Posted by: dg798 Posted at: 2018-07-03T21:17:57.906Z Reads: 60

```
doesnt bind when i turn it on again and the green light on the transmitter is still flashing.
it never turns a solid green
```

---
## \#11 Posted by: dg798 Posted at: 2018-07-03T21:20:08.826Z Reads: 55

```
and after the first pair when i turn the vesc back on without the binding plug the receiver blinks red slowly
```

---
## \#12 Posted by: dg798 Posted at: 2018-07-03T21:39:44.801Z Reads: 55

```
would it have something to do with the fact that the stering wheel isnt connected. when i disconnect the throttle the green light stays solid green the whole time.
```

---
## \#13 Posted by: Slak Posted at: 2018-07-04T08:35:15.819Z Reads: 52

```
As it is a modified GT2B, check if the antenna is not unsoldered from the main PCB (can happen if you don't protect the antenna early enough in the mod process, very fragile...). There are pictures of what you have to look for in this thread :

https://www.electric-skateboard.builders/t/gt2b-transmitter-antenna-repair/2790
```

---
## \#14 Posted by: dg798 Posted at: 2018-07-04T12:51:01.876Z Reads: 46

```
ok i will check and post back
```

---
## \#15 Posted by: dg798 Posted at: 2018-07-04T12:53:22.245Z Reads: 45

```
Wow you are a life saver the antenna did pop off. Will fix and post back
```

---
## \#16 Posted by: dg798 Posted at: 2018-07-04T12:56:44.403Z Reads: 45

```
I don’t understand where to put the “core” of the antenna.
```

---
## \#17 Posted by: Slak Posted at: 2018-07-04T15:49:31.771Z Reads: 43

```
Glad to read that !
```

---
## \#18 Posted by: dg798 Posted at: 2018-07-04T16:36:38.034Z Reads: 45

```
![image|375x500](upload://nY8YrVy1wTfy76vjyZEvQVXPMie.jpg)
```

---
## \#19 Posted by: dg798 Posted at: 2018-07-04T16:47:19.364Z Reads: 42

```
Good @Nemesis?
```

---
## \#20 Posted by: Nemesis Posted at: 2018-07-04T17:45:25.568Z Reads: 43

```
The stiff wire covered in clear plastic pointing upwards on the left is your core wire, the one the right is the mesh shield.
![coax|374x475](upload://9yJO5rTFuVrZj2KgHyoE1NPJL4D.PNG)
```

---
## \#21 Posted by: dg798 Posted at: 2018-07-04T18:03:16.956Z Reads: 41

```
So the core goes in the middle and the mesh shield goes on the outer?
```

---
## \#22 Posted by: Nemesis Posted at: 2018-07-04T18:07:34.513Z Reads: 40

```
From what i read on the other GT2B thread yes that's correct.
```

---
## \#23 Posted by: dg798 Posted at: 2018-07-04T18:19:30.489Z Reads: 38

```
Tried and it still didn’t work. Will resolder. Maybe it was a bad solder job
```

---
## \#24 Posted by: dg798 Posted at: 2018-07-04T20:06:49.738Z Reads: 36

```
redid the solder but still doesnt work.
any ideas?
```

---
## \#25 Posted by: dg798 Posted at: 2018-07-04T20:08:59.306Z Reads: 36

```
is the other side of the antenna that only has the shielded wire supposed to go on the other outer contact?
```

---
## \#26 Posted by: Nemesis Posted at: 2018-07-04T21:30:11.999Z Reads: 37

```
No harm in trying both combinations. posting pictures of the GT2B and the area youre working in will help to get answers.
```

---
## \#27 Posted by: dg798 Posted at: 2018-07-04T21:31:29.314Z Reads: 35

```
just did and it still didnt work
```

---
## \#28 Posted by: dg798 Posted at: 2018-07-04T21:33:43.055Z Reads: 39

```
![image|375x500](upload://jgiB1FbK1koWoSBOFUwdmqP8dqO.jpg)
```

---
## \#29 Posted by: dg798 Posted at: 2018-07-04T21:35:01.636Z Reads: 36

```
Can’t really get a good pick of the antenna soldering part
```

---
## \#30 Posted by: dg798 Posted at: 2018-07-04T21:36:49.691Z Reads: 35

```
But the antenna is all soldered up. 
Here’s a video of the problem:
https://www.icloud.com/iclouddrive/0AyGd5mLpztFEsA67hni8OHfw#IMG_0865
```

---
## \#31 Posted by: Nemesis Posted at: 2018-07-04T21:45:09.772Z Reads: 35

```
I cant view the video because :apple: 
Bro im a noob too and really you need pro help.. but this doesn't look correct at the bottom centre!!


![saved23|690x483](upload://yEaO41mbjS578brBrWingY6iAQF.PNG)
```

---
## \#32 Posted by: dg798 Posted at: 2018-07-04T21:45:54.583Z Reads: 34

```
its hard to see but no solder is touching one another
```

---
## \#33 Posted by: dg798 Posted at: 2018-07-04T21:47:23.473Z Reads: 36

```
any pros want to chime in, ie @FLATLINEcustoms @Slak @Sebike
```

---
## \#34 Posted by: Sebike Posted at: 2018-07-04T22:26:50.030Z Reads: 37

```
![antennaGT2B|666x500](upload://i6pcRz1KrhyVdBFmQDg7op9I5CL.jpg)

:unicorn: :balloon: to @whitepony for the pic
```

---
## \#35 Posted by: dg798 Posted at: 2018-07-04T22:37:36.754Z Reads: 36

```
still doesnt pair
```

---
## \#36 Posted by: dg798 Posted at: 2018-07-04T23:28:23.972Z Reads: 36

```
Try watching this video:
https://photos.app.goo.gl/JyUcQXKuWu9Mmmkh9
```

---
## \#37 Posted by: lrdesigns Posted at: 2018-07-05T01:27:58.549Z Reads: 37

```
![image|689x382](upload://1ghcvjPaTeZpjaGt7oujBGwTfWL.jpg)

The antenna is only meant to attach at one end not both. Your antenna looks real messed up now. 

The 30mm clear bit after the brass tube is the top end of the antenna and should not be touching anything.

Edit. Sorry if sounded harsh, trying to help. I will try get a better photo of mine to show you.

![image|666x500](upload://bHijJv95C7snOAXhtjIe6ig0zY3.jpeg)
```

---
## \#38 Posted by: dg798 Posted at: 2018-07-05T01:30:56.367Z Reads: 36

```
yeah i realized that and i fixed it so the top isnt touching anything but it still doenst work
```

---
## \#39 Posted by: dg798 Posted at: 2018-07-05T01:48:56.918Z Reads: 34

```
ok i resoldered it and only the side with 2 wires is attached and the other side is free but it still doesnt pair
```

---
## \#40 Posted by: FLATLINEcustoms Posted at: 2018-07-05T11:13:47.269Z Reads: 33

```
How did your antenna wire get so short?

What are the two bigger red wires going to off to the right in the pic?

can you show me the battery on the other end of the three wire plug?
```

---
## \#41 Posted by: dg798 Posted at: 2018-07-05T11:48:38.486Z Reads: 31

```
I kept on messing up trying to strip the mesh and the shield so it’s now short
```

---
## \#42 Posted by: dg798 Posted at: 2018-07-05T11:50:21.328Z Reads: 31

```
[quote="FLATLINEcustoms, post:40, topic:60801"]
What are the two bigger red wires going to off to the right in the pic?
[/quote]

Charging port wires
```

---
## \#43 Posted by: FLATLINEcustoms Posted at: 2018-07-05T14:55:45.148Z Reads: 32

```
Take a picture of your battery where you soldered and the whole board and the USB charge port.
```

---
## \#44 Posted by: dg798 Posted at: 2018-07-05T21:13:19.190Z Reads: 33

```
![image|375x500](upload://sNymNKmHBmMJXPhfMxtK7Dew6aL.jpg)![image|375x500](upload://3poY1FF0H0G5nj0dMNeaQT708BB.jpg)![image|375x500](upload://49NgO7iJ3NDtVxPjeTcLVvedXS9.jpg)
```

---
## \#45 Posted by: FLATLINEcustoms Posted at: 2018-07-05T21:19:54.756Z Reads: 31

```
The controller turns on and green light flashes?

Chargers fine?

Check your adjustment knobs, maybe the trigger isn't centered?

How did it unbind, don't they come binded?
```

---
## \#46 Posted by: dg798 Posted at: 2018-07-05T21:32:04.731Z Reads: 30

```
yes green light flashes and charges fine and knobs are good.
```

---
## \#47 Posted by: Sebike Posted at: 2018-07-05T21:50:58.068Z Reads: 28

```
Looks to me as if you have soldered the antenna and ground to the wrong pads..
ground looks like it's soldered to the antenna pad, and antenna is soldered to a pad that should be left empty. 

I don't have my own remote here to confirm, but that's what it looks like to me.
```

---
## \#48 Posted by: dg798 Posted at: 2018-07-05T21:51:36.342Z Reads: 26

```
ok will redo and post later although i doubt it will work.
```

---
## \#49 Posted by: Sebike Posted at: 2018-07-05T21:52:50.291Z Reads: 26

```
even if it won't work, at least wires will be back where they belong :sweat_smile:

good luck
```

---
## \#50 Posted by: Sebike Posted at: 2018-07-05T21:56:27.470Z Reads: 27

```
That's my experience as well. If you buy a remote with receiver you don't have to bind as it comes plug n play (at least with flipsky). Only had to bind when I got an additional receiver.
```

---
## \#51 Posted by: dg798 Posted at: 2018-07-05T22:00:12.536Z Reads: 24

```
any other reason why the remote isnt working?
```

---
## \#52 Posted by: Sebike Posted at: 2018-07-05T22:11:45.630Z Reads: 25

```
maybe post pics of your receiver as well with signal cable connected plus binding plug, just to make sure they're in the right spots
```

---
## \#53 Posted by: dg798 Posted at: 2018-07-05T22:13:45.450Z Reads: 25

```
![image|375x500](upload://t2mkiHfmKG7Ecwa2KX4ja8b2ghh.jpg)
```

---
## \#54 Posted by: dg798 Posted at: 2018-07-05T22:19:29.174Z Reads: 24

```
is this good?
```

---
## \#55 Posted by: Sebike Posted at: 2018-07-05T22:21:45.749Z Reads: 24

```
ok. seems fine. let us know when antenna has been resoldered. 

here's another pic that'll help you see where to solder antenna/ground

https://www.electric-skateboard.builders/uploads/db1493/optimized/3X/7/d/7d564983200ca8e9c537c2f0b80afb6cd58c5d18_1_374x500.jpg
```

---
## \#56 Posted by: dg798 Posted at: 2018-07-05T22:23:21.527Z Reads: 21

```
it says switched battery light indicator??
what am i looking for?
```

---
## \#57 Posted by: dg798 Posted at: 2018-07-05T22:32:08.298Z Reads: 22

```
where is the antenna?
```

---
## \#58 Posted by: Sebike Posted at: 2018-07-05T22:33:54.467Z Reads: 24

```
nevermind that text. here's a close up..
![lol|561x444](upload://Ag6bN7dNU3oqt3R4MkvXUrEHlcs.jpg)
```

---
## \#59 Posted by: dg798 Posted at: 2018-07-05T22:34:41.110Z Reads: 23

```
and ground is the mesh shield on the antenna right?
```

---
## \#60 Posted by: Sebike Posted at: 2018-07-05T22:35:28.991Z Reads: 20

```
yah 55 chars
```

---
## \#61 Posted by: dg798 Posted at: 2018-07-05T22:36:15.227Z Reads: 23

```
ok will resolder and try again and repost soon.
thx for the help
```

---
## \#62 Posted by: dg798 Posted at: 2018-07-05T22:54:33.806Z Reads: 21

```
Reaoldered and remote still blinking
```

---
## \#63 Posted by: Sebike Posted at: 2018-07-05T23:03:04.115Z Reads: 23

```
you mean the remote is blinking without you pressing the bind button?
```

---
## \#64 Posted by: dg798 Posted at: 2018-07-05T23:04:13.566Z Reads: 22

```
Right it’s blinking green
```

---
## \#65 Posted by: Sebike Posted at: 2018-07-05T23:04:41.307Z Reads: 22

```
so if you switch it off and switch it back on it's still blinking?
```

---
## \#66 Posted by: dg798 Posted at: 2018-07-05T23:09:23.302Z Reads: 20

```
Yep
10 charc
```

---
## \#67 Posted by: Sebike Posted at: 2018-07-05T23:15:19.735Z Reads: 18

```
and when you switch on the esc + receiver with the binding plug, does the receiver flash red and then turn solid red after remote is switched on (pushing binding button)?
```

---
## \#68 Posted by: dg798 Posted at: 2018-07-05T23:23:47.238Z Reads: 17

```
no the red is always solid its the green that blinks
```

---
## \#69 Posted by: dg798 Posted at: 2018-07-05T23:27:05.350Z Reads: 18

```
the green however becomes solid when the throttle pcb isnt plugged into the main board but still doent bind
```

---
## \#70 Posted by: Sebike Posted at: 2018-07-05T23:31:29.390Z Reads: 18

```
without bind plug .... is it still solid red even with remote switched off?
```

---
## \#71 Posted by: dg798 Posted at: 2018-07-05T23:33:41.367Z Reads: 19

```
when the remote is switched off nothing is on.
when just the remote is on the its solid red and blinking green.
also i thought i may have pushed the failsafe button on the receiver at some point so i pushed it again and now whenever just the receiver is turned on with no binding plug the light on the receiver is solid red forlike 3 seconds then blinks and ETC
```

---
## \#72 Posted by: dg798 Posted at: 2018-07-05T23:37:14.869Z Reads: 20

```
take a look at this:
https://photos.app.goo.gl/JyUcQXKuWu9Mmmkh9
```

---
## \#73 Posted by: Sebike Posted at: 2018-07-05T23:39:17.454Z Reads: 22

```
ok. it''s all a bit messy and confusing now. lol.

 best thing is if you could post a video of everything starting from scratch, nothing connected, then connect receiver, switch on, switch off, then with the binding plug trying to bind aso. 

hard to figure out what's happening and if this is an error on your side or on the remote/receiver.
```

---
## \#74 Posted by: dg798 Posted at: 2018-07-05T23:40:02.538Z Reads: 21

```
take a look at the video i just posted.
thats exactly what it is about
```

---
## \#75 Posted by: dg798 Posted at: 2018-07-05T23:43:35.417Z Reads: 22

```
good?
10 charc
```

---
## \#76 Posted by: Sebike Posted at: 2018-07-05T23:45:57.017Z Reads: 21

```
for some reason it only loads until 37 sec

it looks as if receiver does bind though as it first flashes red and then stops flashing..
```

---
## \#77 Posted by: dg798 Posted at: 2018-07-05T23:47:38.932Z Reads: 20

```
right thats the problem.
```

---
## \#78 Posted by: dg798 Posted at: 2018-07-05T23:48:37.392Z Reads: 18

```
any ideas?
```

---
## \#79 Posted by: Sebike Posted at: 2018-07-05T23:49:55.587Z Reads: 19

```
i don't know whats happening after the first 37 seconds... :smile: and until then everything seems fine.
would be good to see the remote side as well
```

---
## \#80 Posted by: dg798 Posted at: 2018-07-05T23:50:33.391Z Reads: 17

```
ok i will take a new video
```

---
## \#81 Posted by: dg798 Posted at: 2018-07-05T23:56:41.599Z Reads: 16

```
ok i took a new video more in depth and its uploading now
```

---
## \#82 Posted by: Sebike Posted at: 2018-07-05T23:58:50.422Z Reads: 16

```
if you always have a constant flashing on the remote, it sounds as if binding button is constantly pushed in, or there's a short or maybe you accidentally damaged something on the pcb? 

did you try to bind without pushing the binding button on the remote? if that works (ie if receiver led goes from flashing to solid) something's causing the binding on the remote to short out
```

---
## \#83 Posted by: dg798 Posted at: 2018-07-05T23:59:24.451Z Reads: 17

```
i will try to bind without button
```

---
## \#84 Posted by: dg798 Posted at: 2018-07-06T00:00:53.796Z Reads: 17

```
just tried and it binded without pushing the button when the bind key was in but when i took the bind key out it didnt bind again.
```

---
## \#85 Posted by: Sebike Posted at: 2018-07-06T00:04:49.074Z Reads: 18

```
ok.. so for some reason your remote is faulty constantly trying to bind. that sucks. :neutral_face: 
inspect the pcb carefully for any damage and see if there is somewhere you might have caused a short, maybe while soldering that antenna...

GL
```

---
## \#86 Posted by: dg798 Posted at: 2018-07-06T00:05:32.926Z Reads: 18

```
theres nothing i can see.
i guess i will just have to get another one when i get some more money.
```

---
## \#87 Posted by: Sebike Posted at: 2018-07-06T00:06:51.591Z Reads: 19

```
life sucks. :wink:
did you get that 2nd video uploaded yet?
```

---
## \#88 Posted by: dg798 Posted at: 2018-07-06T00:07:51.075Z Reads: 19

```
i am now
10 charc
```

---
## \#89 Posted by: dg798 Posted at: 2018-07-06T00:22:15.302Z Reads: 19

```
https://youtu.be/wa-i3ztIGuo
```

---
## \#90 Posted by: dg798 Posted at: 2018-07-06T00:23:29.896Z Reads: 19

```
its pretty in depth
```

---
## \#91 Posted by: dg798 Posted at: 2018-07-06T00:27:52.118Z Reads: 18

```
good??
10 charc
```

---
## \#92 Posted by: Sebike Posted at: 2018-07-06T00:30:51.895Z Reads: 18

```
Doesn't work. Sais video clip is not available.
```

---
## \#93 Posted by: dg798 Posted at: 2018-07-06T00:32:07.758Z Reads: 18

```
try this one:
https://www.youtube.com/watch?v=wa-i3ztIGuo&feature=youtu.be
```

---
## \#94 Posted by: dg798 Posted at: 2018-07-06T00:36:37.142Z Reads: 17

```
can u watch that one?
```

---
## \#95 Posted by: lrdesigns Posted at: 2018-07-06T00:43:39.505Z Reads: 17

```
nope?
![image|690x440](upload://eVVrtEvna1jWFLJflODgKtqCjct.jpg)
```

---
## \#96 Posted by: dg798 Posted at: 2018-07-06T00:45:48.116Z Reads: 17

```
give me a sec
```

---
## \#97 Posted by: dg798 Posted at: 2018-07-06T00:46:52.963Z Reads: 17

```
https://youtu.be/wa-i3ztIGuo
```

---
## \#98 Posted by: dg798 Posted at: 2018-07-06T00:47:20.281Z Reads: 17

```
the problem was the video was private and now its public so it should work
```

---
## \#99 Posted by: dg798 Posted at: 2018-07-06T00:50:56.977Z Reads: 17

```
can you view it now?
```

---
## \#100 Posted by: dg798 Posted at: 2018-07-06T01:11:49.290Z Reads: 17

```
is it good???
```

---
## \#101 Posted by: Sebike Posted at: 2018-07-06T08:18:49.643Z Reads: 14

```
Video is fine now. Your receiver behaves just the way it should. Slow blinking without bind plug is normal as it waits for the remote and wants to pair.
Remote should not be doing that rapid flashing without binding button being pushed. You said that it wasn't flashing with throttle not connected right? If you leave throttle unplugged and turn receiver on (without binding plug), does the receiver stop flashing?
If so, it is correctly paired and something might be wrong on the throttle side.
```

---
## \#102 Posted by: dg798 Posted at: 2018-07-06T11:49:06.842Z Reads: 13

```
I will try to pair it without the throttle later today and let u know what happens
```

---
