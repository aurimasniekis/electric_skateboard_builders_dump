# Could a single drive handle abec 107’s?

### Replies: 21 Views: 1151

## \#1 Posted by: Mattmccrary8 Posted at: 2017-09-19T02:13:09.172Z Reads: 245

```
Could a single drive 6374, 18/36t, 12s4p handle the abec 107’s. Or is 97’s the most it could handle? Anyone have experience with that? Also does anyone have experience with 18t?
```

---
## \#2 Posted by: Cobber Posted at: 2017-09-19T02:14:14.838Z Reads: 246

```
all depends on motor kv bro
```

---
## \#3 Posted by: faithfulpuppy Posted at: 2017-09-19T02:21:23.509Z Reads: 246

```
i'm assuming you're using a 149kv motor? it will "handle" it fine as in it won't catch fire, but you'll be going extremely fast without all that much torque.  Change your gearing ratio to something like 16:40 for optimal performance

[here](http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":12,"motor-kv":149,"system-efficiency":85,"motor-pulley-teeth":18,"wheel-pulley-teeth":36,"wheel-size":107}|) is your config as described and [this](http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":12,"motor-kv":149,"system-efficiency":85,"motor-pulley-teeth":16,"wheel-pulley-teeth":40,"wheel-size":107}|) is closer to ideal.  We really need to know your kv and ideally your weight and riding conditions though.
```

---
## \#4 Posted by: BenL Posted at: 2017-09-19T02:50:45.822Z Reads: 230

```
Vs 83mm wheels it should have 2*pi*107/2*pi*83 = 1.289 times the top speed, and I believe the torque is also proportional  so (83/107) = .77 times as much torque.
```

---
## \#5 Posted by: Mattmccrary8 Posted at: 2017-09-19T02:54:48.735Z Reads: 219

```
My motor is a 190kv is 12s to much
```

---
## \#6 Posted by: Namasaki Posted at: 2017-09-19T03:04:33.728Z Reads: 218

```
12 x 4.2 = 50.4v
50.4 x 190 = 9576 rpm
9576 x 7 = 67032 erpm
The erpm limit for vesc 4.12 is 60000

You might be able to get away with it if you set the erpm limit to 60k in the bldc tool 
and turn off "limit erpm with negative torque"

I think you would have problems with 18/36 gears and 107mm wheels even with a dual drive.
```

---
## \#7 Posted by: Mattmccrary8 Posted at: 2017-09-19T03:09:28.323Z Reads: 209

```
Even if I set the limit to 60k? Since 67k is over, would I lose motor efficiency as well since it’s limited. Resulting in a lost of speed so I should just run 10s to begin with. It would be a 12s4p pack from TB. I thought Li-on is less voltage?
```

---
## \#8 Posted by: Namasaki Posted at: 2017-09-19T03:11:33.922Z Reads: 209

```
Li-ion charge up to 4.2 just like Lipos.
10s will yield less speed and less torque.
If your gonna run tall gears and big wheels to obtain high top speed, then Imo, your gonna need 12s for added torque to make it work.
Higer voltage increases speed and torque.
You can try the 190 with erpm limit set to 60k but turn off the negative torque limiter so your brakes don't come on while your accelerating at 38mph

Note: using 16/40 gears instead of 18/36 with 107mm wheels would only drop about 8mph off your speed at max erpm according to my gear speed calculator.
That's not much to give up for better efficiency.
```

---
## \#9 Posted by: bartroosen12 Posted at: 2017-09-19T10:48:03.844Z Reads: 186

```
You can go with the new 125kV from hobbyking maybe? It also has sensors so better torque when you start.
I'm sure 107mm is really no problem.
https://hobbyking.com/en_us/dt6376-14p-sensored-motor-125kv.html?___store
You could go with a 36T or 40T wheelpulley made for flywheels and a 15T or 20T motorpulley, it just depends on fast you wanna go
```

---
## \#10 Posted by: Mattmccrary8 Posted at: 2017-09-19T11:16:03.888Z Reads: 169

```
I don’t want to buy a new motor if I was going to buy one it’d be another 6374 to make a beast. I want about 35mph and 15-16 miles of range
```

---
## \#11 Posted by: flywithgriff Posted at: 2017-09-19T11:24:46.305Z Reads: 162

```
That's a reasonable want, if you are running dual 6374 with the 107's.
```

---
## \#12 Posted by: Mattmccrary8 Posted at: 2017-09-19T12:30:08.010Z Reads: 151

```
What would you do if you were me? If I want the 12s4p pack and I already have a 190kv TB motor? What gear ratio, wheel size would be the sweet spot in your opinion?
```

---
## \#13 Posted by: faithfulpuppy Posted at: 2017-09-19T19:44:08.248Z Reads: 136

```
For 12s use a 149kv or 170kv to avoid going over the 60,000 erpm limit
```

---
## \#14 Posted by: Mattmccrary8 Posted at: 2017-09-19T20:02:53.516Z Reads: 132

```
I already ordered the 12s battery, I can just limit the erpm at this point because I have a 6374 190kv motor. I’m going to run 97’s with a 16/36 setup. Does anyone know the odds of me burning up my vesc
```

---
## \#15 Posted by: faithfulpuppy Posted at: 2017-09-19T20:24:54.644Z Reads: 131

```
statistically, pretty high. you'll probably burn at least one, it's practically considered part of the learning process at this point
```

---
## \#16 Posted by: Namasaki Posted at: 2017-09-19T22:21:29.085Z Reads: 132

```
[quote="Mattmccrary8, post:12, topic:33466"]
What would you do if you were me?
[/quote]

I would go with what you have. 
Use BLDC mode, NOT FOC
set ERPM limit in bldc tool to 60k and -60k and turn off "limit erpm with negative torque"
Don't spin your motors up with the board upside down on the work bench unless your trying to test the erpm limit setting and if so, do it at your own risk.
Go ahead and try 97mm wheels with 16/36 gears although I think 90mm wheels are a better choice especially with that gearing.

I am running Both 6355s on one build and 6374s on another and what I have noticed is that the 6374s have more natural torque so that they require less throttle(current) than the 6355s to go up hills.

So you have some torque advantage with the 6374 motor and also with 12s voltage. 
So you will probably do ok with 97s and 16/36.
I recommend that you order the Metr bluetooth module and get the Metr app. Then you can monitor your FET temp on the fly.
Worst case, if your FET's get too hot the vesc will back off power.
It might be a good idea to lower the temp threshold in bldc tool since it is set fairly high by default.
```

---
## \#17 Posted by: Namasaki Posted at: 2017-09-19T22:35:42.974Z Reads: 118

```
Burning up Vescs is not part of the normal learning process. 
If you buy quality Vesc such as Ollinboards Vescs or Enertion Focbox or Trampa Vesc6,
I've been using Ollinboards Vesc4.12 for over a year and they have been rock solid.
```

---
## \#18 Posted by: faithfulpuppy Posted at: 2017-09-19T22:53:19.040Z Reads: 117

```
oh, for sure. my intention is that he should budget to get a second one should something go wrong with the first one.
```

---
## \#19 Posted by: Mattmccrary8 Posted at: 2017-10-10T16:15:53.084Z Reads: 102

```
The temp thing happened to me! How can I fix it! I’m screwed
```

---
## \#20 Posted by: Namasaki Posted at: 2017-10-10T17:40:40.165Z Reads: 102

```
What Vesc are you using 
What gears
What wheels 
What motor 
What is your weight
```

---
## \#21 Posted by: E1Allen Posted at: 2017-11-29T09:31:24.950Z Reads: 81

```
Matt. I'm running 16/36 12s with 97mm. On dual 6374 with FocBox. I have my ERPM limits set to 60k. I have my motor max to 65a and ESC to 60a.  So far the most battery amps I've pulled is 71a combined. I've pulled about 120 motor amps combined. I had to sit on my board and apply full throttle. It's got stupid amounts of torque. I topped out at 35mph.  I'll be doing further testing this weekend. I ordered the evolve 107s and I already purchased 18t motor gears.  If both those installed doesn't Rob torque I'll leave it. It's going to make it less efficient at lower speeds but my 48 inch deck has plenty of room for 12s6-8p😁😁.
```

---
