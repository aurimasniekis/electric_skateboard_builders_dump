# How do i know that my board is done charging

### Replies: 6 Views: 194

## \#1 Posted by: KrisKraanen Posted at: 2019-02-12T23:42:45.937Z Reads: 78

```
hi fellow builders, i have this bms https://www.electric-skateboard.builders/t/new-ip67-rated-bms/57782/42 8s version and this style charger
https://www.banggood.com/AC-110-or-220V-to-DC-0-60V-8A-480W-Adjustable-Regulated-Switch-Power-Supply-Driver-Transformer-for-LED-Strips--p-1323728.html?rmmds=myorder&cur_warehouse=CN 

when do i know my board is fully charged....?
```

---
## \#2 Posted by: evoheyax Posted at: 2019-02-12T23:46:19.236Z Reads: 75

```
By checking the voltage. With that guy, you should use a wattsup watt meter in between the charger and your battery.

Are you sure your bms though can take 8a input? The issue with thw ones without adjustable voltage is they will always pull max amps when charging a battery, and that will break them.
```

---
## \#3 Posted by: KrisKraanen Posted at: 2019-02-12T23:57:28.069Z Reads: 65

```
yes its specified 8 amp
```

---
## \#4 Posted by: KrisKraanen Posted at: 2019-02-13T00:01:19.871Z Reads: 56

```
wattmeter to find when its done charging?
like to see what the voltage it is at?
```

---
## \#5 Posted by: wafflejock Posted at: 2019-02-13T00:16:01.055Z Reads: 50

```
Yes check the battery voltage, take your number of cells in series multiply by 4.2 and that's your max charge voltage, if the voltage is below that you aren't done charging.  You can also compute the charge time if you know the battery capacity (Ah, for example 10Ah) and you know the charge rate (in Amps lets say it's 8A) then you can take the capacity and divide by charge rate 10Ah/8A = 1.25hrs to charge (add some more time for cells to balance out along the way but this is best case scenario, no extra time bleeding off power or refilling and assuming 0 charge to start).  Same thing works in Wh and with Watts but then need to include voltage on both sides too so it sort of cancels out in this case, but yah if you have 185Wh battery and 100W charger (actually charging at this wattage) it's 1.85hrs to charge.  There are little Watt meters you can get for boat batteries apparently and other similar ones from a company called "drok" that I used in the past as a simple on board meter for how much juice I had left but have since replaced with the metr bluetooth module and app (also gives you this info).

---

Personally use a balance charger instead of the BMS+random power supply setup for charging still not convinced switching things and carrying my charge circuit with me everywhere is a good idea.
```

---
## \#6 Posted by: deucesdown Posted at: 2019-02-13T00:49:15.457Z Reads: 37

```
The standard for lithium ion charging is CC/CV with C/10 termination.

The first thing you need to know is if your PSU is "constant current". I believe there are 3 possible behaviorswhen a load like a battery pack is connected:
- hold max amps by controlling voltage (constant current)
- trip a protection circuit when max current is reached. I bought a psu similar to the one you linked, with a current knob, that does this :(
- brown out and/or make a fire

If you have a cc psu with adjustable voltage, that's pretty close to cc/cv. Full would be indicated by the voltage reaching 8x4.2v, and the current hitting max charge rate divided by 10 (0.8a for your psu). you need a way to measure this.
```

---
