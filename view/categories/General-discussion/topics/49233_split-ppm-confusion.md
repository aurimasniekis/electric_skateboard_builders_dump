# Split PPM Confusion

### Replies: 34 Views: 1843

## \#1 Posted by: GJHS Posted at: 2018-03-16T00:07:28.728Z Reads: 223

```
Hey Guys.  After reading a bunch on the difference between canbus and Split PPM, I am left with one confusion

Which settings do you split when running dual motors via Split PPM?

I have a dual Kaly 6355 build using FOCBoxes and a 10s4p 30Q battery

BLDC Hybrid

Motor Max: 50a (Kaly Max 60a)
Motor Min (regen): -30a
Batt Max: 50a
Batt Min (regen): -7a
Absolute Max: 130a (default)

I set each vesc individually and did a motor detection for each.  Which settings are split?  I split my regen not sure if Motor Max, since each vesc is running independent?

Can someone clarify and confirm my settings?

Thanks
```

---
## \#2 Posted by: abenny Posted at: 2018-03-16T00:09:05.975Z Reads: 216

```
if im not mistaken you dont split any settings. you set each motor up individually to the foxbox as you would a single drive, and then once theyre both configured individually you connect a y split ppm cable
```

---
## \#3 Posted by: GJHS Posted at: 2018-03-16T00:10:41.267Z Reads: 215

```
I would think at least regen since both motors are sending power back to one battery
```

---
## \#4 Posted by: faithfulpuppy Posted at: 2018-03-16T00:10:49.290Z Reads: 202

```
yes, you split the (usually white) wire coming out of your ~~resistor~~ receiver. leave the black and red only connected to one ESC though.
```

---
## \#5 Posted by: faithfulpuppy Posted at: 2018-03-16T00:11:53.990Z Reads: 194

```
you mean like what should divide in two? yeah, if you only want 40a regen then set each esc to 20.
```

---
## \#6 Posted by: GJHS Posted at: 2018-03-16T00:12:37.499Z Reads: 186

```
I was worried about Battery Max
```

---
## \#7 Posted by: faithfulpuppy Posted at: 2018-03-16T00:14:41.857Z Reads: 175

```
whatever the number you set for one ESC is, the two ESCs together will do double that. If you set batt max to 60 on each ESC, they can draw up to 120 together. 

the ESCs aren't "aware" of each other's existence, treat them like two seperate systems
```

---
## \#8 Posted by: GJHS Posted at: 2018-03-16T00:16:31.993Z Reads: 166

```
Ok that's what I thought so 10s 30Q 15a discharge, I am fine with 50a for each, right?

How would you set it lower than the Motor Max?
```

---
## \#9 Posted by: faithfulpuppy Posted at: 2018-03-16T00:18:38.156Z Reads: 165

```
what's your parallel number? 10s doesn't tell me much about max current
```

---
## \#10 Posted by: GJHS Posted at: 2018-03-16T00:19:14.010Z Reads: 161

```
10s4p 30Q Battery
```

---
## \#11 Posted by: b264 Posted at: 2018-03-16T00:20:12.237Z Reads: 156

```
Motor Min and Battery Min should both be negative.
```

---
## \#12 Posted by: faithfulpuppy Posted at: 2018-03-16T00:20:34.318Z Reads: 153

```
with 4p, your maximum discharge is 15 * 4 = 60a, 60/2 = 30, so i wouldn't do over 30a per vesc
```

---
## \#13 Posted by: GJHS Posted at: 2018-03-16T00:21:01.085Z Reads: 148

```
yes sorry I will correct the post
```

---
## \#14 Posted by: E1Allen Posted at: 2018-03-16T00:23:02.829Z Reads: 145

```
Also does your battery have a Max discharge limit BMS of 60 or 80 amps. Don't want to exceed that either
```

---
## \#15 Posted by: Sebike Posted at: 2018-03-16T00:23:59.794Z Reads: 144

```
Wait a second... I'd say batt max and min should be no more than half of what you would have set for a single motor system, unless you're running the vescs off of two separate batteries...
```

---
## \#16 Posted by: GJHS Posted at: 2018-03-16T00:25:31.551Z Reads: 142

```
Even if the Vesc are running independent?
```

---
## \#17 Posted by: Sebike Posted at: 2018-03-16T00:33:49.016Z Reads: 141

```
Someone correct me if I'm wrong, but yes, even when vescs are running independently. 

Batt max is roughly how much each vesc is allowed to pull from the battery, right, and that shouldn't exceed half of what the battery can safely deliver if you have two vescs pulling amps from your batts. 

Batt min is how much you allow vesc to pump back into the batt, and cell specs stay the same even if you'd have 10000000 independent vescs 😊, so you don't want to charge cells with heavier current just because you happen to run dual motors.
```

---
## \#18 Posted by: GJHS Posted at: 2018-03-16T00:36:03.471Z Reads: 133

```
See, confusing.  If I set my battery max to  25a wouldn't it be the same as setting my Motor to 25a?
```

---
## \#19 Posted by: Sebike Posted at: 2018-03-16T00:40:43.970Z Reads: 135

```
Short answer is no. If battery max and motor max were the same thing, we wouldn't have two separate settings 😏 A bit confusing yes.
```

---
## \#20 Posted by: GJHS Posted at: 2018-03-16T00:43:12.777Z Reads: 134

```
So if I set my Battery Max to 25a i shouldn't see any performance difference?
```

---
## \#21 Posted by: Deckoz Posted at: 2018-03-16T00:47:03.097Z Reads: 127

```
30q are know to be 20a cells even though they are 15 by the manufacturer

4p * 20a = 80a / 2esc = 40a/esc bat max

Regen no more then 2c
3Ah * 4p = 12Ah * 2capacity = 24a/2esc = -12a bat min per esc
```

---
## \#22 Posted by: Sebike Posted at: 2018-03-16T00:47:42.288Z Reads: 126

```
You could probably set your batt max to 30 if your  bms allows a 60a discharge,  and you won't kill your batteries. So with batteries that are still working, I'd say that's a performance boost 😁
```

---
## \#23 Posted by: GJHS Posted at: 2018-03-16T00:49:18.490Z Reads: 125

```
I don't have a discharge BMS, only a 80a charge only
```

---
## \#24 Posted by: Deckoz Posted at: 2018-03-16T00:50:00.891Z Reads: 121

```
Regarding motor amps vs battery amps

https://www.electric-skateboard.builders/t/the-derek-evo-4wd/49103/37?u=deckoz
```

---
## \#25 Posted by: Sebike Posted at: 2018-03-16T00:59:10.225Z Reads: 118

```
Then either go the conservative route with 30a batt max per vesc, or go crazy with the - up to- 40a /vesc.. I don't think one should exceed that though.
```

---
## \#26 Posted by: GJHS Posted at: 2018-03-16T01:00:29.274Z Reads: 118

```
to think I have been running 50a for weeks.  Luckily short rides
```

---
## \#27 Posted by: Sebike Posted at: 2018-03-16T01:01:08.649Z Reads: 118

```
80a bms for charging only is unnecessary bulk. You could as well use something a lot smaller.
```

---
## \#28 Posted by: Deckoz Posted at: 2018-03-16T01:23:44.851Z Reads: 116

```
The gist I got from PM

It's a 6355. Which are typically rated for 2000w. 

On a dual setup of 4p 30q with a max batt amp of 40/esc or less to maintain the constant current capability of the cells

2000w \ 36v = 55 amps...

Your battery can only provide 40 amps

36v * 40a = 1440w

If you set a motor max of 60. You can achieve 60 motor amps up until 24v or 66% duty cycle. At which point every % of duty cycle increase will cause a motor amper output decrease to stay within the 40a(1440w) battery max limitation.

Basically your battery can't overpower the motor..
```

---
## \#29 Posted by: Nordle Posted at: 2018-03-16T15:09:22.748Z Reads: 102

```
[quote="faithfulpuppy, post:4, topic:49233"]
yes, you split the (usually white) wire coming out of your resistor.
[/quote]
It's the white wire coming out of your "receiver", sure there are also resistors inside that one, but 2 different storys actually
```

---
## \#30 Posted by: professor_shartsis Posted at: 2018-03-16T16:46:05.000Z Reads: 96

```
@GJHS here is some related information from a different discussion: 

[quote="professor_shartsis, post:20, topic:49277, full:true"]
an esc works by a similar principle to a dc to dc buck converter in continuous mode which can also lower the effective voltage while increasing the amps. **the battery is periodically connected and then disconnected from the winding at a frequency on the order of 25khz. During the times the winding is disconnected from the battery, the winding is shorted to itself which allows the current generated during the brief on times to continue circulating during the off times. since the current continues to flow in the winding during the off times, the “motor amps” are numerically higher than the “battery amps.”** the battery may see 10a @ 50v, 10% of the time which averages to 1a, while the motor effectively sees 10a @ 5v the entire time. In reality the current rises in the motor from, say, 9.5a to 10.5a during the 10% on times, then decays from 10.5a to 9.5a during the off times.

as the back emf voltage produced by the motor increases with increasing speed, it is necessary to increase the on time (duty cycle) of the circuit to maintain the same number of motor amps, which draws more and more battery amps.

**Pack V * duty cycle % = V effective**

(V effective - V bemf)/Resistance=Motor Current
[/quote]

[quote="professor_shartsis, post:22, topic:49277"]
**50v battery * 10% duty = 5v effective volts**

**(5v effective - 0v bemf) / 0.0625ohm winding = 80a motor amps**

5v * 80a motor amps = 400w electrical watts

80a motor * 80a motor * 0.0625ohm = 400w copper loss

400w / 50v battery = 8a battery amps
[/quote]

[quote="professor_shartsis, post:24, topic:49277, full:true"]
(1/KV)*RPM=BEMF V

(1/100kv)*100RPM=1V BEMF
[/quote]

[quote="professor_shartsis, post:28, topic:49277, full:true"]
KT (torque per amp) can be calculated directly from KV:

**KT (newton meters torque per motor amp) = 60/(2 * pi * kv)**

**0.0954nm/a = 60/(2 * pi * 100kv)**

**therefore 80a motor current * 0.0954nm/a = 7.632 newton meters torque @ 100kv**

7.632 newton meters torque * angular speed of the motor in radians per second = mechanical watts

(1000rpm * 2 * pi)/60 = 104.719 rad/sec

7.632 newton meters torque * 104.719 radians per sec angular speed= 799.22w mechanical power

799.22w mechanical power / 1000w electrical power = 79.92% electrical to mechanical efficiency

the difference between the electrical power and mechanical power appears as ohmic heating in the motor windings.
[/quote]
```

---
## \#31 Posted by: faithfulpuppy Posted at: 2018-03-16T17:29:46.910Z Reads: 80

```
Whoops, that was a hell of a slip. Stupid fingers.
```

---
## \#32 Posted by: Deckoz Posted at: 2018-03-16T18:30:08.369Z Reads: 78

```
That reminds me...I once accidentally text a real estate agent I shampooed my balls instead of the carpet...

It was really awkward after that as I didn't catch it for a day or two when I wondered why he never responded. @faithfulpuppy
```

---
## \#33 Posted by: abenny Posted at: 2018-03-17T17:12:40.195Z Reads: 72

```
he was obviously giving you time to clean the carpet before he came to look at the house :joy:
```

---
## \#34 Posted by: mattyB Posted at: 2019-04-07T04:45:17.541Z Reads: 26

```
what is PPM?
```

---
