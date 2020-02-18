# Help on Vesc settings

### Replies: 7 Views: 1905

## \#1 Posted by: mnelson3690 Posted at: 2017-02-20T21:10:13.295Z Reads: 245

```
Hi, I am new to E skating. I am trying to figure out good settings in the bldc tool for my setup. I have a vesc, 6374 motor, and 10s3p battery. Anything will help. I am confused on what amps I should use and volts
```

---
## \#2 Posted by: Namasaki Posted at: 2017-02-21T04:04:05.040Z Reads: 234

```
post screen shots of your current settings and lets go from there
Also we need to know more about your setup.
Motor KV in particular.
```

---
## \#3 Posted by: rpn314 Posted at: 2017-02-21T04:13:39.648Z Reads: 247

```
Make the max battery current limit be at least a little below what your battery can handle. I'd set your Voltage cutoff start to around 32 or 33 and the Voltage Cutoff End around 30 or 31. Higher if you want to get more longevity (life) out of your batteries, lower if you want to get a little more range per charge.
```

---
## \#4 Posted by: jaykup Posted at: 2017-02-21T15:14:46.458Z Reads: 229

```
For a 6374 motor:
**Motor max (amps)** = Watt rating of motor / nominal voltage of battery pack
3000 ish watts / (10s * 3.6v)
3000w / 36v = 83.33 amps so 80 amps would be max, but 60 might be good to start with. and still provide plenty of power.

**Motor Min** is braking force, -40 is fairly weak, -60 is a good braking level, -80 is very strong.

Battery Amps - How much the battery can output.  Assuming the battery was built using Samsung 25R 18650 cells, the [Datasheet](https://www.powerstream.com/p/INR18650-25R-datasheet.pdf) shows 20A max continuous discharge rate per cell.  10S3P is 3 cells in parallel, so 3*20A = 60A max battery discharge.  In practice you could go beyond this in pulses, but the VESC will overheat at some point anyway and reduce power with amperage over 35 for more than 1-2 minutes.  Don't worry too much about this, you only need 5-10 amps to maintain speed and acceleration time is short enough it all works out.  Big hills are really the only area where you will notice.

Max charge rate is 4A per cell, so 3P*4A=12A max charge rate.

Based on that info, your settings for the battery would be:

**Batt Max**: 60A
**Batt Min**: -12A

Battery Voltages:
Min Voltage = doesn't really matter?
Max Voltage = 43v (10s * 4.2v + 1v for bufffer)

For the battery cutoff start and end, lets take a look at the [Samsung 25R Battery discharge curves](https://www.e-cigarette-forum.com/forum/attachments/image-jpg.497865/)

Looks like at 10A (average consumption) around 3.2v is getting pretty close to empty, and 3.0v is very close to being empty.  The datasheet says it can go as low as 2.5v, but you would only gain maybe 5% capacity and permanently might lose 20%+ capacity over time compared to running down to 3.0v.  So 3.2v and 3.0v would be good numbers to help protect the battery pack and still provide long range.

Battery Cutoff Start = 10s * 3.2v = 32v
Battery Cutoff End = 10s * 3.0v = 30v

Finally, if you are running in BLDC mode, make sure you run motor detection, especially if you have a sensored motor.  You can also look into FOC mode but I'm running 12s and don't want to fry my VESC again so I'm not an expert on that.  Vedder has some [good tutorials](https://www.youtube.com/watch?v=bYYNbxPXNEU) on FOC setup and motor detection.
```

---
## \#5 Posted by: Jcullinan09 Posted at: 2018-04-28T01:40:30.789Z Reads: 119

```
Is this a fair evaluation of what to adjust BLDC settings to??

Given a **SINGLE** 6374 190kv motor: 
**Motor Max** = 60 amps
**Motor Min** = -60 amps
**Batt Max** = 60 amps
**Batt Min** = -12 amps

Given a **DUAL** 6374 190kv motor
**Motor Max** = 30 amps
**Motor Min** = -30 amps
**Batt Max** = 30 amps
**Batt Min** = -6 amps
```

---
## \#6 Posted by: yanggatang Posted at: 2019-01-07T04:45:31.385Z Reads: 56

```
I think only the battery max and min changes.
```

---
## \#7 Posted by: Jcullinan09 Posted at: 2019-01-07T06:48:57.063Z Reads: 53

```
Yeah, after learning a bit more about esk8 I’m pretty confident only battery limits change!
```

---
