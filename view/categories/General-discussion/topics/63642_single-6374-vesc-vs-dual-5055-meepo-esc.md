# Single 6374 VESC vs dual 5055 MEEPO ESC?

### Replies: 11 Views: 566

## \#1 Posted by: Jmding Posted at: 2018-08-02T20:19:57.700Z Reads: 132

```
Building my first board, aiming for a lightweight daily commuter with about 10 mi range, 22 mph top speed, and enough torque to carry my 210 lb frame up SF hills. And all this on a budget 

Was planning on going 10s1p LiPo, paired with either
1) a single 6374 and a VESC or
2) dual 5055s and the Chinese ESC/receiver combo that is common on eBay, and used in the MEEPO and similar

The total build price, nominal total motor wattage, and even max ESC continuous current are similar across both setups but these ratings are so untrustworthy that I was hoping to get your practical opinion on this. There's also the matter of 1WD traction being inferior to 2WD, and the VESC control interface (once properly set up) being much superior to the MEEPO ESC's... Any thoughts?
```

---
## \#2 Posted by: boardman Posted at: 2018-08-02T20:42:33.998Z Reads: 125

```
What is the mAH capacity on the lipo? I don't think you're going to be able to get that 10 mile range you want from it unless it exceeds 4ah
```

---
## \#3 Posted by: Jmding Posted at: 2018-08-02T21:26:54.065Z Reads: 122

```
5000 mAh is the quoted capacity
```

---
## \#4 Posted by: DAddYE Posted at: 2018-08-02T21:34:17.592Z Reads: 121

```
Meepo/wowgo/ownboard have ESC that works amazingly well on HUB motors, they’re not meant for belt ones. 

I’m from SF as well and I don’t think a 6374 10s can bring you up step hills. 

I would suggest to get a Turnigy 6376 (145kv 45a ... amazing beast) or the TB 6480. 

However you’re in SF you might want two motors because if one belt breaks while you’re on a downhill your are screwed

I’ll suggest to get two 6355, 12s and two VESC from hobby king.
```

---
## \#5 Posted by: Jmding Posted at: 2018-08-02T22:53:29.039Z Reads: 110

```
The MEEPO etc ESCs struggle with belt drives because they are electronically limited to something like 8000 eprm to electronically limit top speed for their hub motor configurations, but you can get the "belt drive" version of the MEEPO ESC that doesn't have this limit. I'm more concerned about the relative quality of the ESC and the apparently jerk behavior of the controls (YouTube reviewers seem to complain somewhat about this with the MEEPO).

Yeah, it may not be enough heat dissipation given the grade and my weight, but which setup do you think would do better on an Sf hill though, the single 6374 or dual 5055? Or just generally, which setup do you think would perform better?
```

---
## \#6 Posted by: torqueboards Posted at: 2018-08-02T23:09:33.678Z Reads: 99

```
I wouldn't cheap out on it if your climbing SF hills.. You end up going single motor and you climb too many hills, you'll burn out motor #1. Then you'll have to buy 2 more motors for a dual motor setup. In total that's 3 motors when you could of bought 2 to begin with :). If you're not climbing many hills and on flat ground, single 6374 or 6355 that way you can upgrade to a dual later on.
```

---
## \#7 Posted by: Grozniy Posted at: 2018-08-02T23:46:13.540Z Reads: 95

```
My opinion:
Get 1 vesc
Get 1 sk3 6374(it's actually bigger than stated, around 80mm long)
Get at least 15mm HTD5M belt
Get 40/44T wheel pulley on 90mm(83mm would have even more torque) wheels and 15T motor pulley for torque
You'll need around 20Wh * 16km = 320Wh. So 10S 8Ah with >20C lipo or a 10S3P 30Q or 10S2P 20700b cells.
If you didn't need hill climbing, you could get away with 10wh * 16=160Wh
```

---
## \#8 Posted by: Jmding Posted at: 2018-08-02T23:55:42.610Z Reads: 89

```
So better to go dual 5055 / MEEPO ESC?

I get the feeling dual 63XX is overkill and unnecessary board weight, given that boosted uses what appears to be dual 5030 motors. The thing that gives me hope for the single motor solution is that  if you compare the quoted wattage of sk3 5055 and 6374 motors, the 6374 is supposed to handle as much power as dual 5055s. Again, nominal ratings aren't trustworthy, but given the numbers are all from the same source, and given boosted is using motors barely half the size of a pair of 5055s, it kinda seems like a single 6374 would be enough. Then again if you're telling me that people are burning out their motors climbing hills with 63XX boards geared to sabe, ~20 mph top speeds, there's no arguing with the evidence.
```

---
## \#9 Posted by: torqueboards Posted at: 2018-08-03T01:57:19.453Z Reads: 84

```
I wouldn't bother dual 5055's unless you're riding specifically on flat ground. Even boosted upgraded from 50mm motors to 63mm motors. Boosted are probably running 6330-6340 sized motors. Marbel upgraded from 50mm to 63mm. Evolve is probably running 5070s. 5055's are easier to burn out because they are smaller + they can't handle as much heat or can heat up quicker. Evolve customers are upgrading to 63mm. 63mm motors are bigger and more forgiving.

Mostly, it depends on if you're climbing 5-10+ hills back to back or if you're just climbing 1 hill. If it's just 1 hill then you can almost use any of the options.

Single 6374 (if you're staying single) or Dual 6355.

It's not worth $15-30/motor to go cheap. Remember, you're standing on this as well as on a steep hill either uphill or downhill. Last thing you want is your motor to crap out in the middle of a hill. You're life is worth more then a few dollars in my opinion.
```

---
## \#10 Posted by: Wilsonliang777 Posted at: 2018-08-03T02:19:26.937Z Reads: 77

```
I am running dual 5065 190kv (racerstar $45) lipo 9s 7000mah 25c with eBay cheap belt ESC, 90mm wheels.  This setup gets me 8 to 10 miles on flat and max 22mph.  It gets me up some hills but if I am doing hills all the time I might get around 5miles on a charge.   I got my esc from  dicky for around $65, no need to buy it from meepo or wowgo.    The esc works very well but becarefull on the brakes.   Brakes are strong and sudden.
```

---
## \#11 Posted by: dareno Posted at: 2018-08-03T04:08:31.575Z Reads: 65

```
I live in a very hilly area and went through the same thing you are right now and it cost me more in the long run.  Hills put a lot of pressure on you gear so overkill does not exist.  I weigh about the same as you and the only thing that pulls me up hills comfortably is my dual 6374 on 10s.  Originally it had 50mm motors on it and they were getting very hot after a few ks so I upgraded and so far so good with about 40 cycles through the battery.  If you're big get big motors and a decent battery or you will regret it in the long run.good luck and enjoy
```

---
