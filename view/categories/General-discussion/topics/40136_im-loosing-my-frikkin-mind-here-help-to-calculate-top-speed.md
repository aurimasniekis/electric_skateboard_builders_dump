# Im loosing my frikkin mind here! Help to calculate top speed

### Replies: 9 Views: 613

## \#1 Posted by: mmaner Posted at: 2017-12-04T20:53:34.638Z Reads: 157

```
I dont know what Im missing but I've been trying to figure this out for half a day.

To calculate top speed I would normally calculate the RPM (MAX Voltage * KV = RPM), then calculate the Gear Ratio (wheel pulley teeth / motor pulley teeth = Gear Ratio) and finally Max Speed (RPM * Gear Ratio * Wheel Size =  MM/Min converted to MPH by Result * 1 mm/min 0.000037 = mph).  But Im getting crazy values...

RPM
MAX Voltage * KV = RPM
36V * 208KV = 7488 RPM

GEAR RATIO
wheel pulley teeth / motor pulley teeth = Gear Ratio
60 / 15 = 4:1

MAX SPEED
RPM * Gear Ratio * Wheel Size  >>  MM/Min convert to MPH
7488RPM * 4 * 150 = 4492800 MM/Min
4492800 MM/Min * 0.000037 = 166.2336 MPH

Somebody point out where I went wrong as I've lost my original notes and have googled my ass off today.  thanks
```

---
## \#2 Posted by: MysticalDork Posted at: 2017-12-04T20:57:11.727Z Reads: 152

```
You've got your gear ratio backwards. It should be 1:4 or 0.25. the 4:1 would be if you had the 60t on the motor and the 15t on the wheel.
```

---
## \#3 Posted by: pennyboard Posted at: 2017-12-04T20:57:44.463Z Reads: 145

```
When I run it, I get 33 mph. I think @MysticalDork is right, your ratio is flipped
```

---
## \#4 Posted by: Colson003 Posted at: 2017-12-04T21:01:17.974Z Reads: 143

```
[quote="mmaner, post:1, topic:40136"]
7488RPM * 4 * 150 = 4492800 MM/Min
[/quote]
7488RPM / 4 * 150 = 280,000 MM/Min
But if 150 is the diameter then 150 times pi = 471.23mm. 
7488 / 4 = 1872RPM * 471.23mm = 882,142.56mm/min
882,142.56 * 0.00037 = 32.6MPH
```

---
## \#5 Posted by: aponty Posted at: 2017-12-04T21:20:37.291Z Reads: 129

```
http://calc.esk8.it/#{"batt-type-lipo":0,"batt-cells":10,"motor-kv":208,"system-efficiency":85,"motor-pulley-teeth":15,"wheel-pulley-teeth":60,"wheel-size":150}|

says 28mph (rounded) after efficiency considerations
```

---
## \#6 Posted by: mmaner Posted at: 2017-12-04T21:40:35.126Z Reads: 108

```
[quote="Colson003, post:4, topic:40136"]
7488RPM / 4 * 150 = 280,000 MM/Min
But if 150 is the diameter then 150 times pi = 471.23mm. 
7488 / 4 = 1872RPM * 471.23mm = 882,142.56mm/min
882,142.56 * 0.00037 = 32.6MPH
[/quote]

That was fuggin epic, I just had a braingasm, it now makes so much more sense than it did before.  I always got numbers pretty close to what I expected so I didn't question it until I tried to automate the calculations in Excel.  Even then it was mostly where it should be unless I used a crazy gear ratio.  Using the wheel circumference to calculate the MM/Min was genius.

For anyone else trying to understand the math behind this calculation, here ya go...

    **MAX SPEED**

    Wheel Size * PI = Wheel Circumference
    Motor RPM / Gear Ratio = Wheel RPM * Wheel Circumference = MM/Min * 0.000037 = Max MPH

    150mm * PI = 471.23mm Circumference
    7488RPM / 4 = 1872 Wheel RPM * 471.23mm Circumference = 882159.22  * 0.000037 = 32.64 MPH
```

---
## \#7 Posted by: FredrikHems Posted at: 2017-12-04T21:40:54.351Z Reads: 85

```
The way i do it:

36v * 208kv = 7488 - this is the max motor rpm

7488 : 4 = 1872 - this is the Max wheel rpm

150mm/wheel size * 3,14 = 471mm - this is the distance you will move per rotation of the wheel, in mm.

1872 * 471mm = 881 712 mm per min. This equals to 881.712 meter per min. 

881.712 * 60 = 52 902,72 meter per hour. - This equals to 52.90272 km/h.

So If you have a Max voltage of 36v (bit strange), a motor with 208kv, 1:4 gearing and 150mm wheels; then 52 km/h will be your theoretical max speed
```

---
## \#8 Posted by: mmaner Posted at: 2017-12-04T21:43:26.109Z Reads: 80

```
Not much different than what @Colson003 showed but I appreciate the finesse.   

[quote="FredrikHems, post:7, topic:40136"]
If you have a Max voltage of 36v (bit strange)
[/quote]

I was using Nominal Voltage, still working on finalizing all of these formulas as I haven't been getting reliable values.

Thanks for the help.
```

---
## \#9 Posted by: PXSS Posted at: 2017-12-04T23:21:01.125Z Reads: 63

```
Let me put it in a cleaner manner for others looking....


---

Voltage x motor kv = revolutions per minute (RPM)

Number of motor pulley teeth / number of wheel pulley teeth = gear ratio (GR)

RPM x GR = Wheel RPM

Wheel diameter (in mm) x pi = wheel circumference (in mm)

Wheel Circumference x Wheel RPM = Distance traveled (in mm) per minute (DPM)

To convert to kilometer/hour:
DPM * 60 / 1,000,000

To convert to miles/hour:
DPM * 60 / 1,609,344
```

---
