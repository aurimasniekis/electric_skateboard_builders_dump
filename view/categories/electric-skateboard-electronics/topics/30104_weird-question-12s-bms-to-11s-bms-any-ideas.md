# Weird Question: 12s BMS to 11s BMS, Any Ideas?

### Replies: 8 Views: 808

## \#1 Posted by: nmiller14 Posted at: 2017-08-08T19:54:38.703Z Reads: 96

```

For my build I bought a 12s BMS( I orignally planned to do a 12s system)
After specking my motor out I decided  stay below the 60,000 erpm's so I would prefer to just run an 11s system.
Any ideas on how to pull that off?
Hardware
-11 5000mah 1s batteries
-44V 48V 50.4V 12S 60A Lithium ion Li-ion LiPo Li-Polymer Battery BMS PCB System

Could I possibly just wire in a small resistor and make a "12th dummy battery", I have no idea.
Anyways any help would be much appreciated. Thanks
```

---
## \#2 Posted by: willpark16 Posted at: 2017-08-08T20:03:35.955Z Reads: 93

```
Would not reccomenD it better off selling the bms and getting the proper one
```

---
## \#3 Posted by: flywithgriff Posted at: 2017-08-08T20:04:35.556Z Reads: 92

```
Not possible. Just run a 12a system and limit erpm in the vesc setrings.
```

---
## \#4 Posted by: nmiller14 Posted at: 2017-08-08T20:12:47.016Z Reads: 87

```
Will do. The reason I wanted to drop to 11s was to physically limit the erpms. If I limit it in just the vesc settings what kind of risk am I running?
```

---
## \#5 Posted by: flywithgriff Posted at: 2017-08-08T20:34:49.496Z Reads: 79

```
None as long as you set it
 correctly.
```

---
## \#6 Posted by: nmiller14 Posted at: 2017-08-08T20:36:23.820Z Reads: 76

```
perfect. Thanks for your input
```

---
## \#7 Posted by: Namasaki Posted at: 2017-08-09T20:04:01.278Z Reads: 62

```
Turn off the " Limit ERPM with negative torque
And set limits to -60k and 60k
You'll likely not exceed 60k anyway unless your flying down a long steep mountain road or turning your board upside down and pulling the throttle
```

---
## \#8 Posted by: Slak Posted at: 2018-05-25T15:23:20.035Z Reads: 37

```
@nmiller14 : Read this old thread, it's interesting and can help you ;)

https://www.electric-skateboard.builders/t/bms-hunting-no-more/49040
```

---
