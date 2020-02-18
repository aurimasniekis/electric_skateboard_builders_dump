# Unity fatal issue, will get stuck in full throttle without the remote even being turned on, BE CAREFUL!

### Replies: 28 Views: 1178

## \#1 Posted by: never4getf150forums Posted at: 2019-10-13T22:33:57.515Z Reads: 317

```
this happened on @ARetardedPillow  custom cgt build, the damn board was on for about 20 seconds and then as I was about to start heading my way to the local park for a  test spin the thing just took off with the remote being OFF the whole time.

the best thing was I even managed to capture the moments on video..

so glad it went under a car that was parked and not one that was moving, cause otherwise good bye 2,000$ :frowning:

here is the video [of the full throttle on the latest FW](https://streamable.com/oncp7)
```

---
## \#2 Posted by: AlanZhou Posted at: 2019-10-13T22:40:34.285Z Reads: 309

```
https://forum./t/issue-with-unity-and-metr-at-module-while-logging-data/10021

Similar issue?
```

---
## \#3 Posted by: ARetardedPillow Posted at: 2019-10-13T22:50:11.915Z Reads: 303

```
Same issue
```

---
## \#4 Posted by: Flasher Posted at: 2019-10-14T01:49:03.214Z Reads: 289

```
Jeff is working a patch to immediately fix this. The metr must not be logging until he does. I'd suggest unplugging the metr while you wait if you want to continue riding.
```

---
## \#5 Posted by: Blitz Posted at: 2019-10-14T10:31:32.223Z Reads: 273

```
I was worried bt modules could do that.

But maybe it's the unity's fault or maybe the unity is different enough to say that those bt modules weren't designed for it?
```

---
## \#6 Posted by: Sn4pz Posted at: 2019-10-14T11:23:26.138Z Reads: 260

```
Read the esk8news thread, deodand broke his thoughts down for us electronic simpletons :joy:
```

---
## \#7 Posted by: Blitz Posted at: 2019-10-14T14:33:53.867Z Reads: 243

```
That's scary as flip,

Looks like I'm sticking to my 25mph, 10s, dual-focbox (1+1) dual receiver board.
```

---
## \#8 Posted by: Santino Posted at: 2019-10-14T17:25:33.247Z Reads: 219

```
Fuck! That's a nightmare...!
```

---
## \#9 Posted by: Deodand Posted at: 2019-10-14T18:54:51.690Z Reads: 209

```
Just so everyone is aware a firmware patch is already live as of last night that solves this issue. It has only been reported to occur with unities running FW 23.45 using the internal metr module while logging data. I have identified the change with FW 23.45 that caused the issue and reverted it, so anyone running 23.45 and metr should update.
```

---
## \#10 Posted by: never4getf150forums Posted at: 2019-10-16T23:07:56.298Z Reads: 149

```
I actually had the metr unplugged and went for a test ride..

it happened again.
```

---
## \#11 Posted by: Sn4pz Posted at: 2019-10-16T23:25:44.098Z Reads: 146

```
Jeez :no_mouth:

You alright at least?

You need a pair of vescs? someone is selling a pair of 4.xx for 75$ on the other forum... lol
```

---
## \#12 Posted by: never4getf150forums Posted at: 2019-10-17T00:22:19.774Z Reads: 140

```
i think i will consider some vesc 4s.. are they focbox? cause those have always worked flawlessly.

and yeah, im good, it happened when i got off the board and shut the remote off, 1 minute later the board still on started to accelerate full throttle and wouldn't stop. hasn't happened to me yet while on the board with the remote on.
```

---
## \#13 Posted by: Sn4pz Posted at: 2019-10-17T00:51:28.127Z Reads: 137

```
Pretty scary :( 

Have you tried a different remote?
```

---
## \#14 Posted by: never4getf150forums Posted at: 2019-10-17T01:11:43.768Z Reads: 132

```
will do soon,
```

---
## \#15 Posted by: deucesdown Posted at: 2019-10-17T01:15:57.337Z Reads: 131

```
[quote="never4getf150forums, post:12, topic:102908"]
it happened when i got off the board and shut the remote off, 1 minute later the board still on started to accelerate full throttle and wouldn’t stop.
[/quote]

This sounds like misconfigured failsafe on the remote. Can you try to replicate this on the bench? If it always goes full throttle after 1 minute it's the failsafe. Maybe you can try the remote+receiver test on another board too, just to make sure.
```

---
## \#16 Posted by: Pantata Posted at: 2019-10-23T14:01:25.161Z Reads: 99

```
This has nothing to do with unity, stop scaring with BS. THat is a failsafe issue with your receiver. Unity has no clue whether your remote is on or not, only whether it is getting signal or not. When you turn your remote off, the faifsafe signal takes over on the receiver and if you have it preset to full throttle then guess what will happen... If it goes full thorttle after 15 seconds then your receiver is faulty, buy a new one.
```

---
## \#17 Posted by: AlanZhou Posted at: 2019-10-23T14:28:25.890Z Reads: 94

```
[quote="Pantata, post:16, topic:102908"]
This has nothing to do with unity, stop scaring with BS. THat is a failsafe issue with your receiver.
[/quote]

It's not the failsafe, he's using a gt2b, I've tried the board out myself, and the failsafe is set up properly
```

---
## \#18 Posted by: Pantata Posted at: 2019-10-23T14:41:39.928Z Reads: 93

```
It's a faulty gt2b receiver. This has happened a few times before.
```

---
## \#19 Posted by: itsrow Posted at: 2019-10-23T18:02:45.923Z Reads: 87

```
If he's using a GT2Be then it is 100% the receiver.
```

---
## \#20 Posted by: professor_shartsis Posted at: 2019-10-23T18:16:46.955Z Reads: 89

```
[quote="Pantata, post:16, topic:102908"]
This has nothing to do with unity, stop scaring with BS
[/quote]


no there was an extremely dangerous firmware coding error during one of the updates in the unity, caused by some type of fault between the built in metr module and the error handling sub routines of the unity. at least 2 different people had to jump off their boards when they went to full throttle (one at around 30mph)... ask @Deodand

[quote="Deodand, post:9, topic:102908, full:true"]
Just so everyone is aware a firmware patch is already live as of last night that solves this issue. It has only been reported to occur with unities running FW 23.45 using the internal metr module while logging data. I have identified the change with FW 23.45 that caused the issue and reverted it, so anyone running 23.45 and metr should update.
[/quote]
```

---
## \#21 Posted by: professor_shartsis Posted at: 2019-10-23T18:21:06.109Z Reads: 89

```
here's what it looks like when it happens to someone in traffic:

https://drive.google.com/file/d/13mr8LzwNI-XkL6TuHCLPTyS1vJYpDZIi/view
```

---
## \#22 Posted by: janpom Posted at: 2019-10-23T20:33:26.082Z Reads: 85

```
Same thing happened to me once. I believe in this case it's the GT2B receiver problem rather than Unity problem. The receiver sometimes goes crazy and sends full throttle signal if it looses connection with the transmitter for more than 30 seconds. I recorded the behavior once. In the video, I switch off the remote. 30 seconds later, the board goes full throttle without me doing anything.

https://www.youtube.com/watch?v=-TsKB68wZvY
```

---
## \#23 Posted by: Pantata Posted at: 2019-10-23T21:54:50.560Z Reads: 78

```
Yes that was a software error, as Deodand is explaining. Had nothing to do with the gt2b giving full throttle when being off after 15 seconds. That's a receiver issue
```

---
## \#24 Posted by: BallsAndWeiners Posted at: 2019-10-24T01:15:22.793Z Reads: 71

```
That could be a failsafe issue with the gt2b. Do this dude...

https://youtu.be/W-1CZ5wXC4g
```

---
## \#25 Posted by: Schulerbible Posted at: 2019-10-24T11:00:20.425Z Reads: 63

```
I had this on my GT2B and Enertion classic Vescs. It was definitely a problem of the GT2b. Since I switched to the mini trigger it never happened again.
```

---
## \#26 Posted by: BallsAndWeiners Posted at: 2019-10-24T13:50:58.648Z Reads: 61

```
[quote="Schulerbible, post:25, topic:102908"]
It was definitely a problem of the GT2b
[/quote]

I've only had this happen on the gt2b when I didn't set the failsafe. After I did, I never saw the problem again for over 3 years with the same remote.
```

---
## \#27 Posted by: never4getf150forums Posted at: 2019-10-25T13:08:20.556Z Reads: 41

```
i tried it, even without metr pro it has issue.

i can't replicated it, has happened a total of 2 times, haven't ridden the board until i get my flipsky remote in to swap it.

after some research it sounds like a fail safe, but trying to activate the failsafe doesnt work either.
```

---
## \#28 Posted by: Vlada Posted at: 2019-10-25T16:54:44.687Z Reads: 36

```
I got full throttle with version 23.45 when I was driving 10km / h. It happened to me quite scary on the bridge. Fortunately, the brake was working. Now I have a new version but still afraid to ride
```

---
