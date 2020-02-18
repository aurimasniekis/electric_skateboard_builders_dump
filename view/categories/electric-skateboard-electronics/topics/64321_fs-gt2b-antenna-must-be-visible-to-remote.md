# FS-GT2B - Antenna must be visible to remote?

### Replies: 12 Views: 324

## \#1 Posted by: multiplexor Posted at: 2018-08-09T06:53:14.061Z Reads: 99

```
Curious.... Does the Antenna need to be visible? With mine, I did a test... I had the board upside down in front of me. With the remote hidden behind my back, I pull the trigger and nothing... I try again making the remote visible and it starts the motors. I immediately put it behind my back and it let go of the trigger. Nothing happens, it keeps spinning at high speeds. I then make the remote visible to the antenna and bam it immediately comes to a stop.

I didn't think they needed that much of a line of sight?
```

---
## \#2 Posted by: telnoi Posted at: 2018-08-09T07:06:28.089Z Reads: 97

```
still worked within an enclosure in my case. Do check if part of the antenna is not broken.
Part of the antenna should be stripped so to speak (meshed wire removed exposing a solid core). That part is very fragile.
```

---
## \#3 Posted by: Acido Posted at: 2018-08-09T07:22:24.466Z Reads: 92

```
Do you have a carbon fiber deck?
Also to me it seems that you didnt set up the failsafe
```

---
## \#4 Posted by: Slak Posted at: 2018-08-09T12:11:29.877Z Reads: 72

```
First, set your failsafe up !
```

---
## \#5 Posted by: multiplexor Posted at: 2018-08-09T16:27:10.798Z Reads: 55

```
Ooo yes true I didn't do that yet. But either way even if I'm hiding it ng the remote simply behind my back, signal shouldn't be lost, no?
```

---
## \#6 Posted by: Mikenopolis Posted at: 2018-08-09T17:49:12.214Z Reads: 47

```
the GT2B had a long range so line of sight shouldn't really be an issue at that distance.

is this a modded remote? you might have a breakage in the antenna or loose solder joint. pictures?
```

---
## \#7 Posted by: multiplexor Posted at: 2018-08-09T19:37:51.001Z Reads: 41

```
naw, I'm still using the original controller. Haven't tried to mod it yet. The receiver antenna too is near the vesc's. Wondering if there's interference or something. Antenna looks totally fine too. I'll try to snap some pics this afternoon of the antenna
```

---
## \#8 Posted by: multiplexor Posted at: 2018-08-09T19:39:52.760Z Reads: 37

```
Oh and it's just a regular land yachtz, no carbon fiber :smiley:
```

---
## \#9 Posted by: multiplexor Posted at: 2018-08-20T05:03:48.792Z Reads: 34

```
So from my tests... The remote works great when the antenna is visible to the controller. However if I place my body between the remote and the antenna receiver, then it intermittently cuts out. As if it can't properly pass through my body. 

In my test, I cut a tiny tiny hole in the back of the board, passed the antenna through it. When i keep the remote in the back it's fine, if I move it in front of me it cuts out sometimes. if I place it in front, but visible to the antenna, it's fine.

soooooooooo weirddddddd
```

---
## \#10 Posted by: threebysix Posted at: 2018-08-20T05:07:15.346Z Reads: 33

```
Are you near a wifi router or home wireless phone when running this test? Those appliances also run on the same frequencies and will interfere with your signal.
```

---
## \#11 Posted by: multiplexor Posted at: 2018-08-20T05:28:32.054Z Reads: 31

```
oohhh hmmm I do have my cell on me. But I'm on the street when i'm testing. Not connected to any wifi. I'll have to try a test with my wifi on my cell disabled hmm
```

---
## \#12 Posted by: threebysix Posted at: 2018-08-20T05:34:26.648Z Reads: 31

```
oh I'm not sure if smart phones/smart phones on wifi will cause interference (signal is pretty weak on these things). I meant specifically wifi routers. My wifi router caused a lot of noise and dropped signals when I was setting up my remote. I was too close to my router and my receiver for my mini remote was picking up a lot of interference which caused my motor to spin sporadically. 

Is your enclosure carbon fiber by any chance? carbon fiber enclosures can also block out signals. 

If all else fails, open up your remote and take a look at its connections.
```

---
