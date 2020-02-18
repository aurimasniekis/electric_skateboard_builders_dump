# Mixed up sensor cables

### Replies: 17 Views: 202

## \#1 Posted by: seaborder Posted at: 2019-03-28T19:46:16.803Z Reads: 88

```
Hey guys I have a little problem I mixed up the sensor cables from my motors because I cutted them half a year ago and now I dont know anymore what color is which. Is there a way to measure that? Or open the motor? Its the one from okp

Thanks!
```

---
## \#2 Posted by: Andy87 Posted at: 2019-03-28T19:54:56.650Z Reads: 86

```
The red one is the positive 

The black one is the ground

Both need to be on the opposite ends of the jst.

The yellow one is next to the black in direction to the middle of the jst and is the temp sensor.

The rest doesn’t matter in which row you connect them, it’s just the hall sensors
```

---
## \#3 Posted by: seaborder Posted at: 2019-03-28T20:00:19.840Z Reads: 83

```
Ill check that
```

---
## \#4 Posted by: seaborder Posted at: 2019-03-28T20:11:24.063Z Reads: 75

```
Ok did everything like that but still bad detection result in the vesc tool. :/
```

---
## \#5 Posted by: olestra Posted at: 2019-03-28T20:15:53.038Z Reads: 72

```
try switching the middle 3 around, there's only like 6 possible combos
```

---
## \#6 Posted by: seaborder Posted at: 2019-03-28T20:16:29.738Z Reads: 68

```
Iam wondering if the hall sensores are broke and I did not recognized it the whole time while riding
```

---
## \#7 Posted by: seaborder Posted at: 2019-03-28T20:37:41.330Z Reads: 63

```
Ok still bad detection result. Somehow I want to know why because early today it worked. Than I had to solder all the connections new in the new build and now the detection wont work.
```

---
## \#8 Posted by: seaborder Posted at: 2019-03-29T19:22:03.799Z Reads: 44

```
ok one sensor worked again the other one not. I was just riding sensorless and man I have to say this @okp motors are sooo awesome!! I recognized it barely that there are no sensors.

:)
```

---
## \#9 Posted by: seaborder Posted at: 2019-03-29T19:22:56.385Z Reads: 39

```
At least one part less that cant break anymore
```

---
## \#10 Posted by: ARetardedPillow Posted at: 2019-03-29T20:07:00.253Z Reads: 36

```
Send pictures
```

---
## \#11 Posted by: dareno Posted at: 2019-03-29T20:29:05.214Z Reads: 35

```
Sensors are for pussies  
Just use the remote like a switch and you never have to worry about cogging.  :sunglasses:
```

---
## \#12 Posted by: wafflejock Posted at: 2019-03-29T20:34:21.968Z Reads: 32

```
Will be trying sensored motor for the first time over the weekend, I recently switched from BLDC to FOC mode and holy hell what a difference, didn't even realize this motor could possibly run so quiet, only problem now is I'm unsure it's getting signal since I don't hear the whine of the motor anymore (have a DaveGA module so that will help but think I need to disconnect the metr.at module which would be a bummer, if anyone knows how to get both working on 4.x hardware please point me in the right direction).
```

---
## \#13 Posted by: Andy87 Posted at: 2019-03-29T20:40:59.629Z Reads: 31

```
Just use the Dave ga in the slave and the metr on the master vesc.
```

---
## \#14 Posted by: wafflejock Posted at: 2019-03-29T20:47:41.441Z Reads: 30

```
Good thought but I only run single drive, was planning to just take off the existing 149kv motor and slightly flakey acting VESC and replace with 200kv (slightly lower torque but slightly higher speed) motor (mostly bearings in old one were sounding a little grindy but still going to try and recover the other VESC for other projects and use the old motor for less critical things, dad is retired EE and wants to try some things).
```

---
## \#15 Posted by: seaborder Posted at: 2019-03-29T20:55:54.579Z Reads: 27

```
yeahh Iam totaly fine with that atm my first build was sensoreless for months its somehow a tiny bit like a manuall car with a clutch. And with the motors np at all:D
```

---
## \#16 Posted by: seaborder Posted at: 2019-03-29T22:03:04.710Z Reads: 23

```
get a 130-160kv I think that will work much better for single drive. All arround
```

---
## \#17 Posted by: wafflejock Posted at: 2019-03-29T22:19:19.574Z Reads: 19

```
ah yah sorry didn't mean to derail your thread was just random question/thought when thinking about the new motor :) I only weigh like 110-115lbs somewhere in that neighborhood and about 5'4" so pretty small dude, will write up a thread once I have a chance to actually try out the new motor and give some real world comparison (I don't ever max out speed even on the existing setup since I use a shorter deck for commuting and hopping the train but will post if the torque difference is massive or not).
```

---
