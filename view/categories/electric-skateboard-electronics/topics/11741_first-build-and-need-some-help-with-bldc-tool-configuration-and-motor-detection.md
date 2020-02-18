# First build and need some help with BLDC-tool configuration and motor detection

### Replies: 8 Views: 1241

## \#1 Posted by: moose Posted at: 2016-10-23T15:17:39.192Z Reads: 118

```
Hi!

After researching, ordering, waiting for the parts and building I've almost finished my first build. Loving this forum, taught me almost everything I've needed to know. Only thing left for me now is to get my VESC and motor to work properly and then finish my build with some enclosures. 

Unfortunately I'm not fully sure about my VESC setup in BLDC-tool, and I'm having trouble doing the motor detection. I could really need some help.

Here are a list of the parts I'm using:
2 x Turnigy LiPo 5000mAh  4s 25c batteries
Turnigy Aerodrive SK3 - 6364-245kv motor
Vesc v.4.12 with firmware v.4.18 from 

Here are some pictures of the board and my configuration in BLDC-tool. Also a video of the failed motor detection.

<img src="/uploads/db1493/original/3X/6/a/6a19de5b8c42f1cc21f5e82e144fddceaa099621.JPG" width="690" height="388">

<img src="/uploads/db1493/original/3X/5/5/55c4e12deed8a51f19d36ac40b32f842a2bcb26e.JPG" width="690" height="388">

<img src="/uploads/db1493/original/3X/4/a/4a1d18eddb53bd69c15d80f02ebb5a219d5a2a48.JPG" width="690" height="388">

<img src="/uploads/db1493/original/3X/c/7/c76e46ca252f6a6a54387f989f9821ee9417fd0d.JPG" width="690" height="388">

<img src="/uploads/db1493/original/3X/b/5/b5cc0c0e48f6355050a674e182cee018f553f44f.png" width="690" height="386">

<img src="/uploads/db1493/original/3X/6/0/6040fd5e4ca806589181a674a48267e7e7d45dfc.png" width="690" height="386">

https://youtu.be/s9Pu_PSzrPs


Appreciate all the help I can get!
```

---
## \#2 Posted by: ArmandR Posted at: 2016-10-23T16:12:31.856Z Reads: 98

```
@torqueboards
```

---
## \#3 Posted by: Jinra Posted at: 2016-10-23T16:19:36.073Z Reads: 100

```
after the failed detection go to the terminal tab and type 'faults'. Paste the result here.
```

---
## \#4 Posted by: moose Posted at: 2016-10-23T17:09:31.875Z Reads: 99

```
Here:

<img src="/uploads/db1493/original/3X/1/5/153d6c49f9cf0d26467d28e4c3a00087e0696a37.png" width="690" height="386">
```

---
## \#5 Posted by: Jinra Posted at: 2016-10-23T17:13:50.792Z Reads: 96

```
I helped someone with the exact same problem a couple weeks ago. We determined it was a bad VESC given that the motor detection worked fine with another VESC on the same motor and the settings were the same. Not exactly sure what the specific problem was though. We also tested a different motor on the same faulty VESC and it still failed.

Who's VESC are you using? Id contact their support
```

---
## \#6 Posted by: TarzanHBK Posted at: 2016-10-23T17:48:13.737Z Reads: 93

```
perhaps look at the solderings, because you have an overcurrent issue.
http://www.electric-skateboard.builders/t/vesc-147a-motor-current-abs-over-current-error/6483
```

---
## \#7 Posted by: moose Posted at: 2016-10-24T22:18:51.204Z Reads: 75

```
Thanks for the help! It was the soldering that was the problem (never soldered before this board...). The motor detection now works great, so now I'm just waiting for the Swedish October rain to stop.

Just to be on the safe side I figured I'd ask. Would you change any of the settings I've made, or does it seem fine?
```

---
## \#8 Posted by: sandrewvdv Posted at: 2016-10-24T22:23:30.979Z Reads: 71

```
-20 Amps on the battery regen seems a bit high? I know I'm using -12 A because I like a smooth stop. Maybe -15 A is a better choice.
```

---
