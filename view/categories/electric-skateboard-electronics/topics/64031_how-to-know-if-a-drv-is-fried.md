# How to know if a DRV is fried

### Replies: 6 Views: 316

## \#1 Posted by: BooYA Posted at: 2018-08-06T14:29:58.476Z Reads: 88

```
Hi guys,
Yesterday FOCBOX was exposed to water and 3 mosfets blew up. I replaced these with new ones and checked connection after soldering to make sure everything is okay MOSFET side.
Tried to run motor detection but failed, values are super high and not corresponding to the usual values of my motor, also the motor won't rotate.
I think that the DRV might be fried as I'm pretty sure the MOSFETs gates were shorted with drain or source so 50V on the gate pin of the DRV seems quite bad to me...
The fault led flashes when I try to run detection. 
But DRV doesn't look bad. 
Do you think I need to replace this one too? 

Thanks for yours inputs 

![20180806_161615|281x500](upload://6RQ0w0w9D8IMsjehVCS644iSXNl.jpg)
```

---
## \#2 Posted by: briman05 Posted at: 2018-08-06T14:47:47.855Z Reads: 72

```
The solder joints on the left side look a little strange like there was heat put on them and the bottom right of the chip looks a little puffy
```

---
## \#3 Posted by: Lospalaz Posted at: 2018-08-08T08:34:04.677Z Reads: 46

```
On the right side, 9th pin from the bottom, I don't see a solder pad.
```

---
## \#4 Posted by: Silverline Posted at: 2018-08-08T08:40:45.499Z Reads: 43

```
Try with "fault" and "faults" in the terminal of the vesc-tool, right after you have run the motor detection
```

---
## \#5 Posted by: banjaxxed Posted at: 2018-08-08T13:56:48.733Z Reads: 29

```
Drv looks fine visually but hard to make out pins needs a clean and another photo and yes check faults in tool
```

---
## \#6 Posted by: BooYA Posted at: 2018-08-10T19:29:03.038Z Reads: 22

```
So I checked on vesc tool, there is no faults when I do motor detection even though the detection fails...
The motor makes a high pitch sound when I try to run it. 
The more I try things, the more I think the drv is fine. Even checked the gate votage regulator, shows 11V on C18/C26.
Do you think that could be a Mosfet problem? Any way to check these?
Thanks guys ![20180810_193651|281x500](upload://d4OFB5a0FkMFfXtCG0dlnNy2HfC.jpg)
```

---
