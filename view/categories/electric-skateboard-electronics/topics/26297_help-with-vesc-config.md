# Help with VESC config

### Replies: 5 Views: 435

## \#1 Posted by: fredrikinn Posted at: 2017-06-27T23:51:52.798Z Reads: 50

```
Hey i'm on my first build, and i'm wondering if i configured my VESC correctly. 

This is my motor and battery: 
Motor:
https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6364-245kv-brushless-outrunner-motor.html
2 x Battery:
https://hobbyking.com/en_us/zippy-compact-5000mah-3s-25c-lipo-pack.html


VESC config:
<img src="/uploads/db1493/original/3X/d/5/d59b43cd6db40b021811bbbfcc6673f45db1fa63.png" width="690" height="383">
```

---
## \#2 Posted by: Alanhunt123 Posted at: 2017-06-28T00:02:52.343Z Reads: 43

```
Looks like you set your maximum input voltage too low. I would set it at something like 26V. LiPo cells charge up to 4.2v/cell, so your fully charged pack voltage should be 25.2v, so 26v should work for it. Your cutoff start and end are also just a tad low, LiPos don't really like to go that low. Maybe set your cutoff end at 20.1v (3.35v/cell) and your cutoff start at 21.3v (3.55v/cell). These settings are more of a personal preference. The higher you set your cutoffs, the more cycles the battery will last for, albeit at a slightly shorter range.

Other than that, you may find the brakes to be a bit weak at only 5A batt min. I would try it to see if you like it, and if it needs more braking power, feel free to increase it. The specs say it can charge at max 5C, so it should be able to handle up to 25A. However, I'd stay below 12A to be safe. Same for your batt max. If the board feels sluggish, try increasing this value.

Hope this helps. Cheers!
```

---
## \#3 Posted by: fredrikinn Posted at: 2017-06-28T00:10:52.557Z Reads: 38

```
Thanks, this helps a lot! I guess it's time to start testing the brakes and speed :)
```

---
## \#4 Posted by: Alanhunt123 Posted at: 2017-06-28T00:43:10.967Z Reads: 32

```
Have fun! Make sure to do all that you can to prevent shorts on those motor wires. I fried my first VESC by not doing so.I would individually tape over all the connections with electrical tape.

Good luck!
```

---
## \#5 Posted by: Jinra Posted at: 2017-06-28T00:49:29.185Z Reads: 31

```
You should actually not change the max input voltage from the default 57v. There's no reason to change it.
```

---
