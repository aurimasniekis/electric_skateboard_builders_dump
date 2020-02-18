# Actual SK3 Power Output

### Replies: 25 Views: 736

## \#1 Posted by: VECTOR.xyz Posted at: 2018-12-10T19:28:52.816Z Reads: 197

```
I've seen on Hobbyking's website that the SK3 6374 192kv can draw up to 4032 watts, which sounds absurd to me because 4 kw can heat up an entire house in winter. This would mean that running the motor at 50.4v (12s) at 80a would heat up an entire house.

To calculate the _actual_ power output of the motor, you could take the angular velocity (in r/s) and torque (in Nm) and just multiply them: **P = M x ω** (Power = Torque * angular velocity)

Using this post:
https://www.electric-skateboard.builders/t/torque-curves-for-sk3s-6354-260kv-6374-149kv-6374-192kv/19721

We take the (RPM / 60 seconds) * (Kgcm * 0.098Nm/Kgcm) = Watts
This ends up being around **370 watts**, which sounds more realistic than 4032 watts.

Am I correct in my calculations?

Vector


Edit: I was totally wrong, look at post #14 for something more reasonable. I ended up getting **2300 watts**.
```

---
## \#2 Posted by: pjotr47 Posted at: 2018-12-10T19:33:28.209Z Reads: 185

```
The 4032watt is not only heat, the most part goes to moving a force forward.... 

With your 4kw heating in your house. The 4kw goes directly to a resistor that transfer the 4kw off electricty to 4kw off heat
```

---
## \#3 Posted by: B-b-q-tom Posted at: 2018-12-10T20:00:58.056Z Reads: 163

```
As for heating your home - yeah 4kw will heat a very small home but will take a few hours by which time your battery would be dead , it would be interesting to know how much of the 4kw claimed output of an electric motor actually gets put into use , I am sure a lot of energy is wasted and possibly even though it has a claimed output we probably aren’t even using all of it
```

---
## \#4 Posted by: craj1031tx Posted at: 2018-12-10T20:23:46.001Z Reads: 160

```
I'm not the first party source on this so take it with a grain of salt but a friend that does robotics competitions (and who I regard as being a subject matter expert with regards to this) said that he dyno'd the 125kV SK8 motor, and with a load it was drawing ~1100 watts at fully duty.
```

---
## \#5 Posted by: Acido Posted at: 2018-12-10T20:28:34.878Z Reads: 156

```
Focbox is capable of around 2500w if i remember right...
```

---
## \#6 Posted by: Acido Posted at: 2018-12-10T20:30:09.787Z Reads: 155

```
Because it has no need to pull more, im not an expert on motors but i see a 3-4 amp draw when going full throttle (95% duty) and i guess thats just the energy needed to fight the traction and maintain speed
```

---
## \#7 Posted by: VECTOR.xyz Posted at: 2018-12-10T20:35:18.719Z Reads: 154

```
If a motor is running with no load, all of the energy used is used by friction, which converts the energy into thermal energy. I'm probably wrong about heating a house, but it was just to make a point (@pjotr47 you're correct).  Still, measurements don't lie (as long as the graphs provided are accurate) and it seems that the most you can get out of an SK3 is ~370 watts. Also, 370 watts is the final amount of power after chemical energy has been converted to electrical energy, and then to kinetic energy, so it might draw more power. 

The graphs in the [other post](https://www.electric-skateboard.builders/t/torque-curves-for-sk3s-6354-260kv-6374-149kv-6374-192kv/19721) may not be complete so we don't see the full torque curve, and maybe the motors can do more than just 370W and maybe I'm just completely wrong.

4kw can run 4 or 5 microwaves or a large clothes dryer, so I just find it hard to believe that a motor the size of a small apple can pull that much power.

I would like to see a full torque curve graph with a wattage peak and everything, but I don't know if anybody has done those tests.
 
Example:
https://www.google.com/imgres?imgurl=https%3A%2F%2Fa.pololu-files.com%2Fpicture%2F0J6476.600.jpg%3F37d25b538bd34ba4233fe286cebf8aa3&imgrefurl=https%3A%2F%2Fwww.pololu.com%2Fproduct%2F1117%2Ffaqs&docid=09GhE8XqF1OheM&tbnid=KhHO47xuiVnQxM%3A&vet=10ahUKEwissffYjZbfAhXdHzQIHVWoAbMQMwhOKAUwBQ..i&w=600&h=500&safe=strict&bih=686&biw=1396&q=dc%20motor%20torque%20curve&ved=0ahUKEwissffYjZbfAhXdHzQIHVWoAbMQMwhOKAUwBQ&iact=mrc&uact=8
```

---
## \#8 Posted by: Andy87 Posted at: 2018-12-10T20:42:15.096Z Reads: 134

```
I don’t know anything but my hair dryer claim 2kw and the motor inside is definitely smaller than a Sk3 6374.
I never questioned this specs as I get my hair dry fast and that’s all that matters.
```

---
## \#9 Posted by: pjotr47 Posted at: 2018-12-10T20:51:04.251Z Reads: 128

```
Haha, The most part of the electricity goes to the resistor so you can dry your hair with hot air. Only a small % goes to the motor(ventilator) so that there is a wind.
```

---
## \#10 Posted by: pjotr47 Posted at: 2018-12-10T21:03:48.339Z Reads: 127

```
[quote="VECTOR.xyz, post:7, topic:77630"]
Still, measurements don’t lie (as long as the graphs provided are accurate) and it seems that the most you can get out of an SK3 is ~370 watts. Also, 370 watts is the final amount of power after chemical energy has been converted to electrical energy, and then to kinetic energy, so it might draw more power.
[/quote]

Why do you think 370watt? When I accelerate 100% from stand still I draw 40A from my battery and there is 60A that goes to the motor
```

---
## \#11 Posted by: Acido Posted at: 2018-12-10T21:05:21.833Z Reads: 123

```
We would put 5 motors on our boards if we could get only 400w out of them lol

400w is nothing...
```

---
## \#12 Posted by: linsus Posted at: 2018-12-10T21:16:59.761Z Reads: 116

```
[quote="VECTOR.xyz, post:7, topic:77630"]
If a motor is running with no load, all of the energy used is used by friction
[/quote]
Wrong, some is friction (bearings), some is Power to actually spin, some is core losses in the stator.

[quote="VECTOR.xyz, post:7, topic:77630"]
that the most you can get out of an SK3 is ~370 watts.
[/quote]
What? So if you draw (yes, draw, you need load to get amps) 42 volt and 30A in the motor, it still equal to sub 500? 😂 Gooby pls. Power is mainly devided by the watts to do the work and the losses involved, a good Electric motor usually has an efficiency of 95%. (99% world record by ABB.)

[quote="VECTOR.xyz, post:7, topic:77630"]
chemical
[/quote]
Wat. We not making crysal meth here. 

[quote="VECTOR.xyz, post:7, topic:77630"]
4kw can run 4 or 5 microwaves or a large clothes dryer, so I just find it hard to believe that a motor the size of a small apple can pull that much power
[/quote]
Everything is relative. Bldc is a big step up from brushed motors when it comes to packning Power. One thing that stays linear is the copper mass. More copper = better/stronger motor

Sorry if i sound like a douche. Its my default mode.

Id tell you to pick up a book on Electric Power and driveapplications but I maybe this post is abit easier to swallow : http://vedder.se/2014/10/chosing-the-right-bldc-motor-and-battery-setup-for-an-electric-skateboard/
```

---
## \#13 Posted by: pat.speed Posted at: 2018-12-10T21:25:03.484Z Reads: 102

```
Idk how the heck you came to 370w but it’s wrong. The only thing I can think of that you might be meaning is he actual output force of the motor is 370w, but should that be measured in Nm or ft/lbs. 

Btw the motor dictates how much power is draw, if I run my board with no load it will be like 2a draw, with me on it it’s more like 5a. If my brother and I were on it, we went up a huge hill at 60km/h, from a dead stop then I would be pulling upwards of 60a but not constantly.

Btw we have the vesc which measures all of this anyway. We just need to keep increasing the load till the motor stalls or overheats
```

---
## \#14 Posted by: VECTOR.xyz Posted at: 2018-12-11T03:04:10.194Z Reads: 94

```
My bad guys, I made an incredibly stupid physics error: **ω** (angular momentum) is measured in RADIANS per second and not rotations per second, changing the kinetic power output of the motor to around 2300w.

BLDC motors are pretty capable, so I suppose 2300w sounds about right. (370w did sound kind of low)

This number is derived from hard data, so the motor can do _at least_ 2300w of output because the previously mentioned post doesn't have complete data from 9000 rpm to 0 rpm. It would be cool though to fully test an SK3 or any one of the sensored esk8 motors out there and see how efficient the VESC/BLDC combo is, converting the electricity into mechanical motion. 

Calculating the power draw, on the other hand, should be done on the DC side because calculating power draw on 3 phase AC is not as simple as voltage * amperage.

**Double check your math, always.**

@linsus 
[quote="VECTOR.xyz, post:7, topic:77630"]
chemical energy has been converted to electrical energy, and then to kinetic energy
[/quote]
I was refering to the chemical reactions taking place in the battery, but how did you know about the meth?:
```

---
## \#15 Posted by: Jmding Posted at: 2018-12-11T06:41:28.092Z Reads: 81

```
What are you looking to do @VECTOR.xyz? I am having trouble understanding what the root motivation of this line of inquiry is. Are you trying to compare motors? Or define what the total power capacity of these systems are?
```

---
## \#16 Posted by: linsus Posted at: 2018-12-11T07:33:50.057Z Reads: 71

```
Fair enough, but its still electrons traveling through a wire and one should not confused battery amps with motor amps. And when doing motor calculations, whats on the other side of the controller is somewhat irrelevant
```

---
## \#17 Posted by: linsus Posted at: 2018-12-11T07:37:11.079Z Reads: 71

```
Actually I much rather do calculations on a 3phase motor not some damn hybrid situations. So disagree on the math part
```

---
## \#18 Posted by: VECTOR.xyz Posted at: 2018-12-11T09:09:59.208Z Reads: 67

```
I found it hard to believe that a sk3 motor could output more than 5 hp (4032 w), and that maybe 4032 w is not an accurate representation of  what the motor could actually do.
```

---
## \#19 Posted by: lrdesigns Posted at: 2018-12-11T09:32:07.560Z Reads: 65

```
They can probably do 8000w for like 1 second. Its all about how its used. 

Duration and load. 

The only real way to know is to test it in your application, test the temp after a run and if its is too high you can turn amps down in the vesc tool or vise versa.
```

---
## \#20 Posted by: Jalapeno Posted at: 2018-12-11T12:01:04.045Z Reads: 62

```
That's why when you ask someone to check your math you give the formula, the result and the intermediate calculations just like in a test.
Interesting question though :)
```

---
## \#21 Posted by: Jmding Posted at: 2018-12-11T16:10:24.946Z Reads: 52

```
Gotcha. Makes sense. To figure that out, I would 1) use the fact that people here are regularly driving these motors at 12s and 80A motor current, find out how Vedder is measuring voltage and current on the AC side, and calculate a typical input power that way. 2) Use the efficiency numbers from the charts in your first post to calculate the mechanical output power, or just estimate it at ~80% efficiency which seems to be a conservative estimate based on the plots.

The other thing is, there are a lot of people that run 6355 motors at 12s and 80A as well, even though the stator is almost half as long as that from the 6374. Boosted also runs their motors (which are tiny, probably something like 5025) at 30A max. This says to me that typical use cases do not draw maximum allowed current for very long at all, and we can probably configure VESC to drive 6374 at a good deal more than 80A.
```

---
## \#22 Posted by: Hummie Posted at: 2018-12-11T16:45:12.274Z Reads: 52

```
Peak power will be max speed it can spin x the max torque based on the magnetic saturation point of the stator material and the leverage based on radius

Continuous power would hugely depend on the ambient temp, airflow and ability to dissipate heat, and the max operating temp of the magnets.
```

---
## \#23 Posted by: VECTOR.xyz Posted at: 2018-12-11T18:51:16.871Z Reads: 44

```
Don't know the math for 3 phase AC, but I found this calculator.

https://www.rapidtables.com/calc/electric/Amp_to_kW_Calculator.html
```

---
## \#24 Posted by: Boardnamics Posted at: 2018-12-11T20:28:57.146Z Reads: 40

```
An sk3 can totally make more than 400w. Without a doubt. It really depends on if you're talking about burst power or continuous power. Our motors can make obsurd amounts of power for a limited time. Unlike an engine, there is not really any mechanical limitations that prevent the motor from making above its continuous rating.

The only issue is heat and maybe saturation of the magnetic field at some point. The windings can handle it but the magnets are the first to go from the heat.
```

---
## \#25 Posted by: Okami Posted at: 2018-12-11T20:38:15.233Z Reads: 39

```
yeh I think u should re-edit your first post and put 2.3kw there.. otherwise it can make some flaming if someone doesnt read your 14# post :smiley:

The real kinetic energy in watts sounds like good comparison. I have taken my sk3 (192kv, 6374) only to about 1500W (electrical) due to battery output limit but im sure someone have pushed it a lot more.
```

---
