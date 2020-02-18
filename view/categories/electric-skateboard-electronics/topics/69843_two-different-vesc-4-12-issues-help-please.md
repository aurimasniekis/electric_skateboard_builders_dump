# Two different vesc 4.12 issues&hellip; help please?!

### Replies: 11 Views: 235

## \#1 Posted by: RonnyFox Posted at: 2018-10-02T13:07:43.116Z Reads: 69

```
Vesc 
Low voltage output
Continuity

Hi guys, I am having multiple issues with 2 flipsky vesc 4.12 units. One is taking in 42V and putting out 26.4V and the other just randomly popped the fuse in the antispark while I was riding and locked up the motors..?? When I replaced the fuse and plugged the motor back in it immediately popped again.... there is massive resistance in the motor without connection to the battery so tested for continuity and only get a reading on one of the phases. No idea what is happening but pretty sure I’m without a board atm!! 😫😰
```

---
## \#2 Posted by: Andy87 Posted at: 2018-10-02T13:10:40.248Z Reads: 67

```
could you give us some more information?
```

---
## \#3 Posted by: RonnyFox Posted at: 2018-10-02T13:15:41.999Z Reads: 67

```
![image|281x500](upload://9zJBJqH211Mfpx0KZ2VIuQXOZ7n.png)
```

---
## \#4 Posted by: Kug3lis Posted at: 2018-10-02T13:41:36.922Z Reads: 59

```
Looks like broken windings inside motor which shorts and causes vesc to short too which probably if havent yet killed vesc kills fuse every time you plug it in
```

---
## \#5 Posted by: RonnyFox Posted at: 2018-10-02T17:10:30.571Z Reads: 38

```
Idk man the motor still runs fine when connected to the other vesc... seems unlikely that would be possible if windings were fuct...?
```

---
## \#6 Posted by: dareno Posted at: 2018-10-02T17:45:10.165Z Reads: 40

```
[quote="RonnyFox, post:5, topic:69843"]
man the motor still runs fine when connected to the other vesc…
[/quote]

While this is basic troubleshooting and tempting its really not a good idea to connect a suspect motor to the other vesc to test it.  Sounds like a phase issue tbh.  
@b264 whats that process for testing phases on motors?  
Also and this is a long shot based on another members issue but check the capacitor connections on the vesc.  He was having stuttering and resistance problems and found one of the vesc caps had a broken connection.  Worth a look.
```

---
## \#7 Posted by: b264 Posted at: 2018-10-02T19:00:22.149Z Reads: 33

```
[quote="dareno, post:6, topic:69843"]
whats that process for testing phases on motors?
[/quote]

Disconnect the motor from everything and disregard the sensor cable, if present.

Connect phase A to phase B and verify by hand spinning that there is choppy braking
Connect phase A to phase C and verify by hand spinning that there is choppy braking
Connect phase B to phase C and verify by hand spinning that there is choppy braking
Connect phase A to phase B to phase C  and verify by hand spinning that there is strong, smooth braking

If any of the first 3 brakes feel different, the motor has an issue.  They should feel *identical*.  The last brake should feel smooth and not be cogging.
```

---
## \#8 Posted by: dareno Posted at: 2018-10-02T19:08:51.193Z Reads: 28

```
What he said :point_up_2:
```

---
## \#9 Posted by: Kug3lis Posted at: 2018-10-02T19:10:04.299Z Reads: 27

```
[quote="RonnyFox, post:5, topic:69843, full:true"]
Idk man the motor still runs fine when connected to the other vesc… seems unlikely that would be possible if windings were fuct…?
[/quote]

[quote="RonnyFox, post:1, topic:69843"]
there is massive resistance in the motor without connection
[/quote]

Well you said you have resistance, so maybe blown mosfet?
```

---
## \#10 Posted by: RonnyFox Posted at: 2018-10-03T02:39:46.872Z Reads: 18

```
Would a blown mosfet have that effect? The motor seems fine and has continuity when tested without connection to vesc.
```

---
## \#11 Posted by: RonnyFox Posted at: 2018-10-03T02:41:49.583Z Reads: 17

```
And does anyone have any ideas about the other vesc and the 26v output? I don’t even know where to start with that issue!? 🤦🏼‍♂️
```

---
