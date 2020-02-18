# VESC/Motor detection issues

### Replies: 3 Views: 236

## \#1 Posted by: zzlotnick Posted at: 2018-03-27T05:37:03.227Z Reads: 43

```
Hey guys,

I have a setup with a 190KV 3150W BLDC motor from DIYelectric hooked up to a VESC and Miami electric power switch. This is then connected to 2 5s 5000 mAh batteries (in series). I have settings for my VESC that I can upload, but could someone suggest settings that they know would work (or at least not break my DRV chip). I’ve broken two VESCs and am not sure why. When I do motor detection is stutters once forward and quickly stutters backward while screeching. Any help would be great!

- Zach
```

---
## \#2 Posted by: torqueboards Posted at: 2018-03-27T07:05:10.793Z Reads: 41

```
If you have sensors connected and your not on the correct BLDC setting. It could do that.

Try without sensors first on BLDC. I'd only try sensored once you ride on BLDC and learn how to use the VESC first.
```

---
## \#3 Posted by: zzlotnick Posted at: 2018-03-27T13:34:12.316Z Reads: 24

```
@torqueboards I’m not trying sensored mode. Everything is currently in sensorless BLDC mode.
```

---
