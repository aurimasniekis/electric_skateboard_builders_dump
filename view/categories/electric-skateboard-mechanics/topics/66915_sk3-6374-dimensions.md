# SK3 &ldquo;6374&rdquo; dimensions

### Replies: 22 Views: 562

## \#1 Posted by: xilw3r Posted at: 2018-09-03T12:34:51.420Z Reads: 148

```
Hello good people,

I wanted to ask anyone who has bought the SK3 6374 motors in the long forgotten past, were they always only 59mm in diameter?

I know, it is written in the dimension drawing on HK, but I still feel rather mislead. Why on earth call it a "63" motor then.

I bought an Sk3 to replace my rather shitty Emax motor, which was actually 63mm in diameter (but the magnet to stator gap is rather big, magnets are not curved and are not glued in straight, so i hope to get more power out of the superior build quality of the sk3)
```

---
## \#2 Posted by: anorak234 Posted at: 2018-09-03T14:08:22.760Z Reads: 131

```
They have always been off, Hobbyking is weird that way. Despite that though, the sk3s that I’ve had and used pretty intensely for various applications have each performed well for 3 years minimum with no maintenance - I can’t complain.
```

---
## \#3 Posted by: dareno Posted at: 2018-09-04T00:23:15.244Z Reads: 112

```
Hobby king shenanigans.  The sk8 is 63 but it’s nearly 80 long.  Makes it a bit of a squeeze on 218 even.  
But good solid powerful lump it is.
```

---
## \#4 Posted by: kalebludlow Posted at: 2018-09-04T00:27:35.195Z Reads: 109

```
Had to go with 6364 for this reason :frowning:
```

---
## \#5 Posted by: dareno Posted at: 2018-09-04T18:44:28.074Z Reads: 90

```
Good solid lump it was till yesterday when one decided to shit itself for no reason whatsoever.  And get this I had just red loctited every grub screw on the thing so now taking it apart is going to be very problematic.  @kalebludlow they do fit the 218's just with about 2mm clearance between everything using the tb mounts.
```

---
## \#6 Posted by: xilw3r Posted at: 2018-09-04T19:06:38.567Z Reads: 79

```
bummer, what happened with the motor?
```

---
## \#7 Posted by: dareno Posted at: 2018-09-04T19:12:32.659Z Reads: 76

```
Not sure I was just relocating the electronics to fit a new battery and noticed one motor wasn't spinning as freely as the other.  It won't detect at all and the vesc gives 3 rapid red lights then a pause the 3 over and over.  When I unplugged the phase wires the vesc is fine.  Tried the vesc on the other motor and its cool so I can only assume the motor has a short somewhere and I'm thinking in the hall sensors.  Got to strip it down and see.  The joys of esk8........
```

---
## \#8 Posted by: xilw3r Posted at: 2018-09-04T19:31:51.231Z Reads: 68

```
I think if it was the hall sensor you most likely would have fried your vesc. Do the multimeter test, see if the motor self shorted magically. Same test works for the sensors too, dont really need to strip anything yet I would say
```

---
## \#9 Posted by: dareno Posted at: 2018-09-04T19:39:31.280Z Reads: 68

```
it threw a hall sensor error at me a while ago so I disconnected and went sensorless in the vesc tool with no problems for the last 3 months.  I'm wondering whether one of the connections has come off and causing the restriction.  No smoke or I would'nt have run detection trust me been there done that lol   No smells nothing just won't spin under power.  Have you had that light array happen on a vesc before?
```

---
## \#10 Posted by: xilw3r Posted at: 2018-09-05T08:52:20.767Z Reads: 56

```
Never had any such issues. I havent even tried sensored modes yet eiher, since I only have one motor avilable at the moment. Need to remake my drive to accept the sk3 without shaft length issues. bah

Smoke is not necessary I think, if the enamel peeled off somewhere and the phases are touching it could cause your problem too I believe. Go get that multimeter test done
```

---
## \#11 Posted by: Nowind Posted at: 2018-09-05T08:56:06.192Z Reads: 53

```
Sk3 is around 5984 
One of the best Motors IMO
cheap and relieable
:+1:
```

---
## \#12 Posted by: telnoi Posted at: 2018-09-05T10:39:08.316Z Reads: 48

```
It's probably the motor with the least reported failure rate, at least here.
3k+ km, also zero maintenance. Riding through the shittiest terrain my MTB will allow.

I would like to go bigger for increased braking power, but it looks like it is rather difficult to find a reliable replacement. 

The SK3 delivers a decent amount of power. Should be a good replacement for that EMAX.
```

---
## \#13 Posted by: dareno Posted at: 2018-09-05T18:21:17.773Z Reads: 48

```
Turns out my sk8 threw a bearing which completely disintegrated and ended up breaking the pcb for the hall sensors.  Which in turn has caused an error on the vesc.  
https://www.electric-skateboard.builders/t/new-aps-motor-broken-while-vesc-setup/66829/53
you can see the pics on here.  Not pretty.  
@Nowind what size would be good for 12s?  the 168kv 6374 or the 6368 190?  The sk8 is 190
```

---
## \#14 Posted by: xilw3r Posted at: 2018-09-05T18:28:31.560Z Reads: 44

```
Personally I say go for the highest kv you can get away with, just because the phase wires are fatter and can push more current. And you are asking between a larger and a smaller motor? How is that even a choice :) ?

Bummer about the bearing.. Looks like it didnt destroy the magnets though? If so, then I still say you are lucky
```

---
## \#15 Posted by: dareno Posted at: 2018-09-05T18:32:34.624Z Reads: 40

```
[quote="xilw3r, post:14, topic:66915"]
And you are asking between a larger and a smaller motor? How is that even a choice :slight_smile: ?
[/quote]

:joy: the point was that hk pull their dimensions out of their arse most of the time so all i wanted to know if I will notice the difference between 168 and 190 but yeah I get it go big or go home lol
```

---
## \#16 Posted by: Nowind Posted at: 2018-09-05T18:32:52.867Z Reads: 39

```
[quote="dareno, post:13, topic:66915"]
@Nowind what size would be good for 12s? the 168kv 6374 or the 6368 190? The sk8 is 190
[/quote]


Wheelsize ?
Gearing ?
Desired Topspeed?
```

---
## \#17 Posted by: dareno Posted at: 2018-09-05T18:38:46.695Z Reads: 39

```
97mm
16/36
All I want is to get the closest thing to what i have.  Will the slightly smaller can make much difference to performance or indeed the lower kv drop the top end too much?  I'm heavy so more torque is great but not at the cost of a considerable drop in speed.
```

---
## \#18 Posted by: xilw3r Posted at: 2018-09-05T18:39:42.664Z Reads: 37

```
Yea, all that length delta is stator difference, you will deffinitely notice, no matter from where HK pull out the dimensions.
```

---
## \#19 Posted by: Nowind Posted at: 2018-09-05T18:51:09.987Z Reads: 39

```
I would go with the 168kv
But i´m not that much into Street builds more MTB
```

---
## \#20 Posted by: dareno Posted at: 2018-09-05T18:59:23.001Z Reads: 40

```
I know man been watching your vids for a while now.  Awesome stuff! If I still lived in the uk I would be one of your customers.
 The sk8 motor is actually fine now I've replaced the bearing, I just don't trust them anymore.  I'll grab a set of sk3's can't hurt hey?
```

---
## \#21 Posted by: xilw3r Posted at: 2018-09-05T21:34:26.980Z Reads: 33

```
I thnk the bearings are the same in sk3/8
```

---
## \#22 Posted by: dareno Posted at: 2018-09-05T21:45:01.094Z Reads: 34

```
Maybe I was just unlucky and yeah I'm pretty sure the motors would turn out to be the same underneath the can.  Think I'll just open them both up and upgrade all the bearings just to be safe.  One of the regulars here sent me a good link for quality bearings and I want to remove the sensor array in the good motor anyway as they are definitely crap and have cost me one vesc already.  First sensored motors i've used and yeah no.  Tbh the guts actually look a lot better than the maytech equivalent that threw a magnet on me.  Not much luck with motors lately :roll_eyes:
Thanks for the help.
@xilw3r
@Nowind
```

---
