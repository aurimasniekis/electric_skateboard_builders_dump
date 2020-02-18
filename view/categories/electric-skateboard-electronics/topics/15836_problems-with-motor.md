# Problems with motor

### Replies: 22 Views: 1152

## \#1 Posted by: Philippe1 Posted at: 2017-01-09T20:52:29.085Z Reads: 124

```
I have just put everything together and i tested it today. But my motor stutters and i cannot move at a normal speed. Does anybody have the same problem?
```

---
## \#2 Posted by: torqueboards Posted at: 2017-01-09T22:23:48.956Z Reads: 113

```
Could be loose motor connectors. Could be your not riding it properly. What's your setup/parts?
```

---
## \#3 Posted by: JohnnyMeduse Posted at: 2017-01-09T22:29:00.789Z Reads: 112

```
If you had picture of your connection amd more detail abouth tour setup, it will help us help you..., 🤔
```

---
## \#4 Posted by: Philippe1 Posted at: 2017-01-10T06:55:11.992Z Reads: 97

```
[hier is a video of my setup](https://www.youtube.com/watch?v=UgyuplrcZac&feature=youtu.be)
```

---
## \#5 Posted by: Hummie Posted at: 2017-01-10T08:06:53.620Z Reads: 92

```
if it's the vesc in current mode that's normal.  put it on the ground and ride it and it's likely fine.
```

---
## \#6 Posted by: OskarCastrone Posted at: 2017-01-10T12:16:38.458Z Reads: 80

```
It could also be mounting screws being too long. If so they will touch the stators when trying to spin the motor.
```

---
## \#7 Posted by: Philippe1 Posted at: 2017-01-10T16:01:12.946Z Reads: 73

```
does that make it stutter?
```

---
## \#8 Posted by: Philippe1 Posted at: 2017-01-10T16:18:16.209Z Reads: 73

```
It only stutters when i stand on it and move it
```

---
## \#9 Posted by: Hummie Posted at: 2017-01-10T16:26:24.835Z Reads: 75

```
Do u give it a little push?  How bout a video of what it's doing ?
```

---
## \#10 Posted by: JohnnyMeduse Posted at: 2017-01-10T22:33:43.093Z Reads: 62

```
Are you running foc ?
```

---
## \#11 Posted by: Philippe1 Posted at: 2017-01-10T22:40:44.957Z Reads: 60

```
nope. just BLDC
```

---
## \#12 Posted by: Hummie Posted at: 2017-01-10T22:52:34.679Z Reads: 59

```
maybe try the bldc test again and see if it passes.  if it passes I'm pretty sure the motor is fine.     Some people think they have a bad motor as on the bench it reacts strangely but under load, when riding, its fine.
```

---
## \#13 Posted by: JohnnyMeduse Posted at: 2017-01-10T23:07:26.364Z Reads: 56

```
Does it shutter only at the start or is it impossible to ride ? 

Also, can you post your setting in the bldc tool ?
```

---
## \#14 Posted by: mmaner Posted at: 2017-01-10T23:15:17.749Z Reads: 53

```
Its kind of out in left field, but have you checked the PPM setup?  Turn on display and make sure that the MAX, MID & MIN are set correctly.
```

---
## \#15 Posted by: Philippe1 Posted at: 2017-01-30T15:47:59.538Z Reads: 43

```
when i  try to detect paramaters it says that the detection failed. What do i do?
```

---
## \#16 Posted by: Philippe1 Posted at: 2017-01-30T15:50:32.421Z Reads: 42

```
<img src="/uploads/db1493/original/3X/a/5/a5e7f051fe42a350d352d9a72ba32cd52dd5c7cc.png" width="690" height="431"><img src="/uploads/db1493/original/3X/1/1/11ff439391b3d06e078ad745141d5501405d31f6.png" width="690" height="431"><img src="/uploads/db1493/original/3X/c/8/c8164e8bcab0baada2f0713f5ba5aa78405bb646.png" width="690" height="431"><img src="/uploads/db1493/original/3X/5/c/5cbb5fac2d0e21317c4a5ad1312785be2e51be1e.png" width="690" height="431">

here are some pictures of my settings in BLDC
```

---
## \#17 Posted by: Blasto Posted at: 2017-01-30T15:53:24.612Z Reads: 38

```
unplug your receiver when you do your motor detection
```

---
## \#18 Posted by: Philippe1 Posted at: 2017-01-30T16:12:00.762Z Reads: 38

```
[here](https://www.youtube.com/watch?v=-hVb-UtkaZY&feature=youtu.be) i did a little test ride howe ever it made a weird noise and went extremely slow.

[Here](https://www.youtube.com/watch?v=Ua6iF52VzLw&feature=youtu.be) is the setup and in this video i also tried running the motor on the ground.
```

---
## \#19 Posted by: Philippe1 Posted at: 2017-01-30T16:22:14.520Z Reads: 40

```
even without the receiver plugged in it still says failed
```

---
## \#20 Posted by: Hummie Posted at: 2017-01-30T22:00:54.505Z Reads: 37

```
probably shorted motor.  or maybe the phase wires are touching if your failing the test
```

---
## \#21 Posted by: Ackmaniac Posted at: 2017-01-30T23:51:27.435Z Reads: 32

```
Set the control mode in the PPM tab to disabled. 
Write the settings. 
Do the motor detection. 
When successfully then the apply button. 
Write the settings. 
Enable your control mode again in the ppm tab. 
Write the settings.
```

---
## \#22 Posted by: Philippe1 Posted at: 2017-01-31T16:17:57.968Z Reads: 27

```
Thank you but it didn't make a difference<img src="/uploads/db1493/original/3X/f/6/f61f1c79c1de3acb81cfa2b710012e08e5580901.png" width="690" height="431"><img src="/uploads/db1493/original/3X/0/2/02a031f2ed90cfc3799b3abf69d49b694c3325e1.png" width="690" height="431">
```

---
