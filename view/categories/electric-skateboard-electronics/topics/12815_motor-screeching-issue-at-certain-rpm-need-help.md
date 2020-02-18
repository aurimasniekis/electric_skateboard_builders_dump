# Motor screeching issue at certain RPM (need help)

### Replies: 16 Views: 1815

## \#1 Posted by: Tijmen Posted at: 2016-11-10T14:21:45.223Z Reads: 118

```
I have an issue with my motor. At a certain RPM (I'd say at about 70% throttle), it starts screeching loudly. Before and after this speed it runs fine. Video of it happening:

https://www.youtube.com/watch?v=3enCgApUqK0&feature=youtu.be

Does anyone have any idea what's causing this? I've opened up the motor and nothing seems broken and magnets are where they're supposed to be. I've also taken out the bearings, checked them, greased them and placed them back but no fix. I've run this motor countless times without this happening but now it happens all the time.
I must add that I had a similar noise when throttle was at maximum and batteries at about 70% or higher. I'd always avoid top speed and ride slightly under it to avoid this noise, but now it only happens at the slightly lower RPM.
```

---
## \#2 Posted by: XIII Posted at: 2016-11-10T17:49:43.414Z Reads: 101

```
I have the same thing with my motor from APS ! 
Maybe it's not made for these "higher" rpms and the natural frequency starts to vibrate ?
```

---
## \#3 Posted by: Tijmen Posted at: 2016-11-10T18:10:04.221Z Reads: 95

```
I have just figured out the issue (I think). The main issue I was having is that the ring holding the magnets in place on the outer part of the motor was coming loose, moving up, and making contact with the stationary part of the motor, causing them to grind together which is terrible but luckily hasn't damaged anything. Turns out the every single magnet except one is loose and is free to move up and down. I think and hope that this is also the reason for the screeching.
I will soon be working on securing the magnets back down and that should fix my issue.

I recommend you take your motor apart and check on the magnets. They may be coming loose which might not be an issue now but could be an issue in the future. Re-securing magnets however is one of the simplest fixes so don't worry if this does happen to you.
```

---
## \#4 Posted by: XIII Posted at: 2016-11-10T18:11:43.304Z Reads: 92

```
Will fix this , this weekend! Thanks !
```

---
## \#5 Posted by: Baz_L Posted at: 2016-12-24T10:41:05.648Z Reads: 78

```
Bump. I have a very similar issue, did your fixes solve the problem?
```

---
## \#6 Posted by: laurnts Posted at: 2016-12-24T17:08:39.819Z Reads: 76

```
I recommend bearing replacement. Because this motor are too simple in construction, no electronics and no moving parts. If you switch esc, it still occured, then it's definitely the motor.

When it gets worse over time even at the slowest speed, my best guess is bearing needs to be replaced.
```

---
## \#7 Posted by: Tijmen Posted at: 2016-12-27T12:06:05.160Z Reads: 74

```
I did fix the issue. I believe I made another post with pictures of the ring holding the magnets in place coming loose entirely, allowing the magnets to move.
I used some metal epoxy on each gap above the magnets before moving the ring back into place. It held pretty well, and the screeching was actually gone. I've since ordered an entirely new motor because this one's just messed up, but my best bet is that your magnets are actually coming loose, and at that RPM where it's screeching, it allows them to vibrate at a perfect frequency to screech like that. 

As someone else said, it's also possible it's the bearings, but for me it was the magnets. Somewhat of an easy fix though if you have the right tools laying around.
```

---
## \#8 Posted by: Baz_L Posted at: 2016-12-29T22:46:12.410Z Reads: 66

```
 I hadn't had a chance to look into it until yesterday. I went back and forth a couple of times in the living room, just messing about, and the motor failed. Out of nowhere it just began clicking (as if the magnets were rubbing against the coils), here's a quick video: https://www.youtube.com/watch?v=9jgq_bnqFD4

I took it apart today and it turns out that that is the issue.. There are scratch marks on the magnets and they have come loose a tiny bit. I've just emailed Maytech so I'll let you know when they reply. I've never contacted them before so I'm just hoping that they were cooperative..

Reglueing the magnets seems like a pain to do correctly, so I would much prefer a replacement if I can get one! :cold_sweat:
```

---
## \#9 Posted by: Tijmen Posted at: 2016-12-29T23:38:58.609Z Reads: 61

```
The thing with my magnets was that they slid up (notice space under magnets)
For reglueing I didn't take out the magnets are reglue. I simply pushed them down and put a dab of glue in the gap that it formed above the magnet. Once I did that to all magnets, I pushed the metal ring back down.

Your issue sounds different though. More like they've come loose and are coming further into the motor.

<img src="/uploads/db1493/original/3X/f/4/f4ed89d7f47d8d91f25c784842798fa3f1d4e7d5.jpg" width="375" height="500">
```

---
## \#10 Posted by: Baz_L Posted at: 2016-12-29T23:57:09.322Z Reads: 58

```
Mine have also come up a little bit, but it's much less extreme (about 0.5mm). So I cant put glue in the gaps. I also can't take off the ring and glue them then, because the balancing glue (the blue stuff) is actually covering the ring so I don't want to interfere with it. As you can see in the photo, it's mainly the tops of the magnets that are rubbing. I tried lining everything back up and reassembling but it didn't actually solve the problem (it actually worsened the sound a little bit), so I have my doubts about reglueing... I really need to hear back from Maytech to be honest.. :confused:  <img src="/uploads/db1493/original/3X/9/1/91aa161fcbbf9f619852e666247256d78828db02.jpg" width="666" height="500">
```

---
## \#11 Posted by: Baz_L Posted at: 2016-12-29T23:58:58.820Z Reads: 56

```
Also the bearings are absolutely fine so I know it's a magnet grinding issue..
```

---
## \#12 Posted by: Tijmen Posted at: 2016-12-30T00:58:51.621Z Reads: 54

```
Grind marks on magnets look very similar to mine (also visible on picture)
In theory, magnets moving up should not make the chance of them touching the inner ring of magnets any bigger. After I reglued my magnets, the whole outer housing got a slight wobble. I highly doubt that's because of the reglueing, but I believe it may be because the motor shaft is slightly bent.
The bent shaft could also be what initially got the magnets to get looser.

Honestly I'm just speculating at this point. I'm running on a new motor now thankfully. Currently trying to get it to work in sensored mode (something I haven't done before) and while doing so decided to test the old motor. Turns out it's so busted that it doesn't even work in sensored mode. Glad I bought the new motor.
```

---
## \#13 Posted by: Wilsonliang777 Posted at: 2016-12-30T02:29:23.395Z Reads: 51

```
I had the same issue with my motor a few weeks ago. I started my checking the bearing.  It was only later that I noticed the magnets were out of line.  I used a few drops of glues to hold it in place and have not had any problems with the motor.
```

---
## \#14 Posted by: Baz_L Posted at: 2016-12-30T10:23:18.876Z Reads: 48

```
What type of glue did you settle for?
```

---
## \#15 Posted by: Tijmen Posted at: 2016-12-30T12:10:31.955Z Reads: 48

```
<img src="/uploads/db1493/original/3X/1/6/16b8a0d8fc1e7a1665ebfa0a50d036a52bb4b489.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/7/a/7a2ad4efccd5df6cf867ca603ef1cb681b6d6977.jpg" width="375" height="500">
```

---
## \#16 Posted by: Baz_L Posted at: 2017-01-03T16:09:01.068Z Reads: 39

```
Update on my motor issue. Maytech actually replied to my email!! They're going to take it back and repair it for me. Hope they don't mind that I've disassembled it. Will post some updates on how it goes.
```

---
