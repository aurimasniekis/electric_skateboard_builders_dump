# Question about setup

### Replies: 17 Views: 1024

## \#1 Posted by: anoop54 Posted at: 2017-02-24T13:56:57.773Z Reads: 91

```
Hey Im new to building electric boards, 
My current setup is a 170KV motor, With a 12s li-po pack and a 16T/36T gear ratio set up. 
When riding the board, I don't feel as if enough torque is being produced and so max speed isn't reached. Im using a vsec, any help would be good! Also the wheels have a diameter of 70mm. Mathematically the top speed should be 50km/h. I plan on buying 83 mm wheels, which would further decrease torque, so what is my cheapest option here?
```

---
## \#2 Posted by: mmaner Posted at: 2017-02-24T13:59:41.747Z Reads: 91

```
If you have access to a 3D printer you could print a 32T wheel pulley.  That's probably the cheapest method increasing torque, but it will alos decrease top speed.
```

---
## \#3 Posted by: anoop54 Posted at: 2017-02-24T14:18:30.155Z Reads: 85

```
I do have access to one! If i wanted better speed + torque, Would I need a stronger motor? If so what would you recommend kv wise, I'd like to take full advantage of my 12s supply
```

---
## \#4 Posted by: mmaner Posted at: 2017-02-24T15:01:28.114Z Reads: 72

```
I dont use 12s, too risky for VESC.  That being said, firstly I would go to dual motor setup.  Failing that, you could go to 16/32 and upgrade to a 190kv 6374 motor.  That should give you an increase in torque and speed.
```

---
## \#5 Posted by: TarzanHBK Posted at: 2017-02-24T15:29:26.874Z Reads: 70

```
post a screenshot of your vesc settings.
```

---
## \#6 Posted by: jaykup Posted at: 2017-02-24T15:41:57.168Z Reads: 66

```
Yeah, your setup is pretty good, should have LOTS of power.  It might be the VESC settings or your batteries can't handle the current.  Screenshots would help.  Is it 6355 motor?
```

---
## \#7 Posted by: darkkevind Posted at: 2017-02-24T15:56:57.994Z Reads: 63

```
That will increase speed and reduce torque...
```

---
## \#8 Posted by: mmaner Posted at: 2017-02-24T16:16:26.508Z Reads: 60

```
the decrease in gear size should increase torque and the increase in motor kv should increase speed?  Is that not correct?
```

---
## \#9 Posted by: darkkevind Posted at: 2017-02-24T16:57:41.319Z Reads: 52

```
A decrease in gear size on the wheel will reduce torque. The increase in KV will also reduce torque but increase the speed.
```

---
## \#10 Posted by: Titoxd10001 Posted at: 2017-02-24T18:17:46.938Z Reads: 52

```
Reducing wheel pulley teeth will increase speed while decreasing torque. You want a smaller motor side pulley down to 15 or even 14 but you also want to keep in mind you want 6 teeth in mesh. 

@anoop54 if you account for voltage sag and 95% duty cycle you should be at about 42km/h top speed. What top speed are you getting?
```

---
## \#11 Posted by: jaykup Posted at: 2017-02-24T19:18:33.006Z Reads: 51

```
Motor/wheel pulleys, wheels and kv are all important and impact performance, but if he feels the current setup is not powerful, and the VESC hasn't been setup correctly, that's really the place to start.  I'm running something similar and the board quickly and easily hits 30mph/48kmh.  12s, single 190kv 6355, 16/36 with 80mm wheels.

With his 70mm wheels, 170 KV motor and accounting for voltage sag, he should still be able to hit 40-45 km/h easily and quickly.  If not, the motor isn't getting enough power, either through the VESC settings limiting it, or the battery/wires being wimpy.

If it IS hitting 40-45km/h quickly, but he just wants to go faster, then bigger wheels or different gearing will help with top speed, and slow acceleration a bit.
```

---
## \#12 Posted by: anoop54 Posted at: 2017-02-24T20:31:16.967Z Reads: 49

```
I feel as if my vsec is not setup properly, either that or my motor is defective. I say this because as the motor is running Im able to stop it using my hand and i feel like there should be way more torque than that. Thank you all for your replies. Here are the screenshots, note mac current ramp step has been changed to 0.004. @jaykup @Titoxd10001 @TarzanHBK   @mmaner 

<img src="/uploads/db1493/original/3X/f/b/fbb6b3b6c0f7482070db5894a601a47ba679e2a5.png" width="690" height="356"><img src="/uploads/db1493/original/2X/b/bfeee6e87866829cbaf016e28a156e49eb19b8b4.png" width="690" height="382"><img src="/uploads/db1493/original/2X/8/82d0dce75cf214fce43751932c22beddacef0641.png" width="690" height="360">
```

---
## \#13 Posted by: treenutter Posted at: 2017-02-24T20:38:32.676Z Reads: 42

```
@anoop54 my first thought would be to increase the Motor Max amperage. Also, reduce Max ERPM to 60K or less.
```

---
## \#14 Posted by: Titoxd10001 Posted at: 2017-02-24T20:53:28.784Z Reads: 40

```
Your values are to low for single drive
I would start with and go up as needed
Motor max:60
Motor min:-45
Batt max:45
Batt min:-15
Max erpm:60k
```

---
## \#16 Posted by: mmaner Posted at: 2017-02-25T04:13:29.800Z Reads: 29

```
Yeah, I don't know how I got that all mixed up in my head.  Been a heavy couple of weeks 😀. Thanks for the correction.
```

---
## \#17 Posted by: anoop54 Posted at: 2017-03-02T05:42:09.164Z Reads: 25

```
Hey guys, why does motor max have to greater than motor max?
```

---
## \#18 Posted by: Tronik Posted at: 2017-03-07T02:18:20.675Z Reads: 20

```
i dont know but i overvolt my brushed motors by 33%, with a matching esc.  I plan to go even higher.  60 v esc with 60 or 72 lion, all on 4motors... so... 4wd 36v brushies.  when i hit em with 60v, i think they will actually be ok, ..hopefully they can take it, dual motors would be a bad ass burnout perhaps
```

---
