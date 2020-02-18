# E-MTB motor kv vs gear ratio

### Replies: 6 Views: 546

## \#1 Posted by: FredrikHems Posted at: 2018-04-27T22:32:06.491Z Reads: 118

```
So I have come to the point where I have start thinking about what motor kv and gearing I should use for my future E-MTB build. I want to do pretty heavy offroading, so ground clearance is important. The plan is to use a pretty standard trampa board with 200mm/8inch wheels. So I want to hear your opinion on this:

130kv with 1:4 ratio 
VS
90kv with 1:3 ratio 
Both would be on 12s and would give around 43 km/h top speed :wink:

And if there would be any, what do you think about the torque difference in these setups?
The 90 kv would leave significantly more room for ground clearance, which cant be bad for an offroad build :yum:
```

---
## \#2 Posted by: Der6FingerJo Posted at: 2018-04-27T23:06:58.768Z Reads: 106

```
If the motors are otherwise identical the 130kv motor would be able to carry more amps since it has fewer, probably thicker, windings which is why i would tend to use 130kv over 90kv.

However some motors are connected differently internally. It's called delta or wye connection. Essentially delta connected motors achieve a higher top speed than wye connected motors using the same windings (the factor is cubic root of 3).

If the 90kv motor is a 150kv delta motor switched over to wye it could be batter amp wise. If it's however a regular delta motor it can't handle that much current.

I know this is hard to understand at first, but if you want to read up on it you can also find this under star/delta keywords.

Oh and i also think that the mechanical stress on the motor itself would be less with 1:4 gearing, so that is a bonus point for 130kv too.

Personally i'm very much a fan of my 130kv overion motors, which are branded maytech motors. They are somewhat sealed and have hall sensors, perfect for mtb.
```

---
## \#3 Posted by: Acido Posted at: 2018-04-27T23:28:13.096Z Reads: 90

```
Shoot for around 45kmh 
Im building a 12s 190kv board with 1:5 or 1:5.5 gear ratio on 8inch wheels
If you want clearance put the battery between your legs and get a mount that can be as vertically mounted as possible
```

---
## \#4 Posted by: professor_shartsis Posted at: 2018-04-27T23:50:30.785Z Reads: 87

```
130kv, 2 motors, 4:1 reduction, 90a motor limit, 60a battery limit, 200mm tire, 46v battery, 0.1ohm winding:
https://image.ibb.co/kArXjH/130kv.jpg

90kv, 2 motors, 3:1 reduction, 90a motor limit, 60a battery limit, 200mm tire, 46v battery, 0.1ohm winding:
https://image.ibb.co/mxidPH/90kv.jpg

geared for speed: ~55mph (bottom left & top middle charts)
130kv, 2 motors, 2:1 reduction, 90a motor limit, 60a battery limit, 200mm tire, 46v battery, 0.1ohm winding:
https://image.ibb.co/meRCJc/55mph.jpg
```

---
## \#5 Posted by: FredrikHems Posted at: 2018-04-28T09:47:36.244Z Reads: 60

```
@Acido  Yea, I have heard the trampa boards arent really made for speed :yum: 
The ground clearance I am talking about is the one from the wheel gear down to the ground, as this will sit far lower than the motor mount itself :wink: The plan is to top mount the batteries

@professor_shartsis If only I would understand 1/10 of these graphs, haha :joy::sweat_smile:
@Der6FingerJo Thank for the info dude, I have not really read too much about the delta vs wye, but the motors are from APS if that would matter :smiley:
```

---
## \#6 Posted by: Der6FingerJo Posted at: 2018-04-28T15:03:37.098Z Reads: 55

```
@professor_shartsis damn that's impressive! Haven't seen something like it before, still trying to process all the information :D
```

---
