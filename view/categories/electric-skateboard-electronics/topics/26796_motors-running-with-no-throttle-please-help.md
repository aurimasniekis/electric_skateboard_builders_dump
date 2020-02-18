# Motors running with no throttle! please help!

### Replies: 18 Views: 914

## \#1 Posted by: filmerskier97 Posted at: 2017-07-05T01:48:39.468Z Reads: 66

```
hey everybody just completed my build and after riding up hills my motors jerk under braking or coasting. Whats even weirder is that when i pick up the board the motors run with out me pressing the throttle. Has anyone seen this before? I am running 12s on 190kv motors with vescs. Please help! I posted a video of the issue https://www.youtube.com/watch?v=xVntPJafk5w
```

---
## \#2 Posted by: JLabs Posted at: 2017-07-05T01:51:54.860Z Reads: 64

```
Did you set the min and max pulse width in the VESC settings? Post some screenshots of all your settings please
```

---
## \#3 Posted by: flywithgriff Posted at: 2017-07-05T01:58:10.010Z Reads: 63

```
After riding up hills? So we should assume there were no issues before you started riding?
```

---
## \#4 Posted by: psychotiller Posted at: 2017-07-05T02:11:17.092Z Reads: 59

```
Sounds like you need to hit the apps tab in bldc and set your min and max pulsewidths for your remote.
```

---
## \#5 Posted by: filmerskier97 Posted at: 2017-07-05T02:26:41.199Z Reads: 53

```
I do remember setting the min and max pulse widths. I remember making the blue line go all the way to 100 if that makes sense cant remember what i set for the brake. could that be the culprit? I'll post my settings soon.
```

---
## \#6 Posted by: JLabs Posted at: 2017-07-05T02:28:51.913Z Reads: 48

```
Yes it could be. If you use the Ackmaniac firmware mod he has an auto calibrator that does the whole process accurately for you with no guess and check work.
```

---
## \#7 Posted by: filmerskier97 Posted at: 2017-07-05T03:17:51.918Z Reads: 47

```
<img src="/uploads/db1493/original/3X/5/3/53ad81c01bab202d14a968d32cbba310dac560d2.jpg" width="690" height="431"><img src="/uploads/db1493/original/3X/3/5/3508aefaa38aecbd11dd7668f87c2bfb47c215ad.jpg" width="690" height="431"><img src="/uploads/db1493/original/3X/b/d/bd92b8ffd6e0f37342dc196d2370653dde0bdac1.jpg" width="690" height="431">

Let me know if this info helps more than happy to take any other screen shots or run any other tests! you guys are awesome!
```

---
## \#8 Posted by: filmerskier97 Posted at: 2017-07-05T03:19:55.740Z Reads: 41

```
ya i cant replicate the issue on the bench. and ya it seems to worsen after i climb hills
```

---
## \#9 Posted by: filmerskier97 Posted at: 2017-07-05T03:59:37.628Z Reads: 41

```
@jlabs is the ackmaniac firmware mod available for mac? i wouldn't think so.....
```

---
## \#10 Posted by: psychotiller Posted at: 2017-07-05T04:14:11.888Z Reads: 41

```
After you bind your remote/receiver again. Throttle up your board. as it's coasting to a stop, remove the bind plug. Then turn off your board and turn it on again. The fail safe will be set. Then do your ppm settings again and make sure to write your changes.
```

---
## \#11 Posted by: filmerskier97 Posted at: 2017-07-05T04:45:46.066Z Reads: 38

```
ill give it a shot!
```

---
## \#12 Posted by: filmerskier97 Posted at: 2017-07-05T20:08:38.836Z Reads: 30

```
update- on my test run today it ran buttery smooth with no issues for about 4 miles. After a couple speed runs i stopped and the motors were doing the same twitching and running themselves just like in the video. But then I kept riding and it went away for like ten minutes and then did it a little bit again...... Which gets me wondering maybe I have a heat issue? It could be that im pushing the setup too hard but still not sure how that would make the motors jerk and run without throttle. Any thoughts??!
```

---
## \#13 Posted by: psychotiller Posted at: 2017-07-05T20:37:48.642Z Reads: 27

```
My thoughts are (again perspective-laid up in pain) Don't ride that board anymore until it is fixed. Something bad is going to happen. Start switching out suspect parts for fresh ones until you cant re-create the problem.  Be safe.

I can send you another remote. Honestly, it still sounds like the remote is faulty to me.
```

---
## \#14 Posted by: filmerskier97 Posted at: 2017-07-05T20:49:20.755Z Reads: 26

```
I agree im going to sideline it for now. If you could send that different remote for testing that would be huge! let me know if you need my address
```

---
## \#15 Posted by: JohnnyMeduse Posted at: 2017-07-05T20:59:23.430Z Reads: 28

```
Sorry man but you PPM setting are way off, and this is what cause your problem... maybe this tutorial could help you

http://www.electric-skateboard.builders/t/vesc-faq-setting-up-receiver-and-brakes-ppm/244
```

---
## \#16 Posted by: psychotiller Posted at: 2017-07-05T21:49:41.593Z Reads: 24

```
Sure. Which remote/receiver do you have again? 

And your address again?:
```

---
## \#17 Posted by: filmerskier97 Posted at: 2017-07-05T21:55:45.958Z Reads: 23

```
no need to say sorry I appreciate the help im going to take a look at the tutorial for sure!
```

---
## \#18 Posted by: filmerskier97 Posted at: 2017-07-06T18:40:09.173Z Reads: 20

```
i did notice looking at my ppm setting on both the master AND the slave i have the "multiple ESCs over CAN" box checked and looking at the info on forum i should disable it on the slave. could that be causing the issue??
```

---
