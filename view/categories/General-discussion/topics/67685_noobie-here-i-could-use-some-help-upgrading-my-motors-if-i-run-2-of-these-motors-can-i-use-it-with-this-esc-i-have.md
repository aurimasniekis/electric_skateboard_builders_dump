# Noobie here, I could use some help upgrading my motors. If I run 2 of these motors can I use it with this ESC I have?

### Replies: 9 Views: 203

## \#1 Posted by: queue_together Posted at: 2018-09-11T03:46:50.042Z Reads: 86

```
My current motors/mounts crapped the bed and I need to upgrade and would rather invest in some higher quality parts.

The motors I want to get: products/electric-skateboard-motor-6355-260kv?variant=712632074263

The ESC I have: http://www.diyeboard.com/v11-dual-belt-motor-sine-wave-foc-esc-speed-controller-p-522.html

I currently use these motors: http://www.diyeboard.com/dual-belt-drive-1400w2-n5055-motor-power-truckfront-truck-kit-p-422.html


I don't mind if I miss out on top performance if my ESC can't handle the new motors, but would the performance with the 2 new motors and current ESC be at least equivalent to that of my current motors, until I can afford to upgrade my ESC?

Thank you!
```

---
## \#2 Posted by: Skunk Posted at: 2018-09-11T04:28:10.211Z Reads: 79

```
I too wanna upgrade my riptide motors (same as the 50xx diy)
Following to see if anyone suggests a motor upgrade that esc can handle.
```

---
## \#3 Posted by: Andy87 Posted at: 2018-09-11T14:14:57.401Z Reads: 63

```
The controller controls the motors and not the motors the controller.
The kV is nearly the same so also no max erpm problems.
I‘m not that expert but I would say that should work...
The controller is rated to 50a constant at 10s.
So he will also don’t give more energy out to the motors. Doesn’t matter if 55xx or 63xx
```

---
## \#4 Posted by: queue_together Posted at: 2018-09-11T16:44:43.895Z Reads: 54

```
Do you think I should get the 190kv or the 260kv motors if I'm using a 10s3p battery?
```

---
## \#5 Posted by: Kug3lis Posted at: 2018-09-11T16:47:16.284Z Reads: 53

```
Your motors at the moment are 270kv so with 190kv or 260kv u will loose speed but will gain some more torque
```

---
## \#6 Posted by: Sn4pz Posted at: 2018-09-11T18:52:51.070Z Reads: 45

```
not sure if ur esc can handle it, but its a common motor for an evolve replacement 

https://www.banggood.com/de/Racerstar-5065-BR5065-140KV-6-12S-Brushless-Motor-With-Gear-For-Scooter-p-1110304.html?cur_warehouse=CN

theyre going to have much more torque than the motors you already had... lol
```

---
## \#7 Posted by: dareno Posted at: 2018-09-11T19:49:54.838Z Reads: 39

```
@Skunk certainly don’t go 140kv with the standard battery.   You’ll be able to walk faster.  Give you a nice exhilarating 11 mph weighted.
```

---
## \#8 Posted by: Skunk Posted at: 2018-09-11T19:52:30.513Z Reads: 38

```
I'm eyeing those 260kv tb motors now lol
```

---
## \#9 Posted by: dareno Posted at: 2018-09-11T20:15:53.151Z Reads: 36

```
That'll give you similar performance with the standard battery defo.  I have a single drive 280 kv on 6s lipo(well I did before the kids wrecked it) and that gets up in the 22 mark.  First thing i ever built.  

@queue_together If you are planning on upgrading to vesc at some point then with 10s I would probably go with the lower kv option (around the 200)  This will keep the max erpm under the threshold.  
The thing you need to consider is how far do you want to go?  That esc and battery is set up to work together from the factory and can't be changed. If you go vesc then you will have to be careful when you set your battery max because the bms in the battery is a low amp unit and will pop if you go above 15 amp per motor.
```

---
