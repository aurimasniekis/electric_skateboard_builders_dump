# Raptor- Replaced VESC and remote&hellip;problems

### Replies: 9 Views: 1208

## \#1 Posted by: sprocket12 Posted at: 2016-08-31T01:40:18.145Z Reads: 93

```
So we replaced the VESC on  Raptor single drive and a remote.  I did motor detection and got the settings from the old VESC (I think).  I also recalibrated the new remote.  Anyway, it's a death trap now.  It will cut out randomly and decide to just stop.  This happens within the first two minutes and then has issues with any remote commands (accelerate, stop, slow start, etc.).  When first turned on it seems fine but then BAM!

Here are the VESC settings
<img src="/uploads/db1493/original/2X/8/83ef1bd669507f8f16b29e54143dd0ad2ac5931f.png" width="690" height="364">
<img src="/uploads/db1493/original/2X/f/f69a5f8fabe406998a6684f78f5b7afe8d9b96f6.png" width="690" height="364">
<img src="/uploads/db1493/original/2X/0/0402d7861bebf5232ad7497bda71b07bfe6636b4.png" width="690" height="364">
<img src="/uploads/db1493/original/2X/9/97caf29f741b1cecc73964919dcd4695599e6e1c.png" width="690" height="364">
<img src="/uploads/db1493/original/2X/0/0ee402126cfe366ab20b4c7b7dc1966122b23168.png" width="690" height="364">
```

---
## \#2 Posted by: Blasto Posted at: 2016-08-31T02:06:30.287Z Reads: 80

```
Try ppm only on your app page, your max and min settings seam to be off. It should be something close 1 min and 2 max.

Untick the can fowarding and traction control (single motor)

Set your max erpm to 70000
```

---
## \#3 Posted by: sprocket12 Posted at: 2016-08-31T02:47:45.035Z Reads: 75

```
Ok.  Updated to new settings, except remote.  It is a new 'Winning' remote.  It won't zero out without setting it to 1.35.  Otherwise it will take off.  

Anyway, no difference.  Same results...
```

---
## \#4 Posted by: JohnnyMeduse Posted at: 2016-08-31T02:49:05.365Z Reads: 75

```
Did you charge the remote, also witch binding procedure did you follow
```

---
## \#5 Posted by: JohnnyMeduse Posted at: 2016-08-31T02:53:05.211Z Reads: 71

```
Also, your remote setting are a bit off, did you set the pulsewith parameter usine the display
```

---
## \#6 Posted by: JohnnyMeduse Posted at: 2016-08-31T03:15:01.201Z Reads: 73

```
This might help you

http://www.electric-skateboard.builders/t/vesc-faq-setting-up-receiver-and-brakes/244
```

---
## \#7 Posted by: sprocket12 Posted at: 2016-09-03T22:57:57.428Z Reads: 61

```
So I wanted a chance to update and test before I replied.  It didn't help.  Still 'stutters' at random times.  I've had it on the bench with no load and I have seen it happen.  Since the VESC and remote have been swapped, could it be the motor?  Battery????  I'm stumped.
```

---
## \#8 Posted by: onloop Posted at: 2016-09-04T00:09:21.478Z Reads: 59

```
I would say the two likely issues are.

1. Motor shorting inside. Open it and check for small burn marks. To open the motor you will need to remove it from the mount. Remove the motor pulley. Then remove the circlip at the Base of themails exposed shaft.

2. The fail safe needs to be reset on the remote.
Binding procedure as follow:

1).Check and make sure all the wires are mounted,and the remote is off, insert the bind plug into CH3(Bind) on the receiver;
2).Switch on the boards power, you can see the receiver red light flash;
3).Press and hold on the bind button on the remote and then switch the remote on;
4).You should notice the transimitter go from flashing red to solid red,and also the solid red of the receiver;
5).Once you see a solid red light, you now know the two are binded together,and please pull the bind plug out (do not turn off the power or touch the throttle) this is important, so the remote can record the throttle nutural position to set as the fail safe.
6).Then you can test it again by turning off the controller and it should flash. if you turn the power on Transmitter back on it should go back to solid red.

3. Set the ppm / deadband setting in vesc.
```

---
## \#9 Posted by: elkick Posted at: 2016-09-04T10:52:00.896Z Reads: 43

```
You need to update your firmware, it has the max ramp step error: http://www.electric-skateboard.builders/t/psa-remember-to-reset-your-max-current-ramp-step-when-programming-your-vesc/6262
```

---
