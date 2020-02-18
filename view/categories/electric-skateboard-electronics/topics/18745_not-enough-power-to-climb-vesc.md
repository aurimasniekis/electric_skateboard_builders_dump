# Not enough power to climb vesc?

### Replies: 9 Views: 946

## \#1 Posted by: marcoluz Posted at: 2017-03-08T11:12:35.949Z Reads: 115

```
Hi there, i don't have any idea but i am not getting enough power to climb. in the begging everything was running good... i don't know what have changed. My set is 10s4p samsung lion cells, maytech vesc, maytech 6355 motor... single and antispark switch... even with battery voltage around 38v. i don't have bms <img src="/uploads/db1493/original/3X/7/e/7e45b6aeb3785815396f89e2fd69f7da656beefd.png" width="690" height="431"><img src="/uploads/db1493/original/3X/e/f/eff941a74183b955325d665819e5e4c8af10768f.png" width="690" height="431"><img src="/uploads/db1493/original/3X/8/e/8e4dc0402778656f748cb09c52a1deefbea56b74.png" width="690" height="431"><img src="/uploads/db1493/original/3X/4/0/40ac6078f32891b1df2d36b76dc5f50fbfb02bdc.png" width="690" height="431">
```

---
## \#2 Posted by: catweazle Posted at: 2017-03-08T20:33:41.536Z Reads: 78

```
Hi marcoluz,
your "max current ramp step" value is 40000. I think it should be 0.04.
Could be that you have this...

http://www.electric-skateboard.builders/t/psa-remember-to-reset-your-max-current-ramp-step-when-programming-your-vesc/6262
```

---
## \#3 Posted by: Namasaki Posted at: 2017-03-08T23:09:14.775Z Reads: 67

```
Good eye @catweazle 
I can't see how his Vesc isn't dead already.
```

---
## \#4 Posted by: marcoluz Posted at: 2017-03-09T11:22:55.871Z Reads: 52

```
great. thank you so much. is it the reason for my climb problem?
```

---
## \#5 Posted by: marcoluz Posted at: 2017-03-09T11:46:53.850Z Reads: 50

```
<img src="/uploads/db1493/original/3X/7/5/75abc1d762e7384c2e210f74ad5d82f060acb221.jpg" width="666" height="500">is this the reason why? Cables too thin?
```

---
## \#6 Posted by: Maxid Posted at: 2017-03-09T12:27:02.554Z Reads: 50

```
:scream: 
that solder job looks really bad - you are lucky the batteries are still alive.
```

---
## \#7 Posted by: marcoluz Posted at: 2017-03-09T12:31:09.756Z Reads: 50

```
Ehehehe... Did my best.
```

---
## \#8 Posted by: Maxid Posted at: 2017-03-09T13:14:34.376Z Reads: 48

```
how did you get the idea that using like 16AWG cable on the battery is a good idea? I mean you are using 10AWG on the connector so why not everywhere?
```

---
## \#9 Posted by: catweazle Posted at: 2017-03-09T13:37:44.289Z Reads: 44

```
The setting should be changed to 0.04.
Set it to 0.004 and write config...then it should be at 0.04 if you have this bug in your firmware(what version do you have?).
You can double-check it when you read the configuration, after you saved.
You could give it a try then...after looking at your batteries I think there could be more problems.

Here is a post of someone who had this Problem, too. His value was 50000:
http://www.electric-skateboard.builders/t/vesc-dvr8302-fault/13478/7
```

---
