# ND &#124; Calculator

### Replies: 20 Views: 617

## \#1 Posted by: NordeHQ Posted at: 2019-03-10T08:27:30.208Z Reads: 227

```
I have built a calculator based on a physical models for parts selection, or to check setup performances: 

[https://norde.cc/calculator.php](https://norde.cc/calculator.php)

For the time being, you can determine your motor power, capacity, and gear ratio based on your requirements. You can also check your range, your system efficiency and your top speed based on your parts. Here is a screenshot:

![calculator_home|690x336](upload://nfdgzm14ITfm7fJeFhZBAO4OE0X.jpeg) 

[details="Fields explanation"]

**Power calculation**
-

* **Rider weight:** Your weight in kg
* **Speed:** The average speed you would like to achieve
* **Start time:** Time to achieve your average speed
* **Flat distance:**  Range you would like to achieve on flat road
* **Climbing distance:** Range you would like to achieve on slope 
* **Slope:** Slope gradient on the road
* **Motor efficiency:** The efficiency of your motor
* **Motor configuration:** Dual or single
* **Battery type:** Chemical technology of your battery
* **Battery configuration:** Number of cells of your battery

**Drivetrain calculation**
-

* **Motor pulley:** Number of teeth for your motor pulley
* **Wheel pulley:** Number of teeth for your wheel pulley
* **Wheel diameter:** Diameter of the wheel (in mm)
* **Center distance (Optional):** Center distance between your motor pulley and your wheel pulley
* **KV Motor:** Motor kv constant
* **Battery type:** Battery technology
* **Battery configuration:** Number of battery cells

To perform a calculation, you can press "Enter" on a field.
[/details]
  


Enjoy!
```

---
## \#2 Posted by: nuttyjeff Posted at: 2019-03-10T09:11:41.441Z Reads: 181

```
Thanks for your contribution, but I don't really know how to use it :sweat_smile:
```

---
## \#3 Posted by: NordeHQ Posted at: 2019-03-10T09:23:52.406Z Reads: 176

```
I have added some explanation on how to complete the form. You can press enter to perform calculation. 
Does it make more sense now?
```

---
## \#4 Posted by: murloc992 Posted at: 2019-03-10T09:29:24.530Z Reads: 172

```
The range calculation makes my 12S6P dual at 25KM/h appear as a 100+KM range one if I only go flat. :smiley: I really doubt it. Even adding inclines I still get 60KM of combined range. Never ever is it going to be so. :smiley:
```

---
## \#5 Posted by: NordeHQ Posted at: 2019-03-10T09:50:17.711Z Reads: 160

```
@murloc992 Thanks for your input. What is your range normally? 

I am waiting for more feedbacks like this to find parameters that fit everyone the best. For the time being, you may want to put the motor efficiency to 50% which may give you a good error margin.
```

---
## \#6 Posted by: murloc992 Posted at: 2019-03-10T09:52:31.376Z Reads: 149

```
As it is a dual pneumatics setup I expect no more than 30-40km if I hold 25km/h and never do some very fast accelerations. What is your loss constant for dual motors?
```

---
## \#7 Posted by: NordeHQ Posted at: 2019-03-10T12:37:14.569Z Reads: 138

```
I don't use a loss constant.
If you are interested in power calculation, here are the formulas that I used : 

 The process is first to calculate forces, then power, voltage, current and finally capacity.

During a ride, we will consider two steps:
* Acceleration phase
* Nominal phase (flat or slope)

__Force__
-

**Acceleration phase**

Let's consider the acceleration phase. 
We take into account three forces: 

_Rolling resistance: f_roll = f.m.g_

* f: friction coefficient for urethane on asphalt, f=0.015
* m: rider mass in kg
* g: acceleration of gravity, g=9.81m/s²

_Aerodynamic resistance: f_aero = 1/2.ρ.Sx.V²_

* ρ: air density ρ = 1,204 kg/m^3
* Sx: drag surface, for an average size rider I estimated Sx = 0.6m²
* V: average speed in m/s

_Inertia: F_ie = m.a_

* m: rider mass in kg
* a: acceleration in m/s²

The acceleration is expressed:

_Acceleration: a = V/t_start_

* V: average speed in m/s
* t_start: start time in s

_Total forces: F_acc = f_roll + f_aero + f_ie_

**Nominal phase on flat**

There are only two forces left:

_Rolling resistance: f_roll = f.m.g_

_Aerodynamic resistance: f_aero = 1/2.ρ.Sx.V²_

_Total forces: F_flat = f_roll + f_aero_

**Nominal phase on slope**

The weight is added: 

_Rolling resistance: f_roll = f.m.g.cos ∝_
* ∝ the gradient slope

_Aerodynamic resistance: f_aero = 1/2.ρ.Sx.V²_

_Weight: F_weight = m.g.sin∝_

_Total forces: F_slope = f_roll + f_aero + F_weight_

__Power__
-

To convert forces into mechanical power that applies on the wheel, we use: P_meca_wheel = F.V
* F: total forces in N
* V: average speed in m/s

To get the mechanical power that applies to the pulley motor, we use: 

_P_meca_motor = P_meca_wheel/µ_
* µ: efficiency of the drivetrain, for a pulley-belt setup we consider: µ=80%

Finally, the electrical power that needs to be provided to the motor is expressed:

_P_elec_motor = P_meca_motor/e_
* e: efficiency of the motor

Then, we calculate P_elec_acc, P_elec_flat, P_elec_slope for each phase. 

**Dual/Single**
If the setup is dual, we divided P_elec by two.

**Displayed power**
The displayed power is the max power among each power phases

**Voltage**
-
* For LiPo/Li-ion technology: _U=3.7V*S_, with S the number of cells
* For LiFePo4 technology: _U=3.2V*S_

**Current**
-

_I = P_elec/U_.
We get I_acc, I_flat, I_slope for each phase.

The average current is expressed:

 _I_avg = p.I_slope + (1-p).I_flat_
* p: percentage of route in slope. 

_p = d_slope/(d_slope+d_flat)=d_slope/d_total_
* d_flat: Range on flat road (flat distance)
* d_slope: Range on slope (climbing distance)
* d_total: Total distance

**Capacity**
-

_C = I_avg.t_
* t : travelling time

_t = V/d_total_
* V: average speed
* d: total distance
```

---
## \#8 Posted by: NordeHQ Posted at: 2019-03-10T12:38:19.722Z Reads: 106

```
I have just noticed that you said you are on pneumatics. I have integrated this yet. Calculations are made for urethane on asphalt.

I need more data for pneumatics setup, but I am working on it
```

---
## \#9 Posted by: murloc992 Posted at: 2019-03-10T13:15:32.311Z Reads: 99

```
Perfect dude. I would love to see the most science-inducing calculator around. Keep up the good work!
```

---
## \#10 Posted by: mmaner Posted at: 2019-03-10T15:22:59.112Z Reads: 96

```
You can use an efficiency modifier in your formula where thane is calculated at 90% and pnumatics are calculated at 75% (as an example). 

 Something like this...

Wh / 30 * efficiency % = range in Miles

Wh / 30 * 1.6 * efficiency % = range in KM

You can read more about it here...
https:///esk8-iq-the-math-and-the-science-of-electric-skateboarding-part-2/
```

---
## \#11 Posted by: NordeHQ Posted at: 2019-03-10T16:27:20.328Z Reads: 86

```
Thank you for your link. Yes, for the time being people could do something like that by moving the "motor efficiency" parameter, but I would like to find the coefficient of friction for pneumatics on asphalt. I will just change that and the total weight of (rider + board).

Just in case, because I think it is not obvious, but there is a second page with drivetrain calculation. You can navigate through the buttons on the left.
```

---
## \#13 Posted by: NordeHQ Posted at: 2019-03-19T23:49:30.277Z Reads: 60

```
The new version is online!

**[Calculator Update](https://norde.cc/calculator.php)**
--



Now you can use a mode to check what kind of performances you can except with your parts, and another one to choose your parts.

If you have any suggestion, let me know!
```

---
## \#14 Posted by: sofu Posted at: 2019-03-20T01:02:59.960Z Reads: 54

```
Is there an option to use imperial? Also is this supposed to happen or am I missing something?

![image|690x308](upload://nRHzlqX6W2vI7B44eZpQ5RQqjzP.png)
```

---
## \#15 Posted by: FranciscoV Posted at: 2019-03-20T03:44:51.456Z Reads: 45

```
@sofu Reverse Wheel and motor pulley
```

---
## \#16 Posted by: sofu Posted at: 2019-03-20T03:58:13.297Z Reads: 41

```
I'm dumb 🤦🏻‍♀️
```

---
## \#17 Posted by: NordeHQ Posted at: 2019-03-20T20:56:12.881Z Reads: 29

```
I can add imperial, but it will take me more time than the other updates. Do you need it for all the fields, or only for specific ones, like top speed?
```

---
## \#18 Posted by: sofu Posted at: 2019-03-20T22:34:49.898Z Reads: 29

```
i guess only specific ones like speed related stuff
```

---
## \#19 Posted by: Sn4pz Posted at: 2019-03-20T22:58:08.710Z Reads: 29

```
Torque would be cool :) 

Emtb folks like that stat, I would imagine
```

---
## \#20 Posted by: NordeHQ Posted at: 2019-03-22T02:12:21.051Z Reads: 26

```
Sure, I plan to add torque as soon as possible ;)
```

---
## \#21 Posted by: NordeHQ Posted at: 2019-03-30T21:36:45.278Z Reads: 16

```
New update: No torque or imperial, but I have added a **belt length** and a **battery** calculators: 

https://norde.cc/calculator.php

Also, for the power calculator, I have divided the battery capacity by 80%, since only 80% of a lithium battery is usable.
```

---
