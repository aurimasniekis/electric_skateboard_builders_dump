# What batteries to upgrade to

### Replies: 9 Views: 646

## \#1 Posted by: chewydinosaurs Posted at: 2017-09-29T05:40:37.977Z Reads: 92

```
At my university there’s a few hills that I occasionally cannot make it up. Im using 2x3cell 4000mah 25c packs that dont give me a whole lot of range. My motor is a 280kv sk3. I was thinking about going up to 2x4 cell 4000 or 5000 mah batteries at 40c. This should increase range a little bit but would it imcrease torque? I know id need to limit the erpm in the bldc tool, I also need to keep this as cheap and thin as possible due to me being broke and the skateboard locks are rather thin at my school so my board cant be too bulky.
```

---
## \#2 Posted by: MysticalDork Posted at: 2017-09-29T05:56:39.337Z Reads: 89

```
Assuming you're using a vesc or derivitive, using an 8s pack will cause that motor to exceed 60k erpm on a full charge, which can (likely will) cause the DRV8032 chip to fail. I'd recommend doubling up on those 3s 4000mah packs to make a 6s2p pack. It'll double your range, and you won't have to worry about frying anything or changing the speed of the board. Depending on your settings, you may also be able to increase your current limits to get a little more power out of the deal too.

If you're set on going to a higher voltage, I suggest you switch to a lower-kv motor. For 8s, you need something below 250kv. For 10s, something under 200.
```

---
## \#3 Posted by: Okami Posted at: 2017-09-29T06:17:37.668Z Reads: 76

```
Have u thought about switching gears? That might also help with torque. What max speed are u getting now / at what speed do u ride on flats usually anyway?
```

---
## \#4 Posted by: chewydinosaurs Posted at: 2017-09-29T17:13:20.054Z Reads: 46

```
I thought I was already running a 6s2p? Or are you suggesting that I just use two 6s2p packs?
```

---
## \#5 Posted by: chewydinosaurs Posted at: 2017-09-29T17:15:57.021Z Reads: 45

```
I'm getting anywhere from 25mph-30mph, I thought about gearing/new motor however it'd be a huge pain for me since the locking screw on the gear for the motor shaft is stripped so Id have to cut through my motor shaft to get the motor off. Basically a different battery setup in my mind would just be simpler and easier
```

---
## \#6 Posted by: MysticalDork Posted at: 2017-09-29T17:42:37.014Z Reads: 45

```
2x3 cell packs would be 6s1p.
```

---
## \#7 Posted by: pat.speed Posted at: 2017-09-30T05:02:48.867Z Reads: 30

```



Try putting a rubber band on the end of the screwdriver it could get he screws out uneless there is locktite. After just put new screws or bolts in. What esc do you have?
```

---
## \#8 Posted by: chewydinosaurs Posted at: 2017-09-30T05:24:04.754Z Reads: 26

```
Definitelt used locktite, the blue stuff so it should come put but it’s really in there good. Im also using a vesc
```

---
## \#9 Posted by: pat.speed Posted at: 2017-09-30T06:18:21.545Z Reads: 23

```
Ah ok well I think the battery upgrade is probably the best idea then
```

---
