# Raptor Mono VESC XML File Wanted

### Replies: 2 Views: 690

## \#1 Posted by: sprocket12 Posted at: 2016-08-16T23:08:39.178Z Reads: 79

```
VESC went bad.  A previously VESC order arrived for a different build.  While warranty stuff is worked out, I'd like to get the Raptor up and running.  Any have a saved config file to post?  I can't get info off of the old VESC and I can't find a file or complete settings online.
```

---
## \#2 Posted by: Jinra Posted at: 2016-08-16T23:14:34.584Z Reads: 78

```
You should do motor detection for you own motor, I wouldn't rely on someone else's motor config. If you want usable motor limits try these:

Motor Max: 60A
Motor min (regen): -50A
Battery Max: Depends on battery (60A max for SCP3, though I'd go lower)
Battery Min (regen): Depends on battery (-12A max for SCP3)
Absolute Max: 130A (default)
```

---
