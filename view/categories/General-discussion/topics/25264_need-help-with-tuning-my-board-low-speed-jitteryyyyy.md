# Need help with tuning my board, low speed jitteryyyyy

### Replies: 12 Views: 606

## \#1 Posted by: Landshark Posted at: 2017-06-13T12:32:59.157Z Reads: 91

```
I recently moved up to Boston for the summer for work (downtown) and the reason I mention this is because trying to use my board this morning to grab coffee was a fiasco.

In Ft Lauderdale where I live I cruise around no problem but it seems here where there is a lot of braking and slow speed starting the board is really glitchy.

For example:
-When I brake at slow speeds the brakes just lock up, doesn't happen at higher speeds thankfully. At a higher speed the brakes are smooth.

-At a slow speed start, the acceleration is very jittery until I get moving a bit.  I've gotten used to giving two good kicks to get going but around here if I'm slowing down and then accelerating again it's really glitchy.

-Sometimes I'll try to accelerate or brake and nothing happens, feels like lost signal.

All these issues are very noticeable in a downtown environment.  So I'd like to get my slow speed settings dialed in so I don't freak out...as much.

I am running BLDC with hybrid sensors on the Focbox X from enertion and have a nano remote.
```

---
## \#2 Posted by: anorak234 Posted at: 2017-06-13T13:11:55.705Z Reads: 84

```
You'll want to post pictures of your FOCBOX settings to allow members to assist you in potential corrections for fixing the problem(s)
```

---
## \#3 Posted by: TarzanHBK Posted at: 2017-06-13T13:25:22.257Z Reads: 75

```
I had the not-so-smooth-on-sensors problem, did a new motor detection with the sensors and everything is fine since then :slight_smile:
```

---
## \#4 Posted by: Landshark Posted at: 2017-06-13T14:32:59.175Z Reads: 74

```
I did lower my battery cutoff start/end to 36/33.6

<img src="/uploads/db1493/original/3X/f/a/fa96ba78b9fdffd944d8086dd5434f1a399caff0.png" width="690" height="431">


<img src="/uploads/db1493/original/3X/d/b/db7bd6d09f5f86690f5990c931ee764a19fe80d6.png" width="690" height="431"><img src="/uploads/db1493/original/3X/c/f/cf6135380a52e48263ca348093c307f72e03710c.png" width="690" height="431">

<img src="/uploads/db1493/original/3X/0/8/083064b45ccd60c8a723d82f6ef32770c8329cf0.png" width="690" height="431">

<img src="/uploads/db1493/original/3X/2/c/2c3cc768e21f492611f810543deaef6f5082e9f8.png" width="690" height="431"><img src="/uploads/db1493/original/3X/6/d/6dd591ee0414b2a00f3e69d28a686178873848f8.jpg" width="690" height="431"><img src="/uploads/db1493/original/3X/1/2/12650950ff06b8cae9dbcb1bc5baa7165fc1ed5b.png" width="690" height="431">
```

---
## \#5 Posted by: t0m_r1dd1e Posted at: 2017-06-13T14:40:23.625Z Reads: 67

```
Lower your Min ERPM at full brake to like 150. That will lower the speed at which your brakes lock. Not sure about the other issues.
```

---
## \#6 Posted by: Landshark Posted at: 2017-06-13T14:47:00.515Z Reads: 67

```
I see a max ERPM at full break, do you mean this?
<img src="/uploads/db1493/original/3X/c/d/cd8f3844005b99ccaf98fdfddaa3d471ec5adb02.png" width="504" height="32">
```

---
## \#7 Posted by: t0m_r1dd1e Posted at: 2017-06-13T14:51:56.693Z Reads: 65

```
Oh yeah sorry that's what I meant.
```

---
## \#8 Posted by: Jinra Posted at: 2017-06-13T14:54:12.706Z Reads: 63

```
Why did you set your comm mode to delay?
```

---
## \#9 Posted by: Landshark Posted at: 2017-06-13T15:06:30.778Z Reads: 63

```
That's what someone suggested I do...
```

---
## \#10 Posted by: Jinra Posted at: 2017-06-13T15:20:21.403Z Reads: 60

```
From Vedder himself

>Commutation mode should always be “Integrate”.
The other parameters are for RPM-based timing advance and some other things that aren’t necessary to adjust in the normal case, so I won’t explain them here yet.
For small low-inductance high-speed motors, the delay commutation mode can be used in case the integrate mode does not work.
```

---
## \#11 Posted by: Landshark Posted at: 2017-06-13T23:43:42.982Z Reads: 49

```
Well with your guys suggestions my board is running better than ever!

I lowered max brake erpm to 150 and reran motor detection with integrate selected instead of delay.

Board doesn't try and throw me into traffic anymore and those low speed jitters are gone, much smoother.

Thanks sooo much! My riding experience has greatly improved 👍
```

---
## \#12 Posted by: TarzanHBK Posted at: 2017-06-14T10:39:49.386Z Reads: 40

```
Have fun and wear your brain safety thing :slight_smile:
```

---
