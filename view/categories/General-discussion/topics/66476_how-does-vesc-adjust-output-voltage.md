# How does VESC adjust output voltage?

### Replies: 17 Views: 580

## \#1 Posted by: Jmding Posted at: 2018-08-29T16:18:22.668Z Reads: 107

```
Does anyone know for sure if the VESC controls motor speed by applying pwm to the output to reduce the effective voltage, or by using a transformer-like mechanism to trade voltage for current?
```

---
## \#2 Posted by: Giga Posted at: 2018-08-29T16:31:19.112Z Reads: 103

```
Maybe try googling "Dutycycle"
Thats how every Esc works, modulation of the dutycycle...
```

---
## \#3 Posted by: Namasaki Posted at: 2018-08-29T16:33:59.396Z Reads: 100

```
That’s how hobby esc’s work
The Vesc has duty cycle option, current control option and watt control option with akmaniac firmware
```

---
## \#4 Posted by: longhairedboy Posted at: 2018-08-29T16:38:58.482Z Reads: 97

```
current control no reverse with brake has been my go-to for the past few years. 

still need to try this watt control thing.
```

---
## \#5 Posted by: Brdchris Posted at: 2018-08-29T16:57:41.809Z Reads: 84

```
What you are describing is bldc (brushless dc). It outputs pwm dc voltage. The motor is an inductive load so it smooths the pwm signal to make current look somewhat like a sin wave.

Foc is slightly different. From what I understand it is actually varying voltage to the base of the transistor so that the VESC outputs a sin wave
```

---
## \#6 Posted by: Deckoz Posted at: 2018-08-29T17:29:32.879Z Reads: 77

```
Voltage in all forms of control is duty cycle. Timing/phase control is either sequential BLDC, or All phase FOC for our applications. Motor speed is kV * voltage. Current is a factor of load required to spin the motor at speed.  

Duty cycle 25%
Voltage at point in time 38.9V
Motor voltage at point in time (38.9 * .25) = 9.725V
RPM motor wants to be at with applied voltage (190kV * 9.725) = 1846 RPM

Current is dependent on load, resistance of a motor and the applied voltage  will give you No-Load Current. Ie for a set of 190kV motors I have the no load current at 9.7v is 1.6A. so at 9.725 motor volts, the load can be no less than 1.6A. add a factor of load to it and the current will increase continuously until the motor can achieve the speed of it's applied voltage * kV ie 1846RPM.
```

---
## \#7 Posted by: Jmding Posted at: 2018-08-29T17:32:42.119Z Reads: 77

```
Gotcha, it pwm's it.  Interesting that pwm decreases voltage but increases amperage.  I guess the power needs to be conserved, so it has to be true.  Thanks!
```

---
## \#8 Posted by: Deckoz Posted at: 2018-08-29T17:43:45.534Z Reads: 72

```
Kind of. BLDC is closer to PWM because the gates open and close on the fets and only two phases are powered are once making a square wave form. FOC is continuous modulation of the amplitude across all phases making a trapezoidal/sine. 

Speed doesn't equal torque. Speed is a result of kv and voltage. 
Torque is a result of efficiency and current at a given voltage.

> Kv = RPM per volt
Rm = motor resistance in Ohms
Io = No load current

> Kq Torque constant.(units = N m):
Kq = 30/(pi Kv) 

> RPM and TORQUE at current I:
RPM = Kv(I – Io)
Q = Kq(I – Io)

> MOTOR EFFICIENCY:
η = Mechanical power out/electrical work in
η = (V- I Rm)(I - Io)/(V I): V and I= working voltage and current.

> CURRENT AT MAX EFFICIENCY:
Imax = sqrt(V Io/Rm)

> Torque at max efficiency:
Qmax = Kq (Imax – Io)

> RPM at max eff:
RPMmax = Kv( V – Imax Rm)
```

---
## \#9 Posted by: Namasaki Posted at: 2018-08-29T18:06:32.819Z Reads: 60

```
I’m not a scientist or electrical engineer. 
All I know is that with Vesc in current control and no load like when the board is upside down, the wheels spin full speed regardless of throttle position. Only when load is applied does the throttle increase/decrease speed.
To a common man like myself, it seems that the Vesc in current control outputs constant voltage with variable current. 

With my old car esc’s which ran in duty cycle, it was a completely different story. 
With no load, motor speed was variable by throttle position.
```

---
## \#10 Posted by: Deckoz Posted at: 2018-08-29T18:08:23.458Z Reads: 63

```
[quote="Namasaki, post:9, topic:66476"]
wheels spin full speed regardless of throttle position
[/quote]

Not true.

You can see me modulating speed at the beginning of this video and slowly ramping to full 

https://youtu.be/lLq1TqGgnI0
```

---
## \#11 Posted by: Sebike Posted at: 2018-08-29T18:09:20.593Z Reads: 59

```
I don't recognize that... Easy on the throttle makes wheels turn slowly even with no load.
```

---
## \#12 Posted by: Jmding Posted at: 2018-08-29T18:10:16.576Z Reads: 58

```
I think the VESC controls voltage, and measures current.  Thus to "control" current, it's applying PID control, varying the voltage until it achieves the desired current draw?
```

---
## \#13 Posted by: Namasaki Posted at: 2018-08-29T18:11:05.773Z Reads: 57

```
Are you running in watt control mode?
I run in current control BLDC no sensors and mine doesn’t work that way
I get full speed at 1/4 throttle with no load
My car esc’s had variable speed from zero to full throttle with no load.
```

---
## \#14 Posted by: Deckoz Posted at: 2018-08-29T18:15:15.344Z Reads: 56

```
No watt control in 3.xx ;) only watt limits.
```

---
## \#15 Posted by: Namasaki Posted at: 2018-08-29T18:19:03.308Z Reads: 57

```
I’m using 2.18 on Vesc 4.12 there is no watt limiting on this version. 
So I guess things have changed with the newer firmwares.

Guess I’m just an old dog that won’t  learn new tricks.
```

---
## \#16 Posted by: skatardude10 Posted at: 2018-08-29T18:58:45.698Z Reads: 54

```
Ah, so Ackmaniac's firmware still has the added watt control feature just integrated as the standard max wattage part of current control in the new 3.xx+ firmwares, where max wattage set = 100% throttle, decreasing to say 50% wattage at 50% throttle and so on (based on linear throttle curve) as opposed to just a limit in the standard firmware?

I haven't had a chance to test and feel the difference between standard 3.xx+ compared to Ackmaniac's, but when I heard the standard firmware had watt limits now, I assumed it basically meant it worked the same as Ackmaniac's controlling wattage linearly based on duty cycle and not just as a limit.
```

---
## \#17 Posted by: Giga Posted at: 2018-08-30T08:34:05.377Z Reads: 42

```
[quote="Namasaki, post:3, topic:66476"]
That’s how hobby esc’s work
[/quote]

No, thats how every ESC works.

[quote="Namasaki, post:3, topic:66476"]
The Vesc has duty cycle option, current control option and watt control option with akmaniac firmware
[/quote]
Thats how you tell the controller what to do, but has nothing to do with the output of the ESC. 
Since the Mosfets (at least in our use-case) has simplified only 2 states, Open or Closed, you can just modulate the dutycycle. Current control is measuring the current (by shunts) and adjust the dutycycle/pwm-output to it.

[quote="Brdchris, post:5, topic:66476"]
Foc is slightly different. From what I understand it is actually varying voltage to the base of the transistor so that the VESC outputs a sin wave
[/quote]
Practically FOC works after the same principal: the mosfet still has only 2 states (again simplified, no ramp up, no ramp down, no leakage, no resistance...), Open or Closed, so to get the desired sine wave you need for FOC, you simply vary the dutycycle and get something like this: 
![image|475x500](upload://xRpviLgCVqgiDMJWLeqbOHgoM2o.png)
(from here: https://www.ijareeie.com/upload/2013/july/15_COMPARISON.pdf)

So every ESC basically just does PWM, but the thing is, what is the desired "wave"-form (block, trapezial, sine wave, triangular wave...) and how good is your timing...
```

---
