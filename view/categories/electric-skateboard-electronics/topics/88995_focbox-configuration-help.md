# FOCBOX configuration help

### Replies: 7 Views: 153

## \#1 Posted by: MrDGOrman Posted at: 2019-04-01T15:37:52.351Z Reads: 65

```
Hi everyone

I've tried using the search feature but I can't seem to locate a setup that resembles mine so I thought I'd make a post. I'm looking for help with the configuration of my FOCBOX. I'll list my setup below:

- Motor:
-- Single belt drive Eskating 6374 190Kv (https://eskating.eu/product/eskating-pro-motors-6374-190kv-waterproof-sealed-and-sensored/)
- Wheels:
-- Trampa Gummies 125mm
- Pulley config:
-- Motor pulley is 15t, wheel pulley is 44t
- Battery:
-- 12s6p Samsung 30Q cells
- Speed controller:
-- Enertion FOCBOX (single drive **not** Unity)

I'm not sure what numbers I should use in the FOCBOX setup. I was hoping that someone else has a similar setup (or is clued up on this stuff) and can help me. I want to have good acceleration to help at traffic lights but also enough range to go on a nice long ride.

I'd really appreciate some pointers. I use the Vesc Project tool if that helps.

Thanks,
Dan
```

---
## \#2 Posted by: mackann Posted at: 2019-04-01T20:31:10.660Z Reads: 56

```
Why did you go with that big battery for a single drive? With that big battery will the vesc be the limit for single drive. 60A battery A and 68 motor A I would suggest.

My suggestion is to get 1 more motor and vesc then you could still set 60A battery A on both and 68A motor A for double power, the battery can still handle it. You will probely get 60-70km range with dual so thats problebly more then you need.
```

---
## \#3 Posted by: Battosaii Posted at: 2019-04-01T20:33:12.011Z Reads: 54

```
Yeah @mackann is right I'm using a slightly bigger battery 12s8p on 4wd 6p is crazy big for a single motor

I'd do 60 battery amp and 80 motor amp that's pretty much maxing out a 1wd system
```

---
## \#4 Posted by: olestra Posted at: 2019-04-01T21:58:15.867Z Reads: 45

```
he could be going for maximum range, rather than using 6p for amp draw
```

---
## \#5 Posted by: MrDGOrman Posted at: 2019-04-02T08:54:59.727Z Reads: 29

```
The reasons for the large battery is more range over speed and it's "future proof". I do plan on getting an additional motor to improve torque but for the most part I want to have great distance. But yes, eventually I'll be having a dual setup (probably in a few months time).

Is the FOCBOX only rated to 60A? I don't want to damage the FOCBOX but I want to get the most potential out of it!
```

---
## \#6 Posted by: mackann Posted at: 2019-04-02T09:13:47.909Z Reads: 25

```
I think their is ppl using up to 80A on it, but I would not go more then 60A on a focbox since thats max it rated for.
```

---
## \#7 Posted by: MrDGOrman Posted at: 2019-04-02T09:20:48.824Z Reads: 21

```
Okay that's worth noting then I guess. Thanks!
```

---
