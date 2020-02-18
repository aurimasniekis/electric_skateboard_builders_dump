# FVT ESC overheating?

### Replies: 6 Views: 1052

## \#1 Posted by: FlimFlamPhlegm Posted at: 2016-06-22T01:35:38.303Z Reads: 110

```
I made my first build and it's working decently so far, it can climb everything i've thrown at it so far (5-10% hill inclines), but when I go up more than 1 hill my ESC overheats and throttles the speed, even when the battery is 80-90% charged. The motor also gets quite hot to the touch. 

My build is: 

-Carvon V2 Hub single
-FVT 120A ESC
-Turnigy 20C 5000mAh Li-Po
-Wiiciever

I removed my fan from the FVT ESC as I heard that it functioned fine as long as you provide it with airflow, so I cut a hole in my enclosure for the airflow, but it seems to overheat nonethenless. This is how I mounted the ESC.

<img src="/uploads/db1493/original/2X/f/f1b7ddd16e2babc18f4047091049da17cf92698d.jpg" width="370" height="499">

My ESC settings are: 
Motor Timing: High
Motor Acceleration: High (with 150% accel curve on the wiiciever)
Cut-off voltage: 3.0V/cell
Direction: Forward w/o Reverse

Does anyone have any ideas on how to prevent the throttling from overheating?
```

---
## \#2 Posted by: lox897 Posted at: 2016-06-22T01:49:00.747Z Reads: 106

```
Try lowering your motor timing. Have you tried putting the fan back on?
```

---
## \#3 Posted by: FlimFlamPhlegm Posted at: 2016-06-22T04:09:34.415Z Reads: 94

```
alright i'll try lowering it when I fix the cheap POS ESC

For some reason, the wiiciever stopped syncing so I unscrewed the case to see if the ESC reciever wire had a short in it, and when I opened it, both capacitors were loose and had no connection. I'm going to pick up 2 replacement caps tmr and see if I can reprogram it after then.

Also, i'm replacing the crappy thermal pad they had in the ESC with some computer thermal paste to see if that helps a bit.
```

---
## \#4 Posted by: evoheyax Posted at: 2016-06-22T17:40:00.338Z Reads: 70

```
[quote="FlimFlamPhlegm, post:1, topic:4978"]
Motor Timing: High
Motor Acceleration: High
[/quote]

This is what caused me to both blow out this esc and an rspec motor, at different times. Always use no higher than medium. You will break stuff with settings any higher.
```

---
## \#5 Posted by: longhairedboy Posted at: 2016-06-22T17:42:53.372Z Reads: 66

```
I've been running a pair of these in my 6S dual drive for quite some time now. I got them from DIY. I leave them at the default settings which seem to make them last a lot longer.
```

---
## \#6 Posted by: FlimFlamPhlegm Posted at: 2016-06-23T05:42:05.896Z Reads: 53

```
welp thanks for all the advice on settings, but i think some SMD components failed as it still fails to detect the receiver even with new caps. I checked all the connections, and even redid the ESC reciever wire, and it still doesn't work so i'm going to see if I can grab another one for 30USD and just leave the fan on this time. If not, i'll probably just buy a VESC
```

---
