# My Vesc Settings

### Replies: 4 Views: 454

## \#1 Posted by: magsm Posted at: 2017-08-09T21:08:10.651Z Reads: 74

```
Here are my settings for the vesc. Does this look ok?

Also, right now I'm running a single 6355 190kv from Torque Boards with a 12s4p battery. In a couple days I'll add another 6355. When that happens, should I change anything to the settings (like with Amps or Voltage or Battery min) other than setting up slave/master and connecting over canbus? 

<img src="/uploads/db1493/original/3X/e/b/ebd68c762dfd75e3cb2a08eb4273555acfe8dd8b.png" width="690" height="412">
<img src="/uploads/db1493/original/3X/f/e/fe99a1152d25e377c8f46a3fabcac5da21d908b5.png" width="690" height="425">
<img src="/uploads/db1493/original/3X/b/0/b0bdf384c41cb53d2298bb3577101da5dd634a57.png" width="690" height="417">

Thank you!
```

---
## \#2 Posted by: Jinra Posted at: 2017-08-09T21:18:52.530Z Reads: 65

```
Batt min is a bit low, your brakes at high speed might be pretty weak. You can safety go up to -16A. Also, doesn't look like you configured PPM values, they may work at default, but might not be accurate.
```

---
## \#3 Posted by: magsm Posted at: 2017-08-09T21:54:11.727Z Reads: 54

```
How should I configure the PPM values?
```

---
## \#4 Posted by: Jinra Posted at: 2017-08-09T21:56:56.281Z Reads: 54

```
use the "display" box in app config > ppm. Throttle all the way up and record max value, then throttle all the way down and record min value.
```

---
