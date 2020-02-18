# VESC flashing GREEN light? help

### Replies: 10 Views: 595

## \#1 Posted by: Brando Posted at: 2017-08-18T05:36:19.339Z Reads: 85

```
I am running dual motor foc mode with torque board's VESCs (208KV on 10S). My board was upside down on the test bench and I tested the throttle. both motors spun up to top speed and then my master vesc's motor shreeched to a halt. After this, my VESC will not work. when I boot it up, the Blue light comes on as usual, but the red light never does that triple flash. Instead, the Blue remains solid and the green led starts blinking.
So I don't think this is DRV failure, that results in a red flashing light. Apparently green stands for "command" whatever that means.
When I plug it into my PC, windows says "could not recognize this usb device". BLDC tool wont connect.
I have never seen this issue on a thread before. What happened? Did the motors spin too fast? I turned off limit eRPM with negative torque. My battery is at 37V so my eRPM was 37V*208KV*7= 53,872eRPM. should be safe right?

EDIT: after rebooting it again, the green light no longer shows. Just solid blue. windows doesn't even see it anymore.
```

---
## \#2 Posted by: L3chef Posted at: 2017-08-18T05:47:01.561Z Reads: 83

```
Are you running can bus or split servo?
```

---
## \#3 Posted by: Brando Posted at: 2017-08-18T06:05:39.118Z Reads: 78

```
Can bus.
10 char
```

---
## \#4 Posted by: Dazeto Posted at: 2018-07-30T00:41:16.879Z Reads: 46

```
i have the same issue with the slave vesc, only it happened after the motor cables got caught up by the motor itself then the board shutoff and wouldn't turn on again until i disconnected everything and plugged the charger. reconnected and only master vesc works. any help greatly appreciated
```

---
## \#5 Posted by: briman05 Posted at: 2018-07-30T03:13:07.272Z Reads: 43

```
So the phase wires got caught in the motor? You could have broken a solder joint.
```

---
## \#6 Posted by: Dazeto Posted at: 2018-07-31T02:05:10.337Z Reads: 36

```
well, there are very tiny brown marks on the soldered spots in the red and black cables at the back of the pcb. but how to fix this? idk :sweat_smile:
```

---
## \#7 Posted by: briman05 Posted at: 2018-07-31T02:11:53.232Z Reads: 33

```
I would need to see a picture of it. You could probably just reheat the joint to clean it up and then resolder the wire to the board.
```

---
## \#8 Posted by: Dazeto Posted at: 2018-07-31T02:57:49.354Z Reads: 32

```
i need a better camera than my old iphone 6 :roll_eyes:  but i just took part of the heatwrap off and there are black spots there under the red wire ![image|375x500](upload://iNOtYMwC5dT19tX0qjbPUOLpKV2.jpg)
```

---
## \#9 Posted by: briman05 Posted at: 2018-07-31T03:29:45.166Z Reads: 29

```
It’s hard to tell but just reheat the solder and put the wire back in the solder bed
```

---
## \#10 Posted by: Dazeto Posted at: 2018-07-31T18:00:52.379Z Reads: 23

```
already ordered another vesc lol. but ill give i a try and if it works ill use it in a future board thats tiny and ez to carry.
will post after i do that, thank you very much for the help.
```

---
