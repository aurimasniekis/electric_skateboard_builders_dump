# Motors spinning full speed at 0 throttle

### Replies: 12 Views: 734

## \#1 Posted by: 12meterkuk Posted at: 2017-10-30T05:25:00.733Z Reads: 53

```
I tried watt mode yesterday, and it didn't really respond so i flashed my vescs back to the old firmware. Now its spinning full speed at 0 throttle and stops when i brake. Any advice on how to fix?
```

---
## \#2 Posted by: cwazy1 Posted at: 2017-10-30T05:25:37.839Z Reads: 53

```
check your ppm settings as well as your trim on your remote
```

---
## \#3 Posted by: 12meterkuk Posted at: 2017-10-30T05:26:16.718Z Reads: 50

```
[quote="cwazy1, post:2, topic:36844, full:true"]
check your ppm settings as well as your trim on your remote
[/quote]
<img src="/uploads/db1493/original/3X/2/b/2bd774e3fa62d782aef5677d9f10bb6790bae013.png" width="690" height="345">

My settings right now.

How do i check the remote trim?
```

---
## \#4 Posted by: cwazy1 Posted at: 2017-10-30T05:35:03.090Z Reads: 44

```
okay, lets try something here
1. set control move = disabled. apply. 
2. check the box that says display
3. what does the bar below the display checkbox show? is it centered at 50%?
3. what controller are you using?
```

---
## \#5 Posted by: 12meterkuk Posted at: 2017-10-30T05:37:46.203Z Reads: 44

```
[quote="cwazy1, post:4, topic:36844"]
1. set control move = disabled. apply.
[/quote]

Where is it? can't seem to find it
[quote="cwazy1, post:4, topic:36844"]
3. what does the bar below the display checkbox show? is it centered at 50%?
[/quote]

Its at 50%

[quote="cwazy1, post:4, topic:36844"]
3. what controller are you using?
[/quote]

2.4ghz mini
```

---
## \#6 Posted by: cwazy1 Posted at: 2017-10-30T05:40:49.742Z Reads: 40

```
1. top of ppm page

OK, if you're using mini, its likely a throttle trim calibration issue. 

Do you see the two little white round knob on the controller between your index finger and thumb? One of them should say S and one is T?
```

---
## \#7 Posted by: 12meterkuk Posted at: 2017-10-30T05:41:26.346Z Reads: 40

```
[quote="cwazy1, post:6, topic:36844"]
Do you see the two little white round knob on the controller between your index finger and thumb? One of them should say S and one is T?
[/quote]

yup

10char
```

---
## \#8 Posted by: 12meterkuk Posted at: 2017-10-30T05:42:59.264Z Reads: 35

```
[quote="cwazy1, post:4, topic:36844"]
1. set control move = disabled. apply.
[/quote]

with disabled it will gun the speed without me touching the remote.

With current it will only start when i brake and let go
```

---
## \#9 Posted by: 12meterkuk Posted at: 2017-10-30T05:44:23.883Z Reads: 34

```
[quote="cwazy1, post:6, topic:36844"]
OK, if you're using mini, its likely a throttle trim calibration issue.
[/quote]

I found the issue, thanks so much. My thtrim was turned all the way
```

---
## \#10 Posted by: cwazy1 Posted at: 2017-10-30T05:44:39.425Z Reads: 34

```
so for your records, those are the manual trim settings for the remote. the S is for steering. since you don't use the steering wheel control, ignore this. The T is for throttle. This is the one you'll be adjusting. Think about it as another way of setting your ppm. Your manual trim should be set to zero first and then your ppm should be adjusted to fit. 

turn the remote on, turn the board on, make sure your ppm control is 'current no rev w/ brake', apply. 
If your motor is turning while no throttle is applied, turn the T knob counter clockwise until motor no longer spins.
```

---
## \#11 Posted by: cwazy1 Posted at: 2017-10-30T05:46:32.950Z Reads: 27

```
awesome. 
one more thing you should ALWAYS check with the mini.. while pulling the throttle, turn the controller off. make sure the motor does not 

1. continue to spin forward (meaning you need to turn it further CCW) 
2. hit the brake (meaning you turned it a bit too much CCW)
```

---
## \#12 Posted by: 12meterkuk Posted at: 2017-10-30T05:48:06.362Z Reads: 26

```
Thanks so much, noted
```

---
