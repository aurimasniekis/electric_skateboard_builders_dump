# Pulling 80a from VESC 4.12?

### Replies: 9 Views: 264

## \#1 Posted by: skaterscooter Posted at: 2019-03-12T19:16:48.906Z Reads: 87

```
I have an electric bike and am using a VESC 4.12 to control it. I'm wanting to see how much power I can squeeze out of it but am aware of the '50A continuous' and '240A Max' ratings of the VESC. At the moment, I run my motor at 65A and the VESC only starts to heat up if I'm going up a steep hill - I'm working on some basic heatsinks. With enough cooling, is there any reason why the VESC couldn't handle 80A? Of course that would only be whilst accelerating so only for a few seconds. Any thoughts?
```

---
## \#2 Posted by: Andy87 Posted at: 2019-03-12T19:25:07.409Z Reads: 83

```
As long as you can hold the vesc running cool all should be fine.
What’s your batt max settings at the moment?
Most people get overheating issues from 40A.
This on a hw4.12 based vesc without heatsink.
```

---
## \#3 Posted by: skaterscooter Posted at: 2019-03-12T19:46:22.844Z Reads: 73

```
Sounds good! Haven't had any overheating issues and batteries have plenty of ventilation. I'll push it and see what happens.
```

---
## \#4 Posted by: Sn4pz Posted at: 2019-03-12T19:50:17.691Z Reads: 69

```
Is there a chance the wheel will lock up if the vesc blows?

If that happens... O.o
```

---
## \#5 Posted by: skaterscooter Posted at: 2019-03-12T19:56:31.245Z Reads: 65

```
Doubt it would totally lock up. I've tried shorting all the motor wires together and it's like a strong brak being applied. As it's on the back wheel it should be an abrupt stop. Fingers crossed it doesn't go the other way and accelerate like mad :slight_smile:
```

---
## \#6 Posted by: Gamer43 Posted at: 2019-03-12T19:59:12.000Z Reads: 65

```
The max amount of current depends heavily on whether you are running BLDC or FOC, there is basically twice as much heat generated in FOC than in BLDC.
80A on BLDC is like 16W of power, and close to 28W on FOC.
Because of the 4.12's odd shape, I would say even with a heatsink, 20W would cause it to start overheating.

[quote="skaterscooter, post:5, topic:86976"]
Doubt it would totally lock up. I’ve tried shorting all the motor wires together and it’s like a strong brak being applied. As it’s on the back wheel it should be an abrupt stop. Fingers crossed it doesn’t go the other way and accelerate like mad :slight_smile:
[/quote]

The abrupt braking force is still enough to throw a rider off the board, but it requires multiple MOSFETs to fail short, which is extremely unlikely.

Since brushless motors don't suck total and complete garbage like brushed motors do, any failure in the ESC will result in the motor coasting to a stop.
```

---
## \#7 Posted by: Sn4pz Posted at: 2019-03-12T20:04:53.619Z Reads: 56

```
[quote="Gamer43, post:6, topic:86976"]
The max amount of current depends heavily on whether you are running BLDC or FOC, there is basically twice as much heat generated in FOC than in BLDC.
[/quote]

??? This is the first Ive heard about this... 

I always thought 

[quote="AutoItKing, post:2, topic:66710"]
FOC runs the motor more efficiently and quieter at a cost of higher switching losses
[/quote]
```

---
## \#8 Posted by: Gamer43 Posted at: 2019-03-12T20:10:38.047Z Reads: 50

```
[quote="Sn4pz, post:7, topic:86976"]
> The max amount of current depends heavily on whether you are running BLDC or FOC, there is basically twice as much heat generated in FOC than in BLDC.

??? This is the first Ive heard about this…

I always thought

FOC runs the motor more efficiently and quieter at a cost of higher switching losses
[/quote]


The motor runs cooler, but the ESC runs hotter.
I should have specified that the additional heat generated is in the ESC, my bad.
FOC also has higher conduction losses at the same RMS current. (all three phases are actively conducting while in BLDC only two phases are conducting, however, to achieve the same RMS current on FOC as BLDC, peak currents are higher).
```

---
## \#9 Posted by: Sn4pz Posted at: 2019-03-12T20:18:14.496Z Reads: 46

```
Ah :man_facepalming:

I should have understood :P
```

---
