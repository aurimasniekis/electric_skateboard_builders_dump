# Motor stutters, need help

### Replies: 18 Views: 269

## \#1 Posted by: Jake2k17 Posted at: 2018-08-24T00:32:39.878Z Reads: 95

```
So I have been riding this board for the last couple of months with no problems. The board consists of 
Turnigy Sk3 6364 190kv motor
TB VESC 4.12
2x 5s 5000 mAh lipos (in series)

About 2 weeks ago though, I installed a 10s charge only bms with the help of @Namasaki, and since then when I try to ride the motor stutters. At first it would only stutter when I was at cruising speeds, about 18-20 mph, but then it began to stutter around 10 mph, then 5, and now it won't spin at all, only stutters. I hooked it up to bldc tool, and completely reprogrammed it, but it still stutters, even during the motor detentions, except for sometimes when it would spin, but way faster than it used to when I would change some settings on the VESC. The even stranger thing now is that I have the board wheels up on the table, and when I use the remote and accelerate, it only stutters with low acceleration. Pictures below

![image|690x388](upload://rAmZWTbiSh4TLJBgcICPI8hDCKp.jpg)https://www.electric-skateboard.builders/uploads/db1493/original/3X/4/0/400e1bda65aa514f1ae912ca6b026a11ed340301.png

![image|690x388](upload://9E4zfsfGwLbv5HKI3jodtmKY5t2.jpg)https://www.electric-skateboard.builders/uploads/db1493/original/3X/3/a/3a291004f6ce0e14e901a6a0b4add32fb009e2b0.png
```

---
## \#2 Posted by: Namasaki Posted at: 2018-08-24T00:43:13.355Z Reads: 77

```
Sounds like you might have a connection issue on your motor phase wires.
At first it was intermittent and now its fully disconnected.
Possibly caused by vibration.
Inspect your motor connections. See if the bullet connectors will pull loose from the wires also look for cold solder joints.

I don't see how a charge only bms could have any affect on the motors but also check all your battery connections for cold solder joints
```

---
## \#3 Posted by: mmaner Posted at: 2018-08-24T01:10:07.687Z Reads: 69

```
This ⬆️ &nbsp;
```

---
## \#4 Posted by: Jake2k17 Posted at: 2018-08-24T01:16:58.510Z Reads: 71

```
Thanks guys! I looked under the heatshrink and all of my connectors were good, however the TB Vesc xt90 has shaken loose. @Namasaki, that’s twice you’ve saved my ass, hopefully the last time! Thanks so much
```

---
## \#5 Posted by: b264 Posted at: 2018-08-24T01:23:21.940Z Reads: 68

```
[quote="Jake2k17, post:4, topic:65900"]
xt90 has shaken loose
[/quote]

Get the [smallest size cable ties](https://smile.amazon.com/TR-Industrial-TR88301-Multi-Purpose-Cable/dp/B01018DB2E/ref=sr_1_8) and hook 2 of them end-to-end and put them around the connector, between the wires on each side, so it CANNOT vibrate loose.  Been there before LoLzz
```

---
## \#6 Posted by: Namasaki Posted at: 2018-08-24T01:31:43.603Z Reads: 63

```
I wouldn't have thought that an xt90 would shake loose.
Cable tie is a good idea @b264
```

---
## \#7 Posted by: b264 Posted at: 2018-08-24T02:45:26.538Z Reads: 57

```
Yeah, that way it's A) removable and B) if it cuts into the wire insulation, it won't short onto anything around it because it's on the inside surface of the wire and the tie is nylon
```

---
## \#8 Posted by: Jake2k17 Posted at: 2018-09-14T00:00:32.802Z Reads: 40

```
@Namasaki
@b264  

Sorry to summon you guys, but I resoldeded that connection, and everything worked fine for two weeks, and now the motor makes a clicking sound once and then doesn’t respond at all when I move the throttle. When I plug it into bldc tool, there are not faults, but the motor spins faster than usual when doing motor detection and it keeps on saying bad detection result received. I really need some help
```

---
## \#9 Posted by: Namasaki Posted at: 2018-09-14T00:06:57.601Z Reads: 39

```
Look for another loose connection as before. It could be the same connection or a different one.
Also check battery voltage.
```

---
## \#10 Posted by: Jake2k17 Posted at: 2018-09-14T00:12:31.681Z Reads: 38

```
I checked all connections, and the voltage is 40v (10s). Do you think something is broken inside the motor?
```

---
## \#11 Posted by: Namasaki Posted at: 2018-09-14T00:13:52.871Z Reads: 38

```
[quote="Jake2k17, post:10, topic:65900"]
Do you think something is broken inside the motor?
[/quote]


Possible.
One of the phase wires could be broken.
Although, I don't think it would spin in motor detection if a phase wire is disconnected.
but it could be an intermittent break.
```

---
## \#12 Posted by: Jake2k17 Posted at: 2018-09-14T00:33:39.019Z Reads: 36

```
I’m using a turnigy motor, and it has this really stiff copper wire that breaks a lot. I have checked if up and down, but maybe it snapped on the inside. Can I take apart the motor and solder on silicon wire?
```

---
## \#13 Posted by: Namasaki Posted at: 2018-09-14T00:51:48.237Z Reads: 36

```
Is it an SK3 motor?
```

---
## \#14 Posted by: Jake2k17 Posted at: 2018-09-14T00:53:55.940Z Reads: 35

```
Yeah it’s a 6364 sk3
```

---
## \#15 Posted by: Namasaki Posted at: 2018-09-14T01:01:29.267Z Reads: 32

```
My recommendation is to upgrade to a quality esk8 motor.
SK3's are not the best and you're better off with something that won't keep giving you problems.
```

---
## \#16 Posted by: Jake2k17 Posted at: 2018-09-14T01:12:17.141Z Reads: 28

```
[quote="Namasaki, post:15, topic:65900"]
My recommendation is to upgrade to a quality esk8 motor.
[/quote]

I’m working on my second build, a boosted clone, but I just want something to ride right now. I have a spare 5065 260kv that I was going to limit the ermp on, but it doesn’t fit my 63mm TB mount. Is it possible though to replace those wires?
```

---
## \#17 Posted by: Namasaki Posted at: 2018-09-14T01:15:05.389Z Reads: 27

```
the phase wires are part of the windings and they are insulated with a clear coating.
It would be difficult to solder them with the insulation and without the insulation the wires can short out.
It may be possible to fix it but not easy.
You also should consider the safety factor.
You don't want your motor locking up or braking suddenly while your flying down the road.
Having dependable components is very important.
```

---
## \#18 Posted by: Jake2k17 Posted at: 2018-09-14T01:59:46.744Z Reads: 23

```
Ok thanks so much. I think I will just order one of the 6355s early and throw that on rhere
```

---
