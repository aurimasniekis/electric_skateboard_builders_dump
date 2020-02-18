# Any way to calibrate voltage and mAh used on Vesc6?

### Replies: 11 Views: 228

## \#1 Posted by: Silverline Posted at: 2019-08-02T23:11:52.569Z Reads: 79

```
Hallo

I have a friend which have a Trampa vesc 6 (the none + version) The problem is, that after newer firmware updates, his vesc is not reading the voltage and used mAh correct anymore.  This is pretty annoying.... Any way to calibrate these values in the vesc-tool ??

Thanks
```

---
## \#2 Posted by: Santino Posted at: 2019-08-03T02:24:51.947Z Reads: 75

```
Hi there, PM Frank from Trampa, I have Vesc6 and all readings are perfect with the new firmware.
```

---
## \#3 Posted by: Silverline Posted at: 2019-08-03T08:26:41.258Z Reads: 64

```
@trampa ?   
10char
```

---
## \#4 Posted by: trampa Posted at: 2019-08-03T10:20:30.718Z Reads: 59

```
Dual or single setup?
```

---
## \#5 Posted by: Silverline Posted at: 2019-08-03T12:30:59.802Z Reads: 54

```
Dual via can-bus. But i get the same wrong voltage reading via usb in the vesc-tool.
```

---
## \#6 Posted by: trampa Posted at: 2019-08-04T20:40:32.287Z Reads: 36

```
Probably he didn't hook up the remote and NRF dongle to the same VESC, or PPM remote is attached to the slave VESC. 
In that case you need to ad the battery values also to the slave VESC. 
PPM or any other input should be attached to the VESC you connect to during configuration. 
The additional values like battery capacity and cell number are not written onto both VESCs.
```

---
## \#7 Posted by: Silverline Posted at: 2019-08-04T21:35:58.090Z Reads: 34

```
The "beauty" of the new wizzard i guess ? But thanks...  I will check that Up.

But i'm pretty sure, even connected to the master vesc directly via usb, the vesc tool showing wrong voltage reading (about 1v )
```

---
## \#8 Posted by: trampa Posted at: 2019-08-05T17:01:32.433Z Reads: 34

```
1V / 12 Cells is 0.08V per cell. That is acceptable. 
The Shunts are +-1% precise, so there is always a tolerance in every VESC.
One shunt could have a plus tolerance, the other two minus tolerance...

Frank
```

---
## \#9 Posted by: Pimousse Posted at: 2019-08-05T17:07:13.463Z Reads: 30

```
[quote="trampa, post:8, topic:99624"]
The Shunts are ±1% precise
[/quote]
The voltage is not read by the shunts.
The shunts are used to measure currents.
```

---
## \#10 Posted by: Silverline Posted at: 2019-08-06T09:19:40.852Z Reads: 27

```
But both the "used current" is off, same for the voltage. When he was on a older fw, the vesc was precise.
```

---
## \#11 Posted by: trampa Posted at: 2019-08-06T10:18:21.999Z Reads: 25

```
We will dig into that. I'll need to chat with Benjamin about it.
```

---
