# FOC box braking force increases at low speed

### Replies: 6 Views: 812

## \#1 Posted by: BigBoyToys Posted at: 2017-06-13T09:34:08.088Z Reads: 114

```
Hi all,

Ive been trying to get smoother braking on my 4wd board with out much success.

Braking from high speed works well but once the board has slowed down to about 5 mph, the braking force increases abruptly. 

Ive increased and decreased motor braking vs regen and havent been able to get rid of the issue. 

Ideas?

Brake settings:

Motor min: 30A
Regen: 12A
```

---
## \#2 Posted by: JohnnyMeduse Posted at: 2017-06-13T10:43:39.530Z Reads: 105

```
Have you try @Ackmaniac software... because it can give you the opportunities tu create a special curve for you brake or acceleration.
```

---
## \#3 Posted by: Ackmaniac Posted at: 2017-06-13T11:11:54.310Z Reads: 96

```
Guess you are using BLDC mode.
Set this value to 500 and try it again.
<img src="/uploads/db1493/original/3X/0/d/0d4c69710e4f2a4409cdb4b8192718e60fc80ea6.png" width="690" height="404">
```

---
## \#4 Posted by: Ackmaniac Posted at: 2017-06-13T11:18:59.918Z Reads: 92

```
So my firmware doesn't really make a change here. But with my firmware you could set up different acceleration and brake power for the front and rear axle. Let me know if you are interested. Need a test guinea pig because i don't have a 4WD (yet :grin:).
```

---
## \#5 Posted by: BigBoyToys Posted at: 2017-06-13T12:43:01.795Z Reads: 82

```
I havent tried yours actually but would love to. Sign me up please!

I will give the brake erpm settings a try and report back. Thanks

@JohnnyMeduse thank you.
```

---
## \#6 Posted by: Jebe Posted at: 2017-06-13T12:56:00.146Z Reads: 80

```
https://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286
```

---
