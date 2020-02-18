# Torque Vectoring? Your thoughts?

### Replies: 5 Views: 857

## \#1 Posted by: TheCheat Posted at: 2016-11-16T09:25:08.754Z Reads: 110

```
Given we're starting to see more quad motor builds, wouldn't it be great if we had torque vectoring? In a perfect world, torque vectoring would allow us to use stiffer trucks for high speed stability whilst not sacrificing any carving performance.

Any opinions?
```

---
## \#2 Posted by: Hillso Posted at: 2016-11-16T10:03:22.544Z Reads: 106

```
the wheelbase is long compared to the truck width, is there enough turning torque? maybe it could do the opposite, run turny trucks and use motors as traction control anti wobble
```

---
## \#3 Posted by: Ackmaniac Posted at: 2016-11-16T11:30:38.210Z Reads: 96

```
If you have a dual drive system with the VESC you can already do something similar. Just set the "Traction Control ERPM diff" to 1000 ERPM or even 500. Because the slower wheel will get the power and the faster wheel will be shut off. So when you do a curve the inner wheel will get all the power and the outer wheel won't get powered a all, because the inenr wheel is always slower. That forces the truck to turn even more.

But sadly the VESCs ERPM detection isn't exact enough to do so (+-400 ERPM). That is the reason why i added a offset for the traction control in my modded firmware to not do anything before the difference is higher than this value. Otherwise one motor always gets a bit less power than the other. But you can do the opposite and force that behavior by the above described settings. You should give it a try.

Details:
"Traction Control ERPM diff" set to 1000;
Actual current should be 50A to each motor.
Motor 1 ERPM 40000 
Motor 2 ERPM 40500 
Differenc eis 40500 - 40000 = 500

So Motor 1 gets full power = 50A
Motor B gets half power 1 - (500/1000) * 50A = 25A

If the difference is higher than 1000 ERPM the faster motor gets shut off completely
```

---
## \#4 Posted by: littlem39 Posted at: 2016-11-16T13:01:22.730Z Reads: 80

```
Also thought abouut that. But than found out that this idea has a big problem. When you want to turn, you lean and by doing that you transfer almost all the weight on the inner wheel. And by incresing the speed of outer wheel it will most propably just keep on sliping.
```

---
## \#5 Posted by: Ackmaniac Posted at: 2016-11-16T14:45:35.439Z Reads: 64

```
But it increases the speed of the inner wheel because that is the wheel that is slower.
```

---
