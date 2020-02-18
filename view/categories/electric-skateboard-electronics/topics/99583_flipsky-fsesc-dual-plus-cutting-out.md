# Flipsky FSESC Dual Plus cutting out

### Replies: 10 Views: 267

## \#1 Posted by: Wankerman Posted at: 2019-08-02T05:09:03.151Z Reads: 94

```
I recently bought a FSESC Dual Plus w/pro switch from Flipsky and I was surprised to see that the acceleration cuts out midway at full throttle. I thought this was a problem on older non-plus versions, but I just bought mine.

I'm also pretty conservative in my VESC settings. I'm running 6s2p, 5055 270KV motors in FOC mode with a 38A max motor current as recommended by other users to avoid cutting out, but it still does it. It's my son's board and he's pretty light on the throttle and doesn't really happen to him, but I'd still like to fix the issue. These esc's have a 100A continuous rating (300A burst), so it's not normal.

Anybody else with a FSESC Dual Plus getting cutouts at full throttle acceleration?
```

---
## \#2 Posted by: esk8_hui Posted at: 2019-08-02T06:02:18.144Z Reads: 89

```
Do you bypass bms discharge?
```

---
## \#3 Posted by: gee Posted at: 2019-08-02T06:42:52.919Z Reads: 85

```
https://www.electric-skateboard.builders/t/the-brumbeast-37mph-dual-6374-maytech-12s4p-unity-bergmeister-wheels-fatboy-nano-gear-drive-bigben-enclosure-landyatchz-evo-tb218-first-build/99416/9

I post a similar question and ju5t answered. If you don't mind post your vesc tool settings?
```

---
## \#4 Posted by: bartroosen12 Posted at: 2019-08-02T12:53:49.221Z Reads: 69

```
How much is your max battery amps you set on the vesc?

And you're using a 6S2P? Lipo I guess?

Maybe your battery is to weak and reaches the cutoff voltage of your vesc?
```

---
## \#5 Posted by: Wankerman Posted at: 2019-08-02T15:19:03.994Z Reads: 60

```
I believe this BMS is being used for discharge, yes. It's from an original Backfire Gen 1 (2016) board. I guess it was designed for a single 5055 motor. Now has dual.
```

---
## \#6 Posted by: Wankerman Posted at: 2019-08-02T15:21:07.958Z Reads: 57

```
Yep, it's a Lipo. I never opened it up, but by the range, I'm estimating it to be around 6Ah. I set the battery max to 38A as well. Could be a tad high I guess.
```

---
## \#7 Posted by: esk8_hui Posted at: 2019-08-02T15:48:39.057Z Reads: 50

```
Most of my cut out happened because bms cant handle that much current and shut down to protect itself.
```

---
## \#8 Posted by: Soflo Posted at: 2019-08-02T17:25:12.624Z Reads: 46

```
I'll bet it's your battery not being able to handle the amp draw.  Do you have a  metr or a way to log voltage?
```

---
## \#9 Posted by: Wankerman Posted at: 2019-08-03T05:57:42.138Z Reads: 36

```
Definitely looking like it's the battery. I took a ride earlier and went up a steep hill. The current cut off and the board completely shut itself off 1 second later. I guess we'll live with it for now. Like I said, it's my son's board and his 75lbs doesn't affect it. But a nice 18650 battery upgrade is in this board's future for sure!
```

---
## \#10 Posted by: visnu777 Posted at: 2019-08-03T07:56:34.333Z Reads: 27

```
Just limit the battery current and there won't be any cutoffs, even when you son decides to grow later ;)
Don't forget: Its a dual setup, so if you have a battery that can deliver 35A you have to set the limit to 17,5A per VESC side (basically theyre two vescs).
```

---
