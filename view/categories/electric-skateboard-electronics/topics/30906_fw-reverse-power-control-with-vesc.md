# FW/Reverse power control with VESC

### Replies: 6 Views: 1053

## \#1 Posted by: emipop Posted at: 2017-08-17T18:10:27.224Z Reads: 90

```
Hi friends,

I have an Issue for the past 2 days that I cannot get over.
On the Vesc 2.16 (i think) I cannot get the motors to go full speed/power .

Driving forward I have full power and torque, but backwards they get flimsy and stop very soon when reversing.

I am using Alienware 6374 with hall sensors. Vesc. Remote control with PPM. Dutycycle control mode.

The question is where are the settings or tweaks  in BLDC Tool about that?

THanks..
```

---
## \#2 Posted by: jammin Posted at: 2017-08-17T18:24:26.143Z Reads: 90

```
have you adjusted your throttle trim? You can do that manually (on some remotes) or with software control in BLDC.
```

---
## \#3 Posted by: emipop Posted at: 2017-08-17T18:30:41.970Z Reads: 83

```
Yes, the trim is adjusted properly on the remote.
```

---
## \#4 Posted by: wafflejock Posted at: 2017-08-17T18:36:04.225Z Reads: 81

```
Just to clarify in the bldc tool when you check the display in the ppm setup and you go full reverse you are see 0% and full throttle you are seeing 100%?
```

---
## \#5 Posted by: emipop Posted at: 2017-08-17T20:12:22.509Z Reads: 68

```
Yes it is correct.<img src="/uploads/db1493/original/3X/c/6/c6dc90675efeb5b9785aa071d83b0e6222fa5ea6.png" width="690" height="431"><img src="/uploads/db1493/original/3X/6/c/6cfce92223ea6980099d212cfd42eb3e771db16a.png" width="690" height="431"><img src="/uploads/db1493/original/3X/f/d/fde51652901263c3c1b3a3d26c0486b925ab60ab.png" width="690" height="431"><img src="/uploads/db1493/original/3X/1/3/13fa3a6e1f855fa07dedf54e5c2376e9a76c4e74.png" width="690" height="431">
```

---
## \#6 Posted by: emipop Posted at: 2017-08-18T13:49:26.299Z Reads: 41

```
[Youtube Video](https://www.youtube.com/watch?v=8rbyj_KVXb8)

I have made a brief video with the behavior of the motor.

On every direction the stick is at the end of the travel.

Even directing it on the arrow keys in the BDLC does the same.

(The foot is there just to show power and torque)

Help....
```

---
