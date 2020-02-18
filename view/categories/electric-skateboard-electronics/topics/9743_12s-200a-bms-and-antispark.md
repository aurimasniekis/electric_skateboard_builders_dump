# 12S 200A - BMS and AntiSpark

### Replies: 23 Views: 2539

## \#1 Posted by: racidon Posted at: 2016-09-17T12:01:41.023Z Reads: 236

```
So I've been searching around for a BMS and AntiSpark that can handle 200A. I think I need this due to me going with a motor that has a max current of 120A (getting 2 for now, but may end up with 4). Suggested ESC for this is at least 180A 12S ESC. I've got ahold of 2 of these: http://www.hobbyking.com/hobbyking/store/__25202__Turnigy_dlux_250A_HV_14s_60v_ESC.html 
Let me know if I've done my math wrong? I'd love to be able to use my motors to their full potential thus I don't want to blow shit up :slight_smile:TIA for any help guys
```

---
## \#2 Posted by: Jinra Posted at: 2016-09-17T12:03:39.616Z Reads: 238

```
you do not need a 200 amp bms. 60-80a is likely more than you'll ever pull, even less at 12s.
```

---
## \#3 Posted by: racidon Posted at: 2016-09-17T13:56:35.768Z Reads: 225

```
even with a 5kw motor?
Just don't want shit to burn out. Obviously for something this powerful I'll be putting in fuses and such. But still xD
```

---
## \#4 Posted by: Jinra Posted at: 2016-09-17T13:58:46.967Z Reads: 216

```
what motor do you have that is 5000w? Also, you won't utilize all the power of it. It has the potential to draw the specified wattage, doesn't mean you will. You'd probably have to be climbing vertically with a 300lb load for that.
```

---
## \#5 Posted by: racidon Posted at: 2016-09-17T14:26:45.705Z Reads: 195

```
http://www.hobbyking.com/hobbyking/store/__17987__Turnigy_RotoMax_50cc_Size_Brushless_Outrunner_Motor.html
:slight_smile:
```

---
## \#6 Posted by: Jinra Posted at: 2016-09-17T14:29:41.996Z Reads: 186

```
Yea that's way overkill. You don't need that much for esk8.
```

---
## \#7 Posted by: michaeld33 Posted at: 2016-09-17T14:30:23.522Z Reads: 180

```
Yeah man that's wayy overkill, you're gonna need a different kind of motor for an esk8.
```

---
## \#8 Posted by: racidon Posted at: 2016-09-17T14:58:35.697Z Reads: 173

```
I know it's overkill, that's the point
```

---
## \#9 Posted by: Jinra Posted at: 2016-09-17T15:00:13.569Z Reads: 171

```
It's a lot of wasted power that won't ever be utilized, what's the goal?
```

---
## \#10 Posted by: racidon Posted at: 2016-09-17T15:06:41.343Z Reads: 165

```
does it not mean I could easily gear this whatever I want? worse case I would have 2 motors for 2 op boards?
```

---
## \#11 Posted by: Jinra Posted at: 2016-09-17T15:10:26.707Z Reads: 161

```
the esc you linked is an airplane esc and won't work for esk8 as well, unless you have another method for braking. There's a reason the VESC only outputs 50A because you don't need all that power on demand. Too much acceleration will make it unrideable and will destroy your wheels.
```

---
## \#12 Posted by: michaeld33 Posted at: 2016-09-17T15:10:43.682Z Reads: 158

```
Imagine taking a plane engine. and putting it on a go kart.
```

---
## \#13 Posted by: rpn314 Posted at: 2016-09-17T15:29:02.421Z Reads: 151

```
...for science! :smiley:

But yeah, that motor is overkill to a whole new level. @Jinra's words are wise.
```

---
## \#14 Posted by: racidon Posted at: 2016-09-17T15:41:55.966Z Reads: 155

```
hmm didn't even look at braking to be honest -.-
it had said default "brake - off" but didn't say no braking, how would you know ?
```

---
## \#15 Posted by: SimosMCmuffin Posted at: 2016-09-17T15:56:55.914Z Reads: 155

```
Airplane ESCs have 2 braking options. No brake, or hard, non-adjustable brake.
Car ESCs would be a much better idea.
```

---
## \#16 Posted by: Namasaki Posted at: 2016-09-17T22:34:55.461Z Reads: 136

```
[quote="michaeld33, post:12, topic:9743, full:true"]
Imagine taking a plane engine. and putting it on a go kart.
[/quote]


Sounds like fun!!!!! LoL
```

---
## \#17 Posted by: lowGuido Posted at: 2016-09-18T05:24:36.917Z Reads: 119

```
I WANT you to use that motor.
and I want to see it in action.
I also want crazy gearing for like 70Mph..

chop chop, make it happen.
```

---
## \#18 Posted by: Jinra Posted at: 2016-09-18T05:29:34.563Z Reads: 121

```
RIP racidon
```

---
## \#19 Posted by: racidon Posted at: 2016-09-18T08:35:07.287Z Reads: 112

```
I plan to, but I wasn't aware of the lack of braking capabilities in that ESC even though HK recommended it so I will need to organise another. Probably one from Alien Power System
```

---
## \#20 Posted by: smurf Posted at: 2016-09-18T09:36:02.934Z Reads: 109

```
Ok let's think this through
2 motors at 5kw for 10kw

horsepower is equal to 745.699872 watts:

1 hp(I) = 745.699872 W

So the power conversion of watts to horsepower is given by:

P(hp) = P(W) / 745.699872

13.41 horsepower

Now assuming you're a average weight human you will have a power to weight ratio about the same as a 6 cylinder sports car!
```

---
## \#21 Posted by: saul Posted at: 2016-09-18T10:08:22.078Z Reads: 108

```
why not go quad 6374? 
12s, 50v*50A = 2500 x 4 = 10 KW!
or 14s LiFe 26650

and you can use a quad vesc....costs about the same as those escs...

either way can't wait to see it! :thinking:
```

---
## \#22 Posted by: daanstoorvogel Posted at: 2016-09-18T10:16:40.853Z Reads: 106

```
i was thinking to mount this on a ebike ! , then i got hooked on skateboards.  do you want to go dual with this ??  ( i mean we have seen 2 outrunners wich provide about the same as one of these so, for sience ! ) would be sick to see 2 of these chain driven and geared for wheelies on a trampa !
```

---
## \#23 Posted by: racidon Posted at: 2016-09-18T10:24:24.015Z Reads: 101

```
[quote="daanstoorvogel, post:22, topic:9743, full:true"]
i was thinking to mount this on a ebike ! , then i got hooked on skateboards.  do you want to go dual with this ??  ( i mean we have seen 2 outrunners wich provide about the same as one of these so, for sience ! ) would be sick to see 2 of these chain driven and geared for wheelies on a trampa !
[/quote]

to be totally honest I first wanted to go the leopards 175kv quad but that was going to be quite a stuff around. So I was going to go quad of these. and well thought 2 was going to be mega overkill and honestly not sure they would fit two side by side. The gearing I Think will have to be quite large due to the design of the motors .

@smurf It's basically a very light weight dirtbike equivalent.
```

---
