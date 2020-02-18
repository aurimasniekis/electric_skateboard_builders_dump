# Nano Remote Issues

### Replies: 7 Views: 217

## \#1 Posted by: baxtred Posted at: 2018-10-16T21:41:55.025Z Reads: 93

```
Need some help! I have the newer style nano remote that doesn't seem to have the typical range of PPM values (1.00ms full brake, 1.50ms neutral, and 2.00ms full throttle). Instead it's all over the place.

Here's a couple videos I recorded that compared the torqueboards remote to another similar remote.
https://youtu.be/R0LcWdvQXWE
https://youtu.be/Yvs5Yow_acQ

This is so frustrating. I can't trust the remote and paid quite a bit for it from diyelectricskateboards. Please let me know if you have any ideas. Also how does the reverse switch work? I hold mine for 3 seconds and nothing.
```

---
## \#2 Posted by: CarlCollins Posted at: 2018-10-16T22:22:20.898Z Reads: 75

```
@baxtred
I am not sure but as per my knowledge, there is pulse width shuffle wheel on the NANO remote. have you tried that?
```

---
## \#3 Posted by: baxtred Posted at: 2018-10-16T22:52:52.206Z Reads: 73

```
I don't think so. Can you explain what that is?
```

---
## \#4 Posted by: Jake2k17 Posted at: 2018-10-17T04:40:11.161Z Reads: 59

```
You need to calibrate the remote before riding or it will be very touchy. Imedietly after you turn it on and it binds roll the thumb piece all the way up and all the way down.
```

---
## \#5 Posted by: torqueboards Posted at: 2018-10-17T05:38:54.319Z Reads: 52

```
@baxtred Need to calibrate it as @Jake2k17 mentioned.
```

---
## \#6 Posted by: baxtred Posted at: 2018-10-17T07:37:13.367Z Reads: 48

```
@Jake2k17 @torqueboards 

I truly appreciate the help. I tried the calibration both by turning the board on first, then remote and quickly going full throttle then brake then neutral before the receiver connected. I also tried doing the same thing with the controller turned on first, then the board. Unfortunately both methods still haven't fixed the issue. I have also browsed dozens of posts with the Nano and Nano-X controllers although nobody else is having my issue. 

Maybe I can explain my concerns a little better. 

It seems that the neutral is not at 1.5ms but rather shifted towards the braking region (around 1.3ms). There is a slight workaround, although it has an issue that makes it unsafe. The VESC Tool does allow me to set this 1.3ms as the center point and the board would respond to the controller fairly normally. It would think 1.0ms is full brake, 1.3ms is neutral, and about 1.6ms as full throttle. Unless the controller disconnects or failsafes, at which point the receiver will send the VESC a signal of 1.5ms (I have tested this). This would result in the VESC thinking its receiving about 80% throttle. So with my 6374 setup, a controller disconnection is a 30km/h ride with no way to stop or even slowdown the board. 

I have contacted  support and hopefully they have some ideas. Thanks again for the help!
```

---
## \#7 Posted by: baxtred Posted at: 2018-10-17T07:53:13.218Z Reads: 42

```
I know the older nano remotes had a pot dial that allowed you to fine tune the center. The newer versions seem to have got rid of that (or at least I can't find it).
```

---
