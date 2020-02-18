# X-Car Beast Programming Settings

### Replies: 15 Views: 1029

## \#1 Posted by: kidcisco Posted at: 2017-10-31T03:08:07.190Z Reads: 89

```
For anyone using an Xcar beast ESC from hobby king, what settings are you using? I got the programming card and am interested to hear from anyone who's had some time with it.
```

---
## \#2 Posted by: Jinra Posted at: 2017-10-31T05:38:34.780Z Reads: 77

```
@lowGuido is the resident expert on those things
```

---
## \#3 Posted by: saul Posted at: 2017-10-31T05:41:01.678Z Reads: 78

```
it worked on with braking on mid, then the connection was lost and it went full throttle.
luckly it was geared for only <14mph.

its a good paper weight tho...
```

---
## \#4 Posted by: pat.speed Posted at: 2017-10-31T06:14:04.801Z Reads: 71

```
3.4v lvc 
25%brake 
Timing set to max
```

---
## \#5 Posted by: kidcisco Posted at: 2017-10-31T06:48:37.302Z Reads: 61

```
There's two brake settings:

PERCENTAGE BRAKING [10-100%]
PERCENTAGE DRAG BRAKING [0, 4,8,12,15,20,25,30%]

What exactly is motor timing? Is it how fast you go because I honeslty don't want to go any faster than 15mph and would like to keep things on the slow end for now.
```

---
## \#6 Posted by: kidcisco Posted at: 2017-10-31T06:51:17.927Z Reads: 60

```
These are the settings, FYI. 

<img src="/uploads/db1493/original/3X/1/e/1e48cbe3612eb6d3e72c1f63cd21ea4b2bb47431.png" width="549" height="500">

The ones I'm mostly confused about are:

MOTOR TIMING
THROTTLE PERCENT REVERSE 
THROTTLE LIMIT
PERCENTAGE BRAKING
PERCENTAGE DRAG BRAKE
NEUTRAL RANGE
```

---
## \#7 Posted by: pat.speed Posted at: 2017-10-31T07:34:21.936Z Reads: 49

```
Ok so motor timing is how fast it will go just change that until it's right for you. Throttle reverse is how fast it will go in reverse I think mine is set to 50%. Turn the drag brake to 0. Percent braking you can change until it is as strong as you like. And nuetral range is the range on the transmitter when it is in the nuetral position just leave that how it comes and leave the throttle limit too
```

---
## \#8 Posted by: lowGuido Posted at: 2017-10-31T08:22:44.563Z Reads: 49

```
I use 3.0v cutoff
Forward brake no reverse.
Motor timing very high
Initial acceleration low
0% drag brake
Brake force 70%
Neutral 4%

I put initial acceleration low for my mates who are n00bs. I set it up higher for experienced skaters.
```

---
## \#9 Posted by: kidcisco Posted at: 2017-10-31T18:17:53.000Z Reads: 34

```
@lowGuido @pat.speed

Thanks for the help. Truly appreciate it.
```

---
## \#10 Posted by: kidcisco Posted at: 2017-10-31T18:34:38.849Z Reads: 33

```
@lowGuido

One more question for you, sir. 

The low voltage cut off. I keep hearing lots of people saying stop at different values (3.7, 3.2, 3.4). Isn't 3.0 too low? I thought the lowest you want to safely discharge is 3.2...Or do you ever even ride the board to 3.0 or is that just an extreme low? Becuase my lipo alarm only has value for 2.7 and 3.8 and I want to be as safe as possible with the batteries. Also want to get a somewhat decent range.
```

---
## \#11 Posted by: Brycehoosiers Posted at: 2017-10-31T19:09:48.667Z Reads: 29

```
anything below 3.2v is for lion batteries. I don't know why your alarm would only have two settings one is too high , and one is too low
```

---
## \#12 Posted by: kidcisco Posted at: 2017-10-31T20:02:46.105Z Reads: 29

```
You're right, thats the range for the alarm, not the values. I don't have it hooked up currently so I wasn't clear on that.
```

---
## \#13 Posted by: Brycehoosiers Posted at: 2017-10-31T20:20:01.043Z Reads: 29

```
most people recommend setting the lvc at 3.6v
```

---
## \#14 Posted by: pat.speed Posted at: 2017-10-31T21:17:09.739Z Reads: 27

```
If you download the program and plug it into the computer you can set it up more precisely.  I have my cut off at 3.4 but it usually gets triggered from voltage sag so the cells are at about 3.6v when resting
```

---
## \#15 Posted by: lowGuido Posted at: 2017-11-01T05:03:55.165Z Reads: 23

```
for starters, I don't use the cutoff in the ESC, I have a lipo alarm for that.
and I have it set pretty low because you have to allow for voltage sag. you might find that with the voltage sag that when it hits 3.0v under load it may still have 3.6v
having said that I am usually pretty aware of my pack charge level and how far I can go. I rarely run a pack fully dry.
```

---
