# Can I calculate the (kv*) of this motor?

### Replies: 27 Views: 509

## \#1 Posted by: cubed Posted at: 2019-03-28T01:30:41.787Z Reads: 101

```
Hello everyone,

I've had my eye on this motor for a little bit now, however they only show the power in Watts. Every esk8 calculator I have tried required a kilovolts rating for the motor. How can I calculate this?

https://www.peipeiscooter.com/10inch-10-inch-10x6-00-5-5-wide-tyre-brushless-gearless-dc-wheel-hub-motor-balance-scooter-hub-motor-hally-motor-phub-188.html

Thanks for the help!
```

---
## \#2 Posted by: J0ker3366 Posted at: 2019-03-28T01:36:44.798Z Reads: 92

```
@b264 knows the math for this shit lol
```

---
## \#3 Posted by: cubed Posted at: 2019-03-28T01:38:33.894Z Reads: 89

```
@b264 Please help o mighty math god. I make offerings of skateboard bearings and hub motors :pray:
```

---
## \#4 Posted by: olestra Posted at: 2019-03-28T01:47:55.116Z Reads: 89

```
no load rpm is 629 at 60v, according to chart. that would be 629/60 = about 10.5 kv 

btw, I love how badly named kv is!

also according to chart, max torque is around 441 -- that would be your likely max speed. so 441 rpm * circumference of about a meter gets 441/60 M/s = about 7.35 M/s or 26 kph/ 16 mph when running a 60v system
```

---
## \#5 Posted by: cubed Posted at: 2019-03-28T01:54:57.183Z Reads: 84

```
Thank you! Doesn't that seem like quite a low value however? Most 6374 motors and even some other hub motors are rated at 75kV. Since this is a scooter hub motor I thought it would be more powerful.
```

---
## \#6 Posted by: olestra Posted at: 2019-03-28T02:00:10.036Z Reads: 84

```
there's a reason we need to use gearing to slow down these motors, usually. Kv is not a rating of power, it's theoretical max speed.

Watts is what you are looking for for power. looks like it's a 1800 watt motor. ballpark equivalency is 750 watt = 1 hp... so that's about 2.5HP
```

---
## \#7 Posted by: pat.speed Posted at: 2019-03-28T02:01:29.193Z Reads: 81

```
Kv is how it is rated for speed (rpm/volt) 

kV is kilovolt
```

---
## \#8 Posted by: cubed Posted at: 2019-03-28T02:03:42.723Z Reads: 78

```
Ok so might be a dumb question, on a calculator like so https://calc./#/0

What would I input for the drive trail values? I understand Id need to put in 1 for motor and wheel pulley, but what do I put for the kv and poles values?

Thanks for helping me through this. Also from what the company has told me, this motor can only be configured up to 600W.
```

---
## \#9 Posted by: cubed Posted at: 2019-03-28T02:03:55.345Z Reads: 74

```
Fixed the title
```

---
## \#10 Posted by: olestra Posted at: 2019-03-28T02:04:15.970Z Reads: 75

```
technically it's the reciprocal of the back emf constant, Ke. we should call it  the volt constant of a motor. everyone just says kilovolt. that's why I'm amused by the name RCers and eSK8 ppl use for Kv
```

---
## \#11 Posted by: olestra Posted at: 2019-03-28T02:08:21.128Z Reads: 76

```
you can't, the data isn't provided. if you leave it at 14 poles it will still be in the ball park. 

254 for wheel size. 10.5 for Kv

plug in what battery data you are planning on going with
```

---
## \#12 Posted by: cubed Posted at: 2019-03-28T02:09:50.302Z Reads: 72

```
:pray: Thank you once again :smile:
```

---
## \#13 Posted by: olestra Posted at: 2019-03-28T02:11:49.936Z Reads: 69

```
quite welcome, I'm stuck waiting for a slow data process at work. 

when that happens, I go around a couple of forums and stackoverflow and answer what questions I can
```

---
## \#14 Posted by: b264 Posted at: 2019-03-28T02:58:52.201Z Reads: 61

```
Close. :smirk:

Kv is approximately rpm per volt

kV is kilovolt
```

---
## \#15 Posted by: b264 Posted at: 2019-03-28T03:00:07.230Z Reads: 61

```
I got a similar number based on their ratings which may or may not have marketing department exaggeration, but it's similar to what @olestra got

[quote]
Given:  
tire diameter 254mm  
top speed 35km/h  
top voltage 60V  
top power 600W  

Converted:  
tire diameter 254mm = 0.254m  
top speed 35km/h = 35000m/h = 583m/min  

Calculated:  
tire circumference: 0.254m * π = 0.798m  
top rpm = 583m/min / 0.798m = 731rpm  
motor Kv = 731rpm / 60V = 12.1  
[/quote]

I would actually recommend asking them, and letting us know too :slight_smile:

Also with a Kv that low, hall sensors will be very important, so make sure those are present.
```

---
## \#16 Posted by: cubed Posted at: 2019-03-28T03:23:24.064Z Reads: 52

```
Thank you, will check this! Do you think this is powerful enough to run a longboard with a 10s5p setup? Or should I go for something more powerful.
```

---
## \#17 Posted by: b264 Posted at: 2019-03-28T03:27:45.504Z Reads: 51

```
I would definitely never use that motor for a longboard because it's too big.

If you were trying to make a single-wheeled skateboard (Onewheel-style) that might be another story.  I'm not sure what you want.
```

---
## \#18 Posted by: cubed Posted at: 2019-03-28T03:29:06.448Z Reads: 51

```
Its kinda hard to explain, basically something like this:

https://www.electric-skateboard.builders/uploads/db1493/original/3X/f/7/f708bbcbce3e09599d3e0d78a89b1176d01ac10d.jpeg
```

---
## \#19 Posted by: b264 Posted at: 2019-03-28T03:30:39.985Z Reads: 50

```
In that case, it may be a fantastic motor choice

You're going to need to run fully sensored so make sure the sensors are good and you get them nice and waterproofed after you receive the motor
```

---
## \#20 Posted by: cubed Posted at: 2019-03-28T03:31:19.771Z Reads: 49

```
Ok awesome, just wanna make sure it will actually move me before I buy it :sweat_smile:
```

---
## \#21 Posted by: b264 Posted at: 2019-03-28T03:32:04.557Z Reads: 47

```
Before you buy it, I'd ask for more specs though LoL.  Because after you buy it places are less likely to help you :slight_smile:
```

---
## \#22 Posted by: pat.speed Posted at: 2019-03-28T03:32:35.051Z Reads: 48

```
Shhhhhhh it’s the auto capitals fault, fixed
```

---
## \#23 Posted by: cubed Posted at: 2019-03-28T03:33:06.108Z Reads: 46

```
Will do for sure. Thanks!
```

---
## \#24 Posted by: KaramQ Posted at: 2019-03-28T03:52:41.460Z Reads: 47

```
Dang man, dude that thing your building looks sick, are you going to make a build thread?
```

---
## \#25 Posted by: cubed Posted at: 2019-03-28T03:54:27.865Z Reads: 46

```
Most definitely. Once I get all my parts together Ill have a detailed thread. Gonna put some ski sleds on it to make it work in heavy snow too, should be fun!
```

---
## \#26 Posted by: webst Posted at: 2019-11-27T08:34:30.671Z Reads: 12

```
Have you got wheel/motor parameters from peipeiscooter?
```

---
## \#27 Posted by: Fosterqc Posted at: 2019-11-27T23:03:49.616Z Reads: 7

```
Huh never saw this thread. Good one.
```

---
