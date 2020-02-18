# Enertion VESC-X failing

### Replies: 20 Views: 1410

## \#1 Posted by: Daan_vZon Posted at: 2017-05-01T11:56:22.815Z Reads: 204

```
I just received my Enertion VESC. However, during setup, the VESC gave a 'fault' warning by a red flickering LED, after which a part of the VESC blew up by giving just a little throttle.
I have no idea how the error/failure occurred whatsoever though. I wonder whether anyone recognizes a similar problem with this VESC and/or knows how it could have occurred. I use a 10s Space Cell Pro4 battery and a 6355 260KV motor.

The photo underneath shows the damage/blown up part of the VESC. It's the part connected with the middle phase wire.
<img src="/uploads/db1493/original/3X/0/9/091e42db447dcdefe21f133ca6beb6b6bdcec6a7.jpg" width="281" height="500">
```

---
## \#2 Posted by: makevoid Posted at: 2017-05-01T12:13:37.173Z Reads: 192

```
looks like 1 fet completely burned, what were your latest vesc configs? post screenshots of motor configuration, advanced, and bldc/foc tabs depending on which mode you were
```

---
## \#3 Posted by: Daan_vZon Posted at: 2017-05-01T12:38:42.734Z Reads: 182

```
Yes it did indeed. I used FOC mode and read configuration at start for everything and didn't just change random variables. Here are my latest VESC configurations.

Motor tab:
<img src="/uploads/db1493/original/3X/7/2/72462bb3a684b316093e2d93b1f51ec1db7bd592.png" width="690" height="387">

FOC tab:
<img src="/uploads/db1493/original/3X/0/3/03a4c4c3a07e3576113c6fc2d65709cee9733598.png" width="690" height="387">

Advanced tab:
<img src="/uploads/db1493/original/3X/2/9/293ce601a067caa9dedaec21032859de3c877c53.png" width="690" height="387">
```

---
## \#4 Posted by: makevoid Posted at: 2017-05-01T12:39:24.064Z Reads: 177

```
did you do motor detection on FOC before trying to run the motor (detect and calculate parameters)?
```

---
## \#5 Posted by: Daan_vZon Posted at: 2017-05-01T12:43:18.246Z Reads: 176

```
Yes, I ran full motor detection on FOC before I even let the motor spin by myself once. Pretty sure I did that 100% like it should.
```

---
## \#6 Posted by: makevoid Posted at: 2017-05-01T12:44:46.606Z Reads: 172

```
parameters seem alright to me... maybe a bad mosfet (that component that burned)?
```

---
## \#7 Posted by: Daan_vZon Posted at: 2017-05-01T12:56:28.603Z Reads: 170

```
Ok great, then I know it wasn't me doing completely wrong things. I think the chance it was a bad part is the biggest too. Already luckily got a private message response from @EnertionSupport they want to send me a new PCB for replacement.
```

---
## \#8 Posted by: pyttroll Posted at: 2017-05-01T14:01:16.319Z Reads: 161

```
Not sure if that's the reason but you typically want to stay below 200kv with a 10S, and your ERPM limit is way too high, it should be 60K/-60K, you might have busted your VESC because you reached that limit...
```

---
## \#9 Posted by: Daan_vZon Posted at: 2017-05-01T15:10:53.844Z Reads: 151

```
Didn't spin the motor during setup at around so fast, so probably couldn't have bust it due to exceeding the ERPM limit. Will I be safe when limiting the max/min ERPM to 60K/-60K, without having to buy a lower Kv motor? And would this result in a major decrease in top speed or not so much?
```

---
## \#10 Posted by: pyttroll Posted at: 2017-05-01T15:12:17.238Z Reads: 147

```
I think it should be fine, I guess you'll lose a bit of torque compared to a 190kv motor.
```

---
## \#11 Posted by: Daan_vZon Posted at: 2017-05-01T15:14:22.793Z Reads: 143

```
Ok, that will have to do. I live in quite a flat area, so wouldn't need that much torque.
```

---
## \#12 Posted by: makevoid Posted at: 2017-05-01T16:14:16.195Z Reads: 131

```
well spotted
```

---
## \#13 Posted by: Skatenoob Posted at: 2017-05-09T19:42:52.687Z Reads: 119

```
Do you have any idea on how to accelerate faster? My board can push me from a full stop but it moves extremely slowly.
```

---
## \#14 Posted by: Daan_vZon Posted at: 2017-05-09T19:58:49.143Z Reads: 115

```
For faster accelerating you need more torque as far as I know. You can get more torques by using a lower KV rating motor, smaller diameter wheels, a higher ratio drivetrain (less teeth on the motor puley/more teeth on the wheel puley).
```

---
## \#15 Posted by: Skatenoob Posted at: 2017-05-09T19:59:52.864Z Reads: 110

```
I had a hobbyking esc before my vesc and it accelerated extremely fast but this is so slow, I think it's my programming or something
```

---
## \#16 Posted by: Skatenoob Posted at: 2017-05-09T20:01:44.686Z Reads: 109

```
 I own a maytech vesc and took it for my first ride today, I'm running with a sk3 245kv motor and my battery is a 5000mah 3s 20-30c battery (I run two in series). I have my max motor amps on 60 aswell as the battery and my start up boost is on 0.090 yet I'm still have trouble accelerating, it's very slow and I'd like a bit more kick. I weigh around 75kg and have not had problems like this on my previeous vesc, so if anyone knows how to fix my issue that would be greatly appreciated! Also my wheel pulley is 36 and my motor 16, my wheels are 90mm
```

---
## \#17 Posted by: Qwiksand Posted at: 2017-05-09T21:11:09.604Z Reads: 102

```
I had a similar experience switching to a VESC from an FVT. The RC controllers we commonly use don't limit amps (I was seeing spikes near 150 amps from the little FVT) and BLDC motor torque is directly related to amps, so of course, the cheapie/simple RC controllers will feel more powerful as they are outputting 2 to 3 times the torque depending on your VESC settings.

If you stick to 245kv motors, you'll need to run a dual set-up w/ VESCs to have a similar acceleration feeling to your single hobbyking ESC or you can maximize your VESC by running 12s on a 170kv motor (60k eRPM limit) and gear it appropriately- though it will still not be as punchy as your single, in my experience anyway.

This is the only weakness the VESC has when compared to RC esc's though; all the other customization options, not to mention reliable/quiet brakes, make it my favorite controller by far. Just have to know it's limits.
```

---
## \#18 Posted by: Skatenoob Posted at: 2017-05-10T06:35:06.185Z Reads: 89

```
It makes sense but I've seen you tubers get loads of torque from their single motor and a vesc, what's the max amp limit I can set it to? I just need to find that sweet spot I guess, but I find it odd that even thought the motor max amp is set to 60 the max it has pulled is only around 52a
```

---
## \#19 Posted by: Daan_vZon Posted at: 2017-05-10T17:21:06.126Z Reads: 83

```
The max amp limit will automatically be set when using 'read configuration' in the BLDC tool. Putting the given read value higher will most likely damage your electronics as far as I know.
```

---
## \#20 Posted by: Skatenoob Posted at: 2017-05-12T20:36:07.990Z Reads: 72

```
Thanks, my motor has never gone as high as pulling 60 amps, but my vesc isn't turning on not showing any lights nothing, it was working fine next day I turn it on run the motor for a bout 5 seconds and then it just stopped, no dodgy connections I was only pulling about 40amps and the vesc was around 30 c, now it doesn't do anything :(
```

---
