# VESC - FOC braking trouble

### Replies: 17 Views: 3729

## \#1 Posted by: treenutter Posted at: 2016-01-14T01:33:30.980Z Reads: 197

```
I've got my VESC 4.7 configured with latest firmware (2.8FOC) and I'm having trouble using FOC mode. It will start from as stop very well, but when I apply brakes the motor seems to lose contact with the VESC and the controller doesn't respond for a moment. There's a "tick" sound from them motor and then no resistance at all, even though I'm still applying brake from the controller (GT2B). On the bench, I see that the red light is flashing when this happens. I don't seem to lose connection to the VESC from BLDC Tool, so I don't think that VESC is rebooting.

Any thoughts on what is going wrong? I love the quiet operation but not enough to lose the brakes! [Build thread here][1] pics of BLDC Tool configuration below.
<img src="/uploads/db1493/original/2X/4/4f4585b16bb4db47e79e1c2d6d3bbf4d22586073.jpeg" width="690" height="448">
<img src="/uploads/db1493/original/2X/3/3b01e1a483a13e622b6d9077ad54906fc557c7cc.jpeg" width="690" height="407">

<img src="/uploads/db1493/original/2X/b/bfb5a87343806a77a9136274ea5027cb403ec870.jpeg" width="690" height="435">
  [1]: http://www.electric-skateboard.builders/t/the-village-build-s9-faultine-paris-195mm-sk3-6764-diyes-mount-8s-vesc-127mm-pneumatic-wheels/292
```

---
## \#2 Posted by: psychotiller Posted at: 2016-01-14T03:17:57.594Z Reads: 164

```
On the foc tab have you run the tests and applied the results? I see zeros. 
Also on bldc, you have delay checked. Mine is integrate.

Honestly though, I'm still trying to figure out what everything means.
```

---
## \#3 Posted by: trbt555 Posted at: 2016-01-14T06:34:21.069Z Reads: 160

```
Wouldn't it be great if Mr. Vedder had somebody looking over his shoulder and taking notes ?
It seems a lot of people are in the dark about what a lot of settings in the BLDC tool actually mean.
It's a pity we have this genius piece of hardware at our disposal but nobody fully understands it.
There's a dedicated VESC forum but I think a decent Wiki would be great.
I'm certainly willing to contribute.
```

---
## \#4 Posted by: laurnts Posted at: 2016-01-14T09:51:05.570Z Reads: 160

```
I have the same problem with VESC in FOC doesn't brake very well. It brakes for 0.5 second then theres the tick sound just like you said then it started to loose the brake completely. I thought it was a setting misconfigured, but not quite sure after all.
```

---
## \#5 Posted by: treenutter Posted at: 2016-01-14T15:50:02.460Z Reads: 152

```
@trbt555 I was suggesting the same thing in another thread a few days ago! I was thinking that a configuration guide that covered all aspects of BLDC Tool would be a good start, although there's clearly a need for a hardware wiki as well that might help those interested in building their own VESC from scratch. I think that a configuration guide is needed most, now that there are so many people buying VESC and trying it out.
```

---
## \#6 Posted by: treenutter Posted at: 2016-01-14T15:51:09.867Z Reads: 141

```
@laurnts thanks, it's good to know I'm not alone. @jacobbloy @chaka @sl33py do any off you have ideas about why our braking is failing in FOC mode?
```

---
## \#7 Posted by: treenutter Posted at: 2016-01-14T15:53:03.060Z Reads: 138

```
Thanks @psychotiller! I ran the tests and applied the values to the configuration, the zeros are just showing that I didn't calculate them when I took this screenshot.  I applied "Delay" mode based on a thread I found on ES, but neither Delay nor Integrate seem to have an effect on performance.
```

---
## \#8 Posted by: chaka Posted at: 2016-01-14T16:08:04.889Z Reads: 138

```
Vedder has been very up front about the FOC implementation and it's "in development" status. Too many people are jumping the gun and expecting it to work flawlessly with auto detection.

I still recommend and use BLDC settings. The silent running is nice but I prefer the note our motors produce on bldc.
```

---
## \#9 Posted by: treenutter Posted at: 2016-01-14T21:38:34.679Z Reads: 132

```
Thanks @chaka you're right, FOC is experimental. I was wondering if there was some obvious mistake I had made in configuring it, that might lead to stability and using it as my full-time setting. I really dig the silence! 

Has anyone started using it without any problems? Taken an actual ride with it?
```

---
## \#10 Posted by: trbt555 Posted at: 2016-01-15T06:10:33.593Z Reads: 126

```
I think @okp on ES has.
```

---
## \#11 Posted by: elkick Posted at: 2016-01-15T08:56:40.072Z Reads: 122

```
I'm using FOC now for several weeks in 5 boards without problems (3 dual, 2 single) and I know at least 5 other guys in Europe using it too.
```

---
## \#12 Posted by: trbt555 Posted at: 2016-01-15T09:06:41.825Z Reads: 119

```
So, any significant differences compared to BLDC ?
```

---
## \#13 Posted by: elkick Posted at: 2016-01-15T10:09:16.531Z Reads: 121

```
It's basically the sound only and the fact, that the start from a standstill is smoother and even more comparable to a sensored setup. I also tested the VESC with sensored motors and found no reason anymore for going sensored. 
This might be different with MTB's though.

FOC is nice but not a must.
```

---
## \#14 Posted by: Hummie Posted at: 2016-01-15T17:45:59.454Z Reads: 124

```
I'm running foc. I really like it and it set up easily.  
Doing delay in bldc. 
Did the 3 adjustments/tests on foc tab. 
If u want help, not that I know much,  message me and I'll screen shot what i have and send it to you

My motors are 100kv which Vedder said being so low would be a help
```

---
## \#15 Posted by: treenutter Posted at: 2016-01-15T21:42:42.638Z Reads: 125

```
Thanks @Hummie. Mine is 245KV, I wonder if that's too high. I doubt it though. Will PM you, would love to see how you've got things configured. I suspect that there's a config somewhere that isn't correct. 

@elkick with 5 different boards you've got a lot of experience with FOC! Is there anything besides the automatic detection that you change when you configure your VESCs to run FOC? Settings that help to correct any issues? 

May I ask everyone how long their battery wires are? I read that beyond 20cm the automatic configurations fail and\or become inaccurate.
```

---
## \#16 Posted by: Hummie Posted at: 2016-01-16T01:33:53.115Z Reads: 129

```
<img src="/uploads/db1493/original/2X/7/767dc8256ccb08669e878080d461286642adaf82.jpeg" width="666" height="500"><img src="/uploads/db1493/original/2X/a/abd0a9a7d1c949330ecf82ab70dd2f0edbfca2fb.jpeg" width="666" height="500"><img src="/uploads/db1493/original/2X/d/d3c6e9867a36f43871a2bcbbd22a81c0f8582716.jpeg" width="666" height="500"><img src="/uploads/db1493/original/2X/b/b445a760e4d33cdca80a21de9b35e614d6941738.jpeg" width="666" height="500"><img src="/uploads/db1493/original/2X/9/9df1ca49549f66b50a407ab013a595f11a14eb0b.jpeg" width="666" height="500"><img src="/uploads/db1493/original/2X/d/d2a3b6353f34fc8f576748b2b797b9929fc73ed4.jpeg" width="666" height="500"><img src="/uploads/db1493/original/2X/f/fc266857ed85b00867e457b662aba9ef931d9045.jpeg" width="375" height="500">

This works for me. 

I heard maybe using "boost" in "motor config" "advanced" would be useful with such low kv but I didn't change anything
```

---
## \#17 Posted by: elkick Posted at: 2016-01-16T10:03:45.051Z Reads: 117

```
I had some difficulties in the beginning with 2.4, but they were gone with 2.7 and 2.8. Troubleshooting was alway successful when I installed a new FW and started over from scratch leaving everything at the default values first.

1. switched to FOC in the main window
2. BLDC section: enable delay, motor detection, apply, write config (& adjusted value when using hub motors)
3. FOC tab: top down detection, always klick apply on the right side, at the end: write config
4. Adjusted startup boosted (in advanced tab), but this has no effect with FOC, but just in case I'd switch back to BLDC 
5. Reboot
6. Application config, write config, reboot (!)

And yes, I experienced troubles when the battery wires were to long, like 40cm. They are all 20-25cm now.
```

---
