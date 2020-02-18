# \[SOLVED\] Motor Slipping/Stalling Under Load - No Takeoff Torque

### Replies: 20 Views: 2195

## \#1 Posted by: rakejagland Posted at: 2017-07-16T21:00:40.339Z Reads: 130

```
Hey, this is my first build and I am fairly new to the community after many month of research. My current setup is:
-(2x) 5000mah 4s1p lipo batteries
-TORQUEBARDS () VESC hd version 4.12, came with firmware 2.18, changed to 2.15 with matching BLDC Tool
-TORQUEBOARDS 3655 190kv motor
-2.4ghz receiver and torqueboards controller

I have tried to take all the appropriate steps to configuring the vesc and calibrating everything, but I still have major problems. My motor spins fine on the tabletop, but when it has any load on it, like my hand simply resting on the wheel, the motor will slip. The gears and belt are fine, but when power is sent to the motor, it will whine like it is trying to spin and the shaft and housing will strip. Any advise is appreciated.
PS: I do not plan on using the plastic 3D printed pieces on the final version. They are just placeholders for testing and calibration. Machined aluminum pieces will be made soon!<img src="/uploads/db1493/original/3X/0/9/0990e1d75a4f1d2692c98e5b3700cee55fa8fca7.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/0/e/0e55e2767e0ecaada12a05bad5e8130c80178397.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/1/2/126d3afcef02d98333ecc4ff7d7f85bd6366fde2.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/a/f/aff3c3030ea641fbbde3299598bb69cb8ff47b3b.png" width="690" height="388"><img src="/uploads/db1493/original/3X/9/9/9976b05ddac9100d235eda04d65fbd9e0e9bf4d9.png" width="690" height="388"><img src="/uploads/db1493/original/3X/7/c/7cbeda51a5b99e826019686bab2c00018bad225a.png" width="690" height="388">
```

---
## \#2 Posted by: willpark16 Posted at: 2017-07-16T21:11:18.422Z Reads: 120

```
Ur belt is way too long, it could be those 3D pulleys not having deep enough grooves, what's ur gearing ratio
```

---
## \#3 Posted by: Martinsp Posted at: 2017-07-16T21:18:34.378Z Reads: 113

```
Do you mean that your motor is not spinning at all (stalled but trying) or that your small motor pulley slips?
```

---
## \#4 Posted by: psychotiller Posted at: 2017-07-16T21:23:38.584Z Reads: 110

```
Will you check the 2 set screws in the back of your motor that holds the motor shaft in place? Then, will you tighten your belt?
```

---
## \#5 Posted by: Martinsp Posted at: 2017-07-16T21:30:37.158Z Reads: 108

```
I think that he wont be able to tighten the belt (except for some idler pulley) because he is at the end of the slot on his mount. Shorter belt or bigger pulley would solve this.
```

---
## \#6 Posted by: rakejagland Posted at: 2017-07-16T22:09:40.036Z Reads: 106

```
@willpark16 Yes, my motor belt is too long, but the teeth are not stripping. The motor is stalling. I have stronger gears and aluminum motor mount that  will allow for more room to tighten the pulley coming soon. My ratio is 16 tooth: 36 tooth (2.25:1).

@Martinsp My motor is not  spinning at all when there is any resistance force (like my hand resting on the wheel, let alone the force of me on the board). It stalls and stutters until I let off the throttle. There is no pulley/belt slipping.

@psychotiller I don't see the set screws in the back of the motor. Where are they exactly? This is a brand new motor fresh out of the box and has only been tested on my tabletop. Also my motor shaft seems sturdy and well set (not moving in and out of the motor).
 
Are you saying that my motor stalling problem is coming from the mechanics of my drive train setup? Because it seems like more of an electrical or VESC configuration issue. The motor slips and stalls even without translating any force past the motor shaft.

Thanks
```

---
## \#7 Posted by: Martinsp Posted at: 2017-07-16T22:11:11.796Z Reads: 96

```
Ahh ok I get it now. And what happens when you try to accelerate but not from full stop. Give it one push and try it. The point is to find out if you have a problem of not enough power or only not enough power to get you going from full stop.
```

---
## \#8 Posted by: rakejagland Posted at: 2017-07-16T22:38:39.703Z Reads: 93

```
@Martinsp Great, The problem only seems to occur when starting from stop. After crudely tightening everything as much as I can, I have isolated the problem as being not enough power to start from stop. My crude 3D printed makeshift parts give out after that, but the motor has no trouble electrically. (I am fixing the mechanical stuff as soon as I can get to the shop to machine some aluminum pieces) How should I go about fixing the problem of not enough torque to get me going from stop?

Thanks
```

---
## \#9 Posted by: psychotiller Posted at: 2017-07-16T22:41:03.053Z Reads: 89

```
I'm saying either your motor pulley doesn't have a keyway in it or the set screws aren't tight enough.

Or the two set screws (look at the back of your motor-If you were a set screw, how would you tighten against the shaft?) holding your motor shaft in.
```

---
## \#10 Posted by: Martinsp Posted at: 2017-07-16T22:47:46.408Z Reads: 87

```
What could help you is that you go to motor config tab on your VESC and in the advanced sub-tab or whatever and increase the startup boost. Try just a little bit. It is not advised to set it higher than 0.1 so start at 0.05 and slowly go up and see if you will find a sweet spot. This applies to BLDC only though.
```

---
## \#11 Posted by: Martinsp Posted at: 2017-07-16T22:49:24.681Z Reads: 81

```
@psychotiller  

[quote="rakejagland, post:6, topic:27804"]
My motor is not  spinning at all when there is any resistance force (like my hand resting on the wheel, let alone the force of me on the board). It stalls and stutters until I let off the throttle. There is no pulley/belt slipping.
[/quote]

I think he is not having a problem with motor can spinning free without the shaft.
```

---
## \#12 Posted by: psychotiller Posted at: 2017-07-16T22:52:14.539Z Reads: 75

```
Oh really? My bad...I thought I read this from his original post:
[quote="rakejagland, post:1, topic:27804"]
My motor spins fine on the tabletop, but when it has any load on it, like my hand simply resting on the wheel, the motor will slip.
[/quote]
```

---
## \#13 Posted by: Martinsp Posted at: 2017-07-16T22:55:49.526Z Reads: 70

```
Well the same is in my quote :D The first half is about his motor spinning without shaft and the second is about stuttering. :D I think that it is just a misunderstanding and his motor is stuttering because he mentioned that when he is accelerating NOT from a dead stop it works fine. I might be wrong tho :D
```

---
## \#14 Posted by: psychotiller Posted at: 2017-07-16T23:03:37.598Z Reads: 70

```
The stuttering is called cogging. If the OP isn't running a sensored set up it's going to happen. Its a non issue and doesn't hurt anything. Just push off, or use a sensored motor and sensor compatible esc or vesc.

The slipping if there actually is any would be the issue that needs fixed. I outlined how to fix slipping. If his belt is "skipping" Tighten the belt.
```

---
## \#15 Posted by: rakejagland Posted at: 2017-07-16T23:03:42.299Z Reads: 68

```
@psychotiller Yeah I do have some mechanical probs but I know I can fix those with some time. Thanks so much for the input though! The set screws were actually a little loose.

@Martinsp YES! That helped a ton! Now I do have mechanical limitations in my drivetrain, but like I said, I have better parts on the way.

Thanks again for the help! I'll  be back if I have more troubles I can't find answers to after I fix the makeshift drive mechanics. Should I change the topic to *SOLVED*?
```

---
## \#16 Posted by: Martinsp Posted at: 2017-07-16T23:05:44.794Z Reads: 64

```
No worries, I am happy i could help. :)

I guess you should, if you know how. I never figured out how to change the name of my own topics :D :D
```

---
## \#17 Posted by: Martinsp Posted at: 2017-07-16T23:08:46.150Z Reads: 65

```
@rakejagland I just noticed, you have a sensored motor. Why dont you use sensors? I tried them and now I would never go back. The smoothness is awesome :D
```

---
## \#18 Posted by: jkrider Posted at: 2017-07-16T23:13:27.928Z Reads: 65

```
Where do you connect the sensor wires on the vesc?
```

---
## \#19 Posted by: rakejagland Posted at: 2017-07-17T00:09:37.751Z Reads: 63

```
@Martinsp and @jkrider Honestly, I haven't looked into that much at all. I don't know where to plug it into the VESC. Will it require more calibration using the BLDC Tool and what not? I'm sure I could find another thread or tutorial on this, but I haven't checked. Where would it plug into the VESC?
```

---
## \#20 Posted by: Jinra Posted at: 2017-07-17T00:10:56.812Z Reads: 64

```
See here:
http://www.electric-skateboard.builders/t/honey-driver-honey-velocity-v3-deck-caliber-iis-83mm-evolve-gt-wheels-dual-om5065-200kv-space-cell-pro4-diy-pulleys-enertion-pulley-bones-super-reds-enertion-mounts-winning-remote-chaka-vescs-build-complete/5760/36?u=jinra

The missing wire is the temp wire which I didn't have on that motor.
```

---
