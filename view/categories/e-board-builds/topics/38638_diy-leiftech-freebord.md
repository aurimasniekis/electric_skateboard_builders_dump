# DIY Leiftech Freebord

### Replies: 19 Views: 1430

## \#1 Posted by: Lunasi Posted at: 2017-11-17T17:37:14.413Z Reads: 297

```
Hey guys, so I've been working on a few builds already and am really wanting to customize my leiftech electronic freebord like @okp 

I have a game plan in mind but I really want to do a 12s3p or 10s4p for it. It currently runs on 7s3p and I'm just looking for more power and speed out of it. I'm wondering if anyone on here would be interested in helping me make a custom battery for it with battery sensor and power switch. Once I get that made I can go get a 3D print to fit around the design. Batteries is one aspect of building boards that I prefer to have someone do for me. 

Thoughts, suggestions on who might be able to help? I'll post more here as I start the process.
```

---
## \#2 Posted by: pixelsilva Posted at: 2017-11-17T17:56:23.018Z Reads: 289

```
@barajabali is definitevely the man. Contact him, he'll do the battery for you. His website :point_down:

http://www.chiboards.com
```

---
## \#3 Posted by: okp Posted at: 2017-11-17T21:50:59.415Z Reads: 258

```
@longhairedboy or @barajabali and you'll be in a safe expert place!
```

---
## \#4 Posted by: Lunasi Posted at: 2018-12-15T06:25:58.008Z Reads: 177

```
So this has been a project in limbo for a while but I'm finally getting close to the finish, here's how we've progressed from a year ago.

Old 12s4p recycled into an 8s6p. 120 amp continuous BMS (because... why the F not?)

![20181214_223957|666x500](upload://87Msn96hD74o4BVKahzNpFo3KKq.jpeg) 

Focbox unity freshly delivered last night!

![20181214_223925|666x500](upload://9dsS54sH3yz1IRdBgb1Ogsd5CVu.jpeg) 

@skatardude10 is helping me build the enclosure for the top to house the BMS and the unity and will post some of his progress as we work on it 😁
```

---
## \#5 Posted by: skatardude10 Posted at: 2018-12-15T06:51:43.661Z Reads: 157

```
My pink fucking toe. God damnit.
```

---
## \#6 Posted by: Lunasi Posted at: 2018-12-15T07:07:30.684Z Reads: 155

```
😅😂 dying right now
```

---
## \#7 Posted by: davidbonde Posted at: 2018-12-15T07:47:52.307Z Reads: 147

```
I want to see a tight cornering on video please 🙂🙂🙂 I you were in Copenhagen I would make the battery for you.
```

---
## \#8 Posted by: Lunasi Posted at: 2018-12-15T17:04:49.690Z Reads: 134

```
I'll have to get some videos for ya when I get her up and working! Just need a remote and preferably I may order some new motors/mounts and just go fresh with the whole build. Once the enclosure is done I'm most the way finished though.
```

---
## \#9 Posted by: Lunasi Posted at: 2019-02-08T04:59:45.759Z Reads: 106

```
Okay so @skatardude10 has almost finished the enclosure, all the parts are in place and I'll hopefully have some pictures this weekend. Decided to go with vescs instead of focbox just because I have a 8s6p 120amp bms and can split that amperage however I like. Since my main board has a 12s4p with lower amp output I can take more advantage of the focbox on that build. Just bought some new SR369 motors and mounts from leiftech as well to clean it all up and start fresh. 

This brings me to to programming it now. I am wondering if the infamous @okp can advise a bit on how to proceed. What are the max settings you've found that the leif can handle without damaging the slip rings? I feel in a bit unfamiliar territory with the settings as there's less information out on the leiftech. Thoughts on recommended vesc settings?
```

---
## \#10 Posted by: okp Posted at: 2019-02-08T07:26:04.435Z Reads: 96

```
hey, If I'm correct I was riding motor : 30/-30 - BLDC/FOC.

These are the value I got setup in the unity but didn't manage to get good weather to give it a ride, maybe tomorrow and I'll report back.
```

---
## \#11 Posted by: stormboard1 Posted at: 2019-02-08T09:01:41.440Z Reads: 97

```
Anyone finished one of these leiftech fiy builds with more power than standard? Thnking doin it
```

---
## \#12 Posted by: Lunasi Posted at: 2019-02-10T06:51:56.946Z Reads: 88

```
![20190209_234638|666x500](upload://rnqpzGeaiYrlpg88DDowWTSfXBq.jpeg) 
![15497814509798433651701918623481|666x500](upload://tn1QtVHprjTHK5OW55m3y9k9H0v.jpeg)
```

---
## \#13 Posted by: DavidC Posted at: 2019-02-10T07:11:44.504Z Reads: 82

```
![IMG_5469|375x500](upload://tMxZWNo8q73n53B769sbw9kYwNd.jpeg) 

![IMG_5470|375x500](upload://7vFi7F96S3IEL0jRtidcxV6i5jl.jpeg)

![IMG_5479|666x500](upload://8coCS26MWsp9yGLCkYXPatQyq03.jpeg) 

![IMG_5478|666x500](upload://1nrPQfxs4SUl25ImIg4s4mYqSqt.jpeg) 

Same problem as okp, I couldn't find a sunny sunday to use it. Only sunday because to use that thing I need a smooth freshly made parking of a supermarket..
```

---
## \#14 Posted by: okp Posted at: 2019-02-10T18:37:18.628Z Reads: 71

```
Here is my v3. 

![DSC00119|690x356](upload://rtU60S1HJQhYdSFdblCctKCMgWo.jpeg)
```

---
## \#15 Posted by: B_in_tha_OZ Posted at: 2019-03-08T06:40:29.249Z Reads: 64

```
Any updates on how the massively bigger battery and pcb goes @Lunasi ???
```

---
## \#16 Posted by: skatardude10 Posted at: 2019-03-08T07:12:25.408Z Reads: 64

```
Max ABS over current. Current clearly limited on both vescs to under 30A battery max each and sensible conservative motor max. It pops in and out randomly, bit we were able to get it to happen consistently. Also looks like the max that's actually being outputted based on the logs is 5A battery max.

It works,  it's just janky as hell and unpredictable ATM. Have you made any progress since our testing Corey? 

I'm guessing maybe it's the little capacitors came loose from that massive BMS she's using, or something along those lines. I'd suggest swapping her unity over to it to isolate the issue to the vescs themselves, or the BMS, or maybe the battery itself.
```

---
## \#17 Posted by: okp Posted at: 2019-03-08T07:17:29.583Z Reads: 61

```
I'm using 8S on my prototype and 35 motor max. Just did few meters as it started to rain but I'm expecting to give it a ride in the next days is the weather gets better.
```

---
## \#18 Posted by: Nowind Posted at: 2019-03-08T07:37:06.376Z Reads: 62

```
Running 8S Lipos

30A Motorcurrent

Vesc4

Works very good
```

---
## \#19 Posted by: Lunasi Posted at: 2019-03-08T17:56:42.581Z Reads: 45

```
Any idea what might be causing the ABS over current @okp

Na, haven't had a chance to take a second look yet @skatardude10 but if you're off sometime let's mess with it again.  

@B_in_tha_OZ minus the fact that I'm getting abs over current when it does ride the power is ridiculous
```

---
