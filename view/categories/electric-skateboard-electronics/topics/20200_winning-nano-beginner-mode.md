# Winning Nano beginner mode

### Replies: 4 Views: 438

## \#1 Posted by: flyboywebb Posted at: 2017-04-03T15:48:54.621Z Reads: 76

```
Hey guys...kinda new to this but I have a winning nano and want to have a beginner mode for my kids. The remote itself doesn't have a beginner switch. Is there a way to use Bluetooth module and BLDC app to create a beginner mode? Thanks much for any help! Randy
```

---
## \#2 Posted by: mmaner Posted at: 2017-04-03T16:00:08.369Z Reads: 70

```
If you use the firmware by @Ackmaniac you can create modes using the Android app and a bluetooth module connected to the VESC.
```

---
## \#3 Posted by: Nordle Posted at: 2017-04-03T16:13:38.491Z Reads: 63

```
You can just reduce max rpm in bldc tool, _only in bldc mode (no foc) i assume._
and be very sure to set the winning remote up correctly
```

---
## \#4 Posted by: yaca Posted at: 2017-04-03T20:26:51.897Z Reads: 42

```
Yes with ackmaniacs firmware and his android app it's easy and fast to change for a beginner. Of course you can also change the setting in bldc tool but instead of reducing the max rpm you better use "Soft RPM limit" for to limit the end speed and for to reduce the power you can reduce "Batt max" or "Max Watt" if you use ackmaniacs firmware.
```

---
