# \[Solved\] Torque Boards nano-remote always at full throttle&rsquo; VESC

### Replies: 11 Views: 1708

## \#1 Posted by: P3rk Posted at: 2017-03-16T08:56:40.927Z Reads: 150

```
Hi team,

I have waited a good 6 months to get all of the parts I need for my first esk8 and I have finally come to put it all together.
I have already searched the forum but if this problem has been listed previously please send me a link and I will delete this post.
Parts I am using:
-torqueboards 6355/190kv motor
-vesc 4.12 firmware 2.18
-enertion spacecell 3
-nanoremote bought from  

I have got to the stage where I am attempting to program my remote. I would like for the throttle to be 'off' when my thumb control is in the center position (this is where it bounces back to when you let it go) however currently my motor powers to full throttle with the remote in this middle position. I have messed around with settings in PPM but have not found the answer.
I would like to be able to go forward (duh) as well as reverse and have no input when the thumbstick is in the center position but just don't know what I need to be changing to do it. :( If anyone knows what I'm on about I would be eternally grateful for any assistance.

P3rk
```

---
## \#2 Posted by: Deakbannok Posted at: 2017-03-16T10:20:10.430Z Reads: 139

```
Use BLDC tools to change the settings on your VESC.


http://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286/
```

---
## \#3 Posted by: P3rk Posted at: 2017-03-16T11:28:36.799Z Reads: 124

```
Yes that had occurred to me. I could not find a tutorial which goes through the parameters I need to change.
```

---
## \#4 Posted by: flywithgriff Posted at: 2017-03-16T13:44:37.225Z Reads: 115

```
It's an easy fix, I had the same issue! You need to set your remote parameters in the BLDC. Let me find the tutorial video and I'll link it here. Give me a bit to find it.
```

---
## \#5 Posted by: flywithgriff Posted at: 2017-03-16T14:07:57.370Z Reads: 109

```
Follow the steps in this video. It will show you how to set the nano remote to neutral throttle at the center resting point on the thumb control.

https://youtu.be/OtuofrQr3F8
```

---
## \#6 Posted by: P3rk Posted at: 2017-03-16T20:00:58.823Z Reads: 88

```
Legend! Thanks so much.
```

---
## \#7 Posted by: DanSkates Posted at: 2017-03-16T22:48:59.678Z Reads: 84

```
Hey @P3rk did you manage to figure it out?  I've finished my first build and had exactly the same problem, checked everything setting in BLDC and couldn't stop it going full throttle for no obvious reason!  I have the same remote too and all it was, was the little accelerator adjustment in the remote just needed turning anti clockwise slightly to calibrate correctly:

<img src="/uploads/db1493/original/3X/4/d/4df89b22ace8b5c812091a4f5f044dd3fe23c072.png" width="404" height="315"> 

 You may be more experienced than me and have already checked this but sharing just in case you haven't as it caught me out! :slight_smile:
```

---
## \#8 Posted by: P3rk Posted at: 2017-03-16T23:17:26.985Z Reads: 75

```
Thanks Dan I thought this might have something to do with it but don't have a screwdriver to fit it! I'll pick one up this afternoon.
```

---
## \#9 Posted by: DanSkates Posted at: 2017-03-16T23:29:42.216Z Reads: 75

```
Ah yeah if you've not adjusted it yet that'll defo be it!  It was a bit of an AHAAAAAA moment when I adjusted it :smile:
```

---
## \#10 Posted by: DanSkates Posted at: 2017-03-28T05:47:18.524Z Reads: 57

```
Hey @P3rk did this solve the problem?
```

---
## \#11 Posted by: P3rk Posted at: 2017-08-15T01:18:06.123Z Reads: 39

```
Hey guys sorry been MIA 
yes that did solve the problem! thanks a bunch guys.
```

---
