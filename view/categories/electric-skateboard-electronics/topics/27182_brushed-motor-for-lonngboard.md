# Brushed Motor For Lonngboard

### Replies: 9 Views: 1230

## \#1 Posted by: bjm0017 Posted at: 2017-07-09T22:39:55.276Z Reads: 86

```
Would it be possible to make a longboard using two of these: https://www.vexrobotics.com/217-4347.html brushed motors. They have a power output of ~350 W per motor, They would be run with 70mm wheels and a 3.75:1 ratio per motor. 

I am not too concerned with efficiency and range at this point. Here is a full chart of its specs: http://motors.vex.com/vexpro-motors/775pro 

Has anyone tried to make a board with brushed motors? Any feedback would be great!
```

---
## \#2 Posted by: ShutterShock Posted at: 2017-07-09T22:51:39.418Z Reads: 85

```
Ah! I remember these motors!  My robotics team and I were amazed at the performance increase over the standard 775 motors.  Vex products are great, however I doubt that this would be even possible for an esk8 application.

For one, the shaft is much too small to mount one of the pulleys that people usually use for boards on, and I think it is quite underpowered.  When we used these motors for our robot, we had some pretty large planetary gearboxes on them, and while you could gear it down for an esk8, I doubt it would be enough speed or strength to effectively move a person.  Also, the esk8 motors are all way more powerful than this, clocking in between 1000 and 3000W of power.
```

---
## \#3 Posted by: Michaelinvegas Posted at: 2017-07-09T23:48:31.579Z Reads: 68

```
Hey @MoeStooge what U think?
```

---
## \#4 Posted by: bjm0017 Posted at: 2017-07-10T00:11:07.237Z Reads: 58

```
@ShutterShock, I wasn't sure if 700W was enough for a basic application with reasonable speed, I was just planning to use a Spark for speed control. 

Do you have any experience with buying parts in Canada? Hobbyking is quite challenging in Canada for many reasons. This was the main reason for using FRC parts.
```

---
## \#5 Posted by: NickTheDude Posted at: 2017-07-10T00:15:13.836Z Reads: 56

```
I'm in Canada as well so I feel your pain. I get a lot of my stuff from  cause they have free worldwide shipping over 300 bucks, plus their well established and have good parts.

As for hobbyking I haven't had too much trouble. I believe you need to order from their US warehouse for batteries though.
```

---
## \#6 Posted by: ShutterShock Posted at: 2017-07-10T00:15:27.580Z Reads: 54

```
Honestly I am not super sure.  It may be enough to keep you moving, but I would imagine that you would have to push start it.  It sounds like a cool project to me, maybe with the more extreme gear down, you would be able to do it.

Unfortunately not, I live in California, so no problems with HK shipping for me.  I never even thought to use FRC parts.  One of my friends suggested using a CIM motor but those are super heavy haha.

If you are able to calculate the kv of those motors, you may be able to use the esk8 calculator to figure out some more detailed potential.  ¯\_(ツ)_/¯

[Esk8 Calc](http://calc.esk8.it/)
```

---
## \#7 Posted by: bjm0017 Posted at: 2017-07-10T00:30:31.873Z Reads: 50

```
[quote="ShutterShock, post:6, topic:27182"]
One of my friends suggested using a CIM motor but those are super heavy haha.
[/quote]
I got the same thing from one of our guys. 

[quote="ShutterShock, post:6, topic:27182"]
If you are able to calculate the kv of those motors, you may be able to use the esk8 calculator to figure out some more detailed potential.  ¯_(ツ)_/¯
[/quote]
I was just using the specs from vex DC motor testing. Here are the numbers that I am using: http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":3,"motor-kv":843,"system-efficiency":45,"motor-pulley-teeth":12,"wheel-pulley-teeth":45,"wheel-size":70}|
```

---
## \#8 Posted by: MoeStooge Posted at: 2017-07-10T00:46:51.316Z Reads: 44

```
700w not enough pwr.  You would have to run a reduction Jack shaft and would go 8 mph to keep from melting it down.
```

---
## \#9 Posted by: ShutterShock Posted at: 2017-07-10T01:35:26.279Z Reads: 33

```
Yeah that is what I was thinking would happen haha, if it doesn't melt before getting to that speed.  

They're great for robotics, probably not for esk8.  The CIM is a possibility but the watt rating on it is only 300
```

---
