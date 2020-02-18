# Need some help with my first e-longboard with schematic

### Replies: 22 Views: 2846

## \#1 Posted by: pcbacon Posted at: 2016-07-15T01:47:06.345Z Reads: 124

```
So I have all my parts on the way but I am having a little trouble with the schematic of my e-board. I have 2 5000 Mah 6s 30c lipo packs (Turnigy) I want to run them in Parallel but also want to not have to open the bottom up every time I need to charge the batteries I know you can charge in parallel. I am going to use a 3 position switch. I have a very rough copy of what I was thinking. http://imgur.com/Oyk5GmC
```

---
## \#2 Posted by: Blasto Posted at: 2016-07-15T01:51:00.426Z Reads: 128

```
All the current going to your esc will need to go through the switch, that's a lot of current for a switch to handle, it will need to be very beefy. Almost like a blade switch

<img src="/uploads/db1493/original/2X/4/464c19a80cb0fa8a0d226c5465c45a711776fb3c.jpeg" width="480" height="359">

You don't want a blade switch.

May i suggest having 2 xt60 connectors (one on each battery) and using a xt90 anti spark as a master switch
```

---
## \#3 Posted by: pcbacon Posted at: 2016-07-15T02:11:53.864Z Reads: 118

```
could you maybe draw me a schematic? so i can tell what you mean
```

---
## \#4 Posted by: Blasto Posted at: 2016-07-15T02:30:53.665Z Reads: 113

```
http://www.electric-skateboard.builders/t/beautiful-diagrams-no-words-just-pics/3179/3?u=blasto

Do what @emepror did

<img src="/uploads/db1493/original/2X/c/c24eced31c776ed31bb4198d8318bf3747f71998.png" width="478" height="500">

He put the balance lead in // , the xt60 charge port in // and used a xt90 loop key as a master switch

// = parallel
```

---
## \#6 Posted by: pcbacon Posted at: 2016-07-15T02:45:29.791Z Reads: 96

```
okay thank you do I have to take out the xt90 (cut off switch) to charge?
```

---
## \#7 Posted by: Blasto Posted at: 2016-07-15T02:46:19.076Z Reads: 96

```
Would be recommended, that will make sure you have no power to your esc
```

---
## \#8 Posted by: pcbacon Posted at: 2016-07-15T02:48:31.424Z Reads: 93

```
and one last question can I use two balance ports instead of soldering two together
```

---
## \#9 Posted by: Blasto Posted at: 2016-07-15T02:52:10.706Z Reads: 91

```
I wouldn't recommend that, since the your power leads are always in //.

You maybe can do a Y harness for the balance plugs if you don't want to cut them (understandable)
```

---
## \#10 Posted by: pcbacon Posted at: 2016-07-15T03:10:23.129Z Reads: 87

```
i couldnt find any y spliters for a 6s lipo
```

---
## \#11 Posted by: pcbacon Posted at: 2016-07-15T03:13:32.987Z Reads: 88

```
http://www.3drcparts.com/6x-parallel-split-jst-xh-6s-6-cell-balance-cord/
never mind I found one
```

---
## \#12 Posted by: Blasto Posted at: 2016-07-15T03:21:35.524Z Reads: 81

```
That would do, tape up the connectors you don't need. If you cut them off the risk of having some wire short together is greater.
```

---
## \#13 Posted by: pcbacon Posted at: 2016-07-15T03:30:15.919Z Reads: 83

```
alright thank you so much for your help man I don't think I have any other questions ill be building next week when everything arrives ill send some pics when i'm done.
```

---
## \#14 Posted by: emepror Posted at: 2016-07-15T22:01:35.762Z Reads: 70

```
I found a 6 cell Y splitter on i believe hobbyking, its been a while. the XT90 cutoff works great but I've gotten lazy and just leave it plugged in. I've had no issues with doing that. Also when you go to solder up the connector for the batteries, ESC, charge port, its basically a double ended Y.
```

---
## \#15 Posted by: pcbacon Posted at: 2016-07-16T02:00:31.837Z Reads: 64

```
alright man thanks for the help, I order a y splitter from Ebay it's on its way thank you for your help
```

---
## \#16 Posted by: pcbacon Posted at: 2016-07-16T05:11:08.041Z Reads: 63

```
okay wait I am a little confused about something so I have already ordered an 80Amp ESC and my batteries are 5000mAh 22.2v and 30c with a peak of 40c this means if I run them in parallel they will produce 300A will the ESC be fine with 300A even tho it's only an 80A ESC?
```

---
## \#17 Posted by: Blasto Posted at: 2016-07-16T05:14:21.794Z Reads: 58

```
Your batteries will be able to to burst up to 300A. But your motor will not pull no where near that current.

All depends on what motor you'll using
```

---
## \#18 Posted by: pcbacon Posted at: 2016-07-16T05:15:19.873Z Reads: 56

```
but is it fine like will nothing blow up?
```

---
## \#19 Posted by: JohnnyMeduse Posted at: 2016-07-16T05:20:31.678Z Reads: 59

```
No nothing will blow up, the motor will only take what it need. (it like a car with 900hp, on the freeway it will only use what it need to do the job)
```

---
## \#20 Posted by: pcbacon Posted at: 2016-07-16T05:21:54.984Z Reads: 60

```
okay okay thank you
```

---
## \#21 Posted by: pcbacon Posted at: 2016-08-08T23:29:44.402Z Reads: 59

```
Hi emepror I am having some trouble with replicating your schematic here is what mine looks like it doesnt turn on when i put in the xt90. <img src="/uploads/db1493/original/2X/c/cf01597af3137c1c3bfb176f22e3a8398499b5dc.JPG" width="375" height="500">
```

---
## \#22 Posted by: emepror Posted at: 2016-08-15T21:58:27.910Z Reads: 50

```
sorry for the late reply, you have the XT90 as a loop key correct? Also how do you have your batteries connected?
```

---
## \#23 Posted by: Davey Posted at: 2017-04-28T17:03:22.222Z Reads: 20

```
Sorry for gravedigging but how did this turned out?
```

---
