# Calibrating Nano-X with Unity

### Replies: 2 Views: 169

## \#1 Posted by: ajplant96 Posted at: 2019-04-21T20:57:00.793Z Reads: 58

```
So I’ve just finished wiring everything up and went to do the setup over bluetooth/android app for my board but found that the remote calibration section isn’t recognising my Nano-X. It’s connected but when I go to calibrate it in the setup nothing happens. What exactly should I be doing in the setup process? Hoping I’m just doing something wrong rather than there being an issue with any of the components.
```

---
## \#2 Posted by: McErono Posted at: 2019-04-21T21:01:23.449Z Reads: 56

```
make sure your remote is paired first:
https://enertionboards.zendesk.com/hc/en-us/articles/115000503174-How-to-bind-calibrate-your-Nano-X-controller

then you choose your preferred ppm mode in focbox UI: forward/brake, hit "calibrate" in r-spec mode (!) and it should work.

and never forget you have to calibrate (hit full throttle, full brakes) EVERYTIME you turn the remote on. Always remote first, calibrate, then turn on the board.
```

---
