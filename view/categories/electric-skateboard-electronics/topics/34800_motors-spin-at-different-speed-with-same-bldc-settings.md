# Motors spin at different speed with same BLDC settings

### Replies: 43 Views: 1297

## \#1 Posted by: cwazy1 Posted at: 2017-10-04T23:14:58.175Z Reads: 88

```
I'm sure people have run into this weirdness before, I'd just like to know how you deal with it. 

I'm running dual focboxes with split ppm. Both are powered by a 12s4p pack. And they drive 6355's, 

The 6355's are about 100 miles apart. I used one as a single setup for a few weeks before going dual. 

I've tried tuning the motor max to compensate, but is this the advised method? 

I've also tried tuning this with the belts on, and belts off, which one is going to be more accurate? 

How have you guys dealt with this?
```

---
## \#2 Posted by: Jinra Posted at: 2017-10-04T23:16:21.153Z Reads: 81

```
first step is to find the kv of each motor. Run the motor on the bench and type 'kv' in the terminal section to find the kv of the motor. Then compare with the other motor.
```

---
## \#4 Posted by: cwazy1 Posted at: 2017-10-04T23:17:49.811Z Reads: 82

```
any specific throttle I need to apply?
```

---
## \#5 Posted by: Jinra Posted at: 2017-10-04T23:18:08.536Z Reads: 83

```
I do max, but do it a couple times to get a good average.
```

---
## \#6 Posted by: cwazy1 Posted at: 2017-10-04T23:18:54.790Z Reads: 75

```
kk, let me run some tests real quick
```

---
## \#7 Posted by: cwazy1 Posted at: 2017-10-04T23:20:45.593Z Reads: 71

```
getting between 1350-1370 rpm/v on one a 1320-1330 rpm/v on another
```

---
## \#8 Posted by: Jinra Posted at: 2017-10-04T23:21:57.749Z Reads: 67

```
Pretty much the same kv, which means something else is wrong on your setup. One motor is taking more amps to turn than the other, it could be belt tightness, bad tolerances, bad pulley/mount config, or a number of other things.
```

---
## \#9 Posted by: cwazy1 Posted at: 2017-10-04T23:23:19.015Z Reads: 68

```
Ah okay, thanks for helping me verify the kv. 

If it is something with a mechanical part, does the motors being not in sync have any detrimental effect?
```

---
## \#10 Posted by: Jinra Posted at: 2017-10-04T23:24:31.626Z Reads: 67

```
one will work harder than the other which may cause it to heat up more. Either way you're wasting energy that could be put towards propelling you instead.

Probably no danger, but inefficient.
```

---
## \#11 Posted by: scepterr Posted at: 2017-10-04T23:24:50.095Z Reads: 65

```
If you switch the ppm connectors between the 2 focbox same thing happens to each motor or does it flip?
```

---
## \#12 Posted by: cwazy1 Posted at: 2017-10-04T23:25:21.162Z Reads: 61

```
thats a good question... standby
```

---
## \#13 Posted by: cwazy1 Posted at: 2017-10-04T23:27:06.323Z Reads: 62

```
same thing.
```

---
## \#14 Posted by: scepterr Posted at: 2017-10-04T23:28:00.151Z Reads: 60

```
Try flashing both to default and start fresh?
```

---
## \#15 Posted by: cwazy1 Posted at: 2017-10-04T23:29:23.153Z Reads: 63

```
I actually already tried that. I had it on 2.18FW and then flashed to ack's 2.53FW and they both showed the same result
```

---
## \#16 Posted by: scepterr Posted at: 2017-10-04T23:30:09.952Z Reads: 63

```
Are the motor detection results the same or close between the 2? Ppm signal looks the same in both?
```

---
## \#17 Posted by: cwazy1 Posted at: 2017-10-04T23:30:15.751Z Reads: 65

```
I see, the motors actually showed the same async even with everything off including the motor pulleys.
```

---
## \#18 Posted by: Jinra Posted at: 2017-10-04T23:32:07.731Z Reads: 65

```
are you determining one is slower?
```

---
## \#19 Posted by: cwazy1 Posted at: 2017-10-04T23:32:24.146Z Reads: 64

```
ppm signal the same on both. 

detection results the same on both, 130/1100/750
```

---
## \#20 Posted by: cwazy1 Posted at: 2017-10-04T23:33:06.555Z Reads: 64

```
I'm watching the belt RPM speed as I throttle to different percentages.
```

---
## \#21 Posted by: cwazy1 Posted at: 2017-10-04T23:34:49.595Z Reads: 56

```
I have one motor max at 65 with max watt at 900 and another at 50 with max watt at 850 (both have non-limiting battery maxes), and they spin around the same when setup like that.
```

---
## \#22 Posted by: Jinra Posted at: 2017-10-04T23:38:26.105Z Reads: 55

```
belt RPM speed? How are you measuring that? Also I thought you said it was different when you took off the belts too.
```

---
## \#23 Posted by: cwazy1 Posted at: 2017-10-04T23:42:40.537Z Reads: 56

```
with the belts on - I was eyeballing the rate at which the belts would spin using the text printed on the belt. Its very apparent in lower throttle ranges. ~10-20% throttle

with the belts off - I was watching the can, also eyeballing the rate at which the text would spin.
```

---
## \#24 Posted by: Jinra Posted at: 2017-10-04T23:44:43.925Z Reads: 54

```
Did you make sure the PPM values are exactly the same? (Check dead zone as well)
```

---
## \#25 Posted by: cwazy1 Posted at: 2017-10-04T23:45:20.189Z Reads: 54

```
yeah they are all exactly the same.
```

---
## \#26 Posted by: psychotiller Posted at: 2017-10-04T23:47:28.354Z Reads: 54

```
Then it's belt tension.
```

---
## \#27 Posted by: Jinra Posted at: 2017-10-04T23:48:34.264Z Reads: 54

```
He mentioned this happened without belts as well.

@cwazy1 Try swapping PPM on each VESC like @scepterr said and seeing the results.
```

---
## \#28 Posted by: cwazy1 Posted at: 2017-10-04T23:48:37.809Z Reads: 56

```
I've tested without belts and just watching the can rotation speed. Same difference in rpm.
```

---
## \#29 Posted by: scepterr Posted at: 2017-10-04T23:50:19.051Z Reads: 56

```
What if you switch motors between vescs? If the behavior is the same it's the motor(maybe bullets), if not it's the focbox
```

---
## \#30 Posted by: cwazy1 Posted at: 2017-10-04T23:51:09.464Z Reads: 53

```
[quote="Jinra, post:27, topic:34800"]
@cwazy1 Try swapping PPM on each VESC like @scepterr said and seeing the results.
[/quote]

I tried this, same result.. The slow motor is still the slow motor.
```

---
## \#31 Posted by: psychotiller Posted at: 2017-10-04T23:54:18.234Z Reads: 51

```
Do you have an extra vesc? Try swapping out the slow side.
```

---
## \#32 Posted by: BigBoyToys Posted at: 2017-10-05T00:07:26.207Z Reads: 50

```
I would think this is likely due to one motor having sligtly more friction while turning and therefore requiring more current to spin at low speeds. Can you feel any difference when spinning them by hand? Id suggest riding it to see if there is a big temp difference or if it seems to torque steer from uneven power delivery. If niether of those happen i
I dont think you have a real problem.
```

---
## \#33 Posted by: scepterr Posted at: 2017-10-05T00:10:17.635Z Reads: 49

```
I think that could be checked by setting each motor to run at like 2k rpm or whatever is considered slow and see what current it draws with no load, could be done at several rpm levels to see where they split
```

---
## \#34 Posted by: cwazy1 Posted at: 2017-10-05T00:11:34.886Z Reads: 50

```
How do I actually do this from bldc tool?
```

---
## \#35 Posted by: scepterr Posted at: 2017-10-05T00:12:01.146Z Reads: 48

```
While in real-time, use the box on the right with motor controls 
Has duty,rpm,current,brake,position
```

---
## \#36 Posted by: cwazy1 Posted at: 2017-10-05T00:12:48.511Z Reads: 44

```
ahh in real time.. thats what I wasn't doing when I tried it last time.
```

---
## \#37 Posted by: cwazy1 Posted at: 2017-10-05T00:13:09.043Z Reads: 46

```
unfortunately I do not. I just sold my old TB VESC
```

---
## \#38 Posted by: scepterr Posted at: 2017-10-05T00:13:22.128Z Reads: 46

```
That box is visible everywhere you just won't see what's happening unless in realtime
```

---
## \#39 Posted by: cwazy1 Posted at: 2017-10-05T00:13:44.957Z Reads: 47

```
There isn't any noticeable difference in spinning the cans, I'll try to see if I notice any torque steer, but I haven't noticed anything stand out ish in the last week or so of riding it.
```

---
## \#40 Posted by: psychotiller Posted at: 2017-10-05T00:45:53.483Z Reads: 46

```
You could try switching the slow side vesc to the other side and see if you get the same result? Just trying to see if it's a problem with that vesc/settings
```

---
## \#41 Posted by: scepterr Posted at: 2017-10-05T01:38:12.393Z Reads: 48

```
Did you get stuck riding in a circle? 😋
```

---
## \#42 Posted by: cwazy1 Posted at: 2017-10-05T01:45:56.995Z Reads: 50

```
yeah I'll have to try this to isolate if it is a VESC issue or a motor issue.
```

---
## \#43 Posted by: cwazy1 Posted at: 2017-10-05T01:47:12.619Z Reads: 50

```
haha, I went out for a 8 mile ride just now, felt fine, nothing abnormal and board pulled dead straight. Its just aesthetically strange to have a motor take much longer to stop when giving throttle while upright.
```

---
## \#44 Posted by: mmaner Posted at: 2017-10-05T01:49:11.199Z Reads: 48

```
I personally have never had both motors spin equally.  Understand that every electronic piece of an eskate build  expects to run under a load, so bench results are not very usable.
```

---
