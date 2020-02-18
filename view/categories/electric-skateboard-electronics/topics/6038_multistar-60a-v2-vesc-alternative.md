# Multistar 60A v2 - vesc alternative?

### Replies: 13 Views: 1830

## \#1 Posted by: Lizardking0069 Posted at: 2016-07-13T17:12:01.423Z Reads: 181

```
Like many people here in esk8 i have been waiting for vescs to come back in stock for a long time. I researched multiple alternatives, but most ESCs were either more espensive than the vesc or not in stock. However, in the HV section of hobbyking website I saw a little esc with 60A continuous rating (the vesc is 50A continuous) for $37 and I thought I'd give it a try. 

Link: http://www.hobbyking.com/mobile/viewproduct.asp?idproduct=84705

The Multistar 60A ESC is sold as a helicopter ESC but mine came with the BLheli Multirotor firmware installed, which is great because multirotors can have bidirectionality, meaning forward neutral and reverse. I also bought the multistar programmer. I downloaded the blheli suite and proceeded to configure the esc. I made sure to have bidirectionality on and lowered the motor initial power to the lowest setting and turned off dampened light. I soldered some 5mm connectors and a 90xt to test. Bear in mind this is an OPTO esc so there is no bec and you will need a power source for the reciever. 

Results: tomorrow
```

---
## \#2 Posted by: Lizardking0069 Posted at: 2016-07-13T17:25:49.065Z Reads: 177

```
Settings

<img src="/uploads/db1493/original/2X/3/3f234eedc90b6b0a9899a8cd192e6f07d6c7bfa7.png" width="625" height="500">
```

---
## \#3 Posted by: Namasaki Posted at: 2016-07-13T22:59:24.582Z Reads: 145

```
What about brakes?
If you try to use reverse for braking, you might get launched off the board.
```

---
## \#4 Posted by: themegak Posted at: 2016-07-13T23:07:00.248Z Reads: 140

```
Interested in hearing how this goes...
```

---
## \#5 Posted by: Namasaki Posted at: 2016-07-13T23:25:28.773Z Reads: 137

```
Please be careful and wear a helmet.
```

---
## \#6 Posted by: Lizardking0069 Posted at: 2016-07-14T01:37:02.866Z Reads: 130

```
I couldn't wait so I set it up and tested it out. First thing was that I need to switch motor wires because reverse is forward on the nano torqueboards controller. I had to trim the controller with a little screwdriver to reach the center or zero throttle. I noticed that the low power startup tends to cog the motor and is really slow, but then 3-4 seconds later it jumps to the appropriate rpm for that input. It almost knocked me off the board. The torqueboards 6355 motor is a beast, it easily propels me forward. The freewheel works when going forwards but backwards the board stops abruptly. I'll keep tweaking the esc to see if I can get it to work.
```

---
## \#7 Posted by: Lizardking0069 Posted at: 2016-07-14T16:57:27.985Z Reads: 111

```
<img src="/uploads/db1493/original/2X/f/f3c57f51ee788d197cb7a918a49577cc1ab125f7.png" width="625" height="500">
```

---
## \#8 Posted by: Lizardking0069 Posted at: 2016-07-14T17:02:12.413Z Reads: 107

```
https://youtu.be/thj-JAFgaF0
```

---
## \#9 Posted by: Lizardking0069 Posted at: 2016-07-14T17:25:50.288Z Reads: 99

```
There is a bit of cogging when loaded but acceleration is better. Need to esperiment with demag and timing. Using the high frequency setting there is much less heat. Maybe i can resuce the reverse range so that it only barely activates and works as breaks.
```

---
## \#10 Posted by: Lizardking0069 Posted at: 2016-07-14T23:52:25.797Z Reads: 88

```
<img src="/uploads/db1493/original/2X/9/94c4aee2c5c1bb1f1d261443d625a686663e9531.jpeg" width="640" height="480">

Darn it!
```

---
## \#11 Posted by: Lizardking0069 Posted at: 2016-07-15T00:12:23.141Z Reads: 89

```
 The esc burned while I was sitting on the board trying to set the center throttle on the controller. The wheel was slipping under me trying to accelerate and just when I thought I should get off the board and let it spin freely the esc cought fire. The low rpm power protect should have been "on" and I had it "off". This esc does not have a temperature sensor so that setting could not be changed.

I would not ride with this esc. It doesn't have thermal shutdown like other escs and, while blheli is excellent, it does not have the few but necessary configuration settings for a proper electric skateboard esc. Namely, regenerative breaking and slow acceleration.

It has been a learning experience nontheless, and thankfully I was unharmed and none of the other components was damaged.
```

---
## \#12 Posted by: DeathCookies Posted at: 2016-07-15T06:31:57.340Z Reads: 84

```
If you had used a 120a rated ESC it would not have burned. I'll bet it!
```

---
## \#13 Posted by: Lizardking0069 Posted at: 2016-07-15T11:06:28.232Z Reads: 76

```
Maybe. I noticed that this 60 A continuous esc got hot whenever pushing a load such as myself or at low frequency. High frequency helped keep it cool but it wasn't enough. I'd say thermal shutdown is a must on skateboard escs because of the potential risk of fire.
```

---
