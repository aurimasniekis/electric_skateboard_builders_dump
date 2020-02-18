# Gt2b failsafe question

### Replies: 9 Views: 794

## \#1 Posted by: danielz Posted at: 2018-04-21T08:53:26.381Z Reads: 143

```
Ive correctly set my failsafe, switching the controller off cuts the motors unlike before when they went to 100%. 


However, if i turn the board on with the controller powered off after about 30 secs the motors go to 100% why is the receiver doing this? There is a real time app button in the vesc tool which might be useful to see what the receiver is doing, but i cant see where its graphed.
```

---
## \#2 Posted by: onepunchboard Posted at: 2018-04-21T13:29:10.806Z Reads: 133

```
for some reason when vesc is connected to fail safe it just go full power. 
I tried gt2b and  2 diff failsafe units all of them does the same. vesc has built in failsafe so use that.
```

---
## \#3 Posted by: danielz Posted at: 2018-04-22T03:06:35.434Z Reads: 117

```
The only thing i can see is timeout brake current. But its set to 0 amps already which it clearly ignoring.
```

---
## \#4 Posted by: lrdesigns Posted at: 2018-04-23T08:18:23.087Z Reads: 101

```
Mine does the same, but I heard some others say theirs did not. Weird could not find an answer. 

So you just have to remember to always turn the remote on first. :disappointed_relieved:

To be more clear, if turn on remote, turn on board, ...THEN turn off the remote my board will stay throttle off for unlimited amount of time. Its just I cant have the board powered on without first powering the remote.
```

---
## \#5 Posted by: danielz Posted at: 2018-04-23T09:26:39.123Z Reads: 94

```
Exactly the same here. Its only on startup and with controller off. Subsequently disconnected the controller has no effect. I reckon if everyone tested it might be a widespread issue. Its not a normal failsafe issue as setting the vesc to brake on timeout is ignored. The GT2B receiver must go into some kind of weird mode or something if powered on without the controller being turned on in x amount of seconds?

I really want to see the pwm timing live some how, i have an arduino and raspberry pi, maybe i can knock something up to see whats going on.

Guy here has same issue too
https://www.electric-skateboard.builders/t/failsafe-issue-never-seen-this-before/53057
```

---
## \#6 Posted by: danielz Posted at: 2018-04-24T00:14:48.990Z Reads: 78

```
Here we go I confirm the gt2b receiver is the cause. Hooked it up to an arduino. If you power up the gt2b receiver without the controller on after 30 seconds it changes from my custom fail-safe timing valuve of 1330ms to 1500ms. Hence the motors go crazy!

Now thew question is this by design or have we all got faulty receiever units??? Im guessing people without this problem have the failsafe at around 1500ms so it wont effect them.

Adjust your throttle trim to 1500ms should fix this. however i can only trim mine to 1460ms, im hoping its enough. I dont thing its acceptable for the receiver to ignore the failsafe adter 3o seconds though

https://youtu.be/Sk8cuHxZtyc
```

---
## \#7 Posted by: lrdesigns Posted at: 2018-04-24T01:03:14.310Z Reads: 69

```
[quote="danielz, post:6, topic:53017"]
Im guessing people without this problem have the failsafe at around 1500ms so it wont effect them.
[/quote]

That’s a pretty good theory, never thought about it that way before.
```

---
## \#8 Posted by: danielz Posted at: 2018-04-24T01:06:03.737Z Reads: 64

```
Adjust your throttle trim knob anti clockwise to try get ur trigger center point to 1500ms then reset the failsafe to it. I can get mine to 1460ms only. I hoping its enough to stop it running away lol, ill try in the morning.

EDIT: It was enough, no more worying about run aways.
```

---
## \#9 Posted by: lrdesigns Posted at: 2018-08-27T09:04:09.985Z Reads: 44

```
Finally had a chance to test your theory. And you were right after adjusting my mid point in BLDC to 1500ms the problem was gone. I also needed to re-set the settable fail safe as now it was putting the brakes on.  

Also you get get more adjustment range by adjusting the internal pots. 

https://www.electric-skateboard.builders/t/help-motor-is-running-without-remote-being-on/29172/8?u=lrdesigns
```

---
