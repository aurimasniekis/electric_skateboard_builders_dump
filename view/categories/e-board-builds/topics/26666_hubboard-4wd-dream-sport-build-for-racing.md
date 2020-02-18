# HubBoard 4WD, Dream Sport Build for Racing

### Replies: 9 Views: 1569

## \#1 Posted by: HubBoard Posted at: 2017-07-03T11:10:34.090Z Reads: 287

```
<img src="/uploads/db1493/original/3X/5/6/5669cf9a814c33203d81a95fc9e42e13ec9d3d9a.jpg" width="666" height="500">

Hello, everyone! So happy to see this great, conscious and smart builders in one place!

 I started my first electric skateboard project, and from the beginning it's ambitious.

I purchased a bamboo deck from company NAKED.
[Naked board-deck](http://www.euroskateshop.com/images/Naked-New-York-Longboard-4-p.JPG)

It gave me the look which I wanted to use, Sport, fast, low, and bamboo. I use it now to ride around.

I bought 4 engines from China, called W4 In Hub motors, probably same as DIY electric skateboard offers, or from a similar producer.

[In hub motor](http://www.dhgate.com/product/winning-w4-hub-motor-electric-skateboard/398945306.html#s1-0-1b;searl|2641409112)

They are Orange, 83mm wide, and looked good for the price. I got version 130KV. 

Now I ordered 4 VESC controllers from DIY electric skateboards, I decided to trust these ones as 4.12 is around for a while. I also get one of controllers and receiver offered on their shop.

While I wait for the parts I still didn't decide which battery I should use, I know it has to be (8S-10S) pack for the engines.

I might also use two batteries, one in front one in the back.

And here my question to you beloved Electric Skateboards Builders

Perhaps you have a better eye on battery market as so many things changes quite fast, what you recommend to consider? I'm familiar only with a hobbyking website.


I have plans for this Skateboard to be fast, I want to achieve around 40-45 km/h if possible, but I know distance will be the problem. I know 4 engines will not give this to me but I was thinking about programming front and rear differently, so back gives good acceleration, and front better speed. Is it possible? two batteries are not a problem to me as well as I don't care about weight.

I know about many difficulties that I will encounter with this build, but this is my hobby now and I can't wait to work on it.

Feel welcome to put my thoughts in place and I will be happy to hear any recommendations or ideas!
```

---
## \#2 Posted by: jaymu86 Posted at: 2017-07-03T16:48:01.516Z Reads: 231

```
Parked and can't wait for ride report
```

---
## \#3 Posted by: HubBoard Posted at: 2017-08-18T17:29:27.344Z Reads: 198

```
<img src="/uploads/db1493/original/3X/b/5/b5b7c7a8102ebcc50e62eb7e027dd0f9875b21e6.jpg" width="375" height="500">



Update 1

- I got 4 Vesc controllers, remote, and 2.4 receiver, and connectors.

- Currently searching for batteries for this setup. (8s-10s). Motor 1200 W (one), 130 KV. Single or double power supply.

- Also in need for adapter banana male 5mm (Vesc has female 5mm, got engines with 3.5mm)

- I added PS4 controller for size comparison for people who didn't see vesc size in real life (to me it was shockingly big)

Delimitations:

How to connect 4 Vesc, to control them under one remote controller? I have 4 engines.

Which batteries to use, one or two?
```

---
## \#4 Posted by: wmj259 Posted at: 2017-08-18T19:03:44.390Z Reads: 175

```
I am running a 3x3S lipo battery system on my build. I also have a 4.12 and a 192KV 6374 motor. 

Its better to use a 10S as thats the current "best" battery for the 4.12
```

---
## \#5 Posted by: HubBoard Posted at: 2018-04-23T07:50:24.938Z Reads: 145

```
Been a while out from the project, but now I am back!

Ordering battery now, any wonders about that company? Anyone worked with them? eskating.eu

I am considering 12s5p pack or 12s4p pack, I know bigger will be faster, but also heavier. Still I am pumped to go big and fast. Any thoughts on this one before I order it? After current research I found this option quite best/fast/comfortable as it comes with BMS, switch, and charging port.

https://eskating.eu/product/flat-12s5p-eskating-electric-skateboard-battery-samsung-30q/
```

---
## \#6 Posted by: HubBoard Posted at: 2018-07-04T19:37:55.804Z Reads: 121

```
The prototype is ready. I didn't manage to make 4WD yet ( I lost one screw for the engine) But, for now,
 2WD feels good enough. 
![36704860_1962291867154726_9039584682542366720_n|281x500](upload://oegqznECSPMGRFDVszAHkodewIP.jpg)
![36725261_1962291957154717_1780123649085276160_n|281x500](upload://ybfV2iuSVTJ8HrDxG4xFBE0p84d.jpg)

I made some test now, went throuh some crazy trips.

These are my settings I started with:
![2018-07-04|690x388](upload://e2ket1zLoSBlO0zOJ4wUmYGSgyG.png)

Sample Results (Approx 5km)
![36703690_1962291727154740_3146913166160560128_n|230x500](upload://9GGni5tsTbkhUMYkXuJMiZOzsbR.jpg)

Metr App once showed me max speed exactly 60 km/h, reliable? it felt crazy fast, I couldn,t go faster as wind gave me turbulences and shaking on the board. It's very low anyway and really feels made for speed, bummer is that I can only use flat surfaces, anything else destroys engines.

Right now I am fixing this *** engine, good i got 4 of them :joy:

My biggest current problem is my board suddenly stopped and I got VESC DRV8302 error

Any idea how can I start with esc problem?
```

---
## \#7 Posted by: Battosaii Posted at: 2018-07-04T19:57:04.382Z Reads: 95

```
DRV wizard unless you know how to change the DRV chip
```

---
## \#8 Posted by: HubBoard Posted at: 2018-07-07T10:53:00.857Z Reads: 85

```
The following faults were registered since start:

Fault            : FAULT_CODE_DRV
Current          : -0.3
Current filtered : -0.1
Voltage          : 47.46
Duty             : 0.001
RPM              : 149.8
Tacho            : 3
Cycles running   : 2
TIM duty         : 15
TIM val samp     : 2
TIM current samp : 4200
TIM top          : 16800
Comm step        : 6
Temperature      : 29.67
 
Fault            : FAULT_CODE_DRV
Current          : -0.5
Current filtered : -0.1
Voltage          : 47.46
Duty             : 0.001
RPM              : 143.5
Tacho            : 3
Cycles running   : 2
TIM duty         : 24
TIM val samp     : 2
TIM current samp : 4200
TIM top          : 16800
Comm step        : 6
Temperature      : 29.81
 
Fault            : FAULT_CODE_DRV
Current          : -1.0
Current filtered : -0.2
Voltage          : 47.45
Duty             : 0.003
RPM              : 151.7
Tacho            : 3
Cycles running   : 2
TIM duty         : 49
TIM val samp     : 2
TIM current samp : 4200
TIM top          : 16800
Comm step        : 6
Temperature      : 29.96
 
Fault            : FAULT_CODE_DRV
Current          : 0.1
Current filtered : 0.0
Voltage          : 47.46
Duty             : 0.003
RPM              : 151.3
Tacho            : 3
Cycles running   : 2
TIM duty         : 48
TIM val samp     : 2
TIM current samp : 4200
TIM top          : 16800
Comm step        : 6
Temperature      : 29.96
 
Fault            : FAULT_CODE_DRV
Current          : -0.2
Current filtered : -0.1
Voltage          : 47.45
Duty             : 0.004
RPM              : 150.1
Tacho            : 3
Cycles running   : 2
TIM duty         : 74
TIM val samp     : 2
TIM current samp : 4200
TIM top          : 16800
Comm step        : 6
Temperature      : 29.96
 
Fault            : FAULT_CODE_DRV
Current          : 0.4
Current filtered : 0.1
Voltage          : 47.45
Duty             : 0.006
RPM              : 154.9
Tacho            : 3
Cycles running   : 2
TIM duty         : 107
TIM val samp     : 2
TIM current samp : 4200
TIM top          : 16800
Comm step        : 6
Temperature      : 30.07


I got the faults on my vesc. I also can't run motor wizard to the end, it stucks on measuring R=0

I noticed my voltage hits 47v, I thought is should hold around 43v. 

Any ideas what is wrong in my setup? Now I consider FOCBOX to handle 12s battery better.
Best wishes
```

---
## \#9 Posted by: Lionpuncher Posted at: 2018-07-07T15:37:21.505Z Reads: 54

```
 Thats a blown drv. For sure. Depending on where you live, you can source somebody to fix it and replace the component. Or sell the vesc and get a new one.
```

---
