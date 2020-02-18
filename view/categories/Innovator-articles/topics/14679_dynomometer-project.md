# Dynomometer Project

### Replies: 18 Views: 1833

## \#1 Posted by: KMeyerson Posted at: 2016-12-14T20:46:29.520Z Reads: 208

```
Hello All!

I am again going to start a larger dialogue about BLDC motor design. Thanks to the support in my Hub Motor Design thread, we have made progress and have come to a consensus that an affordable, DIY dynamometer is in order.

The nature of this project is currently in the air. I would like to claim ownership of the designs at this point until further notice, but would like to share them with the community for feedback.

Quicky Design (5 minutes in Solidworks):

<img src="/uploads/db1493/original/3X/1/2/12e6757f341c2d02629fab16b1000e06a00a7bf3.png" width="467" height="500">

<img src="/uploads/db1493/original/3X/0/3/0397ad5e31778cdc4be521ea24243701c681bc03.png" width="516" height="474">

<img src="http://www.electro-tech-online.com/attachments/dyno_dynamometer-png.75647/" alt="Source: www.electro-tech-online.com">

Design Goals for E-Skate (NOT MOUNTAIN BOARD) Version:

* Support for 50-120mm Wheels
* Variable Load and Logging by VESC (Probably going to wait for the 6.0 for accurate results).
* Support for BELTED and HUB drives.
* More to come. I'm busy, but I'll keep chipping away at this.
* EASY TO MILL - Aluminum or Steel plates with bolts. Easy to water/laser cut in bulk.
```

---
## \#2 Posted by: jmasta Posted at: 2016-12-14T21:39:46.993Z Reads: 192

```
It would be interesting to directly measure the torque of your board.  However this is dependent upon the coefficient of friction between the wheels and their contact surface.  I expect the max torque transfer to much higher from urethane to asphalt, than urethane to smooth aluminum.  In addition, rider weight would be another confounding variable 

Your dynamometer would be useful for comparing other systems in a controlled environment.  It would almost be like a standardized baseline.  But keep in mind, the results would relative to one another and not a true measure of real world performance.  You may be able to derive or approximate a scaling factor to account for contact surface and rider weight 

Interested to see how it turns out. Good luck!
```

---
## \#3 Posted by: KMeyerson Posted at: 2016-12-14T22:55:43.379Z Reads: 162

```
I'm sure I can find a compound with a mu close enough to asphalt to coat the drum with.  The triangle is the preliminary arm that connects the drum to the vertical post.  By increasing the tension that pulls/pushes the drum into the wheels, you can simulate various ride weights. The variable BLDC motor used for a simulated load would be mounted on the triangles third, unused corner.

I've put some thought into solving some of these problems. I'm sure more will appear the longer I work on this. Keeping this simple but practical.
```

---
## \#4 Posted by: KMeyerson Posted at: 2016-12-14T23:14:04.301Z Reads: 147

```
Second note:

I didn't check the numbers, but here you go: [General Friction Factors on File](http://www.engineeringtoolbox.com/friction-coefficients-d_778.html).

As I move into more nit-picky stages of this design, we'll pick a few combinations to try out that are close to "dry tire" vs "dry pavement".
```

---
## \#5 Posted by: Pedrodemio Posted at: 2016-12-14T23:34:15.577Z Reads: 147

```
http://www.electric-skateboard.builders/t/hub-motor-design-simulations/13112/117?u=pedrodemio

http://www.electric-skateboard.builders/t/hub-motor-design-simulations/13112/121?u=pedrodemio

<img src="/uploads/db1493/original/3X/5/6/56f1b8e6770c69914d75dd1392e63dd96c49b46a.JPG" width="375" height="500">
```

---
## \#6 Posted by: Trillium Posted at: 2016-12-15T08:18:03.087Z Reads: 114

```
Mine is more rigid of a setup so I can load the crap out of the truck. In mine, the motors are tensioned orthogonally off the wheel surface, so you get more consistent traction with all wheel sizes.

I built it this way mainly so that I can do long duration mechanical validation of the whole system, including the truck and my special urethane assembly.

I would suggest you focus on the software side. I'm willing to share plans for mine at some point when the software is right. I have like 6-7 vescs lying around to use if you were planning on programming those.
```

---
## \#7 Posted by: KMeyerson Posted at: 2016-12-16T19:03:15.473Z Reads: 93

```
I've got a handful too. I don't plan on using VESC 4.12 because of its hardware limitations.

VESC 6.0 or maybe the Infinity ESC. We'll see, holidays are here and I'm going to have less time to work on this.
```

---
## \#8 Posted by: barajabali Posted at: 2016-12-16T19:28:56.079Z Reads: 90

```
It would be nice for a 203mm wheel ;) I
```

---
## \#9 Posted by: KMeyerson Posted at: 2016-12-16T20:05:40.953Z Reads: 84

```
That's monstrous.  I like it.  Then again, at that size you might as well build a mountain board.
```

---
## \#10 Posted by: barajabali Posted at: 2016-12-16T20:22:22.268Z Reads: 77

```
That's what I want it for my Trampas!
```

---
## \#11 Posted by: KMeyerson Posted at: 2016-12-16T20:47:59.092Z Reads: 69

```
125mm by 70mm wheel right? So a huge amount of space to work with. I don't own any rims to dimension or build with, but if I did I'd be happy to work on a large motor.
```

---
## \#12 Posted by: Okami Posted at: 2016-12-16T22:14:26.800Z Reads: 68

```
[quote="KMeyerson, post:7, topic:14679"]
Infinity ESC.
[/quote]

Is this an Esc I have not heard of ? Or it was just meant as a joke.. to non-existing esc ?
```

---
## \#13 Posted by: KMeyerson Posted at: 2016-12-16T22:25:29.540Z Reads: 68

```
See Raphael Chang Infinity ESC development on this forum and on his website.

It's experimental, requires debugging, and a lot of assembly. If you dont feel confident assembling your own VESC or programming it manually, you should stick with the VESC platform.
```

---
## \#14 Posted by: Okami Posted at: 2016-12-16T22:28:13.101Z Reads: 61

```
Cool. Will look into that! Actually you are the first one from which I hear about such esc!

i know ''robot'' ppl do make their own esc's and such.. so yeah, did not know there are other ''diy'' escs around besides the vesc..
```

---
## \#15 Posted by: KMeyerson Posted at: 2016-12-16T22:32:18.408Z Reads: 55

```
There's a lot of development HAPPENEING above and below ground.  You have to look for it though.
```

---
## \#16 Posted by: Okami Posted at: 2016-12-16T22:39:06.563Z Reads: 60

```
I had seen these ''batman'' bms.. somehow missed the infinity esc..

@KMeyerson  Thanks for showing / reminding that something like that exists..

----
I know that most chinese and a lot of other eboard manufacturers basically design and make their own ecs's.. At least it looks to be that way unless they use some ''common industry'' designs / esc's, which are not available to the public but are available to the enterprises / engineers.
```

---
## \#17 Posted by: KMeyerson Posted at: 2016-12-17T06:04:30.583Z Reads: 56

```
The infinity is on the back burner.  

At a glance, one of the biggest advantages we should see from the infinity is the higher ERPM compared to the hardware limited 60K ERPM supported by the VESC.

Only time will tell.
```

---
## \#18 Posted by: Pedrodemio Posted at: 2016-12-17T10:52:22.088Z Reads: 54

```
Did you see the new video from Vedder? If I remember correctly he was running FOC at 150k Erpm
```

---
