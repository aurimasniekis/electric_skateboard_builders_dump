# First Build, part lists and some confusions

### Replies: 5 Views: 215

## \#1 Posted by: Vinsanyon Posted at: 2019-05-17T06:51:37.509Z Reads: 94

```
Hi, guys,
I am planning to building a lightweight carving board as my first build.
Here are my part list:

Deck: Rayne flight v2 
Trucks: caliber 2
wheels: orangatang 85mm blue

ESC: Flipsky [Dual FSESC4.20 Plus ] (https://flipsky.net/products/dual-fsesc4-20-100a-plus-based-on-vesc-with-anodized-aluminum-heatsink?variant=22400696549436)
Remote: Flipsky vx1
Motor: Flipsky 6354 190v
Battery: 10s2p Ownboard pack

Motor Mount: [Boardnamics] (https://boardnamics.com/)
pulley/belts: Torque Board (any more budget-friendly choice here?)
ESC Enclosure: not sure yet

How does this setup looks?

Question here!!: 
_**_I was told that the battery pack or the BMS(which is 25A?not sure) inside can't work safely with 190 kV motor, I have no idea what's that mean._**_
what should I go for? Samsung 30q or Sanyo something? what is discharge current for the battery mean? Which spec of the battery affect board performance? I expectation is about 25miles/h and 10 miles of the range.

Thank you very much for any helps!
(non-native speaker, forgiving me for wired writing :))))
```

---
## \#2 Posted by: Vinsanyon Posted at: 2019-05-17T08:28:32.499Z Reads: 79

```
And what AMP and Volt of fuse do I need for the setup?
```

---
## \#3 Posted by: Dirt_Bag Posted at: 2019-05-17T15:08:23.937Z Reads: 57

```
He are some super cheap belts and pulleys, i have used the, numerous times with no problem

https://m.banggood.com/15mm-Wide-Belts-DIY-ABEC-Flywheel-Pulley-Kit-265mm-255mm-p-1222305.html?rmmds=search
```

---
## \#4 Posted by: Jinra Posted at: 2019-05-17T15:23:25.054Z Reads: 52

```
It would work, but you'd be limited by the BMS that onboard uses which is probably set to about 25-30 amps. The cells themselves (depending which one the pack uses) can probably only discharge 30-40 amps anyway. But if you set your VESC settings to 25-30 amps you should be fine. You can bypass the BMS by resoldering the discharge wires if you want to remove the BMS limiter.

You should probably get a better pack like the meepo 40T pack (60a cell discharge, unsure about BMS) if you want to keep it 10s2p.
```

---
## \#5 Posted by: Vinsanyon Posted at: 2019-05-17T23:02:16.286Z Reads: 32

```
Thank you! Help a lot!
```

---
