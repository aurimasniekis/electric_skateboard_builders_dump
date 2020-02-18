# \[Solved\] Receiver trouble

### Replies: 9 Views: 387

## \#1 Posted by: sleepySteve Posted at: 2017-07-14T00:50:30.076Z Reads: 56

```
Hey All,
I'm currently putting together my first build and am trying to bind the receiver from the TorqueBoards 2.4Ghz Mini Remote Controller.  From what I understand there should be an led lighting up on the receiver but nothing happens when I plug it in to my vesc and power everything up.  I know that the power works on the vesc because I had just programmed it using a programming card and everything worked fine.  I guess my question is if this is a bad receiver or if i'm doing something wrong.
Thanks,
Stephen
```

---
## \#2 Posted by: JLabs Posted at: 2017-07-14T01:14:58.922Z Reads: 50

```
Post a pic of your setup. My guess is that it is no wired properly.
```

---
## \#3 Posted by: sleepySteve Posted at: 2017-07-14T01:24:50.493Z Reads: 48

```
[Receiver Test](https://drive.google.com/open?id=0B8uqN7U4hVXWV3AzVEZ0dWdPeEU)
I took a video of the programming card being lit up then the receiver being switched in.
```

---
## \#4 Posted by: sleepySteve Posted at: 2017-07-14T01:25:27.156Z Reads: 48

```
I shut everything down before I change plugs, not sure if that is apparent from the video
Here's an image too
<img src="/uploads/db1493/original/3X/7/e/7eee919566ea95731824add0867acf085c9b31cd.jpg" width="371" height="499">
```

---
## \#5 Posted by: JLabs Posted at: 2017-07-14T01:50:24.957Z Reads: 41

```
The longer cord is for programming and the shorter one is the PPM cable. Change them around with the black wire to the left in channel 2.

With that esc I think you have to plug the UBEC into channel 4 with ground on the left and power all the way to the right (no middle wire).
```

---
## \#6 Posted by: sleepySteve Posted at: 2017-07-14T01:59:21.159Z Reads: 40

```
I'll try that, thanks.

So I tried what @JLabs recommended.  I figured out the problem, the longer wire from the vesc is for the receiver but it did need power from the UBEC in channel 4
```

---
## \#7 Posted by: JLabs Posted at: 2017-07-14T02:34:26.703Z Reads: 34

```
I'm glad you got it figured out!
```

---
## \#8 Posted by: mmaner Posted at: 2017-07-14T03:16:25.107Z Reads: 30

```
You should probably change the topic, as the problem wasn't with Torqueboards mini remote.
```

---
## \#9 Posted by: sleepySteve Posted at: 2017-07-14T03:17:30.186Z Reads: 29

```
i just changed it, thanks for the heads up.
```

---
