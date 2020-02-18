# Motor sensor not working after bearing change (pics)

### Replies: 8 Views: 515

## \#1 Posted by: Komamtb Posted at: 2018-01-03T15:49:50.513Z Reads: 93

```
Hello, I have an older version of koowheel longboard, after some time both motors bearings gave up, so I replaced hem with new ones. One motor works just as fine, the other one stutters a bit and only starts to spin after after being spin by hand. I can tell the problem is with the senor thing, I have already cheked the main board and the motor sensor wires, they all ar okey. This is there my knowledge ends, I don't know what else I should check. I'm adding a few pictures of the motor, maybe someone could shed a light on this problem?
Btw, I'm not sure if I have cut the motor winding at one spot, It may be. <img src="/uploads/db1493/original/3X/d/1/d1f476db8bde451314693745ab13cf20727b9a16.jpg" width="374" height="500"><img src="/uploads/db1493/original/3X/8/c/8c941d1ee04d24fd5720abfd83845e77dc88fa8f.jpg" width="374" height="500"><img src="/uploads/db1493/original/3X/d/f/df7ac3008802518d25d95c14e3834c2a7217513a.jpg" width="375" height="500">
```

---
## \#2 Posted by: willpark16 Posted at: 2018-01-03T21:54:21.466Z Reads: 62

```
What motor?
```

---
## \#3 Posted by: Komamtb Posted at: 2018-01-04T08:11:26.290Z Reads: 47

```
I'm sorry, but what do you mean? Brand? Specs?
```

---
## \#4 Posted by: Komamtb Posted at: 2018-01-08T10:01:43.209Z Reads: 32

```
Can someone help me please?
```

---
## \#5 Posted by: Martinsp Posted at: 2018-01-08T10:03:55.720Z Reads: 33

```
You most probably broke some solder joint or wire while moving stuff around. So you say if you help the motor to start spinning it works fine?
```

---
## \#6 Posted by: Komamtb Posted at: 2018-01-08T10:10:46.245Z Reads: 32

```
Yes it works, but working in unsensored mode that motor loses a lot of torque, motor wires are fine, each one was tested individually, the hall sensor chip looks fine, not even a scratch on it, I would think it's one of the sensors, but I don't  know how to test that.
```

---
## \#7 Posted by: Martinsp Posted at: 2018-01-08T10:12:57.704Z Reads: 30

```
Do you own/use VESC or is it the original ESC?
```

---
## \#8 Posted by: Martinsp Posted at: 2018-01-08T10:24:33.676Z Reads: 30

```
What you could do then is connect the motor to the VESC/FOCBOX as you normally would and try doing detection first without sensors plugged in and if that went okay, without any weird/unusual behavior we can rule out the phase wires. Next would be doing the same with sensors plugged in. I would expect the detection of sensors to fail at this point since all the "problems" point in the hall sensor cable direction.
```

---
