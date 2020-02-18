# Whats the consequence of running less than 7000-8000rpm on my motor?

### Replies: 12 Views: 781

## \#1 Posted by: wagadugu Posted at: 2016-07-14T09:43:08.001Z Reads: 109

```
Hi guys!

I'm new to understanding this, so  I plan on getting a motor with 230KV from the torgue diyelectricskateboard guy and running a 7s6p battery through it.

To help me understand for dummies, is there significant downside to not reaching the 7000-8000rpm people recommend? So far according to the math sheet, my RPM will hit 5796 (after all calculations)
```

---
## \#2 Posted by: evoheyax Posted at: 2016-07-14T17:09:03.579Z Reads: 86

```
less efficiency which will result in more heat across the board.
```

---
## \#3 Posted by: Jinra Posted at: 2016-07-14T17:12:35.224Z Reads: 84

```
To expand, if you run a higher voltage you can get less current draw = less heat = more efficiency! 10S is a sweet spot for efficiency and stability.
```

---
## \#4 Posted by: evoheyax Posted at: 2016-07-14T17:15:08.406Z Reads: 81

```
everyone says 10s is the best of both worlds, but I find 12s works even better, especially with hummies hubs. And no issues on stability with the vesc for me...
```

---
## \#5 Posted by: Jinra Posted at: 2016-07-14T17:18:21.138Z Reads: 72

```
for sure! If you keep the kV low enough you shouldn't have many problems. The main issue lies in voltage spikes during braking that can cause errors/damage in the VESC on larger motors. I'm betting, with the VESC 6.0, these will be non-issues.
```

---
## \#6 Posted by: wagadugu Posted at: 2016-07-14T19:25:38.904Z Reads: 59

```
Thanks for the great insight! I'm really happy I get to learn allot :slight_smile:

What do you mean by voltage spikes? Also asking from experience, do you believe running a 7s or 8s setup would cause a significant enough of a heatup for me to be concerned?

I intend to be driving at most, 20-30km/h and setting up my VESC with a remote capable of throttle control (probably wiiciever and nyko wiimote) for steady progressive breaking

I also intend to encase my battery and vesc in a carbon fibre casing
```

---
## \#7 Posted by: Jinra Posted at: 2016-07-14T20:08:58.108Z Reads: 54

```
Voltage can spike during braking to unsafe levels (for the VESC), though I'm  unsure as to what causes larger spikes. Given the naturally higher voltage of 12s, it's more prone to this than 10s.

People run with 6s setups all the time, I don't think you'll run into issues unless you're working the motor really hard. I hear the wiiceiver is pretty unreliable, but haven't used it myself. Try not to make your entire enclosure in Carbon fiber as encasing all the electronics in that will cause you to have poor signal.
```

---
## \#8 Posted by: wagadugu Posted at: 2016-07-14T20:21:21.453Z Reads: 50

```
Ah alright I see now, I guess i'll have to do more research on what controller I can get that is both compact and has good throttle control.

Based on my experience reading the forums, the wiiciever seems to only have reliability issues when it isn't soldered to the contact (however I may be wrong, there arent really any live cases or video's I can find of someone riding and using a wiiciever however I have found people on the forum who love it and have 4 of them.

In terms of the Carbon Fiber thing, I think it should be fine for me, the carbon fiber enclosure will only cover the bottom portion and it seems like boards such as the raptor or this guys https://endless-sphere.com/forums/viewtopic.php?f=35&t=75291 dont seem to have any issues. Based on my basic understanding of signal interference, wouldn't the carbon fiber only have an effect if it was in-between the electronics and me?
```

---
## \#9 Posted by: Jinra Posted at: 2016-07-14T20:27:26.103Z Reads: 46

```
Yep you'll be fine as long as it's not completely encased in CF. The raptor is fine because the lid is made of glass fiber instead of CF. The original Raptor had a CF lid which blocked signal and caused cutouts.

the GT2B is a well known reliable controller but is fairly large. You can mod it to be smaller. I use this remote myself http://miamielectricboards.com/shop-1/handheld-electric-remote
```

---
## \#10 Posted by: wagadugu Posted at: 2016-07-14T22:24:27.744Z Reads: 38

```
Wow that looks really good! I wonder if its possible to program it set to different % throttles (that would be amazing!)

My only other concern for it is that I live in Canada :( figuring out how to get it here is going to take a bit of time
```

---
## \#11 Posted by: Jinra Posted at: 2016-07-14T22:25:02.113Z Reads: 36

```
By default it has 2 speed modes. The two modes are basically 100% throttle or 50% throttle.
```

---
## \#12 Posted by: wagadugu Posted at: 2016-07-14T22:28:50.920Z Reads: 37

```
ooooo, I like it, curious to see if you could modify the 100% to 75%
```

---
