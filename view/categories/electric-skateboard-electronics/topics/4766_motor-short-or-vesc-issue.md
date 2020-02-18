# Motor short or vesc issue?

### Replies: 4 Views: 1242

## \#1 Posted by: shred Posted at: 2016-06-16T10:17:02.434Z Reads: 153

```
Hey guys, I would need some help with the following. I already posted most of it as well in my build thread but will post it here now in a separate thread. 

Setup:
10S + VESC + sensor less [url=http://alienpowersystem.com/shop/brushless-motors/alien-6355-outrunner-brushless-motor-190kv-2200w/]190kv 2200W motor from APS[/url] + mini remote

Problem:
When I pull the trigger / accelerate harsh, like fast to full throttle in most cases it just accelerates as it should, but sometimes I get a rattling noise from the motor and the motor actually spins backwards with harsh vibrations. 

Not sure what this is about, VESC settings look ok to me. I as well checked motor connectors, motor wires and VESC motor wire connections also removed the belt so the motor can spin freely. It as well seems that this only happens when I try to accelerate quickly. 

Here is the real time data, look at the most right spike, this is the one where the motor actually stutters / rattles and spins backwards. Max amps are drawn so I'm tempted to think it's a short even though this seems to be odd. It also only seems to happen while accelerating from a stand still. 

<img src="/uploads/db1493/original/2X/f/f24066ad7cbad241dce17da1236abd55eb483b46.jpg" width="690" height="370">

Motor Detection Results:
Integrator limit: 99.59
BEMF Coupling: 767.10

VESC Settings:
<img src="/uploads/db1493/original/2X/c/c44d228f158e90e6453fc66bc14e46abae454c8d.jpg" width="690" height="333">

<img src="/uploads/db1493/original/2X/f/fc103ffffb259667c8e54880acc7ff6afbddc3a7.jpg" width="690" height="333">

<img src="/uploads/db1493/original/2X/6/68d8ba0af914bdd1e9874a6c3e7b860ec89c922c.jpg" width="690" height="333">

<img src="/uploads/db1493/original/2X/1/14ca4e90025947758050fbe1e2d112c149c42842.jpg" width="690" height="333">

Here's a video:
https://www.youtube.com/watch?v=CfvEXWM94Ro

Not sure what this is about, but I don't like it. I wen't again through all the VESC settings, restored the defaults, redid motor detection, did setup all anew but all didn't fix it. The motor looks good, it only has a few km on the clock so is basically new. 

Any ideas?
```

---
## \#2 Posted by: Tarzan Posted at: 2016-06-16T11:02:41.004Z Reads: 111

```
Try to accelerate on the bench and move the motor cables close to the motor.
I had a short inside the motor and that was the issue.
I could fix it with shrink tube.
```

---
## \#3 Posted by: JTAG Posted at: 2016-06-16T23:11:55.472Z Reads: 95

```
I had exact this behavior once, at the same time I had low torque.  Ended up to be one phase wire being  disconnected.
```

---
## \#4 Posted by: shred Posted at: 2016-06-17T06:28:07.387Z Reads: 85

```
Thanks guys! I will need to look at this more closely and do more tests, been doing a short easy ride yesterday before the rain hit without a problem, been pushing it to get it rolling though and been quite careful anyway. 

Not going to have much time on the weekend to look into it but will have some days off next week :)
```

---
