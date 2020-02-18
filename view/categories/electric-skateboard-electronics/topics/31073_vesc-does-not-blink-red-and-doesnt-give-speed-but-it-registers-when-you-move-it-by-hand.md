# VESC does not blink red and doesn&rsquo;t give speed but it registers when you move it by hand

### Replies: 6 Views: 580

## \#1 Posted by: Sander Posted at: 2017-08-19T23:42:50.690Z Reads: 63

```
Hi I believe my VESC is shorted but I'm not sure.
I do not get any faults code.


When I power the VESC, it does not blink red on startup.
But when I move the trigger it lights up the white led but does not move the motor.
When I spin the motor with my hand, it shows in the graph the rpm of the motor.

So what is wrong with this VESC? Did I blow it up?

Pictures:
<img src="/uploads/db1493/original/3X/1/1/11cc9c0651dc44463265a20ed96acd7003f98710.jpg" width="690" height="459">

<img src="/uploads/db1493/original/3X/f/c/fc7d5266576dc92410ca2edbc4fdf8915349d6f0.jpg" width="690" height="459">

You see on the bottom the route is visible, didn't get any good images because my phone is empty and I am using the camera of the laptop.


Thanks.
```

---
## \#2 Posted by: i2oadsweepei2 Posted at: 2017-08-21T15:08:23.625Z Reads: 44

```
I think something similar happened to me when I was setting mine up. I'm still a noob at vesc anything. Is there any chance that the control mode is disabled from when setting up PPM?. Just a thought. Best of luck.

Edit* maybe share your screen shots so others may help.
```

---
## \#3 Posted by: xxlv Posted at: 2017-08-21T15:52:40.355Z Reads: 40

```
most likely defective DRV chip. Had this behaviour many times. Write me a PM maybe i can repair it for you
```

---
## \#4 Posted by: Sander Posted at: 2017-08-21T20:23:14.106Z Reads: 36

```
Well I figured out mine blow up. It was not very easy to see, it works fine but not the driver chip. The routing with the capacitors were blown away so there are no more. ;) And with the blinking was it resetted the config to the default.
```

---
## \#5 Posted by: jtreiman Posted at: 2017-08-22T05:25:33.795Z Reads: 26

```
DRV.... Anyone know a VESC that doesn't murder drv? Seems like this is too common of a problem.
```

---
## \#6 Posted by: Sander Posted at: 2017-08-22T13:00:48.066Z Reads: 22

```
Well in my case it was some metal that bounced around inside there and shorted it.
```

---
