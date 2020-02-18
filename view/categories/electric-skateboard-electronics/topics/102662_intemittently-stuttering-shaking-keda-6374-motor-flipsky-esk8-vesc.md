# Intemittently stuttering/shaking KEDA 6374 motor Flipsky esk8 vesc

### Replies: 6 Views: 129

## \#1 Posted by: kephart Posted at: 2019-10-07T19:41:14.081Z Reads: 45

```
Hi,

I have an intermittent problem with my KEDA 63-64 190KV with a 6S Turnigy 4000mAH 60C battery. From time to time unclear why it stutter and shakes. It happens even with very little load sometimes, even without load with the wheel spinning freely. After a press on the throttle again it mostly goes away. I made a screenshot of the current plot of when it happened without load. The stuttering can be seen at the end to the right. The motor current is high and the motor hardly moves. Does anybody have a clue what can be happening here? When this starts to happen with load on the street I can hardly get anywhere and it stops repeatedly and waits for the timeout delay. Could it be the phase cable connectors? Or the VESC settings?

![Stuttering|690x362](upload://53CKdrNTELnnoA8mUgSx7IXKjuE.png)
```

---
## \#2 Posted by: Ben.Nexus Posted at: 2019-10-07T20:01:12.315Z Reads: 38

```
Is your motor sensored? Does this happen while you're riding?
```

---
## \#3 Posted by: kephart Posted at: 2019-10-07T20:06:06.024Z Reads: 38

```
No, its a sensorless motor.
```

---
## \#4 Posted by: kephart Posted at: 2019-10-07T20:11:05.940Z Reads: 38

```
It happens sometimes when I'm riding too. Then its shuts down for the timeout of 3s and then I can accelerate again, but I'm not 100% sure that is the same problem. I'm trying to get a bluetooth chip working so I can debug with my phone. I'm suspecting bad phase wire connectors. I have cheap car crimp connectors, not sure where to get bullet connectors in Stockholm, Sweden, but I guess they are available online somewhere too and I will get them when I'm ordering something else.
```

---
## \#5 Posted by: Ben.Nexus Posted at: 2019-10-07T22:15:21.146Z Reads: 35

```
If you need bullets, I can ship you some. I don't stock them directly on my store but I have 5.5 and 3.5mm ones
```

---
## \#6 Posted by: kephart Posted at: 2019-11-11T15:18:55.361Z Reads: 15

```
I searched the forum some more and it seems to be related to the phase cables being loose. I tried to fix the cables on the motor side and when coming into my enclosure with zipties and this seemed to do the trick. Haven't had the problem since. I will get bullet connectors too eventually. It happens that a phase cable shakes loose.![20191111_161511|666x500](upload://hucOjkM2wptLZQVJrozuF3G9XG6.jpeg)
```

---
