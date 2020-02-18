# Board accelerates too fast, how do I slow it down?

### Replies: 14 Views: 1490

## \#1 Posted by: toma Posted at: 2017-07-25T03:29:14.173Z Reads: 206

```
Hey Everyone,


I have a custom built board that uses two enertion FOCBOXes (Vesc-x), some hub motors and 8 "ligo" battery packs (Each "ligo" is a 10s1p 18650 battery pack with it's own BMS).

The board accelerates WAY too fast, it's scary. How do I dial it down using BLDC_TOOL?

Do I just limit the current from the motor configuration?

Here is my config:
<img src="/uploads/db1493/original/3X/9/1/919831059988d90863e7015b862da32e68e0a4d7.png" width="690" height="385">
<img src="/uploads/db1493/original/3X/2/6/262e834e77bcbbcf115b2f8e51fc9235396d82a2.png" width="690" height="385">
<img src="/uploads/db1493/original/3X/f/2/f2da558dcaa60465634271732622d2a3e661e3d0.png" width="690" height="385">

<img src="/uploads/db1493/original/3X/9/2/926549dceefdc10b1d3b1226d2a8bec5c8a7dac1.jpg" width="666" height="500">
```

---
## \#2 Posted by: Jinra Posted at: 2017-07-25T03:31:09.556Z Reads: 198

```
You have to calibrate your remote every time you turn it on. Simply throttle back and forth all the way before it pairs (or after) and you should be set. Just be careful not to have it pair while you're in the middle of throttling
```

---
## \#3 Posted by: lrdesigns Posted at: 2017-07-25T04:24:02.165Z Reads: 189

```
If still too much power try going down on battery amps this will lower max system power. Try 10 amps and work you way up 2amps at a time till it feels right.
```

---
## \#4 Posted by: Jinra Posted at: 2017-07-25T04:33:18.537Z Reads: 184

```
amps are actually a bit low for hubs. The remote calibration is definitely the issue.
```

---
## \#5 Posted by: bartroosen12 Posted at: 2017-07-25T09:21:47.405Z Reads: 165

```
Damn 10S8P? :open_mouth:
```

---
## \#6 Posted by: Maxid Posted at: 2017-07-25T09:25:50.768Z Reads: 159

```
Use @Ackmaniac's firmware and set a throttle curve - issue solved
```

---
## \#7 Posted by: Silverline Posted at: 2017-07-25T09:32:47.367Z Reads: 152

```
Can the Ackmaniac fw be flashed to the vesc via BLDC tool ?
```

---
## \#8 Posted by: Maxid Posted at: 2017-07-25T10:40:53.109Z Reads: 144

```
It needs a special BLDC Tool and can then be flashed just as usual.
It is all in the thread here:
https://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286/
```

---
## \#9 Posted by: Silverline Posted at: 2017-07-25T12:38:32.896Z Reads: 115

```
Thanks, i have a look.
```

---
## \#10 Posted by: toma Posted at: 2017-07-25T16:08:04.305Z Reads: 109

```
[quote="Jinra, post:4, topic:28565"]
The remote calibration is definitely the issue.
[/quote]

I ended up recalibrating the remote and dialing down the "motor max" to 20A and "motor min (regen)" to -20A. It's way better now.

[quote="bartroosen12, post:5, topic:28565, full:true"]
Damn 10S8P?
[/quote]

8x10s1p
Here is a link to the battery: http://www.ebikes.ca/product-info/ligo-batteries.html

[quote="Maxid, post:6, topic:28565, full:true"]
Use @Ackmaniac's firmware and set a throttle curve - issue solved
[/quote]

I'll have to check it out.

Thanks everyone.
```

---
## \#11 Posted by: Jinra Posted at: 2017-07-25T16:10:08.757Z Reads: 103

```
I honestly think the settings you had before were better even then there were kind of low for hubs. just try the calibration first before anything else and remember you have to do it every single time you turn on the remote
```

---
## \#12 Posted by: lrdesigns Posted at: 2017-07-26T03:35:45.923Z Reads: 90

```
[quote="Jinra, post:11, topic:28565"]
I honestly think the settings you had before were better
[/quote]

Yeah, its recommended to have a high motor amps and to limit power via battery amps. Like 50a motor and 20a battery.
```

---
## \#13 Posted by: toma Posted at: 2017-08-17T13:12:24.719Z Reads: 64

```
[quote="Jinra, post:11, topic:28565, full:true"]
I honestly think the settings you had before were better even then there were kind of low for hubs. just try the calibration first before anything else and remember you have to do it every single time you turn on the remote
[/quote]

You are mistaken. I tried everything you recommended and things did not improve. And I don't have to re-calibrate every time I turn the board on.
```

---
## \#14 Posted by: Deckoz Posted at: 2017-08-17T21:20:55.211Z Reads: 48

```
Ackmaniac's frmware, Watt mode and throttle curve. yep, its that simple. :)
```

---
