# DIY Vesc not connecting, slight heat, flickering light on power up

### Replies: 18 Views: 1407

## \#1 Posted by: bigben Posted at: 2017-07-02T20:28:11.116Z Reads: 111

```
So, I have successfully set up and been using my enertion vesc 4 (4.18) on my 9s single drive system for a few months now.
I'm building another board that will be dual drive, and as I have 2 enertion vescs and 1 DIY I thought I'd set the enertions up as dual and set the DIY up on the existing system.
I set the 2 enertions up no problem for the dual drive.
So then proceded to get the DIY vesc out of it's bag, re solder the correct size connectors and get on with configuring it.
There just a flicker of light and that is all that it ever gave. A little blue and a little red. Nothing else. Undetectable by the vesc tool, the receiver seemed to power up though. Detected a little heat from the vesc so powered it down and wrote this?
I don't think It's a numpty mistake? Can anyone think of anything obvious? I have been using a 3s lipo as power. (correct polarity)
There seems to be no snap crackle or pop.
```

---
## \#2 Posted by: bigben Posted at: 2017-07-02T20:44:43.190Z Reads: 106

```
<img src="/uploads/db1493/original/3X/0/5/05ae94f1a8858f1ebe46983ac0c9df929fc03da5.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/4/5/454dadd88dedc8d3776846857ee2fe440d2088c2.JPG" width="375" height="500">
```

---
## \#3 Posted by: rpn314 Posted at: 2017-07-03T02:29:36.010Z Reads: 89

```
[quote="bigben, post:1, topic:26628"]
There seems to be no snap crackle or pop.
[/quote]

Good to know these guys aren't showing up!

<img src="/uploads/db1493/original/3X/2/8/288fe0e571bfa25cb1c6393b3d45a86d09126748.jpg" width="500" height="500">

As to your issue, it could be a bunch of things. The biggest flag indicative of a hardware issue is the heat. Where specifically are you detecting a little heat? And did you only see the LED flicker once or is it constantly flickering?
```

---
## \#4 Posted by: bigben Posted at: 2017-07-03T06:03:27.172Z Reads: 85

```
Thanks for getting back to me. The lights only flickered when I powered up.
The heat seemed to be coming from the "coil"? The little drum of copper wire?
```

---
## \#5 Posted by: rpn314 Posted at: 2017-07-04T01:52:51.978Z Reads: 72

```
Hmm. I think that is the large inductor, L1. The black circle above the large rectangular chip (DRV) and below the CAN connector? 
<img src="/uploads/db1493/original/3X/f/f/ff024d8071c532f0ddab6b8267de98ca12d977b4.png" width="690" height="468">
(from Vedder's GitHub)
```

---
## \#6 Posted by: bigben Posted at: 2017-07-04T05:20:31.679Z Reads: 65

```
<img src="/uploads/db1493/original/3X/8/f/8fdc454e9beeecc9776a52bc44960e537dea851d.png" width="690" height="468">
Yep, that's the one.
```

---
## \#7 Posted by: NAF Posted at: 2017-07-04T05:38:44.581Z Reads: 65

```
My L1 exploded a few days ago ...I've bought like them 10 of them now just to have spares for the future. I've replaced it and it seems like it's working all ok now.

Here is L1 part number if you need it:  652-SDR0805-220ML	They are very cheap. I've bought 10 of them :slight_smile:

http://www.electric-skateboard.builders/t/my-vesc-blew-up-but-still-works-perfectly-wtf/26378
```

---
## \#8 Posted by: bigben Posted at: 2017-07-04T06:02:20.543Z Reads: 64

```
That may or may not be the problem? That component seems to be just single stacked on mine? This vesc has never been connected or run a motor so could be a problem from new?
One thing I wanted to check is. On my enertion vesc I plug the hall sensor plug into the top plug as I did on this one.(green circle) but i have noticed there is an identical socket on the left of the vesc? (blue circle)
These plugs are left off of the enertion vescs.
<img src="/uploads/db1493/original/3X/e/8/e8bbd078f863343351403b651370b11867fb0ce0.jpg" width="375" height="500">
```

---
## \#9 Posted by: rpn314 Posted at: 2017-07-04T17:41:21.260Z Reads: 57

```
It's possible you've got some issues with L1 or even your DRV8302 chip (as that is powering the 5V line, where L1 is used, which then powers the 3.3V line which powers the microcontroller). 

Blue circle is only necessary for connecting an STLink-V2 to flash the bootloader. They may be similar pin counts, but they definitely serve very different (and not interchangeable) purposes. You should be fine without it.
```

---
## \#10 Posted by: bigben Posted at: 2017-07-05T19:01:02.149Z Reads: 49

```
@torqueboards I've been promised an email back before the end of the day in a few occasions now. Can you offer any help on this?
```

---
## \#11 Posted by: torqueboards Posted at: 2017-07-05T19:15:10.223Z Reads: 48

```
@bigben - Send me a PM with your order #/email.
```

---
## \#12 Posted by: bigben Posted at: 2017-07-05T20:27:43.647Z Reads: 46

```
What a gent. Thanks @torqueboards
```

---
## \#13 Posted by: bigben Posted at: 2017-07-28T06:40:40.327Z Reads: 39

```
@torqueboards did you get a chance to look at the vesc yet?
```

---
## \#14 Posted by: Da_gree Posted at: 2018-02-08T17:07:36.378Z Reads: 27

```
I'd love to see suggestions for this problem as well. Both my VESC's went dead while successfully bench-testing dual motor setup. Now neither one will light up when powered, despite the fact that the receiver is still getting power and linking up to remote. My coil gets warm on both esc's when powered up. Nothing is burnt, no magic smoke, but can't connect to BLDC tool or get any response whatsoever from either VESC. Sounds like exactly the same problem that @bigben  had. Can I just replace the coils on both boards - I'm 90% sure I can do it myself without causing any damage.
```

---
## \#15 Posted by: bigben Posted at: 2018-02-08T17:23:50.883Z Reads: 27

```
I didn't ever find out the problem, but had the vesc replaced without any quibbling.
```

---
## \#16 Posted by: Da_gree Posted at: 2018-02-08T19:21:50.851Z Reads: 22

```
Thanks, I sent diy an email.
```

---
## \#17 Posted by: rpn314 Posted at: 2018-02-08T19:22:46.266Z Reads: 23

```
The suggestions all involve being able to desolder surface mount components. I stand by my previous assessment:

[quote="rpn314, post:9, topic:26628"]
It’s possible you’ve got some issues with L1 or even your DRV8302 chip (as that is powering the 5V line, where L1 is used, which then powers the 3.3V line which powers the microcontroller).
[/quote]
```

---
## \#18 Posted by: Da_gree Posted at: 2018-02-08T20:37:43.667Z Reads: 18

```
Thanks rpn, I've done some SMD (successfully and unsuccessfully) on ebike controllers. I'm not as skillful as some, but I've watched plenty of videos and have had some successes. I know I'm new here, though.

I unwrapped one of the VESC's and, using an infrared thermometer, found that the source of the heat is actually on the exact opposite side of the L1: positions c43, c44, and c49 got up to 115ºF before I pulled the plug. Never any magic smoke, just hot components.

Is the proper etiquette to start a new thread? Apologies, I'm not an internet power-user. It appears my situation isn't quite the same as Ben's. I've got no flickering light at all on power up, but my receiver still gets power and binds. I heard I was supposed to keep it short and add photos.
```

---
