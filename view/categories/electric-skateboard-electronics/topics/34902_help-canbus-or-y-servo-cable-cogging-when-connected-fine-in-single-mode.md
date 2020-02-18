# Help, CANBUS or Y SERVO cable cogging when connected. Fine in single mode

### Replies: 20 Views: 938

## \#1 Posted by: Funktapus Posted at: 2017-10-06T01:15:52.778Z Reads: 104

```
Hello,
I'm hoping someone might be able to shed some light on my problem. Whenever I connect my dual setup with the CAN BUS cable, both motors shutter when I accelerate on the controller (this is on the bench).

When I disconnect the CAN BUS cable, the motors work fine (separately) when tested. I think it might be VESC TOOL settings as it did work the first time I tried it and I managed to take it out for a test ride. After making some changes in VESC TOOL the problem started.

Another clue is that when I had both motors connected to power without the CAN BUS cable, the master motor would shutter when I accelerated on the controller. But when I disconnected the power to the slave motor, it would spin fine. I then made some changes in VESC TOOL and now the master motor spins fine when both motors are connected to power (without CAN BUS cable).

Any info would be appreciated . Thanks in advance.

My setup is:
6355 190kv DIY motors x2
DIY vescs x2
10s 3p Samsung INR18650-30Q 3000mAh 15Amp
Bestech BMS
Nano X controller

<img src="/uploads/db1493/original/3X/f/0/f0b08e5abea5bda660cc8c826148a3d976eaae5a.jpg" width="150" height="500">

<img src="/uploads/db1493/original/3X/e/c/ecce4fbe13305b6052f403db6b7aa24f9fbce990.jpg" width="150" height="500">
```

---
## \#2 Posted by: Jinra Posted at: 2017-10-06T01:35:47.334Z Reads: 85

```
master should have "multiple escs over can" checked and "send status over can" unchecked.

slave should have the opposite for both.

Is this the case?
```

---
## \#3 Posted by: Funktapus Posted at: 2017-10-06T01:58:57.876Z Reads: 82

```
Hi Jinra, this is the case. If you click the images on my post (it expands to show more) you can see it under the app section.

Here's another clue. 
I just tried using a split servo cable instead (without the 5v) and with same settings on both vescs and I'm still getting cogging on both motors.
```

---
## \#4 Posted by: Jinra Posted at: 2017-10-06T02:12:41.978Z Reads: 75

```
is it cogging on the bench or loaded
```

---
## \#5 Posted by: Funktapus Posted at: 2017-10-06T02:24:06.571Z Reads: 73

```
Both. I tried it loaded and with a push and it just shuddered.  Doesn't cog when setup as single drive though. The shuddering behaviour is more like when you have a shorted motor.
```

---
## \#6 Posted by: JdogAwesome Posted at: 2017-10-06T02:31:29.225Z Reads: 72

```
Are your motors sensored? If so you need to do a motor check for each and have your sensor table numbers different for each motor and VESC.
```

---
## \#7 Posted by: Funktapus Posted at: 2017-10-06T02:41:59.485Z Reads: 67

```
They're sensored but I was setting them up as in unsensored and running the motor detection as unsensored. I can't test them sensored at the moment because I don't have the cable adapters. Would this make a difference?
```

---
## \#8 Posted by: JdogAwesome Posted at: 2017-10-06T03:05:35.430Z Reads: 62

```
No thats fine you can run sensored motor in unsensored mode so thats not it. If there cogging are you sure the motor detection was done properly and did you bump the Low Duty in the detection area to 0.4 instead of the stock 0.05? You should always do that when detecting hub motors.
```

---
## \#9 Posted by: Funktapus Posted at: 2017-10-06T03:19:59.052Z Reads: 61

```
Motor detection was fine except for a 'unkown hall error:255'. Sensor mode is set to 'sensorless' though. They're not hub motors though. Is the low duty still ok at 0.05?
```

---
## \#10 Posted by: Funktapus Posted at: 2017-10-06T04:29:15.628Z Reads: 63

```
Just an update. I thought it might have been a setting in VESC TOOL so I flashed both vescs for BLDC TOOL but I'm still getting the same results there too. Doesn't matter if it's CANBUS or split servo cable, motors are still shuddering. They work fine in single mode though. Here's a quick video.

<iframe width="560" height="315" src="https://www.youtube.com/embed/vQIpa-FnNZA" frameborder="0" allowfullscreen></iframe>
```

---
## \#11 Posted by: Funktapus Posted at: 2017-10-06T04:29:45.855Z Reads: 63

```
https://youtu.be/vQIpa-FnNZA
```

---
## \#12 Posted by: Funktapus Posted at: 2017-10-06T05:46:04.903Z Reads: 60

```
SOLVED.
By chance I found another post (totally different description, same symptom). 
The bolts that hold the motor to the bracket were shorting the motors. I was using the standard ones that came with the mount and they protrude 2-3mm beyond the motor casing and into the motor. 3 out of 4 bolts might be ok but some of the wiring was close enough to cause a short. I've filed them down now and everything is perfect. I've got no idea how @MaxAssist diagnosed that one in his post. The bolts would've been that last place I would have looked at. Thanks for your help everyone.
```

---
## \#13 Posted by: Jinra Posted at: 2017-10-06T05:48:52.916Z Reads: 58

```
but why did they work individually? :thinking:
```

---
## \#14 Posted by: Funktapus Posted at: 2017-10-06T06:36:51.210Z Reads: 56

```
That's exactly what I was thinking. The only thing I can think of is that on its own it wasn't a short. But when both motors have power, the whole dual bracket/truck became part of the circuit (since it was connected to the bolt) and together somehow they made a short.
```

---
## \#15 Posted by: marcmt88 Posted at: 2017-10-06T14:21:24.249Z Reads: 48

```
Can you put up a link to that particular post?
Thanks!
```

---
## \#16 Posted by: Funktapus Posted at: 2017-10-06T20:31:13.797Z Reads: 47

```
http://www.electric-skateboard.builders/t/helps-needed-on-12s4p-dual-6355-setup/32338/5
```

---
## \#17 Posted by: MaxAssist Posted at: 2017-10-07T07:41:30.858Z Reads: 40

```
I'm glad that my post had saved your day as I totally understand your pain. I was pulling my hair while trying every single solution I could think of. Man, it was frustrated but totally worth it bc the more you do, the more experience you'll get.
```

---
## \#18 Posted by: MaxAssist Posted at: 2017-10-07T07:58:56.731Z Reads: 39

```
I think the bolts didn't really short the motors as I'd tested them for a good period of time like that without burning my DRVs (this including FOC). The only reason to explain this IMO is when only one motor connect the battery is still capable to provide enough power for it to spin smoothly. In another hand when two motors hook up the leakage + the amp drawing is too much for the battery to handle. In this case I saw sparks between my belts and mounts and motors over heating under heavy throttle.
```

---
## \#19 Posted by: Graphite Posted at: 2017-10-07T12:57:06.165Z Reads: 40

```
I literally found out the same a while ago when setting up my dual drive. I think this needs to be added to the list things to do when stuff isn't working. Took me forever to find out but I was testing my board and only left 2 nuts on each motor, worked perfectly after that. Really glad I didn't permanently break anything.
```

---
## \#20 Posted by: Funktapus Posted at: 2017-10-07T21:34:27.328Z Reads: 33

```
The reason why I never bothered to suspect my motor mount bolts was because they were the standard ones that came with the kit. I would still like to know what exactly is happening electrical wise. Didn't seem to harm my set up as I triggered the cogging so many times when I was trying diagnose it. What's apparent is that the whole motors/mounts/truck assembly becomes unified as a circuit. I wonder if the same thing would happen if you bridged one phase wire from one motor to another motor.
```

---
