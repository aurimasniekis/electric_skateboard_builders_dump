# E TRAMPA would it be better sensored?

### Replies: 13 Views: 643

## \#1 Posted by: Team Posted at: 2018-01-01T20:06:33.141Z Reads: 144

```
I’m new here but have been building e boards for a couple of years now. I have a electric TRAMPA board with the scramboards kit. 
 I’ve modified the battery and put everything in a home made encloser <img src="/uploads/db1493/original/3X/b/8/b88c2f38cde1d7ca12ed73ea42191c289571fcc3.jpeg" width="374" height="500"><img src="/uploads/db1493/original/3X/b/f/bfead0263b255103faf279a27bd76440dc933c03.jpeg" width="666" height="500">under neath which I think looks much better. 
 It has a 10s 4p 25r battery with twin vesc 4.12. The motors are maytech 250kv 3400w so it has plenty of power. The motors are sensored but I haven’t got that part plugged in, would it be better running sensored?  _`emphasized text`_
```

---
## \#2 Posted by: Namasaki Posted at: 2018-01-01T20:23:03.605Z Reads: 133

```
using the sensors will improve starting from standstill.
That is it should eliminate cogging when starting from a stop without having to push off manually.
```

---
## \#3 Posted by: mmaner Posted at: 2018-01-01T20:23:41.193Z Reads: 134

```
The 1st thing to know is you need to limit your ERPM to 60k it you will likely burn up the VESC's.  I would untick the limit with negative torque box. 

The only aspect if note to using foc is the lack of noise, I like hybrid mode as you get the smooth startup like FOC but do not risk the damage that can occured with FOC.

Edit: you might also consider increasing your motor and battery Max values to get more throttle.
```

---
## \#4 Posted by: trampa Posted at: 2018-01-01T20:48:53.647Z Reads: 114

```
As soon as you ride with bindings you want the sensors to work. Riding without bindings you can give your board a push to get rolling, which is not easily possible with bindings. Try it and you will see! Just make sure to use hybrid mode, so that the sensors are only used for startup.

The combo of 250kv motors with HW 4.12 and 10S4P is not really healthy. 150 KV would be a lot better, especially using FOC. The higher Amp flow is chewing up your battery and ESC fast. Always try to optimize for a super low amp flow. Optimization of Motor KV and battery voltage are your best way to assure an acceptable amp flow. The weakest part of the system is usually your battery. 15A peak per parallel cell is about the max, assuming the use of the typical high drain LG, Samsung, Sony cells. 

Frank
```

---
## \#5 Posted by: mmaner Posted at: 2018-01-01T20:53:34.918Z Reads: 103

```
[quote="trampa, post:4, topic:42498"]
150 KV would be a lot better, especially using FOC
[/quote]

That would be a huge waste of top end. 190kv is perfect for 10s.
```

---
## \#6 Posted by: Team Posted at: 2018-01-01T21:11:55.023Z Reads: 100

```
Thanks for the replies.. I have some knowledge of brushless motors from building quatcopters and various others RC's. is FOC just another name for 'sensored"? I've done quite a lot of research in to vesc's and the setup but that part is still confusing me. 
 I have bindings but they scare the carp out of me, at least without them i can just bail off when needed. I've moved the front springs slightly inboard just allow more steering without bindings. 
 The motors were the ones supplied with the kit (tbh i wasn't impressed with scram boards buts thats a whole other story) they run cool and have more than enough power for what i want, when they break i'll go for some lower KV ones.
```

---
## \#7 Posted by: Aggdaddy Posted at: 2018-01-01T21:19:02.391Z Reads: 97

```
I have a board from scramboards.   My Esc's burned up with the motor combo they installed.   I'm running TB 190kv 6355s and TB 12s OPTO Esc's, but eventually I am going to go with some focboxes.
```

---
## \#8 Posted by: Team Posted at: 2018-01-01T21:28:37.169Z Reads: 92

```
Well i had a nightmare as i order a kit 2 years ago which took 6 months to arrive and was useless, had no power, was built of crap components etc. after a lot of emails and another 8 months they finally sent me the 10s kit with twins vesc's. when i plugged the vesc's in to check the set up they hadn't done the motor detection or anything else. The battery is made of samsung 25r cells which is nice and the rest is ok but i wish i'd sourced all the parts myself as it would of been quicker and may be better quality. live and learn i guess. I keep looking on the Trampa website, the parts look ace so when mine goes up in smoke i'll give there stuff a go..
```

---
## \#9 Posted by: mmaner Posted at: 2018-01-01T22:00:43.996Z Reads: 81

```
[quote="Team, post:6, topic:42498"]
I have bindings but they scare the carp out of me, at least without them i can just bail off when needed
[/quote]

Check out the S2 Bindings, they are just as good for "locking in" and easy to bail out if as the are open on the inside.
```

---
## \#10 Posted by: Aggdaddy Posted at: 2018-01-01T22:04:07.494Z Reads: 80

```
My experience wasn't quite as bad, but the whole build was crap for sure.  I've replaced all the electronics.  The board itself is great.  It's Trampa after all.
```

---
## \#11 Posted by: E1Allen Posted at: 2018-01-01T23:14:38.660Z Reads: 71

```
[quote="Team, post:6, topic:42498"]
is FOC just another name for 'sensored"? I've done quite a lot of research in to vesc's and the setup but that part is still confusing me.
[/quote]

Vector control, also called field-oriented control (FOC), is a variable-frequency drive (VFD) control method in which the stator currents of a three-phase AC electric motor are identified as two orthogonal components that can be visualized with a vector. One component defines the magnetic flux of the motor, the other the torque. The control system of the drive calculates the corresponding current component references from the flux and torque references given by the drive's speed control. 

<img src="/uploads/db1493/original/3X/6/1/61058fd3677cd8daa36a960b8ebfdea9fd6cade7.PNG" width="281" height="500">

FOC is not the same as sensored.
```

---
## \#12 Posted by: trampa Posted at: 2018-01-01T23:19:10.321Z Reads: 69

```
Bailing out at speed is very unhealthy! You will realize that you can't run as fast as you just traveled, and you can hurt yourself easily. So when you ride with straps, its best to ad heel straps as well. Falling together with your board is not as bad as falling with only one foot attached to your board. 

I think a board doesn't need to be super fast to enjoy the ride. Personally I feel safer with bindings and heel straps. 

If you want to optimize, optimize the amp flow by going for 12S and appropriate KV for the desired top speed. 

FOC is field oriented control, running your motor on sinusoidal commutation, making the motor slightly more efficient and almost silent. I would not recommend to run your ESCs in Foc mode! They use supplementary parts, not up to the task. Especially for HW 4 the golden rule for FOC is low KV. Lower RPMs are easy to track for the HW 4.xx.
High RPMs cause issues, likely frying your chipset.

Frank
```

---
## \#13 Posted by: Namasaki Posted at: 2018-01-02T02:19:43.063Z Reads: 55

```
[quote="trampa, post:12, topic:42498"]
I think a board doesn't need to be super fast to enjoy the ride. P
[/quote]

Amen to that brother!!
10-15 mph on a board with carving setup is a lot of fun.
```

---
