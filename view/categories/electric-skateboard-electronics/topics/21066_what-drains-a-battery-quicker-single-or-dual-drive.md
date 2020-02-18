# What drains a battery quicker, single or dual drive?

### Replies: 14 Views: 1145

## \#1 Posted by: thisguyhere Posted at: 2017-04-15T05:49:18.754Z Reads: 177

```
what would drain a pack quicker, a single or dual drive setup?

with a single, it'd draw more current since the one motor would be working harder to get up to speed, climb hills, etc.

with a dual, it's spreading the work across two motors so less of a draw, right?  but since it's two, is it equivalent as what a single motor would draw?

don't need anything scientific, just wondering.
```

---
## \#2 Posted by: willpark16 Posted at: 2017-04-15T06:11:30.568Z Reads: 170

```
Depends weather ur talking about a lot of hills or not and the type of motors
```

---
## \#3 Posted by: Jebe Posted at: 2017-04-15T06:19:40.905Z Reads: 169

```
I think dual drains quicker - motors have an efficiency point at around 70%.
On my single 3kw today I did 26km and had 37volts left :slight_smile:
mix of hills and flats
```

---
## \#4 Posted by: Namasaki Posted at: 2017-04-15T06:27:14.777Z Reads: 168

```
I would guess it's about the same since the load is the same with one motor or two and with two motors, your dividing the load in half.
So a single motor is working twice as hard as dual motors.
I'm guessing that range will not differ much if any but wear on the motor and controller will be less with dual drive.
acceleration and braking will feel better because of more even distribution of torque.
```

---
## \#5 Posted by: Namasaki Posted at: 2017-04-15T06:30:09.991Z Reads: 161

```
How many MHA  is your battery pack?
```

---
## \#6 Posted by: Jebe Posted at: 2017-04-15T06:31:30.023Z Reads: 153

```
10aH 10s4p
```

---
## \#7 Posted by: Namasaki Posted at: 2017-04-15T06:33:53.312Z Reads: 153

```
My battery is only 5ah 10s and I get 12 miles with hills and flats on dual 6355 190kv motors
both Vescs have these settings: motor max 80a / batt max 50a
```

---
## \#8 Posted by: thisguyhere Posted at: 2017-04-15T06:40:47.055Z Reads: 150

```
riding to work it's like a 100ft climb across a mile or so, steepest being about a 10% grade, i would guess.

at the moment running a single 6374 with a 10s4p pack, have the vesc bldc set at 60a motor max.
```

---
## \#9 Posted by: Jebe Posted at: 2017-04-15T06:43:25.281Z Reads: 145

```
do you have a gps tracking app? 
Record your mileage and your voltage before and after your run.
Do this a few times and you can average out your watts/mile
```

---
## \#10 Posted by: thisguyhere Posted at: 2017-04-15T06:46:34.155Z Reads: 137

```
good point, i have been intermittently tracking my rides but didn't correlate it to voltage drain.
```

---
## \#11 Posted by: willpark16 Posted at: 2017-04-15T07:13:32.131Z Reads: 127

```
Why not go 45a and in answer to ur question the single should give u more range
```

---
## \#12 Posted by: thisguyhere Posted at: 2017-04-15T08:19:38.641Z Reads: 115

```
yea tried lower amp draw and didn't like it.  feels sluggish.  going full bore!
```

---
## \#13 Posted by: laurnts Posted at: 2017-04-15T10:02:05.014Z Reads: 106

```
I thought dual is equal to single at the beginning, but the truth is that single large motor is always more efficient. I have build dual hub, dual belt and single belt. Single belt motor or single hub is really efficient.v

I think it has something to do not only with load. My motor have very low kv, 190 or below. On accelerating true, they split the load equally. But on high speed (max rpm) each motor still consume power as they need to spin anyway in order to balance out the load. The mechanical loss also double up.

In the end, dual could be more efficient when you're in an event when one motor cant handle the load. Hills climbing and insane acceleration would benefit from dual. Constant high speed run, a single motor would be wayyy more efficient.
```

---
## \#14 Posted by: Jebe Posted at: 2017-04-15T10:13:06.232Z Reads: 100

```
braking is better with 2 - dont have to have the belt so tight as one where you get cogging braking hard but I still doubt the savings in regards to more friction for one belt verses less tension on tight belts would equal out,
```

---
