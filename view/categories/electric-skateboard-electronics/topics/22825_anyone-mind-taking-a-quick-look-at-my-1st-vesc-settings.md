# Anyone mind taking a quick look at my 1st VESC settings?

### Replies: 3 Views: 507

## \#1 Posted by: lastmango Posted at: 2017-05-11T04:04:38.330Z Reads: 106

```
Hi all... (@flatsp0t—I'm hitting you up).I've been putting my stuff together and after a few problems were worked out (with mechanics, not electronics) I'm ready to get some VESC stuff going. I'm 185lbs & I've got a single Torque Boards 6374 (Hall sensor, but not connected) hooked to a DIY Skateboards VESC & Space Cell 10s3p with integrated on/off, etc.. I did the motor detection & followed the DIY tutorial. So far, so good. I've written everything you see in the shots. My controller (2.4 nano from DIY) should be here tomorrow, so everything I've done so far is without a transmitter/receiver. Really just want to check that nothing is crazy out of line. Also, if I ultimately run in FOC mode, which I think I eventually want to do, will I fry the VESC? Getting a lot of mixed info as I read. 

Random stuff that might help about my setup:

Motor:
TorqueBoards 6374 190kv
 Max Power: 3150 Watts
Max Amps: 80 Amps

VESC:
DIY Skateboards BLDC with micro USB connection
v4.12 Hardware
v2.18 Firmware for FOC

Battery:
10s3p with 40amp fuse

Thanks in advance, all!

<img src="/uploads/db1493/original/3X/c/4/c4701b4a71316c5570d7ee480b3f9b212b4ce389.png" width="690" height="385"><img src="/uploads/db1493/original/3X/0/d/0d1325a1ad98670584cdd99b276b96a51d8c633e.png" width="690" height="385"><img src="/uploads/db1493/original/3X/0/7/079481a2fc5bfd3c9d852b7dc28ce773db731000.png" width="690" height="385">
```

---
## \#2 Posted by: dogeatgod Posted at: 2017-05-11T18:45:48.831Z Reads: 60

```
Battery cut off start and end look to be set the same. You wont get any early signs of nearing limit before shutting down.
Be careful if changing between FOC and BLDC - there's a good few posts on precautions to take.
```

---
## \#3 Posted by: yaca Posted at: 2017-05-11T20:20:23.188Z Reads: 53

```
When you have your remote don't forget to adjust min and max pulsewith. For beginning I would try Motor Max 60 and Motor Min -45 and if this is not enough you can go higher.
```

---
