# FVT Sleeping Lion Dual ESC 8-12s RC Issue

### Replies: 15 Views: 295

## \#1 Posted by: artSkate Posted at: 2018-12-19T03:34:35.539Z Reads: 75

```
Hello skateboard builders.  My **FVT sleeping lion Dual ESC** keeps on loosing connection with my controller (just for a few seconds). Im using this ESC in a mountain board.  I've tried two different controllers and receivers, but the problem persists.  Here is my set up:

dual 6364 kv200 motors
10s5P Li-Ion Pack 15Ah
Mini Skateboard Remote/receiver 2.4ghz


In the middle of riding my mountain board, the ESC starts emitting beeping sounds, as if it has lost connection.  (that also jolts my board and throws me off of it).  Sometimes it happens under big load, sometimes not much load at all.  Keeping my remote (hand) closer to controller seems to help.  BEC voltage is 4.92V.  I tried changing it to 6v with FVT usb link, but the BEC voltage remains at 4.92.  My guess is my receiver is not getting enough voltage.  I will try an external power supply to my receiver.

Has  anyone had this problem before?  Any suggestions on how to fix this are much appreciated.  Thanks.
```

---
## \#2 Posted by: J0ker3366 Posted at: 2018-12-19T03:42:50.491Z Reads: 66

```
I'd advice to go back over every connection. Being an emtb you deal with a lot of vibrations. You could have a faulty connection and when you hit bumps, its disconnects. If your esc beeps like it lost power, then its definitely not your remote. Re check all connections with a voltmeter.
```

---
## \#3 Posted by: artSkate Posted at: 2018-12-19T03:49:55.537Z Reads: 63

```
Thanks.  I'll check all connections.  The beeping that ESC makes is the same beeping when I turn off the transmitter (remote), but receiver is still connected.  For example, if I turn off my controller, but esc power is still on, esc (actually motors) starts to beep and jolt until I either turn the remote back on or turn off power to the esc.
```

---
## \#4 Posted by: J0ker3366 Posted at: 2018-12-19T03:51:19.904Z Reads: 55

```
Open your controller and check those connections as well. Mainly the battery connections @ the batteries and the pcb. But check them all.
```

---
## \#5 Posted by: artSkate Posted at: 2018-12-19T03:53:00.598Z Reads: 44

```
Thanks, will do.
```

---
## \#6 Posted by: dareno Posted at: 2018-12-19T04:34:43.720Z Reads: 44

```
Try a range test on the board.  By that I mean a remote range test.  Stand off the board and see how far the board remains connected.  Sounds like a receiver antenna issue.  Could be interference in the wiring or blocked signal.
```

---
## \#7 Posted by: Nate Posted at: 2018-12-19T05:24:56.905Z Reads: 42

```
That beeping sounds like a software issue. Which software version are you using?
```

---
## \#8 Posted by: MoeStooge Posted at: 2018-12-19T13:20:47.959Z Reads: 35

```
If your esc has data logging turn disable it. Had an esc In the past would audible when it reached the end of logging and do what your describing.
```

---
## \#9 Posted by: artSkate Posted at: 2018-12-19T13:36:18.027Z Reads: 38

```
Morning.  Did the range test.  Only get about 10 feet before loosing connection.  Receiver antennae is brand new with brand new receiver.  I did not alter it in any way.  I tried a receiver without antenna (that come with mini remote), and tried one with antenna, the one with antenna seems to be a bit better.  I tried keeping the receiver in the esc enclosure, and outside esc enclosure.  There was not a whole lot of difference between the two location.  I'll keep on working on it today.  Thanks.
```

---
## \#10 Posted by: artSkate Posted at: 2018-12-19T13:38:59.213Z Reads: 39

```
Im using the latest software fvt website has listed on it (actually the only one listed on it).  I did read in forums here that a previous version was working better for most people.  I dont know where to look for it.
```

---
## \#11 Posted by: artSkate Posted at: 2018-12-19T13:40:59.630Z Reads: 33

```
Thanks.  I'll check it out.  I dont think programming software FVT provides has this setting.
```

---
## \#12 Posted by: Nate Posted at: 2018-12-19T21:48:16.696Z Reads: 31

```
DM me your email. I’ll send you the workable version
```

---
## \#13 Posted by: artSkate Posted at: 2018-12-19T22:32:26.999Z Reads: 28

```
Thanks Nate!

DM Done
```

---
## \#14 Posted by: artSkate Posted at: 2018-12-20T19:19:38.074Z Reads: 24

```
I have resolved RC issue.  After trying a cascade of different approaches here is what worked for me:

1.  Putting receiver outside my esc enclosure.

2.  I have RF proofed the esc enclosure.  I lined the esc enclosure walls with sticky foil tape (same tape they use for insulating AC ducts).

3.  This one had the biggest impact (I think doing this alone may have solved my problem.  I took my controller apart and checked the antennae that was in there.  I then tried putting that antennae on the outside of the remote.  This improved RC signal a bit.  Lastly, I took an old receiver antennae from a receiver that no longer worked.  I swapped that receiver antennae with transmitter antennae.  That made a huge difference.  My range went from 8 ft to 20 ft.  There were no more problems with dropped RC signal, even if an obstacle got in the way of the transmitter and receiver.

Hope this helps someone else.  Ill try to post a video of my modifications on this thread.
```

---
## \#15 Posted by: artSkate Posted at: 2018-12-20T19:28:12.780Z Reads: 21

```
https://www.youtube.com/watch?v=uOlDoRoJI6k
```

---
