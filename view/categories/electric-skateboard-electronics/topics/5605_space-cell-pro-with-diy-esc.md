# Space Cell Pro with DIY ESC

### Replies: 12 Views: 1030

## \#1 Posted by: roonydagoony Posted at: 2016-07-05T18:04:56.516Z Reads: 142

```
Hi,

I currently have DIY's Electric Skateboard Motor 6374 230KV 3200W with the TorqueBoards 12S 120A Car ESC with a 6S lipo battery. (Works beautifully)

I want to use Enertion's SPACE CELL 3 PRO enclosure/battery pack with my mechanics/esc

I was wondering if there are any limitations or compatibility issues (I already have a bunch of xt60 to 5.5mm male and female adapters for connections, so no issues there)

Thanks,
-Roony
```

---
## \#2 Posted by: Namasaki Posted at: 2016-07-06T04:42:51.621Z Reads: 118

```
You should be fine with the space cell 3 pro. I believe has a 40a fuse and at 10s you should be well below 40a pull.
Matter a fact I have run dual 6355 230kv motors total over 5000watts on 6s going full throttle uphill 10%grade and still didn't break 40a.
Well, rider weight does matter. I was 185lbs
```

---
## \#3 Posted by: roonydagoony Posted at: 2016-07-06T13:23:09.855Z Reads: 89

```
that is beautiful to hear
thank you
```

---
## \#4 Posted by: chaka Posted at: 2016-07-06T13:44:12.617Z Reads: 85

```
You will probably have a few issues trying to run a hobby RC type speed controller with the bms on the space cell. Really need a vesc to be able to keep the amp draw and braking current within spec of the bms. This really depends on your riding style, an aggressive rider will pull a lot more power than a casual rider so if you keep you gear ratio low and take it easy on acceleration you may not have any problems.
```

---
## \#5 Posted by: roonydagoony Posted at: 2016-07-06T14:18:43.065Z Reads: 78

```
My ration is 16/36
weight 185 lbs
speed controller is from DIYElectricSkateboard
and medium-to-aggressive style

any issues with this?
```

---
## \#6 Posted by: chaka Posted at: 2016-07-06T14:24:17.306Z Reads: 72

```
Its 50/50, personally I use a bms with a 90amp over-current protection on 10s and I can trip it if I set my VESC too high. On a full charge you will trip the overvoltage when applying the brakes if you have no way of controlling your regen current and voltage limit.
```

---
## \#7 Posted by: evoheyax Posted at: 2016-07-06T14:45:28.640Z Reads: 71

```
And this is why the VESC is killer, but doesn't the DIY esc have limit controls also? I thought those guys were pricy, unless I'm confusing it with another esc...
```

---
## \#8 Posted by: roonydagoony Posted at: 2016-07-06T14:57:18.840Z Reads: 67

```
You're right, a little pricy. But I already have one so I'm trying to use it with my space cell
```

---
## \#9 Posted by: evoheyax Posted at: 2016-07-06T15:02:37.428Z Reads: 64

```
Personally, I have issues with low amps, and find you want 100 amps continuous max on the battery side. This is why the space cell was very disappointing for me. I nodded mine so I can get 50 amps instead of 30, and I notice a huge difference in top speed and torque on hills specifically.

Going up to 100 amps was even better.
```

---
## \#10 Posted by: XvDarkVAngelvX Posted at: 2016-07-06T18:54:21.439Z Reads: 48

```
How can you apply raspberry pi to the Space Cell Pro? What difference would it make?
```

---
## \#11 Posted by: roonydagoony Posted at: 2016-07-06T19:45:48.439Z Reads: 40

```
I doubt you can do much with it, unless you plan on using it as a speed controller.
You'd have to make the program from scratch or somehow repurpose existing speed controlled code onto the pi (However, I haven't seen anything like this anywhere)
The Space Cell comes with incorporated BMS
```

---
## \#12 Posted by: XvDarkVAngelvX Posted at: 2016-07-06T21:18:45.490Z Reads: 35

```
Ok, was just wondering. I have one. But not trying to dig in to much just yet. I want to get my first build going. Then once I cruise for a min. Build my own battery 🔋 pack 📦.
```

---
