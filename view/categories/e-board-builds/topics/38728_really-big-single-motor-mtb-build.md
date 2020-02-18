# (Really) Big Single Motor MTB Build

### Replies: 17 Views: 1345

## \#1 Posted by: gavferry Posted at: 2017-11-19T03:39:59.678Z Reads: 187

```
So I race drones and walking to get them when i crash (which is often) is way too much effort :slight_smile: so i've started working on a setup using a rather large motor i have laying around
https://hobbyking.com/en_us/turnigy-rotomax-50cc-size-brushless-outrunner-motor.html (172kv)
<img src="/uploads/db1493/original/3X/9/9/998dd1212747d0f2e3d6c29677a277d323a34d52.jpg" width="565" height="414">
i know it's a bit ridiculous but it's what i've got, plus it should look pretty cool on my mountain board (190mm/7.4 inch wheels)
i was thinking to limit output with voltage, esc settings and if necessary, an arduino controller to limited pwm values (arduino going on anyway for lighting system etc
anyway the attachments are underway, drive belt etc is the next task, i'm guessing from other posts 15mm 5mm pitch is the way to go... my motor has a 10mm shaft though so i think the normal pulley wheels are no good
Could any of you help me with what and where to get, for both pulleys and the belt... I'm getting a bit confused with what to aim for in regards teeth/ratios etc.
Many Thanks
```

---
## \#2 Posted by: Kug3lis Posted at: 2017-11-19T03:59:23.286Z Reads: 178

```
Ahmm first thing either you put this motor at the end of board, cut the board to fit it or it will not fit. Second if you not going to provide it with decent front support (bearing or etc) it will brake axis.
```

---
## \#3 Posted by: Kug3lis Posted at: 2017-11-19T04:01:50.959Z Reads: 176

```
P.S. you don't limit output with voltage its ESC job to do it
```

---
## \#4 Posted by: PredatorBoards Posted at: 2017-11-19T04:39:53.255Z Reads: 163

```
The answer you are looking for is chain-drive.
```

---
## \#5 Posted by: DilatedPupils Posted at: 2017-11-19T04:41:22.809Z Reads: 158

```
Single drive on mtb is not good either.
```

---
## \#6 Posted by: gavferry Posted at: 2017-11-19T04:45:36.987Z Reads: 152

```
Motor is going at the end, metal mounting being made coming from bolt connecting truck to board, and connected to securely to the truck.
using threaded rods between truck and motor mount to make adjusting tension easy
```

---
## \#7 Posted by: Kug3lis Posted at: 2017-11-19T04:46:33.992Z Reads: 150

```
The motor axis will break this way, motor design was not intended to have side load
```

---
## \#8 Posted by: gavferry Posted at: 2017-11-19T04:47:34.909Z Reads: 147

```
Output limiting I meant by altering what lipo i shove on it,
Predator boards, I was thinking chain drive could be good, any idea on sizes of the cogs
And I know one wheel drive isn't great but I fgur d I'd try like this and upgrade later
```

---
## \#9 Posted by: MysticalDork Posted at: 2017-11-19T04:48:07.204Z Reads: 138

```
That motor has its shaft coming from the can end of the motor, rather from the mount end. This will result in a large bending moment unless something is done to support the shaft.
```

---
## \#10 Posted by: Kug3lis Posted at: 2017-11-19T04:49:00.730Z Reads: 135

```
And how are you going to alter lipo voltage which gets fed to esc?
```

---
## \#11 Posted by: gavferry Posted at: 2017-11-19T04:53:45.849Z Reads: 126

```
Ok, I think I could get a bracket on the end to support the shaft, it is ridiculously thick though (1cm)
Regarding lipos, I've a crazy amount of them of all different sizes, I can feed in 6s to 12s whatever is needed, although if my calculations are correct I'd be breaking the (motorway) speed limit on 12s with this motor
```

---
## \#12 Posted by: Kug3lis Posted at: 2017-11-19T05:11:52.825Z Reads: 116

```
Just forget this motor not worth it (Its made for driving propellers), go with 6384 or 6374 almost same power
```

---
## \#13 Posted by: MysticalDork Posted at: 2017-11-19T05:12:56.063Z Reads: 113

```
Speed is determined by your gear ratio, AND your wheel size, AND your motor kv, AND your battery voltage. You've only stated two variables here.
```

---
## \#14 Posted by: b264 Posted at: 2017-11-19T05:21:28.285Z Reads: 115

```
Honestly this motor is for an aircraft propeller.  The best way to use it for a mountain board is to sell it and buy two 6374 motors.

Edit: it's not because it's too big necessarily, it's because the bolt holes are on the wrong end.  It's not made to take a load perpendicular to the axle (aka: belt or chain)
```

---
## \#15 Posted by: Cobber Posted at: 2017-11-19T05:31:29.849Z Reads: 112

```
[quote="b264, post:14, topic:38728"]
it's because the bolt holes are on the wrong end.  It's not made to take a load perpendicular to the axle
[/quote]

you can change the shaft though... re-mount it, make one... what ever
I changed the shafts in my scorpions
what does the other end look like, can you see the end of the shaft in the bearing?

but if you have the bits...
more trouble than i'd go to for a single... now if you had a pair :smiling_imp: for science and the drv gods
```

---
## \#16 Posted by: MysticalDork Posted at: 2017-11-19T05:58:56.191Z Reads: 108

```
I wonder how a vesc6 would fare against that beastie.... :imp:
```

---
## \#17 Posted by: gavferry Posted at: 2017-11-19T10:13:17.291Z Reads: 82

```
The crazy thing is this is the smaller of the 2 big motors I've acquired... The other is three times bigger, a 150cc equivalent... Figured that might be pushing it though :)
I was thinking of avoiding the vesc's as I didn't think they'd cope. Normal RC ESC for now (150a)
I hear what you guys are saying about the motor, im going to see if I can get a bearing and bracket on the end to support as using what I've got would be good
```

---
