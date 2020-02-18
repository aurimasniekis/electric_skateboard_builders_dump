# Motor Randomly locking/fluttering

### Replies: 20 Views: 619

## \#1 Posted by: stchase24 Posted at: 2017-08-03T00:19:43.296Z Reads: 85

```
Hi,

I noticed my motors locking/fluttering after hitting a divot a few days ago. It would flutter for a second, then run fine anywhere from 2 minutes to 2 days with no issues. Seems to flutter the most on light acceleration. After the first initial flutter, I recharged the remote and board and didn't have any issues for 2 full days of riding. Flutter was back by day 3. I'm currently running dual drive enertion motors. 

Any diagnosis or suggestions before I attempt to open the motor and check for debris? 


<img src="/uploads/db1493/original/3X/2/6/26997aabaf15468d61d5fadd992461be3ca0b5f5.jpg" width="374" height="500"><img src="/uploads/db1493/original/3X/d/5/d5bc6028697015e3e8e2b7cfe5d6486cdcb48204.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/7/7/77bdcd4d29f6378fa82b0505a351d6c3c2df56a6.jpg" width="374" height="500">
```

---
## \#2 Posted by: Montiey Posted at: 2017-08-03T00:55:02.087Z Reads: 81

```
There's no way we can diagnose something like this as is. A video would be the best way to figure it out. What _kind_ of flutter? is the motor cutting out, or does it sound like phases skipping position? What hardware is on your board? Electronics? Have you tried keeping the remote fully charged and see if the issue is persistently removed?
```

---
## \#3 Posted by: stchase24 Posted at: 2017-08-03T01:29:30.711Z Reads: 80

```
@Montiey Thanks for the help! Wheel or wheels lock up as if I slam the brakes, but then resume as normal. Locking might be a better term than flutter. It only occurs when I'm riding the board and at low speeds at the beginning of acceleration. I also weigh 255 lbs. Both motors seem to run fine when I'm not riding the board. My weight probably isn't helping, but I had about 20 miles on the board without issues before the divot. Could debris inside the motor cause something like this? Or maybe a short inside the motor? Video would just look like im slamming the brakes... Board was at 70% battery when latest locking occured. I was still able to get up to 29mph at 80% battery yesterday before experiencing the issue at low speeds with 70% battery today.

Electronics:
2 enertion r-spec raptor 1 motors
2 vescs
4 x 4500 3s lipos wired for 12s
Geree battery capacity reader

Hardware:
Enertion trucks & enertion wheels
Deck is cheap 42" 7 ply drop through
```

---
## \#4 Posted by: Hummie Posted at: 2017-08-03T03:30:26.511Z Reads: 69

```
does it get hotter than the other?  if so probably a short.  louder?   you should run the bldc test on your pc and see if it passes and compare the inductance and resistance between both motors if it does pass
```

---
## \#5 Posted by: stchase24 Posted at: 2017-08-03T13:42:53.858Z Reads: 59

```
@Hummie @Montiey  Here's a video of what just happened on the bench. It looks like a short and the motor with the scratch on it is a little hotter. Ran smooth for about 10 seconds at full blast before doing this.

https://www.youtube.com/watch?v=ATSdJ40oh_M
```

---
## \#6 Posted by: stchase24 Posted at: 2017-08-03T14:07:45.660Z Reads: 57

```
Now it's running fine again.:fearful: Below are the BLDC results for the bad motor and realtime data with the trigger at full speed:
<img src="/uploads/db1493/original/3X/f/0/f036a0785483142bf510fa65dc86978db1737c75.png" width="690" height="381"><img src="/uploads/db1493/original/3X/4/e/4e2cccd6e587fe16deaf0a93c03d70288e549a41.png" width="690" height="449">

Here are the same tests for the good motor:
<img src="/uploads/db1493/original/3X/5/d/5d1e50100c98a5af381581987795baeeca0774b5.png" width="690" height="332"><img src="/uploads/db1493/original/3X/c/a/ca86b6e901d6b1b1ec8e1a142ba1da14504c61e1.png" width="690" height="334">
```

---
## \#7 Posted by: Blasto Posted at: 2017-08-03T14:33:50.290Z Reads: 54

```
Be sure to hit "APPLY" and "write configurations"

seams to have a discrepancy here

<img src="/uploads/db1493/original/3X/5/9/59b7ce6a4644347d31e787f91f8746df552f634c.png" width="690" height="434">
```

---
## \#8 Posted by: Bloop Posted at: 2017-08-03T15:26:06.096Z Reads: 56

```
I think you have a rock or something stuck in your motor ? If you spin the motor with your hand is it working smooth ?
```

---
## \#9 Posted by: stchase24 Posted at: 2017-08-03T15:39:00.490Z Reads: 54

```
Sometimes smooth, sometimes shakey. I think it's a rock too. Are there any guides on how to open the motor and get the rock/debris out?
```

---
## \#10 Posted by: Hummie Posted at: 2017-08-03T16:11:01.900Z Reads: 54

```
blasto can you describe how those variables you circled effect things?


opening the motor take the little c-clip off the shaft with somethign and pull the can off.  easy.  don't lose the clip or possible shims on the axle.
```

---
## \#11 Posted by: Blasto Posted at: 2017-08-03T16:22:34.688Z Reads: 53

```
It's the variables that are acheived by a motor detection, in his screen shot those variables are not applied
```

---
## \#12 Posted by: Hummie Posted at: 2017-08-03T16:30:15.693Z Reads: 50

```
wondering if they reveal how well the motor is coupled between windings and poles or something.  would a more efficient or better designed motor have a higher coupling?
with the min erpm...the motor wont spin any slower than what it says I guess, so if that number is higher then you'd have to push more to get it up beyond the min erpm before the motor will operate?
```

---
## \#13 Posted by: stchase24 Posted at: 2017-08-03T22:20:26.393Z Reads: 43

```
I took it apart, tried to clean it, put back together, ran it and took it apart again after the motor was still getting hot and randomly locking. Inside didn't look too bad other than some tiny magnetic debris. Anything look off here?

<img src="/uploads/db1493/original/3X/0/b/0ba1fa2183c462e29de4d9c9ca8ddc30f0e98f3d.jpg" width="375" height="500">
<img src="/uploads/db1493/original/3X/6/d/6d2eef96dc47d20e70c5816134f91d0e93c2daeb.jpg" width="374" height="500">
<img src="/uploads/db1493/original/3X/9/3/9315007dd62878da0a9732338f3e1678fc5b5cae.jpg" width="375" height="500">
<img src="/uploads/db1493/original/3X/d/5/d52a7a5d81d7a547c65732e4f3039b173b06833f.jpg" width="374" height="500">
```

---
## \#14 Posted by: darkkevind Posted at: 2017-08-03T22:41:38.073Z Reads: 41

```
Sounds like your motor wires are shorting randomly. Check the wires all the way in to the motor housing, the heat shrink may have degraded and is causing a short...
```

---
## \#15 Posted by: stchase24 Posted at: 2017-08-03T22:48:29.360Z Reads: 41

```
Heat shrink goes about a 1/4" into the motor housing as seen in the 2nd pic. Is that too short? 

This guy had a similar problem with the same motors and reinsulated his phase wires at the 1:04 mark in this vid:

https://youtu.be/RdFyoMlbFEY
```

---
## \#16 Posted by: darkkevind Posted at: 2017-08-03T23:07:52.538Z Reads: 39

```
Yes, that's what I'd do if I were you...
```

---
## \#17 Posted by: stchase24 Posted at: 2017-08-05T20:47:24.983Z Reads: 34

```
Definitely looks like the motor is shorting. One of the phase wires inside is slightly burnt as seen below. Bought some paint on liquid tape to try. Looks like lots of enertion raptor 1 dual users have experienced this.
<img src="/uploads/db1493/original/3X/7/9/7944fe0ef8e0f86c90b8772d7547648c8f2d28e6.jpg" width="374" height="500">
```

---
## \#18 Posted by: stchase24 Posted at: 2017-08-05T22:45:56.010Z Reads: 33

```
I seemed to fix the problem by putting heat shrink around the phase wires inside the motor. Ran it full speed for about 25 seconds with no hiccups. I only problem is my motor is now spinning in reverse direction
:scream:
```

---
## \#19 Posted by: JohnnyMeduse Posted at: 2017-08-05T22:47:42.344Z Reads: 33

```
just swap two phase wire
```

---
## \#20 Posted by: stchase24 Posted at: 2017-08-05T22:51:09.785Z Reads: 33

```
Thanks @JohnnyMeduse it's working now!
```

---
