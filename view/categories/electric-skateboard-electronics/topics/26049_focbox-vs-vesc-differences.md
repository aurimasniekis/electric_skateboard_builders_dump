# Focbox vs VESC differences

### Replies: 12 Views: 11212

## \#1 Posted by: NewbieBoardBuilder Posted at: 2017-06-24T05:41:29.546Z Reads: 1045

```
http://www.enertionboards.com/electric-skateboard-parts/vesc-x-programmable-brushless-motor-controller/
Or
diy-electric-skateboard-kits-parts/vesc-the-best-electric-skateboard-esc/
What are the differences and do they both come preprogrammed with standard settings?
```

---
## \#2 Posted by: rpn314 Posted at: 2017-06-24T06:12:26.802Z Reads: 1022

```
First is explained in depth here:
http://www.electric-skateboard.builders/t/new-improved-focbox-official-thread/11102

Second is just a VESC 4.12 with slightly upgraded components

Programming wise, they're essentially identical and you should always program your own settings and not rely on "default" settings on a vesc
```

---
## \#3 Posted by: NewbieBoardBuilder Posted at: 2017-06-24T06:13:46.546Z Reads: 971

```
What are the reviews like?
```

---
## \#4 Posted by: rpn314 Posted at: 2017-06-24T06:15:04.489Z Reads: 944

```
They're both quite good and both are used. Search around for anything much more specific. I don't have personal experience with either.
If price isn't an issue, also consider those by ollin and axle
```

---
## \#5 Posted by: NewbieBoardBuilder Posted at: 2017-06-24T06:18:57.455Z Reads: 932

```
Thanks. What are battery s and c ratings?
```

---
## \#6 Posted by: rpn314 Posted at: 2017-06-24T06:24:17.682Z Reads: 921

```
http://www.electric-skateboard.builders/t/new-user-looking-for-battery-read-this-complete-walkthrough-of-batteries/26010?u=rpn314
```

---
## \#7 Posted by: trampa Posted at: 2017-06-24T06:36:45.013Z Reads: 892

```
They are both speed controllers for motors, based on Benjamin Vedders design (VESC 4.12). They both run the Vedder Software (BLDC-Tool). Very soon the new Software VESC-Tool will be released, which will be supporting the old 4.xx hardware.
Together with the new software, hardware 6.4 will be released into the public domain.
VESC Tool and VESC SIX are in BETA stage, but close to the release.

You will need to set up your system, using Benjamin Vedder's Software. It's quite simple with VESC-Tool, which is available soon. Wizards will guide you.

The difference between the two controllers you showed is : Focbox uses direct Fets and a different PCB layout, based on an early VESC 5 design sketch from Benjamin Vedder. The second model you picked is pretty much the original design of the VESC 4.12,  featuring conventional, non coolable FETs. Direct FETs can handle more AMPs.

There are huge differences in built qualities available! Poor quality Hardware is likely to fail sooner than later. Get yourself informed is my advice. There are roughly 25-30 different manufacturers. 
This forum is full of information about the VESC Open Source software and hardware.

Frank
```

---
## \#8 Posted by: willpark16 Posted at: 2017-06-24T06:38:49.303Z Reads: 833

```
I'll simplify it the foc box is simple and efficient with a slight upgrade and well worth the money I've had one for months with 0 issuers, the non upgraded vescs aren't as good and work but I encountered issues with diyelectricskateboards
```

---
## \#9 Posted by: longjohn Posted at: 2017-06-24T08:05:21.382Z Reads: 788

```
foc man, hardware 6.4 and new control code has me hard as granite :blush: :wink: :wine_glass:
```

---
## \#10 Posted by: Berlad180 Posted at: 2018-04-04T14:06:05.172Z Reads: 463

```
A great replay!
Could you please shed some more light about the difference of the FOC function ..What does it mean to run a vesc on FOC mode ? on what mode does it usually run ? could you please just explain the basic modes that are available, and what do they mean?
```

---
## \#12 Posted by: GXwagon Posted at: 2018-05-15T00:45:37.378Z Reads: 392

```
Ill seconed Berlands question about FOC
```

---
## \#13 Posted by: professor_shartsis Posted at: 2018-05-15T00:52:39.173Z Reads: 378

```
with BLDC, the current plot is “trapezoidal” and with FOC the the current plot is “sinusoidal”...

source: http://www.galilmc.com/news/drives-motion-controllers/trapezoidal-vs-sinusoidal-brushless-servo-amplifiers

_“Trapezoidal vs. Sinusoidal Commutation_

_Trapezoidal commutation is the most cost effective way of controlling a brushless servo motor.  It is perfect for higher speed applications and applications where the motor and mechanics will eliminate the torque ripple that occurs during switching current from one phase to the next.  Hall sensors are required for Trapezoidal commutation._

_Sinusoidal commutation is great for lower speed, direct drive or linear motor applications where the torque ripple of the motor phases needs to be minimized.  Since the current to the motor phases are weighted as sine waves, the torque going through the motor is smooth and has minimal ripple. It also allows the mechanics to be simplified because Hall sensors can be eliminated.”_

http://nptel.ac.in/courses/108103009/module7/lec22/images/1.png

http://pubs.sciepub.com/ajeee/4/6/3/bigimage/fig2.png

http://www.orientalmotor.com/images/stepper-motors/5-phase-stepper-motors-rkii-low-vibration.jpg
```

---
