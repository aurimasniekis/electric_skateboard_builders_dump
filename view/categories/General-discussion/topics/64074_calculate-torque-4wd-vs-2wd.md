# Calculate Torque 4wd vs 2wd

### Replies: 27 Views: 695

## \#1 Posted by: mackann Posted at: 2018-08-06T22:44:51.628Z Reads: 176

```
I'm trying to find out what kv motor will give equal torque on 4wd as 2wd 190kv.
How can I calculate it? 
Reason is I want max top speed(prefered around 45mph) but still have the same torque as dual 6374 190kv setup. 
The setup is 107mm wheels, 6374 3200w motor, 12s6p battery, geared ratio 2.4:1
Do you think 4 6374 230kv will have same or better torque thene dual 6374 190kv?
(And yes I can footbrake and have good protection, I'm not gonna go crazy in town) 
Ty for any help!
```

---
## \#2 Posted by: professor_shartsis Posted at: 2018-08-06T23:02:35.643Z Reads: 172

```
for the same full throttle vehicle thrust with 4WD as 2WD you can use 1/2 the motor amp limit setting with 4WD compared to the 2WD motor amp limit setting (same kv). torque is directly proportional to the motor current so half the current but twice the motors gives the same thrust / acceleration. since heating is proportional to the square of the current you’d see 1/4th the ohmic heating per motor and 1/2 the ohmic heating overall with the 4WD.
```

---
## \#3 Posted by: pat.speed Posted at: 2018-08-07T10:45:37.435Z Reads: 146

```
That’s not what he means, he means what kV motor/ gear ratio should he use in a 4wd as a 2wd to boost speed but maintain torque. 

Example of this would be to half the gear ratio and then double the motors, although if worked out with maths I doubt this is exactly correct. Maybe you could help him do this as you seem to be very good with the calculations
```

---
## \#4 Posted by: professor_shartsis Posted at: 2018-08-07T18:31:52.041Z Reads: 124

```
[quote="pat.speed, post:3, topic:64074"]
That’s not what he means, he means what kV motor/ gear ratio should he use in a 4wd as a 2wd to boost speed but maintain torque.
[/quote]


Well to begin with he can reach 45mph with only 2 motors by switching from 2.4:1 to 2.18:1 gear ratio without changing anything else... however this change would decrease the peak vehicle thrust from 60.8 lbs to 55.2 lbs.

(2) 190kv motors, 0.05ohm, 107mm tire, 46v battery, 100% throttle, 95% max duty cycle, 60a motor amp limit, 30a battery amp limit per motor

https://image.ibb.co/cHXnJz/2_4_vs_2_18.gif
```

---
## \#5 Posted by: longhairedboy Posted at: 2018-08-07T18:42:18.271Z Reads: 106

```
I'm assuming you're running 12S voltages. Reaching 45mph on a belted rear wheel drive system is kind of trivial at this point, and you don't need to go higher than 190KV to do it, as @professor_shartsis (hilarious handle, btw) correctly points out. 

However, the question may remain uinanswered because it is NOT recommended to run 12S at over 190 ACTUAL KV. Now... depending on what motors you get.. the ACTUAL KV will invariably be lower than the stated KV however the amount of difference will vary. 

I would start with motors rated at 200KV and go from there incrementally. The likelyhood that they are actually over 190KV upon being measured on the bench is slim, but they may be higher than the 190KV motors you might have already. 

There's a thread around here that discusses actual KV versus advertised, and there is math and other things you can do to figure out actual KV using BLDC or VESC tool. I don't have a link handy, but maybe somebody else does.
```

---
## \#6 Posted by: skatardude10 Posted at: 2018-08-07T19:32:54.237Z Reads: 101

```
Type kv in BLDC/vesc tool debug console and divide number by 7 assuming 7 pole pairs standard on most motors if I remember correctly. Gotta give this a try myself.
```

---
## \#7 Posted by: professor_shartsis Posted at: 2018-08-07T23:57:36.207Z Reads: 95

```
[quote="pat.speed, post:3, topic:64074"]
he means what kV motor/ gear ratio should he use in a 4wd as a 2wd to boost speed but maintain torque.
[/quote]

now suppose he changes from (2) 190kv motors to (4) 190kv motors & changes the gear ratio from 2.4:1 to 1.77:1... top speed increases from ~40mph to 55mph & peak vehicle thrust increases from 60.8lbs to 90.1lbs...

https://image.ibb.co/gSAiAe/2_vs_4_motors.gif
```

---
## \#8 Posted by: longhairedboy Posted at: 2018-08-08T12:29:25.063Z Reads: 75

```
Indeed. I clocked @jayx at 44mph in january on a beast evo built by @Battosaii 

just found some footage from that day on my go pro last night. I may get around to editing it.
```

---
## \#9 Posted by: Battosaii Posted at: 2018-08-08T12:31:40.085Z Reads: 74

```
Funny you should say that cause that same Evo is going 4wd with quad 6374s and a 12s8p so I doubled up everything lol
```

---
## \#10 Posted by: longhairedboy Posted at: 2018-08-08T12:34:35.628Z Reads: 74

```
wtf are you dragging the battery behind you in a trailer? lol 

this is why i love this place. 12S8P good god. I wouldn't want to weld that one.
```

---
## \#11 Posted by: Battosaii Posted at: 2018-08-08T12:35:53.902Z Reads: 75

```
Haha @Eboosted made me a double stack Evo enclosure I could fit a 10p if I didn't have to fit 4 Focboxes.
```

---
## \#12 Posted by: mackann Posted at: 2018-08-08T13:10:30.324Z Reads: 71

```
I just ordered 4 6374 custom wired for higher kv 220kv.
Will also use eboosted enclosure and evo board and a 12s6p battery and 4 flipsky vesc 6.
107mm abec 11 wheels.
Last to decide if i will go with belt or geared drive.. Hope 3dservice release their fatboy soon..
```

---
## \#13 Posted by: professor_shartsis Posted at: 2018-08-08T14:21:54.451Z Reads: 70

```
[quote="mackann, post:12, topic:64074, full:true"]
I just ordered 4 6374 custom wired for higher kv 220kv.
Will also use eboosted enclosure and evo board and a 12s6p battery and 4 flipsky vesc 6.
107mm abec 11 wheels.
Last to decide if i will go with belt or geared drive… Hope 3dservice release their fatboy soon…
[/quote]

if you're looking to maximize top speed with that setup i find you can hit 70mph top speed @ 240a battery amps & 81.71lbs peak thrust w/ (4) 220kv motors, 0.025ohm, 46v battery, 107mm tire, 1.6:1 gear ratio, 70a motor current limit & 60a battery current limit per motor...

https://image.ibb.co/cZQ7Le/70mph.jpg
```

---
## \#14 Posted by: mackann Posted at: 2018-08-08T17:30:26.969Z Reads: 59

```
haha then i will for sure kill me :P i will go with 1:2.4 i think
Ty for the calculations!
```

---
## \#15 Posted by: professor_shartsis Posted at: 2018-08-09T01:02:14.514Z Reads: 59

```
i believe you'll hit 45mph & 122.5lbs peak thrust with the 2.4:1 gear ratio, 220kv, 4 motors, 70a motor current limit
```

---
## \#16 Posted by: psychotiller Posted at: 2018-08-09T01:14:10.261Z Reads: 60

```
http://esk8builds.com/photo/view/?id=84
```

---
## \#17 Posted by: Wraith Posted at: 2018-08-09T01:17:23.970Z Reads: 60

```
the fatboy mini urethane drives should be out soon as I've seen the custom hangars and pulleys. Should be a matter of time :smile:
```

---
## \#18 Posted by: Nate Posted at: 2018-08-09T01:23:10.809Z Reads: 63

```
How do you calculate vehicle thrust?
```

---
## \#19 Posted by: professor_shartsis Posted at: 2018-08-09T01:34:27.139Z Reads: 61

```
[quote="Nate, post:18, topic:64074, full:true"]
How do you calculate vehicle thrust?
[/quote]

60 / (2 * pi * KV) = **KT (Torque in Newton Meters Per Amp of Motor Current)**

Motor Current Limit * KT = **Peak Motor Torque in Newton Meters**

Peak Motor Torque in Newton Meters * Gear Ratio = **Wheel Torque in Newton Meters**

(Wheel Torque in Newton Meters * 1000mm) / ((1/2) * Tire Diameter in MM) = **Thrust in Newtons, 1 Motor**

https://image.ibb.co/jSury9/lever.jpg

Thrust in Newtons, 1 Motor × 0.224808943 = **Thrust in Pounds, 1 Motor**

Thrust in Pounds, 1 Motor × 0.453592 = **Thrust in Kilograms, 1 Motor**

Thrust, 1 Motor * Motor Quantity = **Vehicle Thust**
```

---
## \#20 Posted by: Nate Posted at: 2018-08-09T03:04:58.092Z Reads: 53

```
I tried to do the math, the numbers got complicated real fast. Thanks for the info anyway.
```

---
## \#21 Posted by: professor_shartsis Posted at: 2018-08-09T03:13:52.539Z Reads: 51

```
[quote="Nate, post:20, topic:64074, full:true"]
I tried to do the math, the numbers got complicated real fast. Thanks for the info anyway.
[/quote]

[quote="professor_shartsis, post:15, topic:64074"]
i believe you’ll hit 45mph &amp; **122.5lbs peak thrust** with the 2.4:1 gear ratio, 220kv, 4 motors, 70a motor current limit
[/quote]


60 / (2 * pi * 220 KV) = **0.04340 KT (Torque in Newton Meters Per Amp of Motor Current)**

70 Motor Current Limit * 0.04340 KT = **3.03841 Peak Motor Torque in Newton Meters**

48 wheel teeth / 20 motor teeth = **2.4 gear ratio**

3.03841 Peak Motor Torque in Newton Meters * 2.4 Gear Ratio = **7.29219 Wheel Torque in Newton Meters**

(7.29219 Wheel Torque in Newton Meters * 1000mm) / ((1/2) * 107 Tire Diameter in MM) = **136.30261 Thrust in Newtons, 1 Motor**

136.30261 Thrust in Newtons, 1 Motor × 0.22480 = **30.64204 Thrust in Pounds, 1 Motor**

30.64204 Thrust in Pounds, 1 Motor × 0.45359 = **13.89898 Thrust in Kilograms, 1 Motor**

30.64204 Pounds Thrust, 1 Motor * 4 Motor Quantity = **122.56819 Pounds Vehicle Thust <---**
```

---
## \#22 Posted by: Nate Posted at: 2018-08-09T05:06:37.318Z Reads: 43

```
Dude this was so helpful. If my calculation are not off, 4x 250kv on 3:1 gear ratio with 6.5 inch wheels will put the vehicle thrust at about 93.65576 Pounds Vehicle Thrust.

Is there a formula to calculate how fast a vehicle will hit top speed with vehicle thrust?
```

---
## \#23 Posted by: professor_shartsis Posted at: 2018-08-09T16:03:44.699Z Reads: 41

```
[quote="Nate, post:22, topic:64074"]
Is there a formula to calculate how fast a vehicle will hit top speed with vehicle thrust?
[/quote]

if there was no air, you could use this:

Force (Newtons) = Mass (KG) * Acceleration (m/s^2)

therefore:

Force (Newtons) / Mass (KG) =  Acceleration (m/s^2)

------------------

A = acceleration (m/s2)
B = the final velocity (m/s)
C = the initial velocity (m/s)
D = the time in which the change occurs (s)
E = the change in velocity (m/s)

A = ((B - C) / D) = (E / D)

therefore 

(B - C) / A = D the time in which the change occurs (s)
```

---
## \#24 Posted by: Battosaii Posted at: 2018-08-09T16:08:39.478Z Reads: 40

```
I wonder if my set up can reach the theoretical weighted speed of 49mph with 4 6374, 12s8p 30q pack and 16/42 pullies on 152mm wheels.
```

---
## \#25 Posted by: professor_shartsis Posted at: 2018-08-09T16:21:15.052Z Reads: 39

```
what are the kv and current limits?
```

---
## \#26 Posted by: Battosaii Posted at: 2018-08-09T16:28:16.171Z Reads: 42

```
190kv running 80motor amps and 40 constant battery amps per Focbox.
```

---
## \#27 Posted by: professor_shartsis Posted at: 2018-08-09T17:46:44.744Z Reads: 41

```
[quote="Battosaii, post:24, topic:64074, full:true"]
I wonder if my set up can reach the theoretical weighted speed of 49mph with 4 6374, 12s8p 30q pack and 16/42 pullies on 152mm wheels.
[/quote]

[quote="Battosaii, post:26, topic:64074, full:true"]
190kv running 80motor amps and 40 constant battery amps per Focbox.
[/quote]

it looks like with 2 motors, you'd hit 49-50mph, judging from where the yellow line, bottom left chart (vehicle thrust pounds, 2 motors) dips below the blue line, bottom left chart (wind drag force, pounds)  (2 motors thrust force @ 50mph = 34.99lbs -- wind drag force @ 50mph = 35.08lbs).

with 4 motors, it looks closer to 54mph, judging from where the red line, bottom left chart (vehicle thrust pounds, 4 motors) dips below the blue line (wind drag force, pounds).

The peak vehicle thrust of 124.88lbs (red line, bottom left chart) begins to drop off at about 25mph, because due to the increasing back emf voltage with increasing speed (red line, top left chart), sustaining 80a motor current above ~25mph would require more than the 40a battery current limit per motor.

(46v battery, 0.050ohm winding, (4) 190kv motors, 152mm tire, 42 wheel teeth, 16 motor teeth, 2.625:1 gear ratio, 100% throttle, 95% max duty cycle, 80a motor current limit & 40a battery current limit per motor)

https://image.ibb.co/cUnDVp/190kv_4motors.jpg
```

---
