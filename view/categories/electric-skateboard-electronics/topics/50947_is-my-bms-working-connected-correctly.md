# Is my BMS working - connected correctly?

### Replies: 7 Views: 571

## \#1 Posted by: Nekrydix Posted at: 2018-04-02T11:21:40.265Z Reads: 84

```
Hi Guys,

I have assembled my first battery and connected it with the balancer cables. Now I just wanted to charge the battery.
How do I know, if my bms is working on a preloaded battery. I preloaded every cell before point welding, thats why my 10s battery is preloaded. 

my setup: 10s4p samsung 30q battery
bms: 10s 20A bms for charge only

On my bms is no signal LED or comparable. 
Are there any voltages that I can measure during charging that tell me BMS is doing its job correctly?

And secondly, do i connected the BMS correctly for charge-only?
![20180402_124003|374x500](upload://6D5WyOYQIZhx73unEqJSM1jO2X2.jpg)

I want to build it according to this sketch:

![AdtkOc0|689x397](upload://21Jc797IFXMmEWA7OemqQEWtITy.jpg)

kind regards and happy easter
```

---
## \#2 Posted by: michaelcpg Posted at: 2018-04-02T12:01:50.092Z Reads: 71

```
That diagram doesn't look to be for a charge only BMS configuration. Also, why are you using such thin wires?
```

---
## \#3 Posted by: Nekrydix Posted at: 2018-04-02T12:06:32.462Z Reads: 66

```
The wires are only for testing. Later i will be using for battery connections 8-10 awg but for charge port you don't need such big wires if the voltage drop is lower than 3%.
```

---
## \#4 Posted by: rich Posted at: 2018-04-02T12:07:41.456Z Reads: 67

```
This diagram would be correct for a BMS for discharging, too where C- = charge and discharge (same port). But in your case that's a wrong sketch, give me some minutes to correct it.
```

---
## \#5 Posted by: michaelcpg Posted at: 2018-04-02T12:08:32.643Z Reads: 64

```
voltage drop isn't particularly relevant to wire size. The primary factor is current
```

---
## \#6 Posted by: rich Posted at: 2018-04-02T12:44:47.558Z Reads: 58

```
For charging 20AWG is totally fine. For Battery wires 12AWG (90A) should be enough, 8-10AWG is overkill and harder to solder. 

This is the corrected sketch how you should connect it for bypassing/charge only.

![sketch_bypassed|689x397](upload://iXmtG2p3UwJNtct2Xk0TxrLplcf.jpg)
```

---
## \#7 Posted by: Nekrydix Posted at: 2018-04-02T17:23:39.689Z Reads: 43

```
thanks for the corrected sketch :)

There are so many bypassing sketch's, that i got a little bit confused.
```

---
