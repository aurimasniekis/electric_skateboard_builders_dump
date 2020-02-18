# Motor connector extension cables

### Replies: 5 Views: 733

## \#1 Posted by: RazzleDazzle Posted at: 2018-05-21T20:23:16.548Z Reads: 147

```
Hey Guys,

will this work to extend the motor cable connectors?

https://www.amazon.com/Female-Brushless-Motor-Extension-Wires/dp/B01NCEJNJB/ref=sr_1_fkmr0_1?ie=UTF8&qid=1526934114&sr=8-1-fkmr0&keywords=4mm+bullet+connector+extension

Also, does someone know what the proper extension cable would be for the sensor wire (i think its a jst connector).  The motors i'm using are the ones from Torque boards (6355)

I just found this one, will it work?
https://www.amazon.com/Apex-RC-Products-Silicone-Brushless/dp/B071DSJ5CV/ref=pd_lpo_vtph_21_bs_t_1?_encoding=UTF8&psc=1&refRID=WC8Z8M5ZYVSMJ7KWENNR
```

---
## \#2 Posted by: clistpdx Posted at: 2018-05-21T20:36:56.896Z Reads: 128

```
I think the 6355 has 5.5mm bullet connectors, so these phase extensions wouldn't work. also, your sensor extension may extend the JST-ZH 6pin 1.5mm pitch found on the 6355 motors, but you'll still need to adapt to the VESC 2.0 pitch connectors w/ something like this: products/vesc-sensor-wires
or build similar.
```

---
## \#3 Posted by: RazzleDazzle Posted at: 2018-05-21T22:08:40.404Z Reads: 112

```
I noticed that the wiring kit i bought from them had the proper adapter.  At least i have 1, now i need to buy another for the second motor.

FOr some reason i can find any 5.5mm bullet connector extension.  Even Diyelectricskateboards doesnt have a 5.5mm male to female.
```

---
## \#4 Posted by: devilzangelz Posted at: 2018-05-21T22:48:48.882Z Reads: 94

```
It really depends on what your ESC has setup as well... 

IF your ESC is 4mm You may consider getting an adapter from [5.5mm to 4mm](products/wire-extensions-4mm-to-5-5mm)  to adapt the 5.5mm connectors to a 4mm plug for your ESC. Then your 4mm extenders will work well. If you do that, then you can get [150mm extenders](https://hobbyking.com/en_us/4mm-male-female-bullet-brushless-motor-extension-lead-150mm.html) or [250mm extenders](https://hobbyking.com/en_us/4mm-male-female-bullet-brushless-motor-extension-lead-250mm.html ) depending how long of a cable you need. Once again, this depends on what size connector your ESC/VESC has.

You could alway go "custom" and solder your own... Pick up some 14AWG wire, 5.5mm bullet connectors, and 4mm bullet connectors.
```

---
## \#5 Posted by: RazzleDazzle Posted at: 2018-05-21T22:55:46.302Z Reads: 91

```
I believe the connector on the Torqueboards ESC is 5.5 as well.  It seems like there's no 5.5 to 5.5 extensions, so i picked up the bullet connectors and will solder them myself.  On the plus side, it will be fit to my custom needs.
```

---
