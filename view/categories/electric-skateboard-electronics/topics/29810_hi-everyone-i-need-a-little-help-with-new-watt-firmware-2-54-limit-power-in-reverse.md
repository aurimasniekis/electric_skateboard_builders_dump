# Hi everyone i need a little help with new Watt firmware 2.54 limit power in reverse

### Replies: 7 Views: 462

## \#1 Posted by: jammy550 Posted at: 2017-08-05T19:04:39.192Z Reads: 77

```
Hi new to the forum but been around for long time reading and reading and then i home built VESC controllers home built battery packs and finally i have a dual motor  EMTB running 2.54 firmware and works perfect i can set watts power output and forward power is limited but when i reverse its like full power and no limit on power its ok for me but if my mates try it out it will throw them off am  i missing some setting some where any advice on these would be really appreciated !! Wicked site guys and girls :wink:
```

---
## \#2 Posted by: Ackmaniac Posted at: 2017-08-05T23:59:42.077Z Reads: 63

```
Please post a Screenshot of your motor general Tab and of the PPM Tab.
```

---
## \#3 Posted by: jammy550 Posted at: 2017-08-06T12:26:21.465Z Reads: 49

```
Hi cool thanks for the reply I will get some screen shots up as soon as I can thanks man :)
```

---
## \#4 Posted by: trancejunkiexxl Posted at: 2017-08-06T15:34:24.025Z Reads: 39

```
hi welcome!!! make sure to calibrate your ppm well, it was a source of trouble for me.. =)
```

---
## \#5 Posted by: jammy550 Posted at: 2017-08-10T20:24:54.327Z Reads: 30

```
Hi guys sorry for delays for the screen shots work and family any hows here are the screen shots i tried to re calibrate the ppm but still no good tried different settings here and there but no good very strange :confused: cheers guys:slight_smile:


<img src="/uploads/db1493/original/3X/5/c/5c66e9df6160738916ceebe9267aa422bf6d6b0e.png" width="690" height="387">

<img src="/uploads/db1493/original/3X/8/d/8d83d5c83de929f4785d5d7dadafa8bcaf24e542.png" width="690" height="387">

These setting are repeated on the slave VESC .
```

---
## \#6 Posted by: Ackmaniac Posted at: 2017-08-12T20:27:50.476Z Reads: 24

```
Just enable in the PPM Tab the checkbox for Enable maximum ERPM for direction switch (..)
When you enable that checkbox then to go backwards you have to be slower than this parameter and release the brake and brake again to go backwards. Then the power is limited backwards like it is limited forward. And while you go forward you are able to make a full brake till stand still without the wheels spinning backwards.
If you want a bit less acceleration power at low speeds then lower your Motor max (maybe 40 for beginners or less).
Motor max is for low speed power (torgue) and battery max (or max watts if enabled) regulates the mid till high speed power.

I also recommend to adjust the throttle curves in the app config to make the control over your board smoother. I recommended settings for the throttle curve already in my firmware mod thread. 

If you use split cables then it is ok to have the app configuration. But if the VESCs are connected via CAN then diable the app config for the slave.
```

---
## \#7 Posted by: jammy550 Posted at: 2017-08-12T20:48:25.020Z Reads: 22

```
Wow cheers I do that I have it connect by CAN not from a splitter your firmware is wicked man I have had it running sweet just the reverse power I was little worried about changing stuff cause of it running so good .The app is so handy for checking watts being used and changing modes very cool I'll post up my results soon as I get chance nice1
```

---
