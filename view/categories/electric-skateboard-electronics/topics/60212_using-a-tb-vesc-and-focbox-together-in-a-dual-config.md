# Using a TB vesc and focbox together in a dual config?

### Replies: 14 Views: 287

## \#1 Posted by: longboardshort Posted at: 2018-06-27T13:18:12.724Z Reads: 91

```
Hey all, couldn’t find anything after a few searches. Has anyone tried this or would advise against? Obviously stay in Bldc, but I’d love to hear some thoughts before I am Guinea-Pig it. Thank you and I apologize if there is a topic and I just couldn’t find it.
```

---
## \#2 Posted by: biggdaddyhawk Posted at: 2018-06-27T13:49:37.834Z Reads: 84

```
Seem like if canbus couldnt be used that each one could be set to master and a Y config could be used....but not sure.
```

---
## \#3 Posted by: esk8taylor Posted at: 2018-06-27T14:29:40.663Z Reads: 74

```
I have this setup and it works just fine. I have the Foxbox as the master the and the TB VESC as the slave.  I did this because I had one of my TB VESCs go bad months ago and didn't want to wait on TB to replace it so I upgraded to a foxbox.  I just got the replacement this week and will save it for a backup.
```

---
## \#4 Posted by: longboardshort Posted at: 2018-06-27T16:34:30.184Z Reads: 64

```
Awesome thanks for the feedback! I typically run split ppm over canbus anywho, so it still sounds like it will be fine. I’ll report back if anything weird happens but just wanted to double check.
```

---
## \#5 Posted by: esk8taylor Posted at: 2018-06-27T18:24:39.224Z Reads: 42

```
I run the canbus for the record.  It works as well.
```

---
## \#6 Posted by: Acido Posted at: 2018-06-27T18:30:20.703Z Reads: 41

```
i do not see a reason why it would not, especially if they run same firmware
```

---
## \#7 Posted by: Benjamin899 Posted at: 2018-06-27T18:31:43.534Z Reads: 41

```
i always here that canbus fries vesc or am i misinformed?
```

---
## \#8 Posted by: esk8taylor Posted at: 2018-06-27T18:32:15.647Z Reads: 40

```
Didn't fry mine.
```

---
## \#9 Posted by: Acido Posted at: 2018-06-27T18:32:58.082Z Reads: 41

```
there are ways it can fry the can chip im not really aware of how and why but if i would run dual i would go split ppm, do not see advantages of canbus
```

---
## \#10 Posted by: esk8taylor Posted at: 2018-06-27T18:34:57.083Z Reads: 39

```
  [quote="Acido, post:9, topic:60212, full:true"]
there are ways it can fry the can chip im not really aware of how and why but if i would run dual i would go split ppm, do not see advantages of canbus
[/quote]
The only advantage I'm aware of is traction control and ease of setup.
```

---
## \#11 Posted by: Acido Posted at: 2018-06-27T18:36:10.088Z Reads: 34

```
shouldn't each vesc take care of its traction if you enable it?
do not see a reason why they need to be connected together for it to work, never used TC tho
```

---
## \#12 Posted by: esk8taylor Posted at: 2018-06-27T18:41:58.519Z Reads: 34

```
[quote="Acido, post:11, topic:60212, full:true"]
shouldn’t each vesc take care of its traction if you enable it?
do not see a reason why they need to be connected together for it to work, never used TC tho
[/quote]

No, that isn't how it works.  Another advantage is being able to see both VESCs over a bluetooth connection.  Benjamin recommends Canbus as does a few of the heavy weights around here including Trampa.  Either should work fine if you aren't looking to control through bluetooth and don't care about traction control.  The advantage to splitting is you can still use one motor if the master VESC fails.  I had a master fail and was unable to skate home.  I had to call an uber.
```

---
## \#13 Posted by: b264 Posted at: 2018-06-27T18:48:25.819Z Reads: 32

```
[quote="Acido, post:9, topic:60212"]
if i would run dual i would go split ppm
[/quote]

or dual receiver.  

That gives you two completely independent drivetrains so if something fails on one, the other should still be working.
```

---
## \#14 Posted by: Acido Posted at: 2018-06-27T18:52:50.269Z Reads: 29

```
this is even better :D
```

---
