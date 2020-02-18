# VESC - FAULT_CODE_DRV. &ndash;&gt;discovered later on: JUST FROM STANDING STILL START &lt;&mdash;

### Replies: 22 Views: 1577

## \#1 Posted by: piepolitb Posted at: 2018-05-18T20:43:36.470Z Reads: 136

```
Hello guys, first post here and REALLY newbie here.

I checked similar discussion, found some, but don't really get the solutions (if any). So please address me to the correct post if needed.

I've got 

- the following 190kv motor  in single configuration
products/electric-skateboard-motor-6355-190kv

- and the VESC
products/torque-esc-bldc-electronic-speed-controller

everything run by 12s battery, in BLDC Sensorless mode.


The system worked fine on bench test and on street test. 
I stopped after few kms to measure the battery voltage and when I tried to restart, I got nothing, just red led blinking 3 times when I push the throttle up.

I walked home and connected the VESC to VESC tool:

- in real time data I get "Fault: DRV"

- when I run the motor detection I get "Bad Detection Results Receiver"


I tried rebooting the VESC, reflashing the firmware and all the basics I read in similar post.

Any suggestions/ideas?
thanks 
Giuseppe
```

---
## \#2 Posted by: Yecrtz Posted at: 2018-05-18T20:47:00.913Z Reads: 122

```
Can you post some screeshots of your settings in the vesc tool? Then it's easier to possibly spot the cause.
```

---
## \#3 Posted by: piepolitb Posted at: 2018-05-18T20:48:29.925Z Reads: 120

```
Hi @Yecrtz, what settings do you need to look at?
```

---
## \#4 Posted by: piepolitb Posted at: 2018-05-18T21:01:17.126Z Reads: 120

```
meanwhile here are some

![image|690x187](upload://kej05VDNBjQ0TeVPhKSGO8abLKM.png)

![image|690x119](upload://Fd2udk4Ny4OGI6OEXANz8McoVa.png)



also strange thing is that when I use the arrow key to spin the motor, it sometimes works with left/right keys while it never works (FAULT: DRV) with up and down keys
```

---
## \#5 Posted by: Ashintar Posted at: 2018-05-18T21:41:18.160Z Reads: 112

```
Looks like you just used the defaults settings.
```

---
## \#6 Posted by: piepolitb Posted at: 2018-05-18T22:03:36.777Z Reads: 112

```
Mostly, they look like a good starting point to me
```

---
## \#7 Posted by: Ashintar Posted at: 2018-05-18T22:24:04.993Z Reads: 111

```
That vesc is known to only be good to 50a continous for the battery max setting,  you have it set to 60 which is prolly caused the issue
```

---
## \#8 Posted by: piepolitb Posted at: 2018-05-18T22:39:07.877Z Reads: 111

```
My mistake but It is unlikely that I got up to 50amp... I was going very slowly fpr the test 

Plus I volounterly stopped my riding as I said: no smoke, no burning. Just silently no more going after reconnecting the power. I think that if I had drained to much current I would have fried the Vesc and I would have noticed. Right?
```

---
## \#9 Posted by: piepolitb Posted at: 2018-05-21T15:07:24.876Z Reads: 101

```
UPDATE: 

if I give it a little "jump start", a little initial rotating speed manually to the wheel, it works: motor spinning and no fault code.

The motor is not spun and I get the FAULT_CODE_DRV just if I give throttle from standing still 

ideas?
```

---
## \#10 Posted by: piepolitb Posted at: 2018-05-21T17:12:00.335Z Reads: 97

```
UPDATE 2:

following @goldenHusky suggestion I tried on another motor (a little one, from a quadcopter) in order to exclude motor issues. 

Same behavior, plus I was able to start from standing still by very very slowly increasing the throttle. 
Which is basically the same thing of jump starting on a bigger motor: not asking for to much torque(and current?) at the beginning.
I think...

ideas?
```

---
## \#11 Posted by: piepolitb Posted at: 2018-05-22T13:55:16.506Z Reads: 89

```
UPDATE 3: 
I tried one more thing, same motor another ESC capable of 7s tops on a desk power supply.
I was expecting the motor to be spun from also standing still, but no... same behavior: motor starts only with a little help.

so, RECAP
- TB VESC + TB motor : no starting from standing still and COFE_FAULT_DRV. It starts with some initial kicking
- TB VESC + little quadcopter motor : no starting from standing still and COFE_FAULT_DRV. It starts with some initial kicking
- old ESC + TB motor : no starting from standing still. It starts with some initial kicking

:thinking::thinking: In this way I can't exclude failure neither in the motor as @goldenHusky suggested nor in the ESC ... right?
```

---
## \#12 Posted by: professor_shartsis Posted at: 2018-05-22T14:41:41.421Z Reads: 86

```
it’s possible you don’t have enough thrust with your gearing and only one motor and 60a to overcome your stationary load. (you mention the problem only occurs using the throttle from a dead-stop)

ways to increase thrust:

-increase your gear reduction ratio
-use 2 motors instead of 1
-increase the motor amp limit

or is it possible you have a battery management system which is causing power cut-outs when you exceed X # of amps?

what’s your tire size and gear ratio?
```

---
## \#13 Posted by: piepolitb Posted at: 2018-05-22T14:51:10.514Z Reads: 85

```
Hi, 
gear ratio is 2:1. 
amp limit is at maximum bearable by the VESC.
Also it was working with current setup, so no, there is no battery management system involved

Problem is that I have the same problem with free motor shaft, no load/weight applied.
```

---
## \#14 Posted by: professor_shartsis Posted at: 2018-05-22T14:58:40.849Z Reads: 83

```
2:1 seems quite low for single-motor drive @ 190kv. tire size?
```

---
## \#15 Posted by: briman05 Posted at: 2018-05-22T15:35:56.717Z Reads: 82

```
one problem is that the motor is in sensorless mode meaning that you need a kick start to get the board going.  The load you have on one motor is greater then the amount of torque needed to get you going. That motor can be ran in sensored mode as it has the sensor wire. Maybe to much amp build up and and blew the vesc.  Also the -40 bat regen is really high are you using lipo or li-ion batteries.
```

---
## \#16 Posted by: piepolitb Posted at: 2018-05-22T15:44:03.171Z Reads: 78

```
@professor_shartsis 70mm diameter

@briman05 yeah I know about the sensored mode, problem is I don't have the adapter cable for the VESC. I need to find some free time to do it myself... after I have found which wire is which of course...

Thing is, as I said before, I need to kick it start also with no load on the shaft, to be clear: belt removed and test bench

Lipo batteries, do you think I need to lower it down? how much?
```

---
## \#17 Posted by: briman05 Posted at: 2018-05-22T15:55:11.284Z Reads: 68

```
If you take the belts off and put it on the test bench your motors should spin freely without any load on them.  I'm not sure what your settings would be for the lipo batteries as am using li-ion  It looks like you are using the vesc tool  that should do the calculations for the cutoff start and end for you.  What is your battery parallel because you need to figure that out in order to set the right regen for your batteries.
```

---
## \#18 Posted by: piepolitb Posted at: 2018-05-22T16:09:29.261Z Reads: 68

```
> If you take the belts off and put it on the test bench your motors should spin freely without any load on them. 

yes, it should... and it did, once upon a time...

> I’m not sure what your settings would be for the lipo batteries as am using li-ion It looks like you are using the vesc tool that should do the calculations for the cutoff start and end for you

cutoff start and end are in terms of voltage and set to 12s settings (40.8 and 37.2).

>  What is your battery parallel because you need to figure that out in order to set the right regen for your batteries

I'm with 12s1p, 5800 mAh, 25c. 
Saying [here](https://rogershobbycenter.com/lipoguide/) that "The safest charge rate for most LiPo batteries is 1C, or 1 x capacity of battery in Amps. ", I set it to 5Amps, just to be safer.

Do you agree?
```

---
## \#19 Posted by: briman05 Posted at: 2018-05-22T16:17:11.731Z Reads: 72

```
Maybe ask @Namasaki he has alot of experience with lipo batteries
```

---
## \#20 Posted by: Namasaki Posted at: 2018-05-22T18:27:30.564Z Reads: 69

```
I’m using 5000mah 60C Lipos that are rated for 5C charge. 
I charge them on the bench with 5a and my Vescs are set at -10a each for regen charging. 

I would recommend that you check the specs on your Lipos for thier max charge rate.
```

---
## \#21 Posted by: professor_shartsis Posted at: 2018-05-22T19:59:06.658Z Reads: 68

```
one thing I do know is it’s “difficult” for a controller to spin a motor from a standstill without sensors... this is partly because it uses the back emf voltage produced by the spinning rotor magnets to “know” the rotor position & which phases to energize & for timing exactly when to commutate... so without sensors or back emf voltage from a spinning rotor, my understanding is at standstill the controller “blindly” energizes phases in sequence in an attempt to get the rotor to turn so that it will generate back emf voltage which then gives it the timing information for subsequent commutations... if the load is too great or not enough back emf voltage is produced to get a good rotor position reading while it’s “blindly” energizing phases at start-up, perhaps it generates a DRV error. this is just a theory, hope it helps.
```

---
## \#22 Posted by: Falcon87407 Posted at: 2018-06-02T22:50:26.257Z Reads: 55

```
I'm having this EXACT issue with a brand new setup.  10s4p Li ion with a 10s BMS VESC and a 6364 190Kv motor.  It also hits full speed at half throttle...
```

---
