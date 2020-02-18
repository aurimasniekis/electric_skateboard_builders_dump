# Vesc 6 Cooling and Max current

### Replies: 13 Views: 1562

## \#1 Posted by: MaxMaker Posted at: 2018-07-15T20:19:14.095Z Reads: 269

```
Hi, so I am trying to use a VESC 6.4 for an electric hydrofoil. Tramps states that it can support 80A continiously and 120A in bursts. Is that RMS current, motor current or battery current? I would like to max out those values for propeller testing. What Firmware do I need to use and what max A values can I safely enter?

The VESC is mounted against a flat polished aluminium housing that sits in a water bath. So I think the cooling is as good as you could do it. 

Help is appreciated since I have no expereience with the VESC. 

The buildlog in case you want to find out more about this project. 
1. Building the surfboard: https://www.youtube.com/watch?v=3TprQ7l5RPE&t=181s
2. Installing the electrics: https://www.youtube.com/watch?v=DsI8MDyxjfE&t=4s
3. Here is the latest update: https://www.youtube.com/watch?v=iioH2H9dPZ4
```

---
## \#2 Posted by: BensonYong Posted at: 2018-07-16T09:50:24.557Z Reads: 237

```
I think 80A continiously mean Esc current,that is the motor current.
```

---
## \#3 Posted by: Kug3lis Posted at: 2018-07-16T10:07:47.421Z Reads: 239

```
From my experience with VESC that current is rated if you can keep case in low temperature, if it doesn't dissipate heat after several mins you will run into thermal cutoff :)
```

---
## \#4 Posted by: trampa Posted at: 2018-07-16T13:06:32.936Z Reads: 218

```
https://www.youtube.com/watch?v=1iwN5LGGM80

If you water cool your housing, 80A should be possible with ease. 
You can also load VESC FW without HW limits, to go above recommended settings.
Jens has been doing 120+A on an MTB.

Frank
```

---
## \#5 Posted by: Silverline Posted at: 2018-07-16T16:25:04.500Z Reads: 194

```
But is the 80amp, motor max current, or battery max current Mr. @trampa ??
```

---
## \#6 Posted by: DeathCookies Posted at: 2018-07-16T16:39:33.606Z Reads: 193

```
There is a difference between Motor max and battery Max. Battery Max should be only 60 continous. Can be Set higher because we dont achieve that **continously** but is safe at 60a.
Water cooled even more. 

Motor max can be even higher. It wont Pull more from the battery than the battery Max limit. The energy will just cycle between the Motor and the vesc mosfets. That is the reason why Motor a is always higher as battery a. 

Battery a = Motor a * duty
```

---
## \#7 Posted by: trampa Posted at: 2018-07-16T17:14:32.455Z Reads: 191

```
If you want to push 80a at full throttle (duty cycle) you need 80A battery max as setting. Otherwise the Vesc will reduce motor Amps to the Battery max value. If we say 80A, we mean 80A current flow towards the motor regardless of the battery max setting.
```

---
## \#8 Posted by: MaxMaker Posted at: 2018-07-17T12:07:22.904Z Reads: 200

```
Ok, thanks. What does duty cycle mean in this context? And what Firmware do I need?
```

---
## \#9 Posted by: trampa Posted at: 2018-07-17T20:08:07.986Z Reads: 190

```
Latest VESC-Tool and FW. Duty cycle (Arbeitszyklus) and the four different Amp settings are important to understand. 

Quick example: 
_Battery voltage 50V, Motor max 80A, Battery max 40A_

At 50% Duty cycle you can push 80A towards the motor while only 40A flow from the battery towards the VESC.
Reason: At 50% duty cycle the motor is operated at 25V (50% of 50V) and 80A = 2000W output
The battery delivers 50V at 40A =2000W

The VESC scales down the voltage and ups the Amps. **2000W Motor side  = 2000W Battery Side**

Once you surpass 50% duty cycle you can't push 80A towards the motor any longer. The Amp flow would be reduced by the VESC till your amp flow is limited to 40A at 100% duty cycle (40A x 50V 2000W). 
The higher "Motor Max" value will give you more power at slow speed, but will be reduced to "Battery Max" at high speed. This can be helpful when you want to go up a hill at slow speed.

So if you want to push 80A at 100% duty cycle (95% is realistic max), you also need to set battery max to 80A (80A x 50V= 4000W).

For braking it is similar, basically just reversed:
 _Battery 12S, 50V fully charged, Motor Max Regen = -40A , Batter Max Regen= -20A_

At high RPM your motor generates at high voltage (e.g. 50V). In this case the "Battery Max Regen" value determines the braking strength. 50V x -20A = -1000W braking power.
At slower speed the motor generates at lower voltage and the "Motor Max Regen" becomes more dominant.
25V x 40A =1000W braking power. Again, your VESC will scale up Voltage towards the battery and lower the Amps. The battery will see 50V and 20A while the motor generates at 25V and 40A.
Your "Battery Max Regen" is set to -20A and this will not be exceeded! The VESC will not allow the motor to generate more Amps at a certain Voltage (Watts) than you can push safely towards your battery at charging voltage (per your definition of "Battery Max Regen"). 
possible: **25V x-40A = 50V x -20A = -1000W**
not possible: **40Vx -40A = 50V x 32A = -1600W** (-32A exceeds -20A Battery Max Regen)
VESC will reduce to: **40V x -25A = 50V x -20A = -1000W**
Motor Amps will be reduced to **-25A** to meet the Battery Max Regen setting

Its pretty much the same thing as for acceleration, just reversed.

Duty Cycle impacts the Motor Voltage. 10% =5V, 20%=10V, .......... 100%=50V.
Amps will be scaled up or down to never exceed  the defined Battery or Motor settings (current control).

**What can you do wrong?**
If you set "Battery Max Regen" too low, you will have weak brakes at speed (since your motor generates at high voltage), which will get better the slower you get and the more the motor voltage drops (assuming that "Motor Max Regen" is set higher as in our example).
When do you need good brakes? At Speed! So check your Battery Max Regen to meet the desired braking strength. This is why you need a big Amp swallowing battery and why small battery packs don't work for good brakes.

Also note: **Symmetric settings** (Battery Max = Motor Max, Battery Regen = Motor Regen). will give you **perfect linear negative and positive acceleration.** No need for funky Watt control modes. The more asymmetric you go, the more you will experience a non linear response. Your battery has to be able to cope with the currents anyway if you want good brakes. You can't store the generated energy in the UNIVERSE.

Do the maths: 
Break strength at full RPM (speed) = Battery Charge Voltage (V) x Battery Max Regen (A) = **X Watt**
Max output power of the electrical System = Battery Voltage (V) x Battery Max (A) = **X Watts**.
Your Battery is usually the Bottleneck!
 
Frank
```

---
## \#10 Posted by: AndyBigD Posted at: 2018-07-18T09:01:44.098Z Reads: 156

```
The clearest description of Battery Amps Vs Motor Amps I've seen so far on this forum!
```

---
## \#11 Posted by: MaxMaker Posted at: 2018-07-18T16:49:52.919Z Reads: 154

```
Thank you. This is for a surfboard, so I don’t need brakes.  The water will absorb any energy. 

So my Batteries can theoretically supply 200A at 50V. I have a 120 A fuse and a 500A relay. I use 8AWG (8mm2) cables throughout. The VESC cables are the bottle neck with AWG 11 (4mm2). 

My motor is rated up to 42V. So I coud run it at 80% duty cycle. So I would input 100A max Motor current and 84A max Battery current. 
100A x 42V = 84A x 50V = 4200W
(Motor Side)= (Battery Side) 
**Is that right?**
```

---
## \#12 Posted by: trampa Posted at: 2018-07-19T12:50:39.731Z Reads: 136

```
Motors are not really voltage rated. You can push full voltage. The motor will be fine with 50V.
Higher voltage decreases Amp flow, which is a god thing.
The VESC cables can be shortened. Resistance is a matter of cable cross section and length!
If you have no brakes, fine.
You better have long motor cables and short battery cables. Long battery cables cause problems with inductance. If the cables get to long you might need to ad additional capacitors.

I would try to start with 80A motor current and 80A battery current. If you want to push 80A at max duty cycle you need 80A from the battery.
```

---
## \#13 Posted by: MaxMaker Posted at: 2018-07-21T17:49:13.271Z Reads: 119

```
It didn’t blow up so far!! I am quite relieved right now. 

Somehow the motor changes spin directions. My PWM signal goes from 1500-2000ms on my Arduino. 1500 is set at middle in the VESC since I don’t use reverse. 

http://www.youtube.com/watch?v=X2ChbSW-MLQ
```

---
