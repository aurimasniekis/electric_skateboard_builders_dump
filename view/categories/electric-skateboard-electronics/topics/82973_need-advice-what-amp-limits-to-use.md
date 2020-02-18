# Need advice: What amp limits to use?

### Replies: 27 Views: 593

## \#1 Posted by: ZachTetra Posted at: 2019-02-03T01:37:50.960Z Reads: 161

```
I've been trying to read up on this but it's all going over my head so please don't post the search link...I tried but I'm just dumb

Parts:
- 12s4p Samsung 30Q 18650 pack
- MayTech 50A/240A dual ESC (for each motor)
- Dual MayTech 6355 (rated 65A max)
- 11:25 sprockets and chain on 90mm wheels

What I think I can do:
- 30mph for 40miles (using the esk8 calculator and assuming 11mi/wh
- pull 80A continuous and maybe 120A burst

What I think is the right amp limits:
- Motor -30/65 each
- battery -40/80

What I'm being told:
- Motor -40/40 to -60/60
- Battery -30/50

Mathematically what do you use as the limits?  I'd imagine that max motor amps is the rated max amps and the max battery amps should match the max charge rating and the burst discharge with a safety factor, and that the regen braking for each motor should add up to the recharge value but I know that the resistance and duty cycles change them drastically

Why am I an idiot

Note:  The board and me combined is only 150lbs/70kg so I'm gonna get HELLA ACCELERATION (calculated 3m/s/s on start-up)
```

---
## \#2 Posted by: J0ker3366 Posted at: 2019-02-03T01:44:07.246Z Reads: 150

```
Run em @ 60/-60 and go from there

That's 30a per esc
```

---
## \#3 Posted by: Sn4pz Posted at: 2019-02-03T01:44:19.336Z Reads: 147

```
30q does 20a cont with minimal consequences, so a 4p pack can output 80a max, and each vesc should be set to either 
* 40a / 40a - for maximum power(this is gonna knock your socks off, be careful)

Or 

* 30a / 30a, for a build with slightly less acceleration and a significantly longer range (40a per motor is draining af!)
```

---
## \#4 Posted by: Noob-at-building Posted at: 2019-02-03T01:48:35.358Z Reads: 142

```
[quote="ZachTetra, post:1, topic:82973"]
Note: The board and me combined is only 150lbs/70kg so I’m gonna get HELLA ACCELERATION
[/quote] 
i weight like 73kg, with a board that has dual TB 6355 and i want more acceleration, its not as fast as you think
```

---
## \#5 Posted by: ZachTetra Posted at: 2019-02-03T01:55:57.096Z Reads: 132

```
Damn...that's just depressing...what's your gear ratio and wheel diameter?
```

---
## \#6 Posted by: Noob-at-building Posted at: 2019-02-03T01:57:31.648Z Reads: 131

```
16:36  mbs 100mm wheels
```

---
## \#7 Posted by: mynamesmatt Posted at: 2019-02-03T02:11:48.828Z Reads: 126

```
[quote="Noob-at-building, post:6, topic:82973"]
16:36
[/quote]

maybe try 16/40 on that size wheel
```

---
## \#8 Posted by: Noob-at-building Posted at: 2019-02-03T02:35:09.903Z Reads: 122

```
i like my top speed being 60kmh :slight_smile:
```

---
## \#9 Posted by: Indiangummy Posted at: 2019-02-03T03:32:53.820Z Reads: 123

```
what vesc and what motor settings are you using?
```

---
## \#10 Posted by: Noob-at-building Posted at: 2019-02-03T03:52:56.296Z Reads: 119

```
dual flipsky 4.12 running on 12s 
motor max 60a
bat max 30a
```

---
## \#13 Posted by: ZachTetra Posted at: 2019-02-03T04:09:20.303Z Reads: 113

```
What do you mean?
```

---
## \#14 Posted by: ZachTetra Posted at: 2019-02-03T04:27:22.167Z Reads: 112

```
Is the ESC amp limit the max in from the battery or the max out to the motor?

Also updated original post
```

---
## \#15 Posted by: Andy87 Posted at: 2019-02-03T05:34:52.953Z Reads: 107

```
[quote="ZachTetra, post:1, topic:82973"]
What I think is the right amp limits:

* Motor -30/65 each
* battery -40/80
[/quote]

Change that to
Motor -50/65 each
Battery -12/40 each
```

---
## \#16 Posted by: AlexBE Posted at: 2019-02-03T05:59:33.317Z Reads: 100

```
Well that's where your lack of torque is coming from.
```

---
## \#17 Posted by: Noob-at-building Posted at: 2019-02-03T06:00:37.264Z Reads: 101

```
yea, still a very nice speed though to accelerate
```

---
## \#18 Posted by: tony74 Posted at: 2019-02-03T08:37:11.623Z Reads: 91

```
Also new here so feel free to tell me why I'm an idiot - but can you tell me how the dual ESCs are going with dual 6355's .. Im hoping to run a single FSESC 4.12 with a 180 kV 6374 but theres so much mixed info on VESCS, some on this site saying they're limited to 27A continuous which seems unlikely and would surely bottle neck the hell out of almost every build ive seen here...

TIA
```

---
## \#19 Posted by: Andy87 Posted at: 2019-02-03T08:46:07.618Z Reads: 91

```
[quote="tony74, post:18, topic:82973"]
FSESC 4.12
[/quote]

Max batt continues is 35a.
You can try to get higher but I would monitor the temperature or get there heat sink case for the 4.12 vesc.
```

---
## \#20 Posted by: tony74 Posted at: 2019-02-03T08:50:42.899Z Reads: 89

```
Thanks, 
So the rating of 50A is more of like a hard limit? Will 35A not severely limit the motor..?
```

---
## \#21 Posted by: Andy87 Posted at: 2019-02-03T08:54:46.241Z Reads: 86

```
Bat amps not motor amps.
You still can set your motor max to 60a for example.
```

---
## \#22 Posted by: rich Posted at: 2019-02-03T08:59:36.148Z Reads: 90

```
[quote="tony74, post:18, topic:82973"]
some on this site saying they’re limited to 27A continuous which seems unlikely
[/quote]

27A is "real" continious without overheating, everything above (continious) and it's getting hot. Of course you can set the batt max higher than that up to 50A but (in summer) the esc's will reduce power or shut down when hitting temp limits. I would try 35A or 40A first.

[quote="Andy87, post:19, topic:82973"]
Max batt continues is 35a.
[/quote]

Is this for 4.12 as well? I thought that was the limit for the mini fsesc 4.20 only because of over current faults.
```

---
## \#23 Posted by: tony74 Posted at: 2019-02-03T09:01:06.729Z Reads: 83

```
Excellent, thanks guys. 
For context I'm not savvy on the difference and went and bought a simple ESC without knowing it had a max output of 1350 W. barely turns the 6374..

EDIT: speed modes found = problem solved
```

---
## \#24 Posted by: Andy87 Posted at: 2019-02-03T09:02:39.240Z Reads: 85

```
[quote="rich, post:22, topic:82973"]
Is this for 4.12 as well
[/quote]

35a is what i would set max for any 4.12hw based vesc without heat sink.
I didn’t  specifically speak about the Flipsky 4.12
```

---
## \#25 Posted by: rich Posted at: 2019-02-03T09:34:38.963Z Reads: 81

```
According to heat it makes sense :fire: 

2 years ago I had V4.12 (45A batt max each) on my mountainboard and in summer the vescs and motors got boiling hot. I had to take breaks because of vescs cutting power. 

I switched to Vesc6, I've mounted them in a small closed box and even in hottest summer they never overheat.
```

---
## \#26 Posted by: ZachTetra Posted at: 2019-02-03T14:24:53.494Z Reads: 68

```
What is concidered hot for each component and how do you check?
```

---
## \#27 Posted by: Andy87 Posted at: 2019-02-03T14:40:00.289Z Reads: 67

```
Your vesc will power down when reaching 80 degree. At 100 degree he will switch all power off.
You can check that via Bluetooth app.
With motors it’s a bit a different story, but if you can’t touch it it’s definitely too hot 😂
Problem is that the epoxy which hold the magnets can be affected due to overheating and damage your motor permanently
```

---
## \#28 Posted by: ZachTetra Posted at: 2019-02-03T16:53:55.553Z Reads: 62

```
When the motor says 65A max what would be a good continuous amount?
```

---
## \#29 Posted by: rich Posted at: 2019-02-03T18:07:38.490Z Reads: 58

```
That doesn't matter because you only set the max. values :wink:

Basically you wrote the answer for correct settings already:

[quote="ZachTetra, post:1, topic:82973"]
I’d imagine that max motor amps is the rated max amps and the max battery amps should match the max charge rating
[/quote]

Yes, that means max motor amps can be set up to 65A (the rating) each vesc, if they get too hot or deliver too much torque you can lower this setting. I would start with -40A motor regen and test in real life if you need stronger or weaker brakes.

With 12s4p 30Q you can set batt max 40A each vesc. 4A is max. charge per cell so In theory you have only 16A in total with your battery which means a setting of -8A batt regen each vesc. This would be a safe setting. On the other hand I've never seen more than about 50-60% of my max batt regen setting in real life running back to battery. So you could increase the batt regen to -10 or even -15A each vesc (at your own risk) but only if you need stronger brakes at high speed.
```

---
