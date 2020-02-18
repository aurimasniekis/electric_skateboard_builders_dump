# PPM or can bus?

### Replies: 7 Views: 790

## \#1 Posted by: dareno Posted at: 2018-06-27T21:34:00.791Z Reads: 147

```
hi, guys and gals just a quick discussion on the benefits of can bus over ppm or vice versa.
I recently had two focboxes pop on me due to bad can bus settings or connection issues, not sure which.
Carl from enertion was absolutely fantastic, spending 2 hours on a sunday trying to get to the bottom of the issue and it was decided that the can bus caused the problem.  I know that connecting one at a time to the battery while the can bus cable is connected can cause this but my issue happened without that event and apparently a loose connection can also cause the problem.  So my question is;

Is a ppm splitter a safer option? Or will this cause any other issues?
I'm sure that I'm not the only one out there that has fried vescs and any help would be greatly appreciated.

P.S Carl really stepped up though and I have new focboxes on the way.  Thanks Enertion!
```

---
## \#2 Posted by: chuttney1 Posted at: 2018-06-27T21:54:24.801Z Reads: 140

```
Depends on the application. I can say that both are safe depending on use. Here's an old thread

https://www.electric-skateboard.builders/t/y-piece-or-canbus/26461/236

If you use PPM with a splitter cable, the signal wire to the second controller is good enough from what I read. You must not have the ground on both controller connected with PPM splitter because it create a ground loop which can short out stuff. 

If it's CANBus, it's very reliable when the hardware is designed correctly. If your FOCBox fails using CANBus, then that is an hardware issue.
```

---
## \#3 Posted by: bigben Posted at: 2018-06-27T21:54:26.982Z Reads: 132

```
http://www.electric-skateboard.builders/t/y-piece-or-canbus/26461
This had a good going over on this thread.
```

---
## \#4 Posted by: i2oadsweepei2 Posted at: 2018-06-27T22:49:17.447Z Reads: 111

```
[quote="chuttney1, post:2, topic:60255"]
If you use PPM with a splitter cable, the signal wire to the second controller is good enough from what I read. You must not have the ground on both controller connected with PPM splitter because it create a ground loop which can short out stuff.
[/quote] 

I’m glad you mentioned that. Think i’ll go back to that thread and get caught up.
```

---
## \#5 Posted by: dareno Posted at: 2018-06-27T22:50:58.943Z Reads: 104

```
@i2oadsweepei2  Its a fucking tennis match trust me lol  still good reading though!
```

---
## \#6 Posted by: bigben Posted at: 2018-06-27T22:53:08.872Z Reads: 100

```
After I started that long thread I ended up using a receiver for each vesc. It gives a bit more backup.
```

---
## \#7 Posted by: dareno Posted at: 2018-06-27T23:26:30.527Z Reads: 95

```
Thanks to all the peeps directing me to the previous thread.  Usually the little forum wizard pops up with the old similar thread notification but didn't happen this time.  Note to self....do a search first!
I'm still in 2 minds but having been burnt by can bus I'm leaning toward splitter.
more research!!
```

---
