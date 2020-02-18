# Motor has no power SOLVED

### Replies: 14 Views: 397

## \#1 Posted by: Babisco Posted at: 2017-12-27T21:02:05.136Z Reads: 103

```
Hi guys just finish building my first eks8, and i can't figure out why it has no power. when i put my hands on the well it's just stuttering.

parts that i've used:

Sk3 190kv 63mm motor
VESC
Two Zippy 8000mah 30c batteries in series 
Torque boards remote

I've done a motor detection and here are my settings for now. 

<img src="/uploads/db1493/original/3X/e/9/e9d2acddeeeeaf3f857c35c057c88216f25a5feb.png" width="690" height="431"><img src="/uploads/db1493/original/3X/1/e/1eaf1becb5f5b1831275d1df82e34f42f2ce35f6.png" width="690" height="431"><img src="/uploads/db1493/original/3X/8/2/82357607f7a5d0e436bd0baa1d34f99171c1e2c6.png" width="690" height="431"><img src="/uploads/db1493/original/3X/2/1/21bcee628a8abcbe1bbb7b71ded3151540f9e9d6.png" width="690" height="431"><img src="/uploads/db1493/original/3X/8/5/85bf4bc7c10921ca839af7544270e23c0d67108b.png" width="690" height="431">
```

---
## \#2 Posted by: Sebike Posted at: 2017-12-27T21:10:27.599Z Reads: 81

```
Trying to spin up the motor with remote or keyboard?
Was motor detection successful?
```

---
## \#3 Posted by: Babisco Posted at: 2017-12-27T21:19:00.451Z Reads: 77

```
i could not use the keyboard to control the motor when the remote was connected, but disconnected it worked fine :slight_smile:
```

---
## \#4 Posted by: Sebike Posted at: 2017-12-27T21:20:39.518Z Reads: 73

```
yeah. 500 chars
```

---
## \#5 Posted by: Babisco Posted at: 2017-12-27T21:23:00.775Z Reads: 72

```
sorry but i dont understand, any easy fix or is the remote shhit?
```

---
## \#6 Posted by: Sebike Posted at: 2017-12-27T21:27:32.879Z Reads: 72

```
I thought you found the solution yourself.  need to disconnect remote to control motor by keyboard. cant use both at once. or maybe this isn't your problem?

uncheck send status over can unless youre using that
```

---
## \#7 Posted by: Babisco Posted at: 2017-12-27T21:29:29.134Z Reads: 71

```
the problem is that the board won't carry me, the motor is just stuttering when there is weight on it :slight_smile:
```

---
## \#8 Posted by: Sebike Posted at: 2017-12-27T21:32:15.179Z Reads: 68

```
just at stand still startup or still stuttering if you kick start it?

you running 10s ?
```

---
## \#9 Posted by: Babisco Posted at: 2017-12-27T21:34:20.247Z Reads: 66

```
yeah running 10s, kick start there is no prob, still startup = stuttering, as i said my first build, maybe this is normal?
```

---
## \#10 Posted by: Sebike Posted at: 2017-12-27T21:34:57.254Z Reads: 65

```
normal for sensorless
```

---
## \#11 Posted by: Babisco Posted at: 2017-12-27T21:36:40.446Z Reads: 62

```
okay, thanks for your time :slight_smile:
```

---
## \#12 Posted by: Sebike Posted at: 2017-12-27T21:42:00.048Z Reads: 58

```
sure. next time you have an issue (and you will, believe me :wink: ) try using the search function on your top right before starting a new thread. a "motor stuttering on startup" would have given you this same answer i no time. Good luck with your new board
```

---
## \#13 Posted by: Babisco Posted at: 2017-12-27T21:43:18.514Z Reads: 55

```
thanks again and thanks for the advise, i'll keep in mind :)
```

---
## \#14 Posted by: onepunchboard Posted at: 2017-12-27T23:22:09.630Z Reads: 42

```
u can change the start up boost to 0.04 and it will have better stand start.
```

---
