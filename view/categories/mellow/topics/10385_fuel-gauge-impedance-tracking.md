# Fuel gauge: impedance tracking

### Replies: 5 Views: 1356

## \#1 Posted by: Mellow Posted at: 2016-09-29T22:38:00.662Z Reads: 127

```
Forum search didn't return much in the way of measuring battery capacity more accurately than voltage readings, so we thought we'd drop this video here. Skip to 17:00 to see a description of how a few pre-builts we've seen on the market act like.

https://www.youtube.com/watch?v=p54wVWxFZ6Q

Anyone else out there using this, or counting coulombs?
```

---
## \#2 Posted by: Pantologist Posted at: 2016-09-30T02:28:15.799Z Reads: 99

```
I'm not positive if @Jtag 's BMS does that exactly or not. It does something more accurate than just voltage I am pretty sure. 

http://www.electric-skateboard.builders/t/diy-6s-to-12s-bms-with-can/2639
```

---
## \#3 Posted by: JTAG Posted at: 2016-09-30T08:49:55.448Z Reads: 87

```
Yes it measures battery voltage (pack and individual cells) and current. For now the software is in such a state that safe charging and discharging is possible. In the following weeks ill look into SOC and SOH determination.
```

---
## \#4 Posted by: Mellow Posted at: 2016-09-30T10:15:02.987Z Reads: 82

```
Thanks for the link to the DieBieMS. Just got caught up with the design and development via JTAG's thread. Literally history in the making, fresh brewed from our neighbors to the north! (We thought the name was German first, but looked a bit further.)

Was there an offline discussion with @Pedrodemio about the fuel gauge algorithm?
```

---
## \#5 Posted by: SimosMCmuffin Posted at: 2016-09-30T11:04:52.134Z Reads: 70

```
I was planning to prototype my team's BMS with TI's BQ769x0-series IC, which does coulomb counting. AKA has a shunt resistor and the IC then iterates the measured current (4 samples per second) to update the coulomb counter. The used capacity can then be fetched by I2C protocol from the internal register by an external MCU, so it doesn't add much processing time to the main MCU.
http://www.ti.com/lit/ds/symlink/bq76930.pdf

Using only the voltage is very... foolish way to figure out how much capacity is left in the battery. With high load the under voltage protection (UVP) will be tripped prematurely, due to voltage droop (cell's internal losses) over the cells, but then you might damage the battery if you lower your UVP voltage, but have a light load.

We might add a standalone fuel gauge from TI later to enhance the accuracy of the capacity measurement and use the BQ769x0 to just balance cells and control charge and discharge fets.
```

---
