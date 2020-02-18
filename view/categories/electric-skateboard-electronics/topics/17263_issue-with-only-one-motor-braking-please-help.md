# Issue with only one motor braking, please help!

### Replies: 7 Views: 623

## \#1 Posted by: Radium73 Posted at: 2017-02-05T20:23:57.450Z Reads: 66

```
For reference, I'm using a SpaceCell Pro4, two Vescs from Enertion, Steez remote, and dual Carvon v2.5 motors.

The problem happens when going directly from throttle to brake. When I do this, only the master Vesc brakes, and the slave just coasts to a stop. When I throttle, then let off to neutral, then brake, both motors work. I don't understand what would cause this, and I haven't been able to find any similar issues on the forums.

Here is video of the [Braking Issue](https://youtu.be/bwDZScnJP8s).

Thanks in advance for any insight!

Also, I'll try and get a new build page put up for this board sometime soon!
```

---
## \#2 Posted by: Hummie Posted at: 2017-02-05T20:53:27.744Z Reads: 58

```
likely your settings are different on both your vescs and you need to adjust them
```

---
## \#3 Posted by: Radium73 Posted at: 2017-02-05T20:58:48.525Z Reads: 59

```
That was my first thought! I have looked over them both a hundred times by now, and I'm almost 100% sure they are the exact same, other than controller ID. I will look once again to be absolutely sure.

I have also tried different canbus cables, and moved the receiver location with no luck
```

---
## \#4 Posted by: Ackmaniac Posted at: 2017-02-05T23:38:00.170Z Reads: 45

```
Just post Screenshots from your Motor, BLDC, Advanced, Application General and PPM tab of both VESCs. 
I guess you activated PPM on the slave VESC. The Controller needs to be disabled on the slave and only "Send status over can" should be activated. But also the stuttering at the beginning is a bit much.
```

---
## \#5 Posted by: Radium73 Posted at: 2017-02-06T22:12:43.089Z Reads: 30

```
I did have PPM selected on the slave VESC, I changed that but it is still happening. I am not getting stuttering anywhere near as bad as in the video I posted anymore, only slightly, and only after I brake immediately after throttle, and then throttle again.

Here are screenshots from BLDC of my settings, starting with the Master VESC:

<img src="/uploads/db1493/original/3X/3/8/3801f18d832afe7ac0d3857cbc332d5b81204065.png" width="690" height="431">
<img src="/uploads/db1493/original/3X/8/0/8087b4024893cd6c00848c9e7940216d893a5277.png" width="690" height="431">
<img src="/uploads/db1493/original/3X/8/1/8184e8b245bf385ef68ae7bcad56966e91c13dba.png" width="690" height="431">
<img src="/uploads/db1493/original/3X/6/a/6a83bbe428853b9aa6bdbd08b2d4b41b29285765.png" width="690" height="431">
<img src="/uploads/db1493/original/3X/6/7/674e524003cb4bd0ca2e3eae2044f373ceba315c.png" width="690" height="431">

Slave VESC:
<img src="/uploads/db1493/original/3X/4/3/431bdf1579f619b9a3557b9fe86386633ad142aa.png" width="690" height="431">
<img src="/uploads/db1493/original/3X/0/e/0e9558610724c087930ef2863b8a41a729ca9243.png" width="690" height="431">
<img src="/uploads/db1493/original/3X/2/f/2fd5de5785c9ce13aa67c3102db9acd82a0c1884.png" width="690" height="431">
<img src="/uploads/db1493/original/3X/f/9/f9bf13ce9c04e17fa248aeeac4e16bb332c40db0.png" width="690" height="431">
<img src="/uploads/db1493/original/3X/d/6/d6fda629dffae2a9a5e49daf1176f7a4d79b98b2.png" width="690" height="431">
```

---
## \#6 Posted by: Ackmaniac Posted at: 2017-02-06T22:55:17.354Z Reads: 25

```
* Disable "Send status over CAN on the Master"
* Set the "Maximum input voltage" to  57 V on both VESC (That is not the maximum of your battery, it is the maximum the VESC can handle, so set it to 57 and i think your problems are solved)
* Set the Battery cutoff start to 30V on both
* Set the Battery cutoff end to 28V on both
* Set "Min ERPM" in Motor Tab to -60000 on both
* Set "Max ERPM" in Motor Tab to 60000 on both
* Make a motor detection for both VESC in the BLDC tab. Do that by pressing start detection and when it shows that the detection was successful press the apply button afterwards. But disable the controller in the PPM tab first. Otherwise the remote disturbs the motor detection
* Your startup boost is quite high, set it down to 0.03 for the beginning
* The "Min ERPM" in the BLDC Tab is a very sensitive value. Please set it to the standard 150 and try if your motor startup is better on the bench.
* Adjust in the PPM Tab you minimum pulsewidth and the maximum pulsewidth (please check the forum how to do that the right way)


Once you made all those changes and it works nicely you can switch to my firmware and do all that stuff again. You can also do that now or later. The good thing is that you see the benefits after you used the standard firmware.
```

---
## \#7 Posted by: Radium73 Posted at: 2017-02-07T05:52:14.287Z Reads: 20

```
This did the trick! Thank you so much!! Brakes also feel a lot smoother and more reliable now, and top speed felt a little higher as well, but might have just been from full charge. It started raining here, so I only got to test for about 10 minutes.

Again, thank you thank you!! This is probably some of the most fun I have ever had in my life!
```

---
