# Choosing motors for first build

### Replies: 27 Views: 505

## \#1 Posted by: ourcore Posted at: 2018-10-26T19:59:26.574Z Reads: 134

```
I'm in the process of choosing parts for my first build and was thinking of using 6364 170kvs, but I'm looking for more options/suggestions. I'll be using a 20700 10s5p pack, 2 ESCape singles, Evolve trucks with Evolve-style mounts, 15T/32T gearing, and 100mm Boa Constrictors. The esk8 calculator tells me I'd need at least around 190kvs to get over 30mph, which is my goal (190kv gets me 32mph weighted), but I'm not sure what my options are for motors. Ideally, I'd like something reliable that will fit on my trucks/mounts and that comes in black to match the other parts. Or should I go 16T and a lower kv to conserve battery? Thanks in advance!

EDIT: I weigh 200lbs and ride mostly on flat surfaces, but some hills. I don't want crazy torque, but I definitely want a responsive ride.
```

---
## \#2 Posted by: Colson003 Posted at: 2018-10-26T20:03:23.013Z Reads: 126

```
http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":10,"motor-kv":170,"system-efficiency":85,"motor-pulley-teeth":15,"wheel-pulley-teeth":32,"wheel-size":100}|

This is the calculator you're using?
```

---
## \#3 Posted by: ourcore Posted at: 2018-10-26T20:05:24.962Z Reads: 124

```
Yes, sir! I was focusing more on the weighted top speed
```

---
## \#4 Posted by: Colson003 Posted at: 2018-10-26T20:18:16.293Z Reads: 117

```
The unweighted is calculated at 3.7 volts per cell, so on a full charge you'll probably exceed the estimated 34mph.
```

---
## \#5 Posted by: ourcore Posted at: 2018-10-26T20:25:25.518Z Reads: 112

```
Ah, I see. In that case, maybe I could start at 170kv.

What are some suggestions for motors that would fit my build?
```

---
## \#6 Posted by: pat.speed Posted at: 2018-10-26T21:18:42.336Z Reads: 105

```
Tb are well known, as are @JLabs ( build kit boards), maytechs are also good and if you don’t mind different colours so are SK3’s and Keda motors
```

---
## \#7 Posted by: Holyman92 Posted at: 2018-10-26T21:28:22.725Z Reads: 99

```
Personally, i skate @torqueboards, i have their largest motors currently and love them. And they're only like 10$ more (I think) over the 6374.

![20181016_184248|375x500](upload://xbqzPAi73Fubwz55goPp57nbCB9.jpeg) 

This is their forward v5 mount (not really my thing) I prefer their v5 reverse mount so I can mount my deck drop through and still get full turns 

![1540589222795733066097|374x500](upload://cqS71eeBwjHip3qA8a7gvk90FRk.jpeg) 

Only running 1 motor rn because issues with flipsky
```

---
## \#8 Posted by: dareno Posted at: 2018-10-26T21:30:12.566Z Reads: 94

```
Hey mate, that calc is not very accurate tbh.  With 10s and your weight 190kv will be fine for those speeds.  170 will be very torquey.  Real world experience is what you need.  I,m 200lbs ish and my 10s 192kv build gets me 55km/h flat out with the wind behind me on 16/36 and 97mm wheels.
As for motors you can't go wrong with @torqueboards Good quality and good back up.  
Maytech are good but pricey.  I personally use sk3/8 and tb and all work fine.
```

---
## \#9 Posted by: Schulerbible Posted at: 2018-10-27T00:30:33.864Z Reads: 81

```
How come you get 55 km/hr out of your setup? Everything same here but 40 lbs less weight and max out around 48 km/hr???
Must be like 30 knots tail wind 🤪
```

---
## \#10 Posted by: dareno Posted at: 2018-10-27T04:47:58.683Z Reads: 73

```
Thats the fastest I have ever done on it to illustrate to the guy he will be fine with 190kv.  Its usually around the 50 mark.  Consistently.  
Oh and I'm obviously a much better rider than you. :sunglasses:
```

---
## \#11 Posted by: Schulerbible Posted at: 2018-10-27T05:13:24.716Z Reads: 68

```
Can't ride consistently 50km, ever seen a discharge curve of a Li-ion cell? 
How about u come down and prove it :grinning:
```

---
## \#12 Posted by: Andy87 Posted at: 2018-10-27T05:14:49.073Z Reads: 63

```
Using lipos will solve that issue 😉
```

---
## \#13 Posted by: dareno Posted at: 2018-10-27T06:08:13.540Z Reads: 63

```
When I said consistently I meant it will do it without any special circumstances like inclines or fully tucking every time.  Obviously there will performance drop across the discharge but not a great deal with decent cells until they get below 60%. You ever ridden a raptor 2?  Thats a 10s4p and trust me they do over 50 km/h  Yours should easily do that.   What set up do you have?
```

---
## \#14 Posted by: Schulerbible Posted at: 2018-10-27T06:09:34.793Z Reads: 60

```
Raptor 1, in principle same as you
```

---
## \#15 Posted by: dareno Posted at: 2018-10-27T06:10:02.918Z Reads: 59

```
&lrm;Settings?
```

---
## \#16 Posted by: Schulerbible Posted at: 2018-10-27T06:11:01.157Z Reads: 59

```
25A / Vesc battery, 60A motor amps
```

---
## \#17 Posted by: dareno Posted at: 2018-10-27T06:11:58.034Z Reads: 58

```
Thats why then.  What cells does it have? The original 25r pack or the 30Q?
```

---
## \#18 Posted by: Schulerbible Posted at: 2018-10-27T06:12:26.078Z Reads: 59

```
original 10s3p, 25R
```

---
## \#19 Posted by: dareno Posted at: 2018-10-27T06:18:22.745Z Reads: 63

```
Get yourself a 30q pack then the sag will be in a different league.  My original 6374 set up had a 10s3p 25r and yes would only do about 50 for about 5 minutes.  Then it would sag out.  That 10s board i was talking about has a raptor 2 battery in it set at 40 per and 80 motor.  Easily does over 50k's.  
You want to ride the one with the 12s in it, thats a fucking animal.
```

---
## \#20 Posted by: Schulerbible Posted at: 2018-10-27T06:27:35.795Z Reads: 62

```
Thanks, I am currently building a new one with a 12s3p Lipo pack that can dump out a lot more amps. Hope I will breach the 50 km/hr mark.
```

---
## \#21 Posted by: dareno Posted at: 2018-10-27T06:31:09.671Z Reads: 59

```
Yeah easily.  Lipo's are my next foray I think.  The more amps the less sag.  Waiting on that Zill battery.
```

---
## \#22 Posted by: Schulerbible Posted at: 2018-10-27T06:39:19.123Z Reads: 52

```
These will be Zill's batteries.;)
```

---
## \#23 Posted by: dareno Posted at: 2018-10-27T06:40:23.552Z Reads: 50

```
We spoke before on this hey?  Game changer for sure.
```

---
## \#24 Posted by: Schulerbible Posted at: 2018-10-27T06:46:44.093Z Reads: 48

```
Yeah absolutely, these batteries will deliver enough juice for my 6384s
```

---
## \#25 Posted by: dareno Posted at: 2018-10-27T06:50:45.059Z Reads: 47

```
Wow, you best be planning on vesc 6 to really appreciate the power.  Honestly my 12s build is too fast be honest.  Its already put one of my kids in hospital. Idiot with no helmet.  12s is different league stuff.
```

---
## \#26 Posted by: ourcore Posted at: 2018-10-27T17:17:25.797Z Reads: 36

```
Cheers! The TorqueBoards 6355 190KV motors seem decent, but would they fit on the Skate Kastle Evolve-style mounts? TB couldn't confirm for me. I'm trying to work around the Evolve trucks.
```

---
## \#27 Posted by: torqueboards Posted at: 2018-10-27T17:32:50.888Z Reads: 34

```
@Ourcore - Yeah, they would fit those mounts.
```

---
