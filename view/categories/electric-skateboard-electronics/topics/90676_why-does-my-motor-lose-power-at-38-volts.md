# Why does my motor lose power at 38 volts?

### Replies: 10 Views: 158

## \#1 Posted by: JBev Posted at: 2019-04-15T23:41:27.336Z Reads: 61

```
This weekend I decided to put some esk8 parts on an old razor bike frame that a friend had lying around. I used a torqueboards 6380 motor, geared 11-80 with a 12 inch wheel. Also, I used a vesc hooked up to an ebike throttle, set to 60 motor amps and 150 battery amps. The battery was five 2s 60c lipos wired in series. I had a lot of fun riding the bike this weekend; but this morning it slowed down and lost almost all of its power at 38 volts. After checking that my battery was balanced(it was), running motor detection again(I'm using BLDC), and charging the battery, I took it for a ride. Once again, it started slowing down and losing torque around 38.5 volts, bringing me to a stop. Does anyone know whats wrong? My vesc voltage cutoff is set to a soft cutoff from 34-31 volts, so that shouldn't be the problem. Also, my motor started making a clicking noise at low RPMs. Could this be related to the loss of power? Thanks in advance for any help.
```

---
## \#2 Posted by: J0ker3366 Posted at: 2019-04-15T23:47:11.788Z Reads: 53

```
Run your motor @ 40-50amps. Youll notice you dont get the same acceleration but the loss in accel is transfered to capacity. I run a 8s3p with six 4s lipos. Run motor @ 40amps and i get the miles i need. I run motor @ 60amps and i get less range.

If youre up for it, id recomend going higher with the lipos in parallel.
```

---
## \#3 Posted by: JBev Posted at: 2019-04-15T23:51:44.999Z Reads: 47

```
I would like to run more in parallel eventually, but I'm more concerned that my board basically stops working when it gets to 38.5 volts. The batteries should still have capacity left at this voltage.
```

---
## \#4 Posted by: J0ker3366 Posted at: 2019-04-15T23:54:08.229Z Reads: 42

```
Youre pulling more amps than the lipos can provide @ that voltage. Adding more P will definitely help you out. Lowering your amps will allow more range but on 1p youre still going to hit a sag before your cutoffs.
```

---
## \#5 Posted by: JBev Posted at: 2019-04-15T23:57:37.256Z Reads: 40

```
Ok. It was just strange because it was working at 36 volts earlier without much sag. It would sag about one volt going up 15% hills(maybe steeper, i'm just guessing) at 25mph.
```

---
## \#6 Posted by: J0ker3366 Posted at: 2019-04-16T00:01:44.793Z Reads: 37

```
Yep pulling more than the lipos can deliver. What lipos are you using?
```

---
## \#7 Posted by: JBev Posted at: 2019-04-16T00:07:49.571Z Reads: 34

```
https://hobbyking.com/en_us/zippy-compact-5000mah-2s-60c-lipo-pack.html
I've been using this setup on a longboard for a few months now and have never had problems handling the same roads in the same conditions. Also, I have ridden this bike around for the past two days without it slowing down around 38 volts. The cutoff happened randomly and seemed weird because I haven't had any problems until now.
```

---
## \#8 Posted by: J0ker3366 Posted at: 2019-04-16T00:14:53.908Z Reads: 27

```
"A few months" on an esk8/ebike 1p lipos will degrade. More so if youre riding daily and running high amps. 

For the time being you can lower motor amps and get a "little" bit of added range but again, youre going to hit a sag before cutoffs.

If you do upgrade your lipos in the future, go for graphenes, higher Ah (think more above 6Ah). Multistar makes a 16Ah 4s (it is pricey) that @MoeStooge uses in his uphill racers. Last i heard from him he was still enjoying them.
```

---
## \#9 Posted by: JBev Posted at: 2019-04-16T00:23:38.136Z Reads: 25

```
Alright, that makes sense. Thanks for helping me out!
```

---
## \#10 Posted by: J0ker3366 Posted at: 2019-04-16T00:26:42.979Z Reads: 25

```
&lrm; Anytime
```

---
