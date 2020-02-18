# Road legal e-scooter conversion using Focbox

### Replies: 25 Views: 781

## \#1 Posted by: zwrtw Posted at: 2018-09-12T09:47:00.365Z Reads: 224

```
I have successfully converted an oldtimer (1968) Vespa 50 scooter to electric. I used an 150kV "Alien Power" c80100 motor (unsensorred) in conbination with a Focbox motorcontroller (I changed the thermal pads inside tho Focbox for better heat conducting ones). The electric motor is where the crankshaft used to be. The converted scooter is EMC tested according to UNECE R10 rev5 and passed the test hands down. After that it was tested by the Dutch road authorities, and also passed this test. So it is possible to use a Vesc/Focbox for road legal purposes...
```

---
## \#2 Posted by: baxter Posted at: 2018-09-12T10:09:33.828Z Reads: 218

```
Photos?

10 char
```

---
## \#3 Posted by: DeathByBacon Posted at: 2018-09-12T10:17:59.923Z Reads: 211

```
Photos? Do you have a build thread for this project?
```

---
## \#4 Posted by: Cobber Posted at: 2018-09-12T10:19:21.496Z Reads: 205

```
So you are still using the CVT?
```

---
## \#5 Posted by: zwrtw Posted at: 2018-09-12T11:42:07.529Z Reads: 185

```
I do not have a build thread, but here are some photo's...
I use a Vespa PK50 engine block. It does not have a CVT, I use the original manual 4 speed gearbox.
I hope this works:
[Electric motor fitting](https://myalbum.com/photo/0tm7I3TROdYx/540.jpg)
[Electric motor where the crankshaft and flywheel used to be](https://myalbum.com/photo/PjsXkjhN6B19/540.jpg)
[Motor with electronics box](https://myalbum.com/photo/mhtEBgQE8rak/540.jpg)
[Electronics box inside the scooter](https://myalbum.com/photo/VmhEbhBLuoKG/540.jpg)
[Close up](https://myalbum.com/photo/TtnsyiSkg7x7/540.jpg)
[Motor inside the scooter](https://myalbum.com/photo/k45dJ034tRwg/540.jpg)
[EMC testing](https://myalbum.com/photo/PhxJfDKtrvr5/540.jpg)
[battery](https://myalbum.com/photo/1FxfV5aCzf0D/540.jpg)
```

---
## \#6 Posted by: zwrtw Posted at: 2018-09-12T11:47:21.013Z Reads: 180

```
I will do a full restoration of the scooter coming winter to get the optics the vehicle deserves... I will turn it into its original bleu color again.
```

---
## \#7 Posted by: sk8l8r Posted at: 2018-09-12T11:49:14.425Z Reads: 178

```
thats a REALLY cool project! very impressive
```

---
## \#8 Posted by: ElskerShadow Posted at: 2018-09-12T12:28:14.067Z Reads: 170

```
very cool project! 
I have done the same with a Motobecane ! 
what is the configuration of your battery pack
```

---
## \#9 Posted by: zwrtw Posted at: 2018-09-12T13:09:14.325Z Reads: 156

```
Thanks! The battery is a 12S15P comfiguration with Samsung 18650 35E cells
```

---
## \#10 Posted by: Kug3lis Posted at: 2018-09-12T13:25:14.556Z Reads: 151

```
I am curious how does 4 speed transmission feel with electric motor...
```

---
## \#11 Posted by: Acido Posted at: 2018-09-12T13:31:23.171Z Reads: 147

```
i think you would be better off with something that can handle more amps and higher voltage
you dont require breaks that focbox has and there are lots of other escs that you can program
```

---
## \#12 Posted by: ElskerShadow Posted at: 2018-09-12T17:20:26.980Z Reads: 128

```
[quote="Acido, post:11, topic:67793"]
i think you would be better off with something that can handle more amps and higher voltage
[/quote]

Do you think VESC 6 , for now I only have used VESC for ebikes 
E scooter would require a VESC 6 ! But I use generally cheap 2000 W ebike ESC from China and it works like a charm. 
Used with a cheap car alternator you can find almost anywhere it has great torque but not the best efficiency
```

---
## \#13 Posted by: Battosaii Posted at: 2018-09-12T18:00:12.753Z Reads: 117

```
I think he meant something not Vesc based as they are limited to 12-13s max, ebikes on the other hand use 16s and above.
```

---
## \#14 Posted by: ElskerShadow Posted at: 2018-09-12T18:21:01.305Z Reads: 112

```
Not necessarily true, for exemple GOVECS e scooter runs on 14 S 
Most ebikes are 36 and 48 V, sometimes more but it's generally for customs needs 

I believe @Kug3lis is developing a VESC to go up to 18s or 16s can't recall would be a great solution 
Right now I am thinking of trying the flipsky 6.6 to try with a e scooter
```

---
## \#15 Posted by: Acido Posted at: 2018-09-12T18:22:28.893Z Reads: 109

```
why does it have to be an VESC, the biggest reason why we are using vescs are their smooth breaks
theres a lot of other escs that can be programmed same as vesc but can handle much more amps and much higher voltage
he does not need breaks, so he is not limited to a vesc
```

---
## \#16 Posted by: Kug3lis Posted at: 2018-09-12T18:36:52.006Z Reads: 108

```
@ElskerShadow it is not VESC its completely different ESC :)

@Acido all other ESC does simple duty control (not foc) they don't care about efficiency and many other things so they all just try to spin motor at any cost :)
```

---
## \#17 Posted by: Okami Posted at: 2018-09-12T19:08:30.472Z Reads: 101

```
Looks cool. Did they also test power / max speed?

Ive always thought such conversion might be hard from legal aspect but i guess if u keep the chassis/original body it can be possible
```

---
## \#18 Posted by: ElskerShadow Posted at: 2018-09-12T19:39:45.043Z Reads: 88

```
I would have thought that VESc was more efficient than 30 $ Chinese ESC that have a lot of heat and are very large.
@Kug3lis it's not VESc based ? My bad then I thought so
```

---
## \#19 Posted by: Acido Posted at: 2018-09-12T19:53:30.533Z Reads: 86

```
I was more thinking of some high end stuff like 18s and 200A :smiley:
Since he said he had a 10p or something huge battery
```

---
## \#20 Posted by: zwrtw Posted at: 2018-09-12T20:51:25.963Z Reads: 87

```
It is all about design decisions. The easy way to make an electric oldtimer Vespa was to transplant a Chinese scooter hubmotor and all its electronics into the Vespa. It would have been the cheaper way as the Dutch road authorities would accept the EMC approval of the Chinese scooter (assuming the Chinese scooter was road legal). I did not want that. I wanted the looks of the original scooter, even the original wheels, motorcasting and a functioning gearbox.

The electric motor was chosen on size to fit in the crankshafthousing, and the Kv etc. The vehicle is only a moped, so max speed is 40~45 km/h. If I want to go faster I take another ICE Vespa (motor-)scooter. Power and torque is more or less equal to the ICE moped. Max battery current is only set to 40A. I have no problems at all with the FOCBOX, but I agree that if you want more speed and/or better acceleration, you need a different controller. 
I like that the VESC variants are so good in sensorless mode. That is one of the reasons I chose it.

The gearbox is easy to use with an electric motor. Drive off in first gear. When you notice the motor loses torque due to being close to the maximum RPM (Kv, Kt, battery voltage...), shift to second gear and so on. Its the gearbox that makes this electrical setup with a small motor and small controler work. On inclines you can simply change the gear reduction to prevent the motor and controller from overheating.
```

---
## \#21 Posted by: lrdesigns Posted at: 2018-09-13T01:14:44.084Z Reads: 75

```
Are the stainless braided wire covers needed for legal reasons or just because you wanted it? 
![image|644x372](upload://r0JTrdpOlkqnCELGnlJbY8XcV2D.jpg)
```

---
## \#22 Posted by: zwrtw Posted at: 2018-09-13T17:28:27.311Z Reads: 61

```
[quote="Okami, post:17, topic:67793"]
Did they also test power / max speed?
[/quote]

Yes they did test the maximum speed as mopeds are only alowed to go 45 km/h.
```

---
## \#23 Posted by: zwrtw Posted at: 2018-09-13T17:30:45.923Z Reads: 61

```
[quote="lrdesigns, post:21, topic:67793, full:true"]
Are the stainless braided wire covers needed for legal reasons or just because you wanted it?
[/quote]

I used the braided steel wire covers for EMC reasons. To get it road legal it had to pass a EMC test. So yes, for legal reasons!
```

---
## \#24 Posted by: Okami Posted at: 2018-09-13T18:56:19.309Z Reads: 54

```
Did u have to pay a lot for doing the test?

Also can u comment on battery size, what range u are getting and did it cost close to 1000eur to make battery or was it less?

Also - did u spotweld or solder it?
```

---
## \#25 Posted by: epss4 Posted at: 2019-06-26T18:34:34.212Z Reads: 22

```
What throttle did you use and how did you link it to the vesc? Thanks!
```

---
