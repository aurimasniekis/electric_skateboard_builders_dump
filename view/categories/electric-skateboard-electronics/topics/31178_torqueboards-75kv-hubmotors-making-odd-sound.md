# Torqueboards 75KV hubmotors making odd sound

### Replies: 28 Views: 1360

## \#1 Posted by: UniqueSnowflakeN27 Posted at: 2017-08-21T18:36:39.334Z Reads: 160

```
**Disclaimer: The video showing the problem is pretty loud, beware!**

So I finally got my hubs today! You can find my [build log here.](http://www.electric-skateboard.builders/t/boosted-clone-vanguard-f-3-dual-75kv-hubmotors-90mm-10s4p-25r-foc/30619)

I started off with removing all the screws, cleaning them & then reinstalling them. The front ones got Loctite 242 & the ones facing inwards got some Locitite 272. [Here's quick video of me applying it](https://www.youtube.com/watch?v=U6hS0LvDc24) - not relevant in any way, I just wanted to try out my new camera.

[Here's the relevant video though.](https://www.youtube.com/watch?v=9BMF4sPfRf4) But beware, I upped the sound levels to capture the sound properly!

The first motor sounds great, the second one not so much. Will it be broken in once I start riding or do I need to open it up and check? 

Pinging @BigBoyToys because he's been my God on hubs while I've researched and @NashNZ because he was intersted in hearing about these! 

Any help is much appreciated!

Cheers
```

---
## \#2 Posted by: Jinra Posted at: 2017-08-21T18:39:40.022Z Reads: 150

```
There's something rubbing against something in there, could be a wire or maybe the stator. I'd open it to check it out.
```

---
## \#3 Posted by: UniqueSnowflakeN27 Posted at: 2017-08-21T18:53:36.385Z Reads: 146

```
Removed the urethane, but I can't seem to figure out how to take apart the motor itself. 

Could @torqueboards shime in on how to do that perhaps?
```

---
## \#4 Posted by: torqueboards Posted at: 2017-08-21T19:59:38.557Z Reads: 133

```
You would have to remove the bolts from the back side of the motor and remove the rear plate that sits on a bearing.

You should then have access to the stator I'd be careful since it's a magnet you can easily clip your fingers. Typically, I'd stick a smaller hex tool in the clamp holes and pull it out that way.

You can try adding more oil to the bearings.
```

---
## \#5 Posted by: UniqueSnowflakeN27 Posted at: 2017-08-21T20:08:24.488Z Reads: 127

```
Ok, I think I understand. 

So right now I've got it down to this:

<img src="/uploads/db1493/original/3X/5/1/514790ed252a52672166f4700ee66fa3a883e435.jpg" width="690" height="460">

<img src="/uploads/db1493/original/3X/d/b/dbfdc9267c32e1c09bd2d76d54108392c9232241.jpg" width="690" height="460">

You mean I can just put a hex tool where the grub screw goes and pull it out? Or is the "rear plate" you're talking about that black(darker than the rest) that's sitting around the bearing in the last picture?
```

---
## \#6 Posted by: torqueboards Posted at: 2017-08-21T20:19:23.810Z Reads: 117

```
Take the bearing and rear plate off first. Then hold it by the grub screw with a hex tool and pull out. You'll get access to the stator and magnets. Careful with the fingers :cry:
```

---
## \#8 Posted by: UniqueSnowflakeN27 Posted at: 2017-08-21T21:16:08.415Z Reads: 112

```
I got the rear plate off and found what I think was the problem! A small peck of debris.

Didn't manage to pull it apart any more and figured I'd instead put it together and see if that solved the problem. But now I can't get it to close properly!

The stator just stick to one side of the magnets and makes it impossible to get it aligned with the backplate.

Is there a trick to it?
```

---
## \#9 Posted by: UniqueSnowflakeN27 Posted at: 2017-08-22T00:07:05.862Z Reads: 105

```
Well it seems that the debris was the cause for the rattling/sound that was there earlier. It's now gone. 

But now something else has happened. There's barely any resistance when turning it. [Here's a video of that.](https://www.youtube.com/watch?v=LljTdL-x57M&feature=youtu.be)

The first wheel I'm turning is the one that's good.
```

---
## \#10 Posted by: BigBoyToys Posted at: 2017-08-22T01:06:57.911Z Reads: 96

```
Sorry just saw this thread now. Glad u figured  out what was causing the noise. As far as the reduced resistance while spinning the wheel, thats pretty curious. If two phases are shorted together you'd get increased resistance, but I cant think of anything off the top of mynhead that would reduce it other than you not having the axle nut on that motor torqued to the same spec as the other side.
```

---
## \#11 Posted by: Jinra Posted at: 2017-08-22T01:27:01.063Z Reads: 93

```
Do what @BigBoyToys said and touch two of the phase wires together to see if there's increased resistance. It doesn't look like anything is wrong from the video. You could always hook it up to an ESC to see how it reacts, just don't apply too much throttle unless it's working correctly.
```

---
## \#12 Posted by: torqueboards Posted at: 2017-08-22T02:05:33.240Z Reads: 90

```
@UniqueSnowflakeN27 It's not entirely easy but you need something that fits into the shaft and long enough to not clip your fingers and you need to notch it into the bearing when you align it.
```

---
## \#13 Posted by: UniqueSnowflakeN27 Posted at: 2017-08-22T06:53:19.033Z Reads: 79

```
Thanks for shiming in!

When I short the wires on the defective motor, there's the exact same amount of resistance there is in the good motor when I short that one as well.

It's as if the magnets are just much weaker in that motor, except I can tell they're not since they offer lots of resistance when shorted. 

I removed them both from the trucks but that didn't make any difference.

Not sure how to proceed from here...
```

---
## \#14 Posted by: Namasaki Posted at: 2017-08-23T04:54:33.338Z Reads: 69

```
Frankly I prefer the free roll and quiet sound of the one you took apart.
Maybe take the other one apart and clean it as well so they both have better free roll.
As long as they push the board when you give it throttle and performance has not diminished then 
"Don't Worry, Be Happy"
```

---
## \#15 Posted by: BigBoyToys Posted at: 2017-08-23T05:48:41.418Z Reads: 66

```
Agreed, try by running motor detection.
```

---
## \#16 Posted by: UniqueSnowflakeN27 Posted at: 2017-08-23T09:49:16.673Z Reads: 62

```
Me too! 

But I can't see how me just cleaning of debris/residues of from the backplate helped. I guess the way I put it back together was perhaps a little better than they do on the assembly line, resulting in less friction/pressure on the bearings? 

Still looks the same and fits just as well as the other one.
```

---
## \#17 Posted by: UniqueSnowflakeN27 Posted at: 2017-08-23T09:52:05.020Z Reads: 61

```
I'll have my 10S pack welded together by next week, so we'll see then! 

But I did hook it up to an old RC ESC and it did twitch, as it should, when counting the cells.
```

---
## \#18 Posted by: evoheyax Posted at: 2017-08-23T14:14:54.222Z Reads: 57

```
If I where you, I'd take the motor, plug it to a vesc. Do detection and see what your top erpm is and get the voltage of your battery at that instance. Devide the erpm by 7 (number of pole pairs) and then, by your voltage and you'll have a kv. Both motors should be the same. The pitch of the noise changes with different kv, so maybe, they aren't a true match? It's actually harder with smaller motors like these cause you need between 25-35 turns to get a good kv. Larger motors need less turns.

Also, do an FOC resistance test. That will give some indication usually if theres a short. Both motors should be close. Do it a few times on each as the numbers can bounce around a bit.
```

---
## \#19 Posted by: UniqueSnowflakeN27 Posted at: 2017-08-23T14:17:02.909Z Reads: 56

```
Sounds like an excellent approach! Thank you, I'll do that when I get back.
```

---
## \#20 Posted by: UniqueSnowflakeN27 Posted at: 2017-08-27T16:04:47.962Z Reads: 47

```
So I got both of them hooked up to my old VESC and did a motor detection and then ran them both for a while in BLDC(sensorless). 

[So far so good,](https://www.youtube.com/watch?v=9LbiOh11bhU) it seems. Their pretty quiet too! I'll have to do some more testing, but both seem to function! The one running is the one I had some trouble with earlier. If it turns out that the "faulty" one is just as good as the other one, I'm tempted to open up that one as well just to see if I can make it go as smooth as the "faulty" one :grin: But I'll have to do some more testing(like @evoheyax suggested)  to make sure it has the same torque/speed later when I've got the rest of the board settled.

Thank you @torqueboards, @Namasaki, @BigBoyToys, @Jinra and @evoheyax for all the help!
```

---
## \#21 Posted by: Hummie Posted at: 2017-08-27T16:41:22.402Z Reads: 42

```
Overly compressed bearing maybe.  Bad bearing maybe.
```

---
## \#22 Posted by: UniqueSnowflakeN27 Posted at: 2017-08-27T16:50:46.616Z Reads: 41

```
Perhaps, but it's as if the magnets are stronger in the other one and when I short the cables the resistance is exactly the same.

 I'll do a test run once the board is done, if there's a big difference I'll open up the other one as well.
```

---
## \#23 Posted by: Namasaki Posted at: 2017-08-27T16:51:23.718Z Reads: 42

```
The motor sounds fine for bldc except when your where cogging it.
```

---
## \#24 Posted by: UniqueSnowflakeN27 Posted at: 2017-08-27T16:52:19.855Z Reads: 40

```
My bad, try again!
```

---
## \#25 Posted by: Hummie Posted at: 2017-08-27T16:52:29.404Z Reads: 39

```
Run them on bldc tool full throttle and compare the amp draw
```

---
## \#26 Posted by: UniqueSnowflakeN27 Posted at: 2017-08-27T16:53:31.970Z Reads: 41

```
Can I do that in BLDC tool?
```

---
## \#27 Posted by: Hummie Posted at: 2017-08-27T16:54:55.544Z Reads: 41

```
Do the live sampling. That sampling can show a lot.
```

---
## \#28 Posted by: Namasaki Posted at: 2017-08-27T16:56:42.776Z Reads: 41

```
and make a video when you do it so we can see it as well.:eye::eye:
```

---
## \#29 Posted by: UniqueSnowflakeN27 Posted at: 2017-08-27T17:02:00.666Z Reads: 39

```
That's... too intimate!

Here's some screenshots though. The first one is from the one I opened.

<img src="/uploads/db1493/original/3X/e/1/e1f353aa845b20115ba26170462910cfdf4b5743.png" width="690" height="388">

<img src="/uploads/db1493/original/3X/6/3/63571b91785dfabdcd0d82729921f23b64963cf5.png" width="690" height="388">
```

---
