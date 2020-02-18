# Battery supports BMS short circuit protection?

### Replies: 3 Views: 561

## \#1 Posted by: RiGo Posted at: 2017-08-04T20:16:21.298Z Reads: 59

```
Can I rely on the overvoltage protection in this BMS as a sort of fuse for shorts downstream from the battery?

If a VESC or wiring shorts, will this be enough or do I need a fuse as well?
```

---
## \#2 Posted by: SilentException Posted at: 2017-08-04T21:45:37.386Z Reads: 53

```
You wrote short circuit protection in the title and then mention overvoltage protection in the post. The two are not directly related though. BMS basically cuts the load in case of short circuit detection and there is a slight delay of this detection and response. As this is nothing fancy or new groundbreaking tech, I think you can rely on it. However...

I'm using a BMS without integrated eSwitch which means I need to have separate anti-spark switch (with fuse). Which is a configuration I would recommend to you as well. I don't know of any SuPower BMS with eSwitch anyhow (maybe they have it since last time I checked)...
```

---
## \#3 Posted by: Jinra Posted at: 2017-08-04T22:08:23.777Z Reads: 48

```
You don't want to rely on a BMS to be a fuse as they can typically handle a lot of current, and you probably dont want to end up breaking a BMS anyway. If you want a fuse, put it before the BMS.

I personally don't run a fuse nor rely on BMS for discharge.
```

---
