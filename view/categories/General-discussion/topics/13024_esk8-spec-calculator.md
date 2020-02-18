# eSk8 Spec Calculator

### Replies: 12 Views: 2178

## \#1 Posted by: Esrapp21 Posted at: 2016-11-14T01:30:20.086Z Reads: 261

```
I'm about to make my first electric board and I have know most of the parts that I'm going to use. I was using this site's spec calculator, and something didn't come up right. Here is my link: http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":12,"motor-kv":130,"system-efficiency":85,"motor-pulley-teeth":1,"wheel-pulley-teeth":1,"wheel-size":83}| . The reason the motor ratio is 1:1 is because I'm using a hub motor, so I figured since no gear ratios are needed, I'd make it 1. I was wondering this will be the actual top speed, or it just isn't meant for hub motors. If it is the actual top speed, I'll probably go for the 75 kV hub motor for more torque, I guess.

BTW, if you are new, here is the original calculator link: http://calc.esk8.it/
```

---
## \#2 Posted by: JLabs Posted at: 2016-11-14T01:37:21.815Z Reads: 251

```
I don't think it is accurate for hub motors, they are "less efficient" and loose a lot of power to heat. I would ask @makevoid on this one.
```

---
## \#3 Posted by: Jinra Posted at: 2016-11-14T01:41:12.467Z Reads: 228

```
Yes if, you're using hub motors just use any number for the gearing ratio as long as it's 1 to 1 (could be 1000 to 1000 and it'd be the same).

See here for the math: http://www.electric-skateboard.builders/t/accurate-speed-tracking/10516/3?u=jinra
```

---
## \#4 Posted by: trampa Posted at: 2016-11-14T20:54:37.192Z Reads: 161

```
http://www.elektro-skateboard.de/wiki/wissenswertes/strom-spannung-reichweite-vii

This one will help.

Frank
```

---
## \#5 Posted by: Esrapp21 Posted at: 2016-11-15T01:27:19.832Z Reads: 136

```
This is a great resource, but it has limited motor and battery options. And customs aren't functional. Plus, it uses the same math as the other calculators, with the addition of wind resistance, etc. I'm looking for a calculator that can calculate a hub motor specs more accurately then just using the 1:1 motor to wheel gear ratio.
```

---
## \#6 Posted by: Jinra Posted at: 2016-11-15T01:45:30.591Z Reads: 114

```
How do you mean more accurate? 1:1 is exactly what a hub drive is.
```

---
## \#7 Posted by: Esrapp21 Posted at: 2016-11-15T01:56:51.992Z Reads: 105

```
Yeah, that's the thing. It seems almost too good to be true. I think @JLabs might be right about power efficiency, and that might be the catch, and that is what I want to find out.
```

---
## \#8 Posted by: JLabs Posted at: 2016-11-15T02:04:30.823Z Reads: 98

```
@jacobbloy would be able to answer the question on hub motor effiency, or @Hummie
```

---
## \#9 Posted by: Jinra Posted at: 2016-11-15T02:14:19.672Z Reads: 91

```
It's about whether or not the motors,esc, and battery are able to overcome load, if they do then you'll get the posted speed or close to it. hubs have a hard time overcoming this load sometimes due to the 1:1 ratio they run.
```

---
## \#10 Posted by: Esrapp21 Posted at: 2016-11-15T03:26:43.323Z Reads: 81

```
So, in your personal opinion @Jinra would a 75 or 130 kV hub motor be better? The goal would be about 20-25, but if possible to squeeze some extra TORQUE out of it :slight_smile:
```

---
## \#11 Posted by: Hillso Posted at: 2016-11-15T07:31:30.623Z Reads: 76

```
definitly the lower kv option. the optimal kv is that who it's max speed matches your wanted max speed. the more max speed a motor have, the lower the torque.
```

---
## \#12 Posted by: Jinra Posted at: 2016-11-15T07:32:46.005Z Reads: 72

```
for 12s for sure go for 75kv. Especially since your target speed is 20-25 mph. 130kv would be too fast.
```

---
