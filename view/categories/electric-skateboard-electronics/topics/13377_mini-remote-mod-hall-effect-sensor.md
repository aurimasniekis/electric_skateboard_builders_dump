# Mini Remote Mod (Hall Effect Sensor)

### Replies: 20 Views: 3315

## \#1 Posted by: chinzw Posted at: 2016-11-20T19:30:01.955Z Reads: 381

```
Hey guys! I finally got some time to get started on this. I will be posting pictures and info as i progress with the design and development.
For this iteration i went with what i had in hand (SS495A from honeywell), its rated 4.5V min, but for some reason it just works with the 3.3v the remote uses. I will change it for a 3.3v rated sensor later down the road, just for peace of mind more than anything else.
As for powering the remote, im using sparkfun's powercell which can output 3.3v or 5v and a 1Ah lipo pack (again, what i had lying around)

Anyways, here's where im at right now:

<img src="/uploads/db1493/original/3X/8/d/8d2458be4080129f51bad1b88ec5502f89f11dd4.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/5/7/579be69ad28ee95d46486205ebebdd0cff428fcd.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/e/9/e99091867cb43483443b21bc67de91b7900b2eb2.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/b/5/b5bbe3925f1638d9f36833f46a6f7de6645aaeb6.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/c/3/c32c8044cc78b050f45bc9feec7cbba493e0d504.jpg" width="666" height="500">

Stay tuned! Ill be posting more progress very soon, ill be working on this all of today hopefully!
```

---
## \#2 Posted by: chinzw Posted at: 2016-11-20T22:59:26.346Z Reads: 356

```
Some more iterations, still not happy with the design, so im printing a double spring version to see how it feels!

<img src="/uploads/db1493/original/3X/3/3/33a187c180bf46e1e5215c5a09ab164cc5a3002e.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/f/6/f6aba7758fc551c16b26dd8e1c226b3186d6f37a.jpg" width="666" height="500">
```

---
## \#3 Posted by: chipoi84 Posted at: 2016-11-20T23:05:45.617Z Reads: 339

```
You should design it like this remote with lcd and everything. It also uses hall sensor. https://www.youtube.com/watch?v=1jJkVAt6YOw
```

---
## \#4 Posted by: chinzw Posted at: 2016-11-21T01:14:31.289Z Reads: 340

```
That, at the moment is just an arduino with an lcd. I dont want to design a new remote, i just want to mod the mini remote to something more user friendly.
```

---
## \#5 Posted by: chinzw Posted at: 2016-11-24T09:05:10.736Z Reads: 326

```
So, i've made quite a bit of progress! Everything seems to be working fine. I need to get some softer springs since just by coincidence, a screw sits right below a magnet and even without springs the wheel returns to center :slight_smile:

Here's the current design:
<img src="/uploads/db1493/original/3X/0/3/033f88cc5c4ee4d92698d1d962ecdd9cd8821dcf.jpg" width="600" height="500"> 
<img src="/uploads/db1493/original/3X/0/a/0ad93cb1bd248b31a3fc7fb7152e21ea1ddd2d29.jpg" width="600" height="500">

And here's the "almost" finished remote:
<img src="/uploads/db1493/original/3X/c/f/cf10e78f362773353ba92bc43c683c4870ea7bd0.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/c/3/c30103c94053e48783313c3e1a1a4a9ff9f7e845.jpg" width="666" height="500">

I had to do some quick modifications for fitment, like cutting a slot for the sensor cables and a relief for the on/off switch. Already have the changes made to my design and will print new cases tomorrow!
```

---
## \#6 Posted by: chinzw Posted at: 2016-11-24T09:11:55.005Z Reads: 299

```
Also, some extra pics for size comparison!

<img src="/uploads/db1493/original/3X/c/6/c649ffd98fdaa8c85254aa1daae5d1be6addabc3.jpg" width="374" height="500"><img src="/uploads/db1493/original/3X/3/3/33fc68c0cb6e194113cccb576592da01172b2667.jpg" width="374" height="500">
```

---
## \#7 Posted by: saul Posted at: 2016-11-24T10:55:20.938Z Reads: 280

```
Really nice. I got distracted from my mini remote mod but I have the same hallsensor working on a diy power glove + mini remote pcb.

I thought about doing the boosted wheel thing but i don't have any springs and didnt want to rely on printed springs...

I have some more ergonomic designs that already have the pcb cutouts 
this is what happens when you keep designing instead of just making a box that works :joy:


http://www.electric-skateboard.builders/t/banana-mote-minitx-3d-printed-enclosure-v0-2-thumb-wheel-ws2801-rgb-led-voltage-meter/10401
```

---
## \#8 Posted by: chinzw Posted at: 2016-11-24T17:49:47.345Z Reads: 257

```
I saw thread! Haha, got a bit derailed!
At the moment im focusing on the functionality of the design rather than ergonomics (altough, it feels great in the hand). I've already added an index finger cutout so that it sits nicer.
On my next version i will probably rotate the thumbwheel assembly 45 degrees so that it matches how our thumb stays at rest (like boosted remote).
Im also planning on flipping the pcbs over so that the on/off switch is on the same side as the thumbwheel. The only problem is that i basically need to rebuild the whole design, its gotten too messy after so many tweaks haha!
```

---
## \#9 Posted by: saul Posted at: 2016-11-25T20:30:00.334Z Reads: 234

```
Yea I had to rewrite mine a few times. But now I have 5/6 styles of controllers to pick from 😂
```

---
## \#10 Posted by: Sarky1 Posted at: 2016-11-25T20:55:07.095Z Reads: 229

```
Would it be worth adding a dead man switch like boosted ?
```

---
## \#11 Posted by: chinzw Posted at: 2016-11-25T21:43:38.390Z Reads: 226

```
@saul haha, yeah, that happens a lot, i usually keep old designs for a bit then just throw them away.
 
@Sarky1 It wouldn't be tricky to do, since the way these remotes work cutting the return from the hall sensor would effectively set the remote to neutral.
I will be redoing the design for a more comfortable fit, and im thinking just using the same shape and thumbwheel design as boosted, so i can add a deadman's switch to it as well.
```

---
## \#12 Posted by: chinzw Posted at: 2016-11-29T16:15:09.062Z Reads: 224

```
Little update. I decided I'm not too fond of springs, so why not stay with the theme and use more magnets? :smile:

<img src="/uploads/db1493/original/3X/3/5/358625e117f419eceaa61917ed2a42bc5bf88a61.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/5/f/5fd32a6e196e12cff662533023b4797edab9c79d.jpg" width="666" height="500">

Everything becomes simpler and the motion is buttery smooth. Checked the hall sensor and it seems unaffected by these extra magnets!
```

---
## \#13 Posted by: Qwiksand Posted at: 2016-11-30T22:13:21.945Z Reads: 199

```
Awesome work here! How are you finding the reliability of the remote/receiver connection, any drops? As good as the GTB2?
```

---
## \#14 Posted by: chinzw Posted at: 2016-11-30T22:16:16.860Z Reads: 201

```
I haven't done any street testing yet, im still running the gt2b until i have some time to print new cases for this new revision. From what i've read here in the forum, the mini remote is as good as the gt2b. The only thing i can see that seems a bit crap is the on/off switch, its just a cheap one; Mine actually works when it wants to i have to solder a new one.
```

---
## \#15 Posted by: NickTheDude Posted at: 2016-12-04T04:14:06.902Z Reads: 198

```
:heart_eyes: Damn, that things awesome.
```

---
## \#16 Posted by: saul Posted at: 2016-12-04T15:29:12.148Z Reads: 190

```
I like the magnet! how much travel can you get with this setup?
```

---
## \#17 Posted by: chinzw Posted at: 2016-12-05T05:01:57.665Z Reads: 182

```
@NickTheDude thanks!
@saul it's got 60 degrees of rotation travel, so the same as a gt2b steering pot
```

---
## \#18 Posted by: phrancini Posted at: 2018-05-14T07:35:53.383Z Reads: 111

```
I'm having problems with this mod. I'm using the same remote and hall sensor just a different case but the concept is extacly like yours.

Everything worked fine for like 2 hrs but then something strange happened, it looked like the throttle stuck open, so the board would keep accelerating and i wasn't able to brake nor going in neutral. at all.

I thought that could be a calibration issue, so i recalibrated my esc/remote and doing so it took a couple of tries because the esc wasn't "sensing" the brakes, and again it worked fine for a couple of minutes, but then again, the same thing happened. I think it could be a sensor/remote issue since if I switch the remote off, the board goes to neutral. 

Any idea of what the problem could be? it seems like the hall sensor get "polarised" like a magnet..
```

---
## \#19 Posted by: chinzw Posted at: 2018-05-14T16:28:46.150Z Reads: 92

```
Try replacing the hall sensor, these sometimes go bad (its rare, but it happens)
```

---
## \#20 Posted by: phrancini Posted at: 2018-05-14T16:47:31.967Z Reads: 92

```
So it seems. Now when I try to calibrate it doesn't recognize one of the magnetic poles on either side. When I get home I'll measure the voltage drops.. Unfortunately I don't have spares atm. I'll have to wait for them to arrive..
```

---
