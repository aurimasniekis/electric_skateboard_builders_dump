# Throtle half useless

### Replies: 11 Views: 209

## \#1 Posted by: KrisKraanen Posted at: 2018-11-08T19:03:55.187Z Reads: 82

```
https://drive.google.com/open?id=1OD0HB2kN6IL3j3HkNOdUtxpeGMhj-vxN 
in the video you can see that only half of my thorttle range is working, this is in current no reverse with braking mode, in Duty mode i do have the entire throttle range to use, but this is not the proper mode
```

---
## \#2 Posted by: mmaner Posted at: 2018-11-08T19:10:02.682Z Reads: 75

```
cant get the video to play...did you do the PPM detection in the VESC tool?
```

---
## \#3 Posted by: KrisKraanen Posted at: 2018-11-08T19:11:30.570Z Reads: 73

```
Yes its the full range, im working on the video its not yet processed on drive think thats why its nit playing, in duty mode the thottle is only 100% when the trigger is al the way up in this mode from the video its there at 50% trigger
```

---
## \#4 Posted by: Sn4pz Posted at: 2018-11-08T19:13:25.612Z Reads: 66

```
uploading your video to youtube is very easy, its a good way to share videos on here (just advising, not angry or anything :) )
```

---
## \#5 Posted by: Jinra Posted at: 2018-11-08T19:15:44.300Z Reads: 61

```
are you a new user using a VESC? sounds like you may not be familiar with how VESCs handle speed and current. Current control will directly control your acceleration not your speed. This means you'll hit full speed at different throttle points depending on current load.
```

---
## \#6 Posted by: professor_shartsis Posted at: 2018-11-08T19:16:00.724Z Reads: 58

```
[quote="KrisKraanen, post:1, topic:73949"]
only half of my thorttle range is working, this is in current no reverse with braking mode, in Duty mode i do have the entire throttle range to use, but this is not the proper mode
[/quote]

my theory is this:

assumptions: 37v, battery, 0.05ohm, 190kv, 90mm tire, 15T motor, 36T wheel, 80a motor current limit, 30a battery limit, 2 motors

https://image.ibb.co/nxMHTV/throttle-range.jpg

^I'm assuming your throttle is programmed for 100% throttle = 80a motor current limit, but because the battery current limit is lower than the motor current limit, at the higher end of the speed range, 80a motor current is not possible (see blue line, top left chart, motor current), so the throttle does nothing above a certain value when at higher rpms.

possible solution: set the motor current and battery current limits to the same value for full throttle range at all speeds:

https://image.ibb.co/ntL82q/throttle-range-2.gif

^with 80a battery & 80a motor limits, 80a motor current is available at all rpms
```

---
## \#7 Posted by: KrisKraanen Posted at: 2018-11-08T19:18:07.464Z Reads: 50

```
https://youtu.be/aVQPoOL4wBw
```

---
## \#8 Posted by: Jinra Posted at: 2018-11-08T19:19:37.751Z Reads: 47

```
Yep that's because there's no load on it.
```

---
## \#9 Posted by: b264 Posted at: 2018-11-08T19:23:06.547Z Reads: 46

```
[quote="Jinra, post:5, topic:73949"]
Current control will directly control your acceleration not your speed.
[/quote]

:arrow_up: this

"Current control" means your trigger controls "amperes" / power level

"PID Speed control" means your trigger controls "km/h" / speed
```

---
## \#10 Posted by: professor_shartsis Posted at: 2018-11-08T19:25:35.866Z Reads: 45

```
@KrisKraanen in the video, your motor appears to already be spinning at no load speed when you attempt full throttle, so because the motor is already at maximum speed, further increasing the throttle will not provide any additional acceleration or rpms...

[quote="KrisKraanen, post:1, topic:73949"]
in Duty mode i do have the entire throttle range to use, but this is not the proper mode
[/quote]

when in duty cycle control mode, by using the throttle you are changing the effective voltage sent to the motor (50% throttle = 50% duty = 50% battery voltage), and so by changing the throttle position you are changing the no load speed of the motor (more voltage = higher no load rpm)

for example, suppose you have a 37v battery and you are at 10% throttle in duty control... the motor "sees" 3.7v... if you have a 100kv motor, you'll get 370rpm no load.

20% throttle in duty control and the motor "sees" 37v * 20% = 7.4v... if you have a 100kv motor, you'll get 740rpm no load.
```

---
## \#11 Posted by: KrisKraanen Posted at: 2018-11-08T23:19:18.859Z Reads: 21

```
So for variable speed control on my eskate i need to use pid?
```

---
