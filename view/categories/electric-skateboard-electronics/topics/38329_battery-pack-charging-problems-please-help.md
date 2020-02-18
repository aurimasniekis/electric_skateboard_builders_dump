# Battery pack charging problems please help

### Replies: 11 Views: 613

## \#1 Posted by: nikoli280 Posted at: 2017-11-14T18:49:26.975Z Reads: 75

```
Hi i have made my battery pack of 50 LG HE4 batteries. I have them in a 10S 5P configuration ending up with max 42V and 12.5Ah.

I have a 10S 60A Suunpower BMS, which i have connected the right way to the pack. The battery leads reads the right values from 3.6V up to 36V

I have also bought a 42V 4A power supply, With a fuse.

I have the two connected via a XT-90 Anti Spark plugs.

My problem is that the pack wont charge.

The powersupply blinks when red to green indicating that the power is cut. I can measure it goes from around 4A to 0 and over and over again. So something is wrong.

I can press the XT90 connector half in and the power will flow constant with 1A. But then the XT90 will get hot, so i pulled it fast.

I can not seem to figure out what is wrong. I have bought and changed the BMS, no smoke or nothing comes from it. So i think it works. 

Can it be the resistor in the XT 90 that makes it work weird or what can i do?
```

---
## \#2 Posted by: Namasaki Posted at: 2017-11-14T18:55:47.183Z Reads: 70

```
I never heard of using an anti-spark connector to connect your charger to the battery. 
It may be messing with the charger's sensing circuit.
The charger negative to the bms P- pad
The charger positive straight to the battery positive
Usually, people wire a DC connector that matches the plug on the charger
```

---
## \#3 Posted by: nikoli280 Posted at: 2017-11-14T18:56:51.231Z Reads: 71

```
Its because the BMS uses same port for discharging and charging. Can it be why it got hot?
```

---
## \#4 Posted by: Acido Posted at: 2017-11-14T19:04:42.980Z Reads: 67

```
oh man my charger has some wierd port like an xlr but a lot smaller, would it work normally if i put an xt90 on there

https://banggood.com/EU-UK-DC-42V-2A-Power-Adapter-Supply-Plug-Battery-Charger-p-1159735.html
where can i buy one of these ports
```

---
## \#5 Posted by: nikoli280 Posted at: 2017-11-14T19:07:56.514Z Reads: 54

```
I just removed the plug and soldered a XT90
```

---
## \#6 Posted by: nikoli280 Posted at: 2017-11-14T20:13:01.844Z Reads: 44

```
Nope it was not that. What the hell can it be. I have changed the connector to XT60 to test.nothing changed.
```

---
## \#7 Posted by: Namasaki Posted at: 2017-11-14T21:26:28.327Z Reads: 41

```
Maybe the resistor is messing with your charger
```

---
## \#8 Posted by: Namasaki Posted at: 2017-11-14T21:29:24.739Z Reads: 42

```
I use the same 3 pin connector. 
It's the size of a CB mic plug.
```

---
## \#9 Posted by: nikoli280 Posted at: 2017-11-14T22:18:30.838Z Reads: 43

```
I changed the connector to a standard XT60 but the same problem persisted. What do i do wrong?
```

---
## \#10 Posted by: PXSS Posted at: 2017-11-14T22:20:39.327Z Reads: 43

```
Your XT90S is probably bad.
Did you replace it with an XT60 loop key?

Here is how I would troubleshoot it:

Bad XT90S Loop key:
Replace both connectors with new ones.

If problem persists then it's either, BMS or charger. 

Bad BMS:
Remove the BMS from in line, if the board charges fine then the BMS is the problem. 

If problem persists, then it's the charger. 

Bad charger:
Replace charger.

If problem persists, then there is something wrong with the battery. 

Bad Battery:
Check all voltages followed by welds and solder joints if it was DIY.
```

---
## \#11 Posted by: nikoli280 Posted at: 2017-12-05T18:51:03.134Z Reads: 30

```
Hi everyone, after months of waiting for new bms, then seeing that it was not a problem with the BMS. i bought a new charger and now it charges flawlessly. But weirdly enough with only 1 Amp but the charger is 2A
```

---
