# Auxiliary Lipo battery anti voltage sag project

### Replies: 13 Views: 591

## \#1 Posted by: ranes Posted at: 2018-07-19T09:07:32.667Z Reads: 142

```
Hi,

My board is Meepo v1.5 and as soon as I climb hills, the board bips (voltage sag) and some power is lost even if battery level is 80%. Once flat road reached, all is ok and autonomy could be 10 km.
I would like to know  what do you think about this project :
![image|690x493](upload://1saFnswzrm937X3bHG2TPU5d4a1.png)

Goal of post and details :
A) Prevent frequent voltage sag on 10S2P original battery AND still using it.
B) Recycle owned Lipo 4S1P 5000mAh @ 30C in order to "help" original battery.
C) I plan to limit output StepUp current to 7A. Input current will be around 21A vs 30A max (37V/15V = 2.5 with 75% efficiency, so ratio = 3).
D) Only BT1 BT2 and BT3 will be measured. Software substracts will deduce BT4 voltage.
E) DC-DC Step-Up 1500W is the following (I know Joules lost will occur but I wish to use my unused Lipo) : 
![image|314x237](upload://eXqSBfkRpD50Yk2CYc0hAVWuLUH.jpg)
F) Fan and radiator will not be used because aluminium box will act as a radiator.
G) Q3 reference is not the right one. I will use a MOSFET matching VgsTh=-2~-4V, RDSon<0.01 ohm, VgsMax=+-20V, IDSnom>40A
H) As soon as BT0 (10S2P) < 36V (3.6V per cell), Aux battery is plug in parallel during for example 10 seconds.
J) I've a doubt concerning StepUp module insertion in my electronic scheme. Needs some in/out capacitances, what about D1 Schottky, ... ?

Many thanks in advance
```

---
## \#2 Posted by: TarzanHBK Posted at: 2018-07-19T09:16:57.293Z Reads: 129

```
Normally we eliminate sag by simply using a better battery, but i like your idea - i think noone has ever thought of an Anti-Voltage-Sag-device before :grin:
It´s interesting to see this as a proof of concept device; i think in realworld it´s just more practical to get a new battery! Check how big and how heavy and how pricy your device will be.
```

---
## \#3 Posted by: Kug3lis Posted at: 2018-07-19T09:25:13.210Z Reads: 125

```
Step up module will not produce the same voltage as battery runs, also step up is switched power supply and the main thing why this would not work is that you will be charging battery not helping it... as the current would flow to  battery
```

---
## \#4 Posted by: E1Allen Posted at: 2018-07-19T11:21:53.183Z Reads: 108

```
[quote="Kug3lis, post:3, topic:62274"]
charging battery not helping it… as the current would flow to battery
[/quote]

That would still help though.  If the battery is charging the pack voltage increases so less sag?

For this project I'd probably get a better battery to start with.  However this proof of concept would be cool.
```

---
## \#5 Posted by: pat.speed Posted at: 2018-07-19T11:45:40.547Z Reads: 103

```
Erm not quite how it works, as the battery needs to power the circuit to charge its self. Basically you’re drawing more current from the battery increasing sag, then putting some back into but not as much as was drawn as the efficiency isn’t 100%
```

---
## \#6 Posted by: Kug3lis Posted at: 2018-07-19T12:14:11.259Z Reads: 98

```
Also the diode after step up will drop voltage so your injecting voltage will be lower than battery
```

---
## \#7 Posted by: ranes Posted at: 2018-07-19T13:02:30.984Z Reads: 86

```
[quote="TarzanHBK, post:2, topic:62274, full:true"]
Check how big and how heavy and how pricy your device will be.
[/quote]
Aux Lipo batt is 450 g weight and don't know for StepUp but can estimate to 250g. Total for about 750g. Price question is not applicable because I already have batteries with dust on the top ;-)
Concerning the StepUp, it's about 20$ and I estimate 15$ for other components.
[quote="Kug3lis, post:3, topic:62274, full:true"]
Step up module will not produce the same voltage as battery runs, also step up is switched power supply and the main thing why this would not work is that you will be charging battery not helping it... as the current would flow to  battery
[/quote]
The voltage of StepUp is adjustable and it's one of my question. What's the best voltage of StepUp ?
The goal of Arduino Pro Mini is to **activate or deactivate in real time the StepUp module**, permanetly sampling the main battery voltage.
When ESC is not consuming, you're right : Aux batt will charge the Main batt. The ideal is to disconnect Aux batt with Q3.
But when (V)ESC is asking for power (around 15A-20A), if 2 batteries are plugged in parallel, I think the internal resistance of VESC is very lower than the Main and Aux batteries. In this case, current will flow from Main AND Aux batteries to ESC, isn't it ?
[quote="pat.speed, post:5, topic:62274, full:true"]
Erm not quite how it works, as the battery needs to power the circuit to charge its self. Basically you’re drawing more current from the battery increasing sag, then putting some back into but not as much as was drawn as the efficiency isn’t 100%
[/quote]
Not sure about you means but Aux batt are 30C. This means they can theorically give 150A. Even if it's bad quality, 15C is 75A and I only need 21A (even 10A will be enough I think, I will adjust). Of course the goal is to plug in parallel Aux batt to Main only when voltage sag is present. When Main batt has enough voltage, Aux will never be plugged in parallel with Main batt. This is the job of Q2 driver.
[quote="Kug3lis, post:6, topic:62274, full:true"]
Also the diode after step up will drop voltage so your injecting voltage will be lower than battery
[/quote]
I think StepUp already have such a diode at output level (I've not yet received this StepUp from China).
In case D1 has to be present, the StepUp is adjustable. I can compensate this drop voltage, no ?
```

---
## \#8 Posted by: pat.speed Posted at: 2018-07-19T21:46:58.205Z Reads: 50

```
My bad I didn’t realise you were going to use another separate battery. What sort of power are you expecting to get out of this? I use something similar for charging my batteries normally and at 12v I can get out about 50.4v at 1.8a and when I crank the source voltage upto 24v then I can push about 5amps through it. With those number I doubt this will help eliminate voltage sag
```

---
## \#9 Posted by: b264 Posted at: 2018-07-19T22:13:44.119Z Reads: 48

```
One HUGE capacitor or super-capacitor on the ESC could do the same thing, but the main problem here is starting with low-quality stuff for money-saving reasons.  There are good reasons it's cheap.  You can pick any two: good, cheap, fast.  Meepo is fast and cheap.

Such a large cap would require robust anti-spark measures to prevent overdrawing the battery while filling the cap...
```

---
## \#10 Posted by: ranes Posted at: 2018-07-20T07:09:03.876Z Reads: 30

```
As the Aux Batt is 15V 5A 30C it's theorically 2200W. Even if we divide this by 3 for example, it's 733W. The 1500W DC StepUp can handle 30A. As I already said, output power of Aux batteries will be 15A at 37V = 550W minus 55W (90% efficiency) = 495W available for ESC when max power consumption of dual motors is 864W (don't forget Main batt is still there in parallel)
```

---
## \#11 Posted by: pat.speed Posted at: 2018-07-20T07:13:21.371Z Reads: 28

```
I am aware of how it works theoretically but with my own real world experience using a similar set up, I didn’t get the expected results, meaning I needed a higher voltage power source.

Edit: How about I test this for you as I already have the parts on hand, could you just tell me the output voltage of the converter you want and the input power from the second battery
```

---
## \#12 Posted by: ranes Posted at: 2018-07-20T07:37:14.293Z Reads: 26

```
Output voltage of converter from Aux batt is planned to be 37V. Input power from Aux batt is Lipo 4S1P at 5000mAh and theorically can deliver 2200Wh but real consumption will have to be measured as the expected output current will be limited to 10 or 15A max...
Many thanks for your help.
```

---
## \#13 Posted by: pat.speed Posted at: 2018-07-20T07:59:46.079Z Reads: 22

```
No worries, I’ll try and do it tomorrow. If I don’t get back to you in a day or two just let me know because I probably forgot...I forget a lot of stuff :(
```

---
