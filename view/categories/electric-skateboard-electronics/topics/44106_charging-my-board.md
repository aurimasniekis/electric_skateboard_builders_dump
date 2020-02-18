# Charging My Board

### Replies: 6 Views: 636

## \#1 Posted by: butt_stallion Posted at: 2018-01-19T14:24:51.521Z Reads: 113

```
I have a 10s3p battery that I am going to build with a BMS.  There will be an antispark switch in the system.  Do I need two connectors coming from the BMS, one for charging and one for the esc?  When I do charge the battery can I just simply unplug the antispark and then charge it or do I need to disconnect the ESC as well?

Thanks for the help
```

---
## \#2 Posted by: UniqueSnowflakeN27 Posted at: 2018-01-19T19:00:08.453Z Reads: 85

```
Yes, there is seperate wires for the battery and for the ESC. Look at your wiring schematic for the BMS and I’m sure you’ll understand.
```

---
## \#3 Posted by: butt_stallion Posted at: 2018-01-26T14:14:48.994Z Reads: 47

```
The schematic my BMS came with says the charging port and discharge port are the same positive port.  Does this mean I only need one wire for charging and for the ESC?  For some reason this is confusing me, I don't want to mess it up.

![0126180910|690x388](upload://A3FqtvGxnHHoxvlQefDmYxJ083I.jpg)
```

---
## \#4 Posted by: chomp Posted at: 2018-01-26T17:54:29.897Z Reads: 37

```
My bms, 10s2p is wired with one male xt60. I use that to plug into esc when riding and when I charge I unplug the esc and plug the battery xt60 into the charger. I can snap a pic later if you need. Lmk.
```

---
## \#5 Posted by: butt_stallion Posted at: 2018-01-26T19:05:24.645Z Reads: 34

```
A picture would be awesome!  Thank you!
```

---
## \#6 Posted by: chomp Posted at: 2018-01-26T19:21:09.630Z Reads: 31

```
![IMG_20180126_102315|374x500](upload://6esCrWeNIeFfwWuYqE0qvWq1aKD.jpg)

The chain is:
42v 2a charger -> antispark -> watt meter -> battery. 

Watt meter is nice because it shows the current volts and amps too. I'm running a kitchen thermometer probe to watch temp since this is the first time charging the pack. To sum it up though, you can just have one plug on your battery and then plug the battery to the charger or your esc.

Also, I bet if you check continuity with a multimeter you'll see that all negatives are connected. Hopefully this clears it up.
```

---
