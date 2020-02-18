# Motor problem (detection?)

### Replies: 21 Views: 303

## \#1 Posted by: damnub Posted at: 2018-06-25T21:19:37.628Z Reads: 76

```
hello!

Im finishing up my first diy build and its a lot of fun. But at the final step im having a problem. The motor makes an awful sound sometimes, like its blocking up or something. Im afraid the motor is broken and I need to wait for another month of shipping.

the hardware I have:
6354 215 KV motor
vesc v4.12
8S lipo 5000mah
80mm wheels

I recorded the problem,
https://www.youtube.com/watch?v=nJCqlLvEttY&

as you can see it sometimes just runs smoothly but if i stop and give power again it starts acting up.

I did detect the motor in bldc
Detection results:
Integrator limit: 101.05
BEMF Coupling: 886.57

thanks for reading
```

---
## \#2 Posted by: Ebisane9 Posted at: 2018-06-25T21:21:24.416Z Reads: 73

```
sensored or sensorless?
```

---
## \#3 Posted by: damnub Posted at: 2018-06-25T21:30:53.442Z Reads: 70

```
its sensorless, and its running BLDC
```

---
## \#4 Posted by: Silverline Posted at: 2018-06-25T21:34:22.640Z Reads: 69

```
My sk3 does the same, if i give full throttle from 0 on the bench... I think it's because the motor is without sensors
```

---
## \#5 Posted by: damnub Posted at: 2018-06-25T21:41:22.899Z Reads: 69

```
[quote="Silverline, post:4, topic:60038, full:true"]
My sk3 does the same, if i give full throttle from 0 on the bench… I think it’s because the motor is without sensors
[/quote]

hmm thats awful.. how did you end up fixing it?
```

---
## \#6 Posted by: Ebisane9 Posted at: 2018-06-25T21:41:39.120Z Reads: 66

```
that answers it! The motor cogs because it has no idea what direction it is meant to go. Set up the board with ackmaniac 3.1 and test it loaded. I'm 99% sure the problem will go away. Sensored motors usually don't have these problems on the bench
```

---
## \#7 Posted by: Benjamin899 Posted at: 2018-06-25T21:57:49.519Z Reads: 62

```
yes same here, he has no clue where he is, but once you are on the board you have a smooth start, relativly speaking for a sensorless motor if you use ackmaniac esc tool
```

---
## \#8 Posted by: Silverline Posted at: 2018-06-25T21:59:41.115Z Reads: 60

```
Exactly... 10 char
```

---
## \#9 Posted by: Blacksheep Posted at: 2018-06-25T23:05:04.689Z Reads: 56

```
I have the same problem but with Torqueboards hubs
```

---
## \#10 Posted by: damnub Posted at: 2018-06-26T12:32:13.559Z Reads: 40

```
So I updated the firmware and I setup up the board with ackmaniac. But im still having the same problem. It does it less often but going from forward to backward will trigger it pretty much every time.

I took screenshots of my esc settings: https://imgur.com/a/TdFx8r7
```

---
## \#11 Posted by: Benjamin899 Posted at: 2018-06-26T12:45:08.916Z Reads: 39

```
did you even read the replies?
```

---
## \#12 Posted by: wafflejock Posted at: 2018-06-26T12:45:59.827Z Reads: 37

```
My guess is most of us use the current no reverse with brake option so we don't see this as often, but as people here are saying basically if you push start the board rolling then the motor will already be rotating the right way and shouldn't have a problem continuing along.  Would try changing modes and bench testing with one direction and brakes only and see if it does the same.
```

---
## \#13 Posted by: damnub Posted at: 2018-06-26T12:57:49.756Z Reads: 35

```
[quote="Benjamin899, post:11, topic:60038, full:true"]
did you even read the replies?
[/quote]
yeah. but I would prefer to actually fix it instead of just using a work around.

[quote="wafflejock, post:12, topic:60038"]
Would try changing modes and bench testing with one direction and brakes only and see if it does the same.
[/quote]
If I use the no reverse option it pretty much disappears.
```

---
## \#14 Posted by: Ebisane9 Posted at: 2018-06-26T13:02:36.835Z Reads: 30

```
Lmao bro it’s not a work around. Jesus just listen or read 😂. Go read about sensored va sensorless. THATS HOW THE MOTOR IS SUPPOSED TO BEHAVE WHEN SENSORLESS. Sheesh i can’t waste my data anymore
```

---
## \#15 Posted by: Holyman92 Posted at: 2018-06-26T13:02:59.265Z Reads: 28

```
damnub, because its sensorless there is no fix, you HAVE to kick start ur board or make it spin by hand 1st when bench testing... its because thay have no way of sensing the orientation and they spaz out lol
```

---
## \#16 Posted by: Holyman92 Posted at: 2018-06-26T13:04:47.141Z Reads: 28

```
its just the nature of the beast my friend, if u want to start it from a dead stop u HAVE to have hall sensors, u can add them in easily w/ some epoxy and by building a circuit or by buying the sensors from APS
```

---
## \#17 Posted by: damnub Posted at: 2018-06-26T13:07:26.280Z Reads: 27

```
[quote="Ebisane9, post:14, topic:60038"]
Lmao bro it’s not a work around. Jesus just listen or read :joy:. Go read about sensored va sensorless. THATS HOW THE MOTOR IS SUPPOSED TO BEHAVE WHEN SENSORLESS. Sheesh i can’t waste my data anymore
[/quote]
ay okay should have done more reading.. Sorry

[quote="Holyman92, post:16, topic:60038, full:true"]
its just the nature of the beast my friend, if u want to start it from a dead stop u HAVE to have hall sensors, u can add them in easily w/ some epoxy and by building a circuit or by buying the sensors from APS
[/quote]
Thanks for your reply ill look into this.


Well thanks for your help yall
```

---
## \#18 Posted by: Holyman92 Posted at: 2018-06-26T13:09:24.489Z Reads: 24

```
yea, i saw this a lot when i first started here and because of this very issue i decided to buy sensored motors instead of SK3's. however i findmyself in brushless sensorless mode most of the time anyways lol
```

---
## \#19 Posted by: linsus Posted at: 2018-06-26T13:50:41.024Z Reads: 25

```
With sensorless motion the vesc attempts to make the motor spin briefly before applying the full action you're performing from the remote. If the motor is already spinning then the vesc will get feedback anyway and the motor will be responsive right away. so if you're already Rolling you wont experience the stutter that has so famously been taken for an error here on the forum. The sound your motor is making in the video however isnt healthy. If starting from an absolute standstill the pre rotation should take place before the full throttle and you wont have that sound. Wont recommend performing the action on the bench without load tho. Can be missguiding. However, you will never have the direct response you seem to be looking for. Hall sensors will provide it however. 

There are sevral ways to tweak the "stutter" you can go read about it on vedders forum. Should be several topics discussing the matter.
```

---
## \#20 Posted by: damnub Posted at: 2018-06-26T14:01:03.710Z Reads: 23

```
thanks for your explained reply.
It makes alot of sense. and I did try it off the bench but i got some other problems so I thought it was all caused by the motor. turns out the shaft and pulley were slipping, and I had almost no torque. (i made a flat spot and now im waiting for the loctite to dry)

ill try to keep the stutter as little as possible so save the motors life.
```

---
## \#21 Posted by: Holyman92 Posted at: 2018-06-26T14:16:23.599Z Reads: 19

```
the sound ur hearing is the motor stuttering and the board vibrating on the countertop lol
```

---
