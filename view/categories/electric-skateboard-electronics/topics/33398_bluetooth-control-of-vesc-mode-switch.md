# Bluetooth control of VESC Mode switch?

### Replies: 4 Views: 351

## \#1 Posted by: amazingdave Posted at: 2017-09-18T12:09:04.735Z Reads: 71

```
Hi, I'm half way through a single VESC build...

Is it possible to have 2 switchable modes on the VESC through an iOS app, like learner mode with limited top speed and soft brakes, and beast mode with all power available?
```

---
## \#2 Posted by: TehAtheist Posted at: 2017-09-18T12:13:22.162Z Reads: 70

```
I use perimetr.at to change modes.
Takes me a few seconds to switch from 40km/h max speed to 18km/h legal speed.
```

---
## \#3 Posted by: amazingdave Posted at: 2017-10-05T14:15:29.088Z Reads: 37

```
Which parameters would you change? Is it possible to have gentle active braking to limit the top speed for a novice? 

Thanks for helping.
```

---
## \#4 Posted by: TehAtheist Posted at: 2017-10-05T15:17:52.072Z Reads: 35

```
Yeah, just adjust the MAX EERPM. 
You'll have to calculate the number though.

http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":8,"motor-kv":190,"system-efficiency":100,"motor-pulley-teeth":15,"wheel-pulley-teeth":30,"wheel-size":90}|

Fill in your stats in the above tool, then check ERPM number, which for me is 39368 RPM.
Top speed is 47km/h:
47km/h ---> 39368 RPM
So for example for a 25km/h limit:
25 km/h ---> 20940RPM

Cheers.
```

---
