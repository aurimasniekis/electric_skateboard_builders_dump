# Strange Winning remote behaviour

### Replies: 10 Views: 1570

## \#1 Posted by: Jakeii Posted at: 2016-09-19T15:43:32.107Z Reads: 164

```
Any help would be appreciated!

Iv'e done the correct (afaik) binding procedure, connect to VESC connect binding pins, turn on remote while holding binding button, removing binding jumper.

And then this happens:
https://www.youtube.com/watch?v=OSyPZzpzHfk&feature=youtu.be

pushing forward does nothing, but if I bring it backward then towards the middle the motor goes for it! I have to hold backwards to stop it.

I've tried rebooting all bit of kit and rebinding

I hope it's something obvious I've missed because I don't want to wait for a new remote :cry:

VESC Settings:
<img src="/uploads/db1493/original/3X/0/a/0a9ff042b9709b937f8967650cd8cbc1a40903b2.PNG" width="690" height="408"><img src="/uploads/db1493/original/3X/8/3/83ff0ae748f13b40bdd03c3c16de897bb384888a.PNG" width="690" height="408">
```

---
## \#2 Posted by: JohnnyMeduse Posted at: 2016-09-19T15:46:53.064Z Reads: 140

```
did you set your "PULSEWIDTH" using the display ?... Also have you run motor detection ?
```

---
## \#3 Posted by: JohnnyMeduse Posted at: 2016-09-19T15:49:18.967Z Reads: 144

```
Maybe this will help you... 
http://www.electric-skateboard.builders/t/vesc-faq-setting-up-receiver-and-brakes/244
```

---
## \#4 Posted by: Jakeii Posted at: 2016-09-19T15:49:31.474Z Reads: 139

```
How do i know what the pulsewidth should be?

Yes, I've done motor detection.

thanks!
```

---
## \#5 Posted by: JohnnyMeduse Posted at: 2016-09-19T15:57:12.531Z Reads: 132

```
You need to use the display... It different for every remote, it depend on how the trim is set. Follow the video inside the link I sent you.
```

---
## \#6 Posted by: Jakeii Posted at: 2016-09-19T15:58:15.206Z Reads: 127

```
Aha! Watching now, It's making sense now cheers,
```

---
## \#7 Posted by: jesser722 Posted at: 2016-09-21T05:46:09.766Z Reads: 86

```
Having the same problem but my motor just makes noises and trys to go when getting started from a stop. Any ideas to fix it?
```

---
## \#8 Posted by: Jakeii Posted at: 2016-09-21T07:02:45.805Z Reads: 82

```
The video solved my issues, have you watched?
```

---
## \#9 Posted by: Eckles Posted at: 2016-12-02T17:56:06.396Z Reads: 53

```
I have exactly the same problem as Jakeii although after following the videos instructions I still have the same problem, the motor just guns it when I press the brake. Any ideas? has could there be other settings interfering?
```

---
## \#10 Posted by: gaetjen Posted at: 2016-12-02T21:30:47.926Z Reads: 41

```
You can also adjust the throttle when you rotate the screw under the red light. It makes it easier to center your pulsewidth
```

---
