# Changing the Capacitor on my VESC

### Replies: 14 Views: 1180

## \#1 Posted by: Jreamer Posted at: 2017-10-25T04:01:48.692Z Reads: 145

```
I got an aluminum case for my VESC's and they don't fit with the standard VESC capacitor that comes with the Torque Board VESC. The kit came with extra capacitors to replace the existing ones, but they are 560u instead of the 680u that the normal ones are. 

Does this matter? Can I safely change this?

<img src="/uploads/db1493/original/3X/3/a/3a3290eeb83418c9d7ebcce4f6e12846db6d9cc0.jpg" width="666" height="500">

Can't seem to get a definitive answer if this is ok.
```

---
## \#2 Posted by: scepterr Posted at: 2017-10-25T04:03:28.141Z Reads: 138

```
That's fine,  low esr rating preferred
I'm using either shorter 3x680uf that are on the bom they fit perfect or 2x1600uf, I haven't seen any difference in vesc behavior. 
<img src="/uploads/db1493/original/3X/5/6/565a779f707fcc9f0ef5611abc3e43c407751d6e.jpg" width="305" height="500">
```

---
## \#3 Posted by: evoheyax Posted at: 2017-10-25T04:14:53.780Z Reads: 127

```
[quote="scepterr, post:2, topic:36434"]
I haven't seen any difference in vesc behavior.
[/quote]

The problem is it depends on the motor, the load, ect.

I recently had my first cap problems from using too small of caps. The result was jittery, almost like cogging, in long sustained or high amp draw situations. Scary, especially at speed.

If you want to get the most out of our motors, like I told you, I would recommenced the larger caps. It's possible the smaller ones will work, especially if you use lower settings than I do.

But bigger is better when it comes to caps...
```

---
## \#4 Posted by: Cobber Posted at: 2017-10-25T04:15:30.121Z Reads: 128

```
what sort of loads are you running?
V & A cont./peak?

it is only a small reduction
I prob. wouldn't do it if you had a eMTB running a 6384 at 12s with 60cm battery leads...
but if your system is small, and scepy has modified his already so...

the caps are there to smooth out battery lead induced inductance spikes that could cook your esc
the longer your battery to esc leads are the more caps you will need to smooth out...
```

---
## \#5 Posted by: scepterr Posted at: 2017-10-25T04:17:00.343Z Reads: 118

```
I'm using either 3x680uf which is standard or 2x1600 which is more
```

---
## \#6 Posted by: Jreamer Posted at: 2017-10-25T04:21:50.454Z Reads: 115

```
Its going to be a dual 6354 16t 36t setup with a 12s2p samsung 30q battery pack. 

Evo said under heavy draw it can stutter, can I just limit the battery amps?
```

---
## \#7 Posted by: Cobber Posted at: 2017-10-25T04:26:01.845Z Reads: 113

```
the most important thing in my mind is to keep your battery to esc leads as short as you can

your system is moderate, so yes throttling it will help
what the magic numbers are I don't know
```

---
## \#8 Posted by: Hummie Posted at: 2017-10-25T06:10:18.033Z Reads: 101

```
this is the most uninformed forum compared to es or vedder's I'd ask there.   I've always thought of  the battery side as the purpose for the caps but maybe it's the motor side too.  maybe the battery is not able to produce the instant high amp demand smoothly to the motor and the caps enable that.
```

---
## \#9 Posted by: Jreamer Posted at: 2017-10-25T06:16:35.873Z Reads: 98

```
Links. I think I'm ready to jump to the next rabbit hole forum.
```

---
## \#10 Posted by: Cobber Posted at: 2017-10-25T06:21:37.139Z Reads: 96

```
I always thought the caps on the motor side were to deal with re-gen current coming back in to the esc @Hummie

shown for example here on a rc car esc on both motor and battery side...

 <img src="/uploads/db1493/original/3X/9/b/9bc7f8e5077c8196c9fcb4f7528b912d1d2d517f.png" width="690" height="468">

[quote="Hummie, post:8, topic:36434"]
this is the most uninformed forum compared to es or vedder's
[/quote]

yeah I'd have to agree, opinion is joined with fact, but thus is the internet

es link @Jreamer :
https://endless-sphere.com/forums/viewforum.php?f=21
```

---
## \#11 Posted by: Hummie Posted at: 2017-10-25T06:44:51.285Z Reads: 85

```
that image has  what looks like caps on both side of the esc which I've seen but is rare and I wonder what it's about.  caps on the motor side?
if you search for vedder vesc forum you'll find it. 

if you find any answers please pass them on
```

---
## \#12 Posted by: Cobber Posted at: 2017-10-25T06:55:56.063Z Reads: 81

```
as I said:

[quote="Cobber, post:10, topic:36434"]
I always thought the caps on the motor side were to deal with re-gen current coming back in to the esc @Hummie
[/quote]

braking spikes compared to throttle spikes...

if they are there just to control the current that enters then leaves the ESC why are they all not just on the battery side to protect the ESC?
```

---
## \#13 Posted by: Jreamer Posted at: 2017-10-25T06:56:49.103Z Reads: 76

```
[quote="evoheyax, post:3, topic:36434"]
I recently had my first cap problems from using too small of caps. The result was jittery, almost like cogging, in long sustained or high amp draw situations. Scary, especially at speed.
[/quote]

What Cap did you switch too? What do you run now? What was the setup that caused the jitters?
```

---
## \#14 Posted by: Hummie Posted at: 2017-10-25T14:29:56.335Z Reads: 64

```
the vesc is an example of having only big caps on battery side.
```

---
