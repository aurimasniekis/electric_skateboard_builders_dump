# FVT Sleeping Lion 120A 6-12S ( Brake Failure )

### Replies: 14 Views: 903

## \#1 Posted by: jeorghe Posted at: 2018-02-12T07:53:40.994Z Reads: 132

```
Hello to all,

I want to share my problem with the FVT controller sleeping lion 120A 6-12s, so it can be useful to someone else.

During the ascent or descent from a hill the brake works only once and after the controller switches off.
A ESC reset is required.

I asked the FVT technical support who promptly replied, but at the moment there is no solution.

I'm using the latest firmware from the FVT site.

Apart from this problem this esc works really well, very powerful and unexpectedly silent if you use a good capacitor on the power line.

The configuration of my mountaion board is:

- 2 motors 6374 149KV ( Low Timing )
- 2 Sleeping Lion 120A 6-12S
- Multistar 12000mAh 10S

Does anyone have any advice?

Thanks in advance ...
```

---
## \#2 Posted by: Namasaki Posted at: 2018-02-12T12:57:18.555Z Reads: 110

```
Best advice I can give you is to ditch the FVT’s and get a couple Vescs.
```

---
## \#3 Posted by: jeorghe Posted at: 2018-02-12T13:07:39.696Z Reads: 105

```
Of course, you're absolutely right, Vesc is the best esc on the market, but I need to stay on an acceptable budget for my portfolio, thanks for the advice :).
```

---
## \#4 Posted by: onepunchboard Posted at: 2018-02-12T16:01:10.131Z Reads: 94

```
Have you tried custom frimwere floating around in this forum?

and also try high timing,
```

---
## \#5 Posted by: Nemesis Posted at: 2018-02-13T14:34:19.065Z Reads: 82

```
I vaguely remember this problem with the FVT happening to others on this forum, unfortunately i cant remember if it was something simple to do with the binding of the remote or break regen overcharge protection or if it was fixed with a software tweak/stepback. 

Keep searching the FVT threads im sure you will find an answer within prev threads, if not answered on this one by someone.
```

---
## \#6 Posted by: vap Posted at: 2018-02-13T21:00:46.301Z Reads: 70

```
Calibrate the ESCs, then Limit brake PWM range to 70-75%.
```

---
## \#7 Posted by: jeorghe Posted at: 2018-02-14T08:31:38.292Z Reads: 61

```
Thanks to all, I will try your advices .
```

---
## \#8 Posted by: jeorghe Posted at: 2018-02-14T08:36:56.166Z Reads: 60

```
Thanks vap, only one question to understand better your advice, you mean : 

1) configure the brake at 100% 
2) recalibrate the esc 
3) limit the brake range to 70%-75%

I need to recalibrate the esc when I change any esc parameter like brake percentage, drag or timing ?

Thanks
```

---
## \#9 Posted by: vap Posted at: 2018-02-14T09:03:55.849Z Reads: 58

```
Oh, i mean PWM range on the controller, not the brake percentage setting in the usb link tool.
Like for example if PWM range is 1050-1500-1950ms on the controller. Limiting low end to somewhere around 1150ms and top end to 1900ms after calibrating at full range can help.
It solved my issue with escs turning off when pushing stick too far.

Or maybe just calibrating them would work :D
```

---
## \#10 Posted by: jeorghe Posted at: 2018-02-14T10:07:15.733Z Reads: 52

```
 Now I understawhat you mean with PWM range, but I do not understand how to limit the throttle PWM in the FVT controller . There isn't  that kind of setting in the instructions.
Could you give me a little more details please ?
```

---
## \#11 Posted by: vap Posted at: 2018-02-14T10:25:24.370Z Reads: 49

```
Sorry, i meant to say transmitter.
If there's throttle limiting on the transmitter, you can try that.
```

---
## \#12 Posted by: jeorghe Posted at: 2018-02-14T10:54:32.558Z Reads: 50

```
Thanks Vap, I am an ex heli rc modeler , I suppose  as many other user in this forum .
You mean the dual rate in the transmitter ... I guess.

If can be useful for you, in order to smooth the throttle and reduce current spikes,  FVT ( and other forums too)  suggested me to add a capacitor in the middle of the cable from battery pack .

The capacitor type is:  63ZLH560MEFC .
```

---
## \#13 Posted by: jeorghe Posted at: 2018-02-18T09:00:59.286Z Reads: 48

```
Finally I solved all the problems regarding esc fvt 120A also thanks to your valuable suggestions.

It is not the best esc on the market but it certainly has a very good price-quality ratio, even if it requires some attention in tuning.

Hoping to help beginners like me this is the problems and solutions:

1) P:after the calibration the motors are not in synch.
    S: An esc had the bec with a voltage not suited to the other esc, so try to feed also with the other esc.

2) P: Throttle is not smooth. 
    S: Add a capacitor in the middle of the cable of battery.

3) The most important (thank to vap)
    P: the escs turns off during a brake in the down / up hill.
    S: Calibrate the esc with brake to 100%, after this limit mechanically in the remote the trigger travel when braking to have a 70/80% brake percentage.

Of course, excuse my terrible English;)
```

---
## \#15 Posted by: artSkate Posted at: 2018-12-11T20:55:35.784Z Reads: 19

```
Hi Vap.  Art here.  Im late to this conversation...  If you are still monitoring this chat, can you advise what usb link or programming box you use to program FVT Sleeping Lion ESC?  Thanks in advance.
```

---
