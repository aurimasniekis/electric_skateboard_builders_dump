# Fail-safe on Mini remote not working?

### Replies: 13 Views: 1048

## \#1 Posted by: slerm Posted at: 2017-08-20T15:41:33.573Z Reads: 151

```
I feel like I set everything up correctly in the bldcc tool. I set the pulsewidth correctly to where neutral is at 50% and max/min are base on reading in the tool. I bound the remote and then unplugged the loop key with the remote on, in neutral. 

However, I'm still having an issue with when it cuts out, the brake is applied for a half second which is terrifying when it happens going fast through an intersection. It always happens at intersections here in NYC (primarily in midtown), which I assume is from all the cameras and sensors interfering. Anyway, is there any way to avoid having the brakes applied? I'd prefer for it to just not respond. It never last more than a split second. ANy advise is appreciated.
```

---
## \#2 Posted by: evoheyax Posted at: 2017-08-20T15:54:11.008Z Reads: 146

```
Never had a drop out with the mini remote (though I ride through the hills of s in residential neighborhoods, not the downtown), so I can't say. Sounds terrifying though, cause I love traveling above 30 mph at all times possible, and I use this remote daily.
```

---
## \#3 Posted by: topherbarnett Posted at: 2017-08-20T17:06:53.727Z Reads: 141

```
By removing the loop key, you are not simulating a failsafe, but a loss of power. Try turning off the remote while running and let us know what happens. If it acts correctly, it sounds like maybe you're having power issues. Maybe overcharging?
```

---
## \#4 Posted by: slerm Posted at: 2017-08-20T17:24:00.048Z Reads: 133

```
No issue when I turn remote off while riding. 

When you says overcharging, are you referring to regenerative braking when on full charge? If so, I don't think that's it because this happens mainly on acceleration or just gliding, not when braking, no matter how charged my battery is. I've had the same issue with my metroboard previously which also uses the same remote.
```

---
## \#5 Posted by: topherbarnett Posted at: 2017-08-20T19:01:30.078Z Reads: 114

```
What ESC are you using? Are all your electrical connections solid?
```

---
## \#6 Posted by: slerm Posted at: 2017-08-20T19:43:06.218Z Reads: 112

```
FocBox, 12s2p 30Q battery, single 190kv 6374 motor

All of my connections seem solid, so I'm not sure what's going on. I assumed it was a loss of remote connection, but maybe not?
```

---
## \#7 Posted by: torqueboards Posted at: 2017-08-20T22:36:25.922Z Reads: 103

```
Try fail safe and setting the knob to about 2 oclock. https://www.youtube.com/watch?v=ywUfqtKF8Zg
```

---
## \#8 Posted by: Namasaki Posted at: 2017-08-27T02:36:22.620Z Reads: 94

```
[quote="slerm, post:1, topic:31104"]
I bound the remote and then unplugged the loop key with the remote on, in neutral.
[/quote]

What loop key are you taking about?  Do you mean the binding plug in channel 4 of the receiver ?
```

---
## \#9 Posted by: slerm Posted at: 2017-08-27T14:11:05.924Z Reads: 83

```
Correct. Meant bind plug, not loop key
```

---
## \#10 Posted by: Namasaki Posted at: 2017-08-27T14:49:29.145Z Reads: 80

```
It's probably not a failsafe issue then. 
Could be a wrong setting on Vesc
```

---
## \#11 Posted by: Ackmaniac Posted at: 2017-08-27T15:29:31.973Z Reads: 78

```
Do it exactly like in this video. It is important to remove the bind cable while the remote and board is still switched on. By this the receiver knows where your idle position is. You can test afterwards by switching off the remote and check the pulsewith signal in bldc-tool. It should still stay at 50%.

https://www.youtube.com/watch?v=ywUfqtKF8Zg

But that only adjusts your failsafe signal so that the board doesn't brake when it losses the signal. Afterwards you need to find out why you loose connection. Maybe you have a carbon fibre enclosure or your receivers cable is broken or the remotes potentiometer gives wrong signals when you squeeze and bend the remote a little.
```

---
## \#12 Posted by: Namasaki Posted at: 2017-08-27T16:36:12.182Z Reads: 69

```
[quote="slerm, post:4, topic:31104"]
this happens mainly on acceleration
[/quote]

I suspect that what you are experiencing may not be brakes at all but rather a sudden loss of torque during acceleration which can feel like brakes and can send you over the handle bars if you are not ready for it.
This could easily be caused by your battery's voltage sagging down to the cut off set in the bldc tool.
I'm curious what your voltage settings are.

Another possible cause could be that you have your ERPM limit set low and you have a check in the box by "Limit ERPM with Negative Torque" (This box is checked by default)
Your 12s and 190kv motor has a possible erpm of 67032 when the battery is fully charged.
If your erpm is set below 60k you might be triggering the negative torque.
Especially if your running very low gearing i.e. Large wheels and wheel pulleys with small motor pulleys

I may be right or I may be wrong, I'm just throwing some ideas at you.

These are the settings I use for 10s and 190kv
<img src="/uploads/db1493/original/3X/3/a/3a5259424316da51199d9d4c32e05821239bf1e0.png" width="611" height="471">
```

---
## \#13 Posted by: fliess Posted at: 2017-11-13T21:25:29.920Z Reads: 47

```
@Ackmaniac, thank you man very much for this post. This is probably a very basic knowledge in between crowd who uses Mini remote, but for me it was very unintuitive that removing binding key when remote is still on matters :confused:
```

---
