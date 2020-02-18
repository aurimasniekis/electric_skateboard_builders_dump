# Power loss under braking \[solved\]

### Replies: 16 Views: 219

## \#1 Posted by: Vampiresquid64 Posted at: 2019-04-10T20:37:55.800Z Reads: 86

```
I just started having a strange issue where, when going downhill and braking, the power totally cuts off. I'll brake at maybe half to 3/4 brake for about 5 seconds and then boom, no power. if i stop and wait a bit then everything seems to come back to normal. This is on a fully charged battery. setup: single sk3 6374 on 10s battery. ratio is 14:36 with 85mm wheels. Never had this issue before and none of the electronics have changed. I recently got bigger wheels but got a smaller pinion to compensate so ratio is exactly the same as before. I'm about 160lbs. also, rode the exact same new-ish setup yesterday with no issues like that. Tested this problem twice on the same hill and got the exact same results both time. Haven't checked anything on my vesc yet.
```

---
## \#2 Posted by: 702vegas Posted at: 2019-04-10T20:39:04.135Z Reads: 82

```
Battery regen?
```

---
## \#3 Posted by: Vampiresquid64 Posted at: 2019-04-10T20:41:18.571Z Reads: 81

```
ohhhh hmmm that might be an idea hadn't considered that before. not sure if theres a way to empirically test, but thats a really good idea thx. and that would make sense because this hill I'm talking about is basically right outside my door
```

---
## \#4 Posted by: 702vegas Posted at: 2019-04-10T20:43:18.167Z Reads: 77

```
Charge to like 98 percent and try the hill again
```

---
## \#5 Posted by: Gamer43 Posted at: 2019-04-10T20:44:26.456Z Reads: 75

```
If you have a bms, it's cutting off regen to prevent overcharging.
I run into this all the time.
```

---
## \#6 Posted by: Vampiresquid64 Posted at: 2019-04-10T20:45:48.695Z Reads: 72

```
is there any way to run it without regen for the first 10% of battery?
```

---
## \#7 Posted by: Gamer43 Posted at: 2019-04-10T20:46:47.067Z Reads: 72

```
No, you won't have braking. You'd need a rheostatic brake (and a big heatsink). The workaround is undercharging your battery to 40-41V

Give up a mile or two range, but gives regen more room to work in.

Another alternative is a mechanical handbrake. Works like a rheostatic brake but bypasses the elctrical aspect :p.
```

---
## \#8 Posted by: Vampiresquid64 Posted at: 2019-04-10T20:51:09.511Z Reads: 63

```
yeah maybe I'll probably just keep that in mind and run my motor a bit before I go down this particular hill at the beginning of my ride.
```

---
## \#9 Posted by: rsalmon Posted at: 2019-04-10T20:57:09.039Z Reads: 65

```
You can always ride uphill for a few meters (maybe half a block?) before starting to brake downhill.
```

---
## \#10 Posted by: Vampiresquid64 Posted at: 2019-04-10T21:33:09.155Z Reads: 61

```
ok update that was definitely the issue. I ran my motor at full throttle for a minute or 2 and had no issues when braking, thanks for the responses guys
```

---
## \#11 Posted by: venom121212 Posted at: 2019-04-10T21:59:23.503Z Reads: 55

```
@hyperIon1 sell a really good rbrake. I've been riding with it for a few months now with no issue.
```

---
## \#12 Posted by: Sn4pz Posted at: 2019-04-11T00:46:06.868Z Reads: 36

```
Have you noticed it getting warm after extended breaking?
```

---
## \#13 Posted by: Vampiresquid64 Posted at: 2019-04-11T01:00:54.532Z Reads: 32

```
no more than usual. but in my original problem heat was not an issue because braking was not extended but mainly because it was within the first minute of me riding
```

---
## \#14 Posted by: Sn4pz Posted at: 2019-04-11T01:02:18.494Z Reads: 31

```
Sorry, I was asking @venom121212 about his rbrake :sweat_smile:
```

---
## \#15 Posted by: venom121212 Posted at: 2019-04-11T01:05:25.627Z Reads: 29

```
I have not but it's also inside my enclosure. It should only be working under extreme conditions (not very often).
```

---
## \#16 Posted by: Sn4pz Posted at: 2019-04-11T01:06:26.664Z Reads: 29

```
True, I just wonder how much heat is generated under those loads

Maybe ill try and test it out :joy:
```

---
