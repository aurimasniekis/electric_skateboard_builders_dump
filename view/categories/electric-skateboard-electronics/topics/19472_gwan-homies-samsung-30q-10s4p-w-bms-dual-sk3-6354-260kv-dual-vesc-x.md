# Gwan Homies &#124; Samsung 30Q - 10s4p w/ bms &#124; Dual SK3 - 6354-260kv &#124; Dual Vesc-x

### Replies: 16 Views: 1853

## \#1 Posted by: aras_96 Posted at: 2017-03-22T15:03:36.468Z Reads: 271

```
Fuck Everyone | Including Myself.

This is my First thread so please be patient with me.

..Hi? So this is my first thread and i would like some information and help if you're willing to give it. I'd like to build as fast of a longboard as i can, something that goes up to 30mph+.

So far i have purchased a few things, i'll list the most important.
- Longboard Deck.
- Caliber II Longboard Trucks, 50 Degrees.
- Orangatang Kegel 80mm Wheels.
- 30 Teeth HDT 5mm Pitch 11mm wide wheel pulley, 20 Teeth HDT 5mm Pitch 11mm wide motor pulley. The pulleys have already been drilled and connected to the wheels.
- Aluminium for my motor mount build, Which i plan to build myself.
- Transmitter and reciever. However i would like to build my own transmitter, so if you can like me a thread that teaches how to do that, that would be great.

I plan to create a 10S4P Samsung 30Q battery pack. Thus this will provide: 12,000mah | 60Amps.
I want to use this with dual Turnigy Aerodrive SK3 - 6354-260kv motors. Which will provide: a total of 4720w of max power, each motor will has a max load of 70a and can run between 8-10s. Dual Vesc-X ESC 

**What do you think about this setup and can you recommend me a bms that would be suitable for this setup and why it is.**

Thank you.
```

---
## \#2 Posted by: Lukas Posted at: 2017-03-22T15:14:20.082Z Reads: 256

```
If you use VESC, be careful with the 260 kv and 10s.
You'd need to set your ERPM limit to 60.000 in the VESC settings. (Don't know if the VESC-X can go higher).
I'd take some 6354 with 190kv. There are a lot of places where you can buy them.
Also the gearing seams a bit too low especially with that kv rating.
20:30 would give you a vmax of about 94 km/h according to http://www.elektro-skateboard.de/wiki/wissenswertes/strom-spannung-reichweite-vii

Most people use 36, 34 or 32 teeth on kegels and from 12 to 16 teeth on the motor pulley.
You can play a bit in the tool i linked you to get the best gearing for your needs.
```

---
## \#3 Posted by: mmaner Posted at: 2017-03-22T15:16:29.229Z Reads: 243

```
That motor KV is too high for the VESC...

    10 x 4.2 = 42v
    42v x 260kv = 10,920 RPM
    10,920 RPM x7 = 76,440  ERPM

The VESCy has an ERPM limit of 60k.  Check out this [thread](http://www.electric-skateboard.builders/t/choosing-the-right-motor-kv-for-the-vesc/3125).

Thats a strange gear setup, I dont think Ive ever seen it before.  Look at this [calculator](http://calc.esk8.it/#{"batt-type-lipo":0,"batt-cells":10,"motor-kv":260,"system-efficiency":75,"motor-pulley-teeth":20,"wheel-pulley-teeth":30,"wheel-size":80}|) for more info.

Use this BMS, its the best available and you can get it with an e-switch installed.
[Battery Protection Circuit Board (BMS/PCB/PCM) for 10S Cells 37V Li-ion and Li-Polymer Battery Packs
Part number: HCX-D223V1](http://www.bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html)
```

---
## \#4 Posted by: Maxid Posted at: 2017-03-22T15:36:27.070Z Reads: 213

```
42V at 60A is 2520W - that is the max Power your system can have (without adding in voltage sag). Not 4720W.
Still plenty - just don't fall in that marketing trap
```

---
## \#5 Posted by: aras_96 Posted at: 2017-03-22T15:46:21.863Z Reads: 205

```
Thanks for the reply, i guess i have no choice but to either reduce my battery voltage or go for that 190kv motor, which i will probably get from torqueboards.
```

---
## \#6 Posted by: aras_96 Posted at: 2017-03-22T15:47:08.937Z Reads: 203

```
Could you tell me how you got that calculation and why its like that, does that also mean that the top speed wont be as high?
```

---
## \#7 Posted by: aras_96 Posted at: 2017-03-22T15:48:59.246Z Reads: 195

```
yeah i've seen that BMS quite a lot on other threads, thanks for the recommendation, for the e-switch does that mean i can add a led push button, two the two wires without it getting damaged.

do you think if i went down to 190kv with the same gearing that it would be okay, as its under 60k erpm.
```

---
## \#8 Posted by: mmaner Posted at: 2017-03-22T15:54:45.547Z Reads: 194

```
You could probably use a push button, but its a 2 pole switch so no LED unless you use a step down converter to drive the LED.  

You should be OK with the gearing you have, I'd try it out and see what you think before I spent more money, especially since its already installed.  If you decide you don't like it buy new motor pulleys and print (or get printed) new wheel pulleys.  Pulleys are pretty inexpensive.
```

---
## \#9 Posted by: Maxid Posted at: 2017-03-22T17:01:01.575Z Reads: 189

```
The limiting factor is your battery.
It can safely output 60A. The maximum voltage it can have at 10S is 42V.
The current times the voltage is your power.

In real life you won't be using 42V because the battery will sag quite a lot to maybe 3.8 or 3.9 in the beginning.
this will reduce the actual power quite a bit.
However: 2000W on a skateboard is no joke and will simply cause you to street your face if not handled carefully.
Topspeed is mainly limited by voltage - not power.
If you want to go faster you need to up the voltage to 12S but that will also increase your ERPM. In your case you need to find a way to get to 60000erpm and then gear your system according to the speed you want.
```

---
## \#10 Posted by: NickTheDude Posted at: 2017-03-22T20:56:35.402Z Reads: 164

```
With a 20/30 ratio you don't need a super high ERPM to hit 30mph. A 190kV motor on 10S with that setup would easily get you to 30mph. Check out this calculator: http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":10,"motor-kv":190,"system-efficiency":80,"motor-pulley-teeth":20,"wheel-pulley-teeth":30,"wheel-size":83}|
```

---
## \#11 Posted by: lowGuido Posted at: 2017-03-23T00:38:41.587Z Reads: 153

```
[quote="aras_96, post:1, topic:19472"]
Fuck Everyone | Including Myself.
[/quote]

I laughed...
```

---
## \#12 Posted by: aras_96 Posted at: 2017-03-23T00:49:20.824Z Reads: 148

```
thats cute baby
```

---
## \#13 Posted by: aras_96 Posted at: 2017-03-23T14:58:49.067Z Reads: 142

```
So i have a total of 4 batterys that i could potentially use, initially i was going for samsung 30q but there is a lot of conflicting information. so i would like one final review by anyone thats willing to help

US18650 VTC5 2600mAh 30A : http://www.gearbest.com/batteries/pp_399867.html
INR18650 - 25R 2500mAh 20A : http://www.gearbest.com/batteries/pp_399862.html
HG2 3000mAh 20A : http://www.gearbest.com/batteries/pp_399870.html
INR18650 - 30Q 3000mAh 15A : http://www.gearbest.com/batteries/pp_399866.html

which is the best out of these, regardless of the price, and is there a better battery that i havent listed?
```

---
## \#14 Posted by: TarzanHBK Posted at: 2017-03-23T15:03:58.484Z Reads: 139

```
30Q is the way to go here ;)
```

---
## \#15 Posted by: Landshark Posted at: 2017-03-23T15:09:56.872Z Reads: 138

```
I'm curious as well...
```

---
## \#16 Posted by: Ryel Posted at: 2017-06-11T01:08:24.330Z Reads: 101

```
This is my first build and I'm interested in using dual SK3s as well. Would 2 190kv motors work well? I'm looking for a high top speed along will lots of torque to propel me up hills.
```

---
