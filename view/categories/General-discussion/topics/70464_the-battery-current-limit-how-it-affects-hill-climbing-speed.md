# The battery current limit &amp; how it affects hill climbing speed

### Replies: 4 Views: 357

## \#1 Posted by: professor_shartsis Posted at: 2018-10-07T18:57:10.067Z Reads: 94

```
I wondered how different battery current limit settings affect hill climbing ability-- so I did a comparison of 30a vs 60a battery current limits per motor (both 100a motor current limit) with (2) 73kv hub motors at 46v with 84mm tires...

the grade chosen for the comparison is a 31.5% slope which is equivalent to the steepest street in san francisco. the minimum force required in both pounds and watts to maintain speed or accelerate on the 31.5% slope is shown on the purple line, bottom left chart (pounds) and the green line, top middle chart (watts). the vehicle thrust in pounds and watts is shown in the red line, bottom left chart (pounds), and red line top middle chart (mechanical watts).

https://image.ibb.co/e1RAdp/climbing_30a_vs_60a_battery.gif

conclusions:

19mph top speed up 31.5% slope with 100a/30a motor/battery current limits
27mph top speed up 31.5% slope with 100a/60a motor/battery current limits

(the top speed is assessed by where the red line dips below the purple line on the bottom left chart)
```

---
## \#2 Posted by: eb1925 Posted at: 2018-10-07T19:10:07.561Z Reads: 87

```
Super interesting man! Now, this is true when the battery amps are the bottleneck. On my single drive build, wheel and belt traction are the bottleneck, so I've found that on single 6374 30 battery amps performs **almost** as well as 60 amps and prevents my wheel and belt from slipping. I weigh 180 pounds.

Do you have numbers on motor and VESC temperatures from both?
```

---
## \#3 Posted by: professor_shartsis Posted at: 2018-10-07T19:21:35.421Z Reads: 85

```
[quote="eb1925, post:2, topic:70464"]
Do you have numbers on motor and VESC temperatures from both?
[/quote]

this is all predicted.

motor numbers used: 
**46v** battery, **(2) 73kv** hub motors with **0.07ohm** resistance and **84mm** tires, **200lbs** rider + board, **0.75** wind drag coefficient, **0.6m^2** frontal area

**motor current** is calculated from:

(effective pwm voltage - back emf voltage) / winding resistance = motor current

**back emf voltage** is:

motor rpm / kv = back emf voltage

**electrical watts** is:

motor current * effective pwm voltage = watts electrical

**torque** in newton meters is calculated with:

(60/(2 * pi * kv)) * motor current

**mechanical power** in watts is:

torque newton meters * angular speed in radians per second

**slope force in newtons** is calculated with:

mass in kg * gravity acceleration (9.8m/s^2) × sin(slope angle in degrees)

**wind force in newtons** is:

(1÷2) * 1.225kg/m^3 air density * front area in m^2 * (meters per second * meters per second ) * standing human drag coefficient
```

---
## \#4 Posted by: eb1925 Posted at: 2018-10-07T19:23:24.991Z Reads: 69

```
Ahhhhhhhhh I see.
```

---
