# VESC/first board noob questions

### Replies: 4 Views: 904

## \#1 Posted by: skelstar Posted at: 2017-10-18T00:21:23.188Z Reads: 52

```
Hi, building my first board and I have read a lot of stuff but I need some clarity:

I want a board to commute on and the main features I'm after are "cruise control" and "braking".

Does the cruise-control get managed by the VESC, or is a feature of the remote? 

I'm guessing that the remote just sends a PWM/pulse signal that varies between 1-2ms.

I plan to make my own remote (maybe mod a nunchuk using arduino/esp8266) and I don't know if I do the cruise-control myself in the remote (i.e. by adjusting the 1-2ms pulse-width), or whether the remote is just a dumb trigger.

Also braking is fairly important. I commute down a few very gentle slopes where currently I just get faster and faster and out-of control. I guess all VESCs do braking.

Thanks for your help in advance.
```

---
## \#2 Posted by: bsancken Posted at: 2017-10-18T00:52:03.521Z Reads: 49

```
I am going to point you here to this thread that has alot of additional features. 
[http://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286](http://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286)
From what I have learned sofar, the remote sends the signal (essentially fwd and rev(also used for braking) and the vesc interprets it. The link has new Fw for the vesc that has some additional features for the cruise ctrl and braking and a lot of other stuff too..
```

---
## \#3 Posted by: skelstar Posted at: 2017-10-18T01:28:06.682Z Reads: 42

```
Ah yeah. I was reading that thread a little earlier. Cheers.

So pretty much anything that is called a 'VESC' will do this (but not 'ESCs')? I guess anything that claims to use the BLDC tool.

It looks very nice and customisable.
```

---
## \#4 Posted by: bsancken Posted at: 2017-10-18T01:42:06.180Z Reads: 36

```
A Vesc is basically a smarter esc. I would look for a vesc that is atleast hardware version 4.12 since thats the newest. 

Again, here is some more reading to do. 
[http://www.electric-skateboard.builders/t/new-vesc-user-read-this-complete-walktrough-of-the-vesc/2980](http://www.electric-skateboard.builders/t/new-vesc-user-read-this-complete-walktrough-of-the-vesc/2980)
```

---
