# Possible Benchwheel Motor Mount Modding

### Replies: 10 Views: 2840

## \#1 Posted by: claudiofiore88 Posted at: 2016-01-16T23:24:15.173Z Reads: 119

```
I've been thinking about upgrading the 50mm motors on my benchwheel e-board to 63mm motors. The only problem is the motor mounts wrap around the  motor only allowing 50mm motors. Would it be feasible to cut around it to fit larger motors or would it compromise the structural integrity of the mount? Would the mounting holes be the same?

<img src="/uploads/db1493/original/2X/f/f1c64f5d28ea636a6f899680cca6dcea4bc1250c.jpg" width="375" height="500">
```

---
## \#2 Posted by: torqueboards Posted at: 2016-01-17T07:09:50.932Z Reads: 107

```
The mount should be fairly fine but looks like it kinda defeats the purpose of that build. I guess, you can always replace that motor mount but I also think those trucks aren't your typical Caliber/Paris.

Some of the 63mm motors have the same bolt on pattern for 50mm and 63mm so it would fit. You would just need the room for the motor.
```

---
## \#3 Posted by: Justin Posted at: 2016-01-17T12:24:04.107Z Reads: 105

```
The mount will probably be a lot weaker, because if you grind off the ridge that wraps around the motor the only thing left is a thin/flat peace of metal which will probably bend fairly quickly. I guess they probably didn't use very high quality metal either, being this is a Chinese budget board.

Btw here you can see the mount without motors:
<img src='/uploads/db1493/original/2X/b/bf0349105734499d57b4d0a5216297d879734188.jpg'>
```

---
## \#4 Posted by: psychotiller Posted at: 2016-01-17T17:05:50.903Z Reads: 99

```
If that mount is cast aluminum, which it probably is, I definitely would not recommend cutting into it.
```

---
## \#5 Posted by: claudiofiore88 Posted at: 2016-01-17T20:32:35.810Z Reads: 97

```
Would it be worth it to "upgrade" the pair of motors to a different pair of 50mm motors? The motors are 290 kv, I believe.
```

---
## \#6 Posted by: torqueboards Posted at: 2016-01-23T03:22:00.062Z Reads: 88

```
It's not worth upgrading to 50mm if the motors are already 290KV. Your issue is the low voltage that the benchwheel offers. IMO However, I doubt those motors would be 290KV unless you tested it.

I'd just go with a new build. 240-260KV even on a single motor on 10S/12S should take a 250lb person up a 15-20% incline.
```

---
## \#7 Posted by: claudiofiore88 Posted at: 2016-01-23T16:04:24.934Z Reads: 87

```
I don't have the equipment to test the kv of the motors. The top speed is supposed to be 18mph which seems slow for a kv that high even on 6s. Maybe the gear ratio is high. I'll just settle with this for now since there aren't many hills around me anyway.
```

---
## \#8 Posted by: lowGuido Posted at: 2016-01-23T20:44:49.712Z Reads: 84

```
or the top speed is electronically limited. in which case it could be a 290kv motor but not spinning to its full RPM.

I think a benchwheel board upgraded to VESC would make a good starters board. 
the VESC programming would remove any limits,
then if it is still not fast enough you could upgrade the battery voltage.
I'm assuming the motors should hold. 

someone with a benchweel setup could probably provide more info on what they have done.
```

---
## \#9 Posted by: claudiofiore88 Posted at: 2016-01-24T02:24:47.134Z Reads: 83

```
I'll probably end up doing that eventually. Hopefully I'll be able to use the boards existing bms.

<img src="/uploads/db1493/original/2X/e/e357b694f8de2901f5f36fc18d89b205deee5da9.jpg" width="666" height="500">

I'm pretty sure it's the bottom pcb since the balance wires go directly do it.
```

---
## \#10 Posted by: lowGuido Posted at: 2016-01-24T02:38:03.879Z Reads: 79

```
hard to tell with all that white goop on there.
```

---
