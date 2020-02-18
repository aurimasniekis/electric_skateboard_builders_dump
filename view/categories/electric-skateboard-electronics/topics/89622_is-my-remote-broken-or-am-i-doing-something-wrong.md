# Is my remote broken, or am i doing something wrong?

### Replies: 11 Views: 205

## \#1 Posted by: humanisticnick Posted at: 2019-04-06T19:57:32.889Z Reads: 88

```
https://youtu.be/baNxexCCTfE

I am so close I can taste it. Everything seems to be working physically but I can't seem to be able to see PPM levels of my remote through the VESC tool. Any ideas?
```

---
## \#3 Posted by: SeanHacker Posted at: 2019-04-06T20:14:47.291Z Reads: 81

```
Right off the bat (I haven't finished the video yet), but you need to have your ppm plugged into channel 1.

Also. Always read configuration before changing any settings.
```

---
## \#4 Posted by: xsynatic Posted at: 2019-04-06T20:15:59.570Z Reads: 79

```
Yo..Why does your remote stay connected after turning it off? I have to restart my whole board to repair. Try Editing it in the Input setup wizard again.

EDIT : ↑ what @SeanHacker said. Plug it into the bottom channel (iirc)
```

---
## \#5 Posted by: humanisticnick Posted at: 2019-04-06T20:17:28.380Z Reads: 76

```
I'll try channel one again tonight
```

---
## \#6 Posted by: SeanHacker Posted at: 2019-04-06T20:20:59.217Z Reads: 74

```
If you get stuck. Let me know. I can team viewer in to help you out if you need. Probably not necessary. But whenever you start the vesc-tool, make sure to always read configuration prior to changing anything. 

![Screenshot%20from%202019-04-06%2013-18-08|43x201](upload://4mCvORPVwMYhLbKr6K0xAhCT7Qs.png)

Also. Remember the the nano series remotes need to be calibrated every time before you power on the board. So... turn on the remote, move throttle up and down fully, then turn on the board. This isn't your issue. But most don't know about this.
```

---
## \#7 Posted by: Dirt_Bag Posted at: 2019-04-07T03:25:59.521Z Reads: 56

```
i had this exact problem a long time ago. the issue was one of the usb plugs on a dual flipsky vesc6 was faulty. it wouldnt relay info correctly. It makes no sense, but when i switched to the other micro usb it worked fine. I sent it to flipsky and they sent a replacement. I dont know how old yours is, but a few months back the fixed the issue of the easily broken usb's
```

---
## \#8 Posted by: humanisticnick Posted at: 2019-04-07T03:55:32.739Z Reads: 53

```
Alright I have it working on one side of the vesc by using CH1, thank you!. However if I connect through the other VESC and do the exact same thing it still shows null on the PPM input. Any other secrets you can share?
```

---
## \#9 Posted by: SeanHacker Posted at: 2019-04-07T10:42:07.793Z Reads: 41

```
So your hooked up through canbus right? Or are you using split ppm?
```

---
## \#10 Posted by: JensSjogren Posted at: 2019-04-07T16:24:29.104Z Reads: 27

```
Currently having the exact same issue on my Vesc 6, drives me nuts.. :S #Following
```

---
## \#11 Posted by: humanisticnick Posted at: 2019-04-07T19:14:15.667Z Reads: 16

```
https://youtu.be/M7tLQPK-HPs

I think I just messed up all the settings. A new VESC tool version came out and I reflashed the firmware and set everything up from scratch.
```

---
## \#12 Posted by: SeanHacker Posted at: 2019-04-07T19:19:29.115Z Reads: 16

```
Definitely looks like belt tension. The belt it probably a bit tighter than the other. You can loosen the belt that doesn't spin as long and it should match up or pretty close to matching up. Glad you got it going.
```

---
